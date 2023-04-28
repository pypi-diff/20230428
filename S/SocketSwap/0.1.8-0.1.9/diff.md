# Comparing `tmp/SocketSwap-0.1.8-py2.py3-none-any.whl.zip` & `tmp/SocketSwap-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7305 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-24 07:46 SocketSwap/__init__.py
--rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-24 08:20 SocketSwap/context_manager.py
--rw-rw-rw-  2.0 fat    12640 b- defN 23-Apr-24 08:20 SocketSwap/proxy.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      642 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/RECORD
-8 files, 17550 bytes uncompressed, 6187 bytes compressed:  64.7%
+Zip file size: 7540 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-28 11:28 SocketSwap/__init__.py
+-rw-rw-rw-  2.0 fat     1061 b- defN 23-Apr-28 11:26 SocketSwap/context_manager.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-Apr-28 11:25 SocketSwap/proxy.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-28 11:28 SocketSwap-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1898 b- defN 23-Apr-28 11:28 SocketSwap-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-28 11:28 SocketSwap-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-28 11:28 SocketSwap-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      643 b- defN 23-Apr-28 11:28 SocketSwap-0.1.9.dist-info/RECORD
+8 files, 18350 bytes uncompressed, 6422 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: SocketSwap/context_manager.py
 Comment: 
 
 Filename: SocketSwap/proxy.py
 Comment: 
 
-Filename: SocketSwap-0.1.8.dist-info/LICENSE
+Filename: SocketSwap-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: SocketSwap-0.1.8.dist-info/METADATA
+Filename: SocketSwap-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: SocketSwap-0.1.8.dist-info/WHEEL
+Filename: SocketSwap-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: SocketSwap-0.1.8.dist-info/top_level.txt
+Filename: SocketSwap-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: SocketSwap-0.1.8.dist-info/RECORD
+Filename: SocketSwap-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SocketSwap/__init__.py

```diff
@@ -1,14 +1,14 @@
 """
 SocketSwap
 
 SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.9"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
 from SocketSwap.context_manager import SocketSwapContext
 from SocketSwap.proxy import start_local_proxy
```

## SocketSwap/context_manager.py

```diff
@@ -1,30 +1,35 @@
 """
 Module to wrap the TCP proxy in a context manager daemon process
 """
 import multiprocessing
 import SocketSwap.proxy as proxy
 import time
 import logging
+from logging.handlers import QueueListener
 
 logger = logging.getLogger("SocketSwap")
-logger.addHandler(logging.StreamHandler())
+logger.addHandler(logging.NullHandler())
 logger.setLevel(logging.DEBUG)
 
 
 class SocketSwapContext:
     
     def __init__(self, *args):
         self.args = args
     
     def __enter__(self):
         logger.info("Starting Proxy Server")
-        self.proxy_process = multiprocessing.Process(target=proxy.start_local_proxy, args=(self.args))
+        log_queue = multiprocessing.Queue()
+
+        self.proxy_process = multiprocessing.Process(target=proxy.start_local_proxy, args=([log_queue, *self.args]))
         self.proxy_process.daemon = True
         self.proxy_process.start()
+        log_queue_listener = QueueListener(log_queue, *logger.handlers)
+        log_queue_listener.start()
         time.sleep(1)
         return self
     
     def __exit__(self, exc_type, exc_value, traceback):
         logger.info("Exiting proxy server")
         self.proxy_process.terminate()
```

## SocketSwap/proxy.py

