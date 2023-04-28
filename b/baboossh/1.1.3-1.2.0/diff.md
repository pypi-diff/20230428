# Comparing `tmp/baboossh-1.1.3.tar.gz` & `tmp/baboossh-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baboossh-1.1.3.tar", last modified: Sun Feb  6 11:13:11 2022, max compression
+gzip compressed data, was "baboossh-1.2.0.tar", last modified: Fri Apr 28 15:38:59 2023, max compression
```

## Comparing `baboossh-1.1.3.tar` & `baboossh-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2022-02-06 11:13:11.581959 baboossh-1.1.3/
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)    35077 2022-01-28 12:18:42.000000 baboossh-1.1.3/LICENSE
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1488 2022-02-06 11:13:11.581959 baboossh-1.1.3/PKG-INFO
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)      682 2022-01-28 12:18:42.000000 baboossh-1.1.3/README.rst
-drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2022-02-06 11:13:11.579959 baboossh-1.1.3/baboossh/
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)      551 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/__init__.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)    18639 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/connection.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     5959 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/creds.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     5531 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/db.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     9317 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/endpoint.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)      743 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/exceptions.py
-drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2022-02-06 11:13:11.581959 baboossh-1.1.3/baboossh/ext_dir/
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)      952 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/auth_password.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     6557 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/auth_privkey.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     3650 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/ext_dir/export_comprograph.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     2612 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/ext_dir/import_nmapxml.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1414 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/payload_exec.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)    13323 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/payload_gather.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1577 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/payload_getfile.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1353 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/payload_putfile.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1822 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/ext_dir/payload_shell.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     2062 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/extensions.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)    10042 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/host.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     6549 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/path.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)    54398 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/shell.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1981 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/tag.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     4583 2022-02-06 11:12:30.000000 baboossh-1.1.3/baboossh/tunnel.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     5038 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/user.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1445 2022-01-28 12:18:42.000000 baboossh-1.1.3/baboossh/utils.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)       27 2022-02-06 11:12:30.000000 baboossh-1.1.3/baboossh/version.py
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)    33362 2022-02-05 17:16:59.000000 baboossh-1.1.3/baboossh/workspace.py
-drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2022-02-06 11:13:11.580959 baboossh-1.1.3/baboossh.egg-info/
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1488 2022-02-06 11:13:11.000000 baboossh-1.1.3/baboossh.egg-info/PKG-INFO
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)      822 2022-02-06 11:13:11.000000 baboossh-1.1.3/baboossh.egg-info/SOURCES.txt
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)        1 2022-02-06 11:13:11.000000 baboossh-1.1.3/baboossh.egg-info/dependency_links.txt
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)       38 2022-02-06 11:13:11.000000 baboossh-1.1.3/baboossh.egg-info/requires.txt
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)        9 2022-02-06 11:13:11.000000 baboossh-1.1.3/baboossh.egg-info/top_level.txt
-drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2022-02-06 11:13:11.581959 baboossh-1.1.3/bin/
--rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)      102 2022-01-28 12:18:42.000000 baboossh-1.1.3/bin/baboossh
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)       38 2022-02-06 11:13:11.581959 baboossh-1.1.3/setup.cfg
--rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1495 2022-02-05 17:20:15.000000 baboossh-1.1.3/setup.py
+drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2023-04-28 15:38:59.401222 baboossh-1.2.0/
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)    35077 2022-12-27 10:47:10.000000 baboossh-1.2.0/LICENSE
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1451 2023-04-28 15:38:59.401222 baboossh-1.2.0/PKG-INFO
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)      682 2022-12-27 10:47:10.000000 baboossh-1.2.0/README.rst
+drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2023-04-28 15:38:59.399222 baboossh-1.2.0/baboossh/
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)      551 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/__init__.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)    18085 2023-04-28 15:35:28.000000 baboossh-1.2.0/baboossh/connection.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     5959 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/creds.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     5531 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/db.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     9317 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/endpoint.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)      743 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/exceptions.py
+drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2023-04-28 15:38:59.401222 baboossh-1.2.0/baboossh/ext_dir/
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)      952 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/auth_password.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     6557 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/auth_privkey.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     3650 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/export_comprograph.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     2612 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/import_nmapxml.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1074 2023-04-28 15:35:28.000000 baboossh-1.2.0/baboossh/ext_dir/payload_exec.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)    13464 2023-04-28 15:35:28.000000 baboossh-1.2.0/baboossh/ext_dir/payload_gather.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1577 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/payload_getfile.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1353 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/payload_putfile.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1822 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/ext_dir/payload_shell.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     2062 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/extensions.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)    10400 2023-04-28 15:35:28.000000 baboossh-1.2.0/baboossh/host.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     6549 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/path.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)    54392 2023-04-28 15:35:28.000000 baboossh-1.2.0/baboossh/shell.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1981 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/tag.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     4583 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/tunnel.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     5038 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/user.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1445 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/utils.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)       27 2023-04-28 15:35:56.000000 baboossh-1.2.0/baboossh/version.py
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)    33362 2022-12-27 10:47:10.000000 baboossh-1.2.0/baboossh/workspace.py
+drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2023-04-28 15:38:59.400221 baboossh-1.2.0/baboossh.egg-info/
+-rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)     1451 2023-04-28 15:38:59.000000 baboossh-1.2.0/baboossh.egg-info/PKG-INFO
+-rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)      822 2023-04-28 15:38:59.000000 baboossh-1.2.0/baboossh.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        1 2023-04-28 15:38:59.000000 baboossh-1.2.0/baboossh.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)       38 2023-04-28 15:38:59.000000 baboossh-1.2.0/baboossh.egg-info/requires.txt
+-rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        9 2023-04-28 15:38:59.000000 baboossh-1.2.0/baboossh.egg-info/top_level.txt
+drwxr-xr-x   0 ncnd      (1000) ncnd      (1000)        0 2023-04-28 15:38:59.401222 baboossh-1.2.0/bin/
+-rwxr-xr-x   0 ncnd      (1000) ncnd      (1000)      102 2022-03-25 18:26:10.000000 baboossh-1.2.0/bin/baboossh
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)       38 2023-04-28 15:38:59.401222 baboossh-1.2.0/setup.cfg
+-rw-r--r--   0 ncnd      (1000) ncnd      (1000)     1495 2022-12-27 10:47:10.000000 baboossh-1.2.0/setup.py
```

### Comparing `baboossh-1.1.3/LICENSE` & `baboossh-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/PKG-INFO` & `baboossh-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: baboossh
-Version: 1.1.3
+Version: 1.2.0
 Summary: SSH spreader made easy for red teams in a hurry
 Home-page: https://github.com/cybiere/BabooSSH
 Author: Cybiere - Akerva
 Author-email: nicolas@cosnard.io
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/cybiere/BabooSSH/issues
 Project-URL: Documentation, https://baboossh.cybiere.fr/
 Project-URL: Source Code, https://github.com/cybiere/BabooSSH
 Keywords: ssh spread redteam pentest
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Security
 Description-Content-Type: text/x-rst
@@ -42,9 +40,7 @@
 
 Documentation
 +++++++++++++
 
 The documentation is under redaction and some things might be missing, but you can find it there: `<https://baboossh.cybiere.fr>`_ .
 
 
-
-
```

### Comparing `baboossh-1.1.3/README.rst` & `baboossh-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/__init__.py` & `baboossh-1.2.0/baboossh/__init__.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/connection.py` & `baboossh-1.2.0/baboossh/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import paramiko
 from baboossh import Db, Endpoint, User, Creds, Path, Host, Tag
 from baboossh.exceptions import *
 from baboossh.utils import Unique
 from paramiko.py3compat import u
 import socket
+import select
 
 class Connection(metaclass=Unique):
     """A :class:`User` and :class:`Creds` to authenticate on an :class:`Endpoint`
 
     A connection represents the working association of those 3 objects to connect
     a target. It can be used to run payloads on a :class:`Host`, open a
     :class:`Tunnel` to it or use it as a pivot to reach new :class:`Endpoint` s
@@ -256,111 +257,66 @@
                 raise ValueError("Supplied user isn't in workspace")
             if cred[0] == "#":
                 cred = cred[1:]
             cred = Creds.find_one(creds_id=cred)
             if cred is None:
                 raise ValueError("Supplied credentials aren't in workspace")
             return Connection(endpoint, user, cred)
-
         if ':' not in arg:
+            host = Host.find_one(name=arg)
+            if host is not None:
+                return Connection.find_one(endpoint=host.closest_endpoint)
             arg = arg+':22'
         endpoint = Endpoint.find_one(ip_port=arg)
         if endpoint is None:
             raise ValueError("Supplied endpoint isn't in workspace")
         connection = cls.find_one(endpoint=endpoint)
         if connection is None:
             raise ValueError("No working connection for supplied endpoint")
         return connection
     
     def identify(self):
-        #TODO
-        """Indentify the host"""
-        if self.transport is None:
-            raise ConnectionClosedError
+        """Identify the host"""
         try:
-            ######## hostname ########
-            chan = self.transport.open_channel("session",timeout=3)
-            hostname=""
-            chan.exec_command("hostname")
-            try:
-                x = u(chan.recv(1024))
-                while len(x) != 0:
-                    hostname = hostname + x
-                    x = u(chan.recv(1024))
-            except socket.timeout:
-                pass
-            chan.close()
-            hostname = hostname.rstrip()
-            ######## uname ########
-            chan = self.transport.open_channel("session",timeout=3)
-            uname=""
-            chan.exec_command("uname -a")
-            try:
-                x = u(chan.recv(1024))
-                while len(x) != 0:
-                    uname = uname + x
-                    x = u(chan.recv(1024))
-            except socket.timeout:
-                pass
-            chan.close()
-            uname = uname.rstrip()
-            ######## issue ########
-            chan = self.transport.open_channel("session",timeout=3)
-            issue=""
-            chan.exec_command("cat /etc/issue")
-            try:
-                x = u(chan.recv(1024))
-                while len(x) != 0:
-                    issue = issue + x
-                    x = u(chan.recv(1024))
-            except socket.timeout:
-                pass
-            chan.close()
-            issue = issue.rstrip()
-            ######## machineid ########
-            chan = self.transport.open_channel("session",timeout=3)
-            machine_id=""
-            chan.exec_command("cat /etc/machine-id")
-            try:
-                x = u(chan.recv(1024))
-                while len(x) != 0:
-                    machine_id = machine_id + x
-                    x = u(chan.recv(1024))
-            except socket.timeout:
-                pass
-            chan.close()
-            machine_id = machine_id.rstrip()
-            ######## macs ########
-            chan = self.transport.open_channel("session",timeout=3)
-            mac_str=""
-            chan.exec_command("for i in `ls -l /sys/class/net/ | grep -v virtual | grep 'devices' | tr -s '[:blank:]' | cut -d ' ' -f 9 | sort`; do ip l show $i | grep ether | tr -s '[:blank:]' | cut -d ' ' -f 3; done")
-            try:
-                x = u(chan.recv(1024))
-                while len(x) != 0:
-                    mac_str = mac_str + x
-                    x = u(chan.recv(1024))
-            except socket.timeout:
-                pass
-            mac_str = mac_str.rstrip()
+            serverKey = self.transport.get_remote_server_key()
+            print(serverKey.asbytes())
+            c,result = self.exec_command("hostname")
+            if c != 0:
+                nextId = Host.getNextId()
+                name = "host"+str(nextId)
+                print("\t>Unable to get hostname - using \""+name+"\". You can change it using \"host edit "+name+"\".")
+                hostname = ""
+            else:
+                name = result.rstrip()
+                hostname = name
+            c,result = self.exec_command("uname -a")
+            uname = result.rstrip()
+            c,result = self.exec_command("cat /etc/issue")
+            issue = result.rstrip()
+            c,result = self.exec_command("cat /etc/machine-id")
+            machine_id = result.rstrip()
+            c,result = self.exec_command("for i in `ls -l /sys/class/net/ | grep -v virtual | grep 'devices' | tr -s '[:blank:]' | cut -d ' ' -f 9 | sort`; do ip l show $i | grep ether | tr -s '[:blank:]' | cut -d ' ' -f 3; done")
+            mac_str = result.rstrip()
             macs = mac_str.split()
-            chan.close()
-
-            ######## host ########
+        except Exception as exc:
+            print("Error trying to identify: "+str(exc))
+            return False
+        try:
             new_host = Host(hostname, uname, issue, machine_id, macs)
             if new_host.id is None:
                 print("\t"+str(self)+" is a new host: " + new_host.name)
             else:
                 print("\t"+str(self)+" is an existing host: " + new_host.name)
                 if not new_host.scope:
                     self.endpoint.scope = False
             new_host.save()
             self.endpoint.host = new_host
             self.endpoint.save()
         except Exception as exc:
-            print("Error : "+str(exc))
+            print("Error creating host : "+str(exc))
             return False
         return True
 
     def open_transport(self, gateway="auto"):
         #TODO check verbosity levels
         sock = None
         if gateway == "auto":
@@ -391,14 +347,35 @@
         if self.endpoint.distance is None or self.endpoint.distance > new_distance:
             self.endpoint.distance = new_distance
         self.endpoint.save()
         transport.close()
         sock.close()
         return True
 
+    def exec_command(self, command):
+        if self.transport is None:
+            raise ConnectionClosedError
+        try:
+            chan = self.transport.open_session()
+            chan.get_pty()
+            chan.exec_command(command)
+            output = ""
+            while True:
+                return_code = chan.recv_exit_status()
+                if chan.exit_status_ready():
+                    output = output+chan.recv(1024).decode("utf-8")
+                    break
+                rl, wl, xl = select.select([chan], [], [], 0.0)
+                if len(rl) > 0:
+                    output = output+chan.recv(1024).decode("utf-8")
+        except Exception as e:
+            raise
+        return (return_code,output)
+
+
     def open(self, verbose=False, target=False):
         if self.transport is not None:
             if not self.transport.is_active():
                 print("Connection to \033[1;34m"+str(self)+"\033[0m went inactive, Closing... ", end="", flush=True)
                 self.close()
             else:
                 if target:
```

### Comparing `baboossh-1.1.3/baboossh/creds.py` & `baboossh-1.2.0/baboossh/creds.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/db.py` & `baboossh-1.2.0/baboossh/db.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/endpoint.py` & `baboossh-1.2.0/baboossh/endpoint.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/exceptions.py` & `baboossh-1.2.0/baboossh/exceptions.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/auth_password.py` & `baboossh-1.2.0/baboossh/ext_dir/auth_password.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/auth_privkey.py` & `baboossh-1.2.0/baboossh/ext_dir/auth_privkey.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/export_comprograph.py` & `baboossh-1.2.0/baboossh/ext_dir/export_comprograph.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/import_nmapxml.py` & `baboossh-1.2.0/baboossh/ext_dir/import_nmapxml.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/payload_exec.py` & `baboossh-1.2.0/baboossh/ext_dir/payload_exec.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,31 +23,21 @@
         return "Execute a command on target"
     
     @classmethod
     def buildParser(cls,parser):
         parser.add_argument('cmd',nargs="+",help='Command to execute on target')
 
     @classmethod
-    def run(cls, connection,wspaceFolder, stmt):
+    def run(cls, connection, wspaceFolder, stmt):
         if connection.transport is None:
             raise ConnectionClosedError
         command = " ".join(getattr(stmt,"cmd",["hostname"]))
 
-        chan = connection.transport.open_channel("session",timeout=3)
         try:
-            chan.exec_command(command)
-            try:
-                x = u(chan.recv(1024))
-                while len(x) != 0:
-                    print(x,end="")
-                    x = u(chan.recv(1024))
-            except socket.timeout:
-                pass
-            print("\r\n*** EOF\r\n")
-        except SSHException:
-            print("Error : exec command did not work, please try shell payload instead.");
-            chan.close()
+            c,output = connection.exec_command(command)
+            print("<Return code: "+str(c)+">");
+            print(output)
+        except Exception as e:
+            print("Error : "+str(e))
             return False
-
-        chan.close()
         return True
```

### Comparing `baboossh-1.1.3/baboossh/ext_dir/payload_gather.py` & `baboossh-1.2.0/baboossh/ext_dir/payload_gather.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,22 +252,26 @@
         os.remove(filepath)
 
 
     def gatherKeys(self):
         files = []
         ret = []
         chan = self.connection.transport.open_channel("session",timeout=3)
-        filelist = self.sftp.listdir_attr(".ssh")
-        for file in filelist:
-            if file.st_size == 0:
-                continue
-            if "rsa" in file.filename or "key" in file.filename or "p12" in file.filename or "dsa" in file.filename:
-                files.append(file.filename)
-        for keyfile in files:
-            c = self.getKeyToCreds(keyfile)
+        try:
+            filelist = self.sftp.listdir_attr(".ssh")
+            for file in filelist:
+                if file.st_size == 0:
+                    continue
+                if "rsa" in file.filename or "key" in file.filename or "p12" in file.filename or "dsa" in file.filename:
+                    files.append(file.filename)
+            for keyfile in files:
+                c = self.getKeyToCreds(keyfile)
+        except FileNotFoundError:
+            # TODO : log somehow the failure
+            pass
 
     def getKeyToCreds(self,keyfile,basePath=".ssh"):
         if basePath != ".":
             keyfile = os.path.join(basePath,keyfile)
         from baboossh.extensions import Extensions
         keysFolder = os.path.join(self.wspaceFolder,"keys")
         filename = str(self.connection.endpoint).replace(":","-")+"_"+str(self.connection.user)+"_"+keyfile.replace("/","_")
```

### Comparing `baboossh-1.1.3/baboossh/ext_dir/payload_getfile.py` & `baboossh-1.2.0/baboossh/ext_dir/payload_getfile.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/payload_putfile.py` & `baboossh-1.2.0/baboossh/ext_dir/payload_putfile.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/ext_dir/payload_shell.py` & `baboossh-1.2.0/baboossh/ext_dir/payload_shell.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/extensions.py` & `baboossh-1.2.0/baboossh/extensions.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/host.py` & `baboossh-1.2.0/baboossh/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     longer to reach a `Host` from one endpoint rather than the other.
 
     The aggregation is checked by :func:`Connection.identify`, which is run on
     every endpoint newly connected. If every `Host` attribute matches with an
     existing Host, the endpoint is considered to belong to it and is added.
 
     Attributes:
-        name (str): the hostname of the Host as returned by the command `hostname`
+        name (str): the hostname of the Host as returned by the command `hostname`, or a random name if not available
+        hostname (str): the output of the command `hostname`
         id (int): the id of the Host
         uname (str): the output of the command `uname -a` on the Host
         issue (str): the content of the file `/etc/issue` on the Host
         machine_id (str): the content of the file `/etc/machine-id` on the Host
         macs ([str, ...]): a list of the MAC addresses of the Host interfaces
     """
 