```diff
@@ -4,21 +4,19 @@
 import sys
 import threading
 import socket
 import ssl
 import select
 import errno
 import logging
+from logging.handlers import QueueHandler
 from typing import Callable, List
 
-logger = logging.getLogger("SocketSwap")
-logger.addHandler(logging.StreamHandler())
-logger.setLevel(logging.DEBUG)
-
 
+proxy_logger = None
 proxy_socket = None
 
 def is_valid_ip4(ip):
     """Check if a string is a valid IPv4 address.
 
     Args:
         ip (str): A string representing an IPv4 address in the format "X.X.X.X".
@@ -135,29 +133,29 @@
         ctx.load_cert_chain(certfile=server_certificate,
                             keyfile=server_key,
                             )
         local_socket = ctx.wrap_socket(local_socket,
                                        server_side=True,
                                        )
     except ssl.SSLError as e:
-        logger.error(f"SSL handshake failed for listening socket: {e}")
+        proxy_logger.error(f"SSL handshake failed for listening socket: {e}")
         raise
 
     try:
         ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
         ctx.check_hostname = False
         ctx.verify_mode = ssl.CERT_NONE
         
         if client_certificate and client_key:
             ctx.load_cert_chain(certfile=client_certificate, keyfile=client_key)
             
         remote_socket = ctx.wrap_socket(remote_socket, server_hostname=sni)
         
     except ssl.SSLError as e:
-        logger.error(f"SSL handshake failed for remote socket: {e}")
+        proxy_logger.error(f"SSL handshake failed for remote socket: {e}")
         raise
 
     return [remote_socket, local_socket]
 
 
 def starttls(use_ssl: bool, local_socket: socket.socket, read_sockets: List[socket.socket]) -> bool:
     """Check if a socket should start a TLS handshake (STARTTLS).
@@ -187,35 +185,35 @@
 
 def proxy_thread(socket_factory: Callable[[], socket.socket], local_socket: socket.socket, use_ssl: bool, server_key: str, server_certificate: str, client_key: str, client_certificate: str):
     """handles each connection read/write in a seperate thread"""
     try:
         remote_socket = socket_factory()
     except socket.error as socket_error:
         
-        logger.error(f"SOCKET ERROR connecting remote socket: {socket_error}")
-        for s in [remote_socket, local_socket]:
-            s.close()
+        proxy_logger.error(f"SOCKET ERROR connecting remote socket: {socket_error}")
+        local_socket.close()
             
         # TODO braucht man hier den noch? (errno.errorcode[errnumber], os.strerror(errnumber))
         if socket_error.errno not in (errno.ETIMEDOUT, errno.ECONNREFUSED):
             raise socket_error
         return None
         
+    proxy_logger.info("Remote Socket connected successfully")
     
     running = True
     while running:
         read_sockets, _, _ = select.select([remote_socket, local_socket], [], [])
 
         if starttls(use_ssl, local_socket, read_sockets):
             try:
                 ssl_sockets = enable_ssl(server_key, server_certificate, client_key, client_certificate, remote_socket, local_socket)
                 remote_socket, local_socket = ssl_sockets
-                logger.info("SSL enabled")
+                proxy_logger.info("SSL enabled")
             except ssl.SSLError as e:
-                logger.error(f"SSL handshake failed: {e}")
+                proxy_logger.error(f"SSL handshake failed: {e}")
                 break
 
             read_sockets, _, _ = select.select(ssl_sockets, [], [])
 
         for sock in read_sockets:
             try:
                 peer = sock.getpeername()
@@ -225,95 +223,109 @@
                     # I don't yet understand how this error can happen, but if it happens I'll just shut down the thread
                     # the connection is not in a useful state anymore
                     for s in [remote_socket, local_socket]:
                         s.close()
                     running = False
                     break
                 else:
-                    logger.info(f"Socket exception in start_proxy_thread")
+                    proxy_logger.info(f"Socket exception in start_proxy_thread")
                     raise socket_error
 
             data = receive_from(sock)
-            logger.info(f"Received {len(data)} bytes")
+            proxy_logger.info(f"Received {len(data)} bytes")
 
             if sock == local_socket:
                 if len(data):
-                    logger.info( b'< < < out\n' + data)
+                    proxy_logger.info( b'< < < out\n' + data)
                     remote_socket.send(data.encode() if isinstance(data, str) else data)
                 else:
-                    logger.info( "Connection from local client %s:%d closed" % peer)
+                    proxy_logger.info( "Connection from local client %s:%d closed" % peer)
                     remote_socket.close()
                     running = False
                     break
             elif sock == remote_socket:
                 if len(data):
-                    logger.info( b'> > > in\n' + data)
+                    proxy_logger.info( b'> > > in\n' + data)
                     local_socket.send(data)
                 else:
-                    logger.info( "Connection to remote server %s:%d closed" % peer)
+                    proxy_logger.info( "Connection to remote server %s:%d closed" % peer)
                     local_socket.close()
                     running = False
                     break
            
 
 
-def start_local_proxy(connect_socket, local_host, local_port, server_key=None, server_certificate=None, client_key=None, client_certificate=None, use_ssl=False):
+def start_local_proxy(log_queue, socket_factory, local_host, local_port, server_key=None, server_certificate=None, client_key=None, client_certificate=None, use_ssl=False):
     """starts a local proxy server"""
     global proxy_socket
-    logger.info("Starting local proxy server")
+    global proxy_logger
+    
+    proxy_logger = logging.getLogger("SocketSwapProxy")
+    proxy_logger.addHandler(QueueHandler(log_queue))
+    proxy_logger.setLevel(logging.DEBUG)
+    
+    proxy_logger.info("Starting local proxy server")
     
     if ((client_key is None) ^ (client_certificate is None)):
-        logger.error("You must either specify both the client certificate and client key or leave both empty")
+        proxy_logger.error("You must either specify both the client certificate and client key or leave both empty")
         sys.exit(8)
 
     if local_host != '0.0.0.0' and not is_valid_ip4(local_host):
         try:
             ip = socket.gethostbyname(local_host)
         except socket.gaierror:
             ip = False
         if ip is False:
-            logger.error(f"Provided listening host is not a valid IP address or host name: {local_host}")
+            proxy_logger.error(f"Provided listening host is not a valid IP address or host name: {local_host}")
             sys.exit(1)
         else:
             local_host = ip
 
 
     # local proxy socket
     proxy_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     proxy_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
     try:
         proxy_socket.bind((local_host, local_port))
     except socket.error as e:
-        logger.error(e.strerror)
+        proxy_logger.error(e.strerror)
         sys.exit(5)
 
     proxy_socket.listen(100)
     try:
         while True:
             in_socket, in_addrinfo = proxy_socket.accept()
-            logger.info( 'Connection from %s:%d' % in_addrinfo)
+            proxy_logger.info( 'Connection from %s:%d' % in_addrinfo)
             pthread = threading.Thread(
                 target=proxy_thread, 
-                args=(connect_socket, in_socket, use_ssl, server_key, server_certificate, client_key, client_certificate)
+                args=(socket_factory, in_socket, use_ssl, server_key, server_certificate, client_key, client_certificate)
             )
-            logger.info(f"Starting proxy thread {pthread.name}")
+            proxy_logger.info(f"Starting proxy thread {pthread.name}")
             pthread.start()
     except KeyboardInterrupt as e:
-        logger.info(e)
+        proxy_logger.info(e)
         sys.exit(0)
 
 
+
 def stop_local_proxy():
+    """
+    Stops the local proxy server by closing the listening socket.
+
+    Note:
+    This function uses a global variable proxy_socket to store the socket object. If proxy_socket is not defined
+    or is already closed, no action will be taken.
+    """
     global proxy_socket
     try:
         if proxy_socket:
             proxy_socket.close()
     except Exception as e:
-        logger.error(f"Exception on closing listening socket: {e}")
+        proxy_logger.error(f"Exception on closing listening socket: {e}")
 
 
 if __name__ == '__main__':
     # for testing
```

## Comparing `SocketSwap-0.1.8.dist-info/LICENSE` & `SocketSwap-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SocketSwap-0.1.8.dist-info/METADATA` & `SocketSwap-0.1.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SocketSwap
-Version: 0.1.8
+Version: 0.1.9
 Summary: SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 Home-page: https://github.com/fyx99/SocketSwap
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -34,25 +34,26 @@
 #### Context Manager
 
 ```python 
 import socket
 from SocketSwap import ProxySwapContext
 
 
-def conn_factory():
+def socket_factory():
     target_host = "localhost"
     target_port = 5432
     remote_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     remote_socket.connect((target_host, target_port))
     return remote_socket
 
 def main():
     
-    with ProxySwapContext(conn_factory, "127.0.0.1", 2222):
+    with ProxySwapContext(socket_factory, "127.0.0.1", 2222):
         # do something you want to proxy
+        # connect to 127.0.0.1:2222
 
 ```
 The ProxySwapContext takes essentially 3 mandatory arguments.  
 
 ## Credits:
 
 The TCP Proxy part is a slim modified version of https://github.com/ickerwx/tcpproxy.
```