@@ -87,25 +88,25 @@
             endpoint.save()
 
     @property
     def distance(self):
         """Returns the `Host` 's number of hops from `"Local"`"""
 
         cursor = Db.get().cursor()
-        cursor.execute('SELECT distance FROM endpoints WHERE host=? ORDER BY distance DESC', (self.id, ))
+        cursor.execute('SELECT distance FROM endpoints WHERE host=? ORDER BY distance ASC', (self.id, ))
         row = cursor.fetchone()
         cursor.close()
         return row[0]
 
     @property
     def closest_endpoint(self):
         """Returns the `Host` 's closest :class:`Endpoint`"""
 
         cursor = Db.get().cursor()
-        cursor.execute('SELECT ip, port FROM endpoints WHERE host=? ORDER BY distance DESC', (self.id, ))
+        cursor.execute('SELECT ip, port FROM endpoints WHERE host=? ORDER BY distance ASC', (self.id, ))
         row = cursor.fetchone()
         cursor.close()
         from baboossh import Endpoint
         return Endpoint(row[0], row[1])
 
     @property
     def endpoints(self):
@@ -240,14 +241,25 @@
         row = cursor.fetchone()
         cursor.close()
         if row is None:
             return None
         return Host(row[0], row[1], row[2], row[3], json.loads(row[4]))
 
     @classmethod
+    def getNextId(cls):
+        cursor = Db.get().cursor()
+        cursor.execute('''SELECT MAX(id) FROM hosts''')
+        row = cursor.fetchone()
+        cursor.close()
+        if row[0] is None:
+            return 1
+        return row[0] + 1;
+
+
+    @classmethod
     def search(cls, field, val, show_all=False):
         """Search in the workspace for a `Host`
 
         Args:
             field (str): the `Host` attribute to search in
             val (str): the value to search for
             show_all (bool): whether to include out-of scope `Host` s in search results
```

### Comparing `baboossh-1.1.3/baboossh/path.py` & `baboossh-1.2.0/baboossh/path.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/shell.py` & `baboossh-1.2.0/baboossh/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1014,15 +1014,15 @@
         port = getattr(stmt, 'port', None)
         self.workspace.tunnel_close(port)
 
     __parser_tunnel = argparse.ArgumentParser(prog="tunnel")
     __subparser_tunnel = __parser_tunnel.add_subparsers(title='Actions', help='Available actions')
     __parser_tunnel_list = __subparser_tunnel.add_parser("list", help='List tunnels')
     __parser_tunnel_open = __subparser_tunnel.add_parser("open", help='Open tunnel')
-    __parser_tunnel_open.add_argument('connection', help='Connection string', choices_provider=__get_option_connection)
+    __parser_tunnel_open.add_argument('connection', help='Connection string', choices_provider=__get_run_targets)
     __parser_tunnel_open.add_argument('port', help='Tunnel entry port', type=int, nargs='?')
     __parser_tunnel_close = __subparser_tunnel.add_parser("close", help='Close tunnel')
     __parser_tunnel_close.add_argument('port', help='Tunnel entry port', type=int, choices_provider=__get_open_tunnels)
 
     __parser_tunnel_list.set_defaults(func=__tunnel_list)
     __parser_tunnel_open.set_defaults(func=__tunnel_open)
     __parser_tunnel_close.set_defaults(func=__tunnel_close)
```

### Comparing `baboossh-1.1.3/baboossh/tag.py` & `baboossh-1.2.0/baboossh/tag.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/tunnel.py` & `baboossh-1.2.0/baboossh/tunnel.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/user.py` & `baboossh-1.2.0/baboossh/user.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/utils.py` & `baboossh-1.2.0/baboossh/utils.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh/workspace.py` & `baboossh-1.2.0/baboossh/workspace.py`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/baboossh.egg-info/PKG-INFO` & `baboossh-1.2.0/baboossh.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: baboossh
-Version: 1.1.3
+Version: 1.2.0
 Summary: SSH spreader made easy for red teams in a hurry
 Home-page: https://github.com/cybiere/BabooSSH
 Author: Cybiere - Akerva
 Author-email: nicolas@cosnard.io
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/cybiere/BabooSSH/issues
 Project-URL: Documentation, https://baboossh.cybiere.fr/
 Project-URL: Source Code, https://github.com/cybiere/BabooSSH
 Keywords: ssh spread redteam pentest
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Security
 Description-Content-Type: text/x-rst
@@ -42,9 +40,7 @@
 
 Documentation
 +++++++++++++
 
 The documentation is under redaction and some things might be missing, but you can find it there: `<https://baboossh.cybiere.fr>`_ .
 
 
-
-
```

### Comparing `baboossh-1.1.3/baboossh.egg-info/SOURCES.txt` & `baboossh-1.2.0/baboossh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baboossh-1.1.3/setup.py` & `baboossh-1.2.0/setup.py`

 * *Files identical despite different names*

