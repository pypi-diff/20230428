# Comparing `tmp/shoal-client-1.0.2.tar.gz` & `tmp/shoal-client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/centos/shoal/shoal-client/dist/tmpkp78pf0l/shoal-client-1.0.2.tar", last modified: Thu Apr 22 19:25:26 2021, max compression
+gzip compressed data, was "/hepuser/colsond/projects/shoal/shoal-client/dist/tmp3p3hmfzv/shoal-client-1.0.3.tar", last modified: Fri Apr 28 17:52:39 2023, max compression
```

## Comparing `shoal-client-1.0.2.tar` & `shoal-client-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 19:25:26.000000 shoal-client-1.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 19:25:26.000000 shoal-client-1.0.2/conf/
--rw-rw-r--   0 root         (0) root         (0)      609 2021-04-22 19:24:17.000000 shoal-client-1.0.2/conf/shoal_client.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-04-22 19:24:17.000000 shoal-client-1.0.2/shoal_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       18 2021-04-22 19:24:17.000000 shoal-client-1.0.2/shoal_client/__version__.py
--rw-rw-r--   0 root         (0) root         (0)     3484 2021-04-22 19:24:17.000000 shoal-client-1.0.2/shoal_client/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4813 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      321 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-04-22 19:25:26.000000 shoal-client-1.0.2/shoal_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       25 2021-04-22 19:24:17.000000 shoal-client-1.0.2/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     3645 2021-04-22 19:24:17.000000 shoal-client-1.0.2/README.md
--rw-rw-r--   0 root         (0) root         (0)     1346 2021-04-22 19:24:17.000000 shoal-client-1.0.2/setup.py
--rwxrwxr-x   0 root         (0) root         (0)    17483 2021-04-22 19:24:17.000000 shoal-client-1.0.2/shoal-client
--rw-r--r--   0 root         (0) root         (0)     4813 2021-04-22 19:25:26.000000 shoal-client-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-22 19:25:26.000000 shoal-client-1.0.2/setup.cfg
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/shoal_client.egg-info/
+-rw-r--r--   0 colsond  (115344) hep      (34244)       13 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/top_level.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)       34 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/requires.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)        1 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)      321 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 colsond  (115344) hep      (34244)     4090 2023-04-28 17:52:38.000000 shoal-client-1.0.3/shoal_client.egg-info/PKG-INFO
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/shoal_client/
+-rw-r--r--   0 colsond  (115344) hep      (34244)        0 2023-04-20 18:14:31.000000 shoal-client-1.0.3/shoal_client/__init__.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)     3484 2023-04-20 18:14:31.000000 shoal-client-1.0.3/shoal_client/config.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)       18 2023-04-28 17:38:17.000000 shoal-client-1.0.3/shoal_client/__version__.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)     1346 2023-04-20 18:14:31.000000 shoal-client-1.0.3/setup.py
+-rw-r--r--   0 colsond  (115344) hep      (34244)     4090 2023-04-28 17:52:39.000000 shoal-client-1.0.3/PKG-INFO
+-rw-r--r--   0 colsond  (115344) hep      (34244)       38 2023-04-28 17:52:39.000000 shoal-client-1.0.3/setup.cfg
+drwxr-xr-x   0 colsond  (115344) hep      (34244)        0 2023-04-28 17:52:39.000000 shoal-client-1.0.3/conf/
+-rw-r--r--   0 colsond  (115344) hep      (34244)      609 2023-04-20 18:14:31.000000 shoal-client-1.0.3/conf/shoal_client.conf
+-rwxr-xr-x   0 colsond  (115344) hep      (34244)    18651 2023-04-26 18:08:03.000000 shoal-client-1.0.3/shoal-client
+-rw-r--r--   0 colsond  (115344) hep      (34244)     3645 2023-04-20 18:14:31.000000 shoal-client-1.0.3/README.md
+-rw-r--r--   0 colsond  (115344) hep      (34244)       25 2023-04-20 18:14:31.000000 shoal-client-1.0.3/MANIFEST.in
```

### Comparing `shoal-client-1.0.2/conf/shoal_client.conf` & `shoal-client-1.0.3/conf/shoal_client.conf`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.2/shoal_client/config.py` & `shoal-client-1.0.3/shoal_client/config.py`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.2/shoal_client.egg-info/PKG-INFO` & `shoal-client-1.0.3/shoal_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 Metadata-Version: 2.1
 Name: shoal-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A squid cache publishing and advertising tool designed to work in fast changing environments
 Home-page: http://github.com/hep-gc/shoal
 Author: Mike Chester, Colson Drimiel, Ian Gable, Alex Lam, Rob Prior, Ryan Taylor, Steve Traylen, Marcus Ebert, Da Meng
 Author-email: heprc-shoal@uvic.ca
 License: 'GPL3' or 'Apache 2'
-Description: # Shoal Client README
-        # Version: v1.0.1
-        
-        shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
-        and using cvmfs-talk to update the active proxy configuration.
-        
-        shoal-client is a simple python script typically configured to run with cron to check for new squids 
-        periodically. Before setting the cronjob in place make sure that shoal-client is
-        configured correctly (see Usage below).
-        
-        With the release of v0.6.4 the shoal-client now offers support for frontier. Running the shoal-client
-        with the --frontier or -f option will produce an output string instead of attempting to update the
-        proxies via cvmfs-talk. See Usage below for more information.
-        
-        
-        ## Installation
-        
-        **Note**: Requires Python 2.4+
-        
-        **Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
-        root permissions.
-        
-        ### Recommended Instalation Method: Use pip
-        
-        1. `pip install shoal-client`
-        2. Copy the configuration file to proper location
-            ```
-            # For python3
-            cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
-            
-            # For python2
-            cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
-            ````
-        3. Check settings in `shoal_client.conf` update as needed
-        
-            
-        ## Usage
-        
-        Confirm the that you configured shoal-client as expected by checking the output of `shoal-client --dump`
-        The output is a list of servers that will be set as proxies using cvmfs-talk. For example you will see 
-        something like the following:
-        
-            http://squid.example1.com:3128;http://squid.example2.com:3128;http://squid.example3.com:3128;http://squid.example4.com:3128;http://squid.example5.org:3128;DIRECT
-        
-        If the output looks resonable now set a crontab entry to run shoal say every 30 minutes:
-        
-            0,30 * * * * /usr/bin/shoal-client
-        
-        New in version 0.6.4 is the --frontier option that will produce an output string suitable for frontier.
-        Users will need to use a simple script that runs shoal-client and uses the output to set the proxies.
-        An example script can be found [here](https://github.com/hep-gc/shoal/blob/master/shoal-client/scripts/frontier_set.sh) in the shoal-client/scripts directory.
-        Example output when running `shoal-client --frontier`:
-        
-            (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
-        
-        ### Flags and Options
-        | Option | Description |
-        | --- | --- |
-        | -d or --dump | Print closest proxies to terminal for testing or debugging. |
-        | -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
-        | -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
-        | -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
-        
-        Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
-        
-             cvmfs_talk proxy info
-        
-        ## Other Installation Methods
-        
-        ### Using Pip
-        
-        1. `pip install shoal-client`
-        2. Copy the configuration file to proper location
-            ```
-            # For python3
-            cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
-            
-            # For python2
-            cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
-            ```
-        3. Check settings in `shoal_client.conf` update as needed
-        
-        ### Using Git
-        1. `git clone git://github.com/hep-gc/shoal.git`
-        2. `cd shoal/shoal-client/`
-        3. `python setup.py install`
-        4. Copy the configuration file to proper location `cp conf/shoal_client.conf /etc/shoal/`
-        5. Check settings in `shoal_client.conf` update as needed
-        
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Shoal Client README
+# Version: v1.0.1
+
+shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
+and using cvmfs-talk to update the active proxy configuration.
+
+shoal-client is a simple python script typically configured to run with cron to check for new squids 
+periodically. Before setting the cronjob in place make sure that shoal-client is
+configured correctly (see Usage below).
+
+With the release of v0.6.4 the shoal-client now offers support for frontier. Running the shoal-client
+with the --frontier or -f option will produce an output string instead of attempting to update the
+proxies via cvmfs-talk. See Usage below for more information.
+
+
+## Installation
+
+**Note**: Requires Python 2.4+
+
+**Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
+root permissions.
+
+### Recommended Instalation Method: Use pip
+
+1. `pip install shoal-client`
+2. Copy the configuration file to proper location
+    ```
+    # For python3
+    cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
+    
+    # For python2
+    cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
+    ````
+3. Check settings in `shoal_client.conf` update as needed
+
+    
+## Usage
+
+Confirm the that you configured shoal-client as expected by checking the output of `shoal-client --dump`
+The output is a list of servers that will be set as proxies using cvmfs-talk. For example you will see 
+something like the following:
+
+    http://squid.example1.com:3128;http://squid.example2.com:3128;http://squid.example3.com:3128;http://squid.example4.com:3128;http://squid.example5.org:3128;DIRECT
+
+If the output looks resonable now set a crontab entry to run shoal say every 30 minutes:
+
+    0,30 * * * * /usr/bin/shoal-client
+
+New in version 0.6.4 is the --frontier option that will produce an output string suitable for frontier.
+Users will need to use a simple script that runs shoal-client and uses the output to set the proxies.
+An example script can be found [here](https://github.com/hep-gc/shoal/blob/master/shoal-client/scripts/frontier_set.sh) in the shoal-client/scripts directory.
+Example output when running `shoal-client --frontier`:
+
+    (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
+
+### Flags and Options
+| Option | Description |
+| --- | --- |
+| -d or --dump | Print closest proxies to terminal for testing or debugging. |
+| -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
+| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
+| -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
+
+Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
+
+     cvmfs_talk proxy info
+
+## Other Installation Methods
+
+### Using Pip
+
+1. `pip install shoal-client`
+2. Copy the configuration file to proper location
+    ```
+    # For python3
+    cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
+    
+    # For python2
+    cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
+    ```
+3. Check settings in `shoal_client.conf` update as needed
+
+### Using Git
+1. `git clone git://github.com/hep-gc/shoal.git`
+2. `cd shoal/shoal-client/`
+3. `python setup.py install`
+4. Copy the configuration file to proper location `cp conf/shoal_client.conf /etc/shoal/`
+5. Check settings in `shoal_client.conf` update as needed
+
+
+
```

### Comparing `shoal-client-1.0.2/README.md` & `shoal-client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.2/setup.py` & `shoal-client-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `shoal-client-1.0.2/shoal-client` & `shoal-client-1.0.3/shoal-client`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from optparse import OptionParser
 from subprocess import Popen, PIPE
 from multiprocessing import Process, Queue
 import requests
 import time
 import netifaces
 import copy
+import socket
 try:
     import queue as Q
 except:
     import Queue as Q
 
 from shoal_client import config as config
 
@@ -35,18 +36,20 @@
 data = None
 server_available_private = {}
 server_available_public = {}
 server_squids = []
 frontier = False
 numsquids = 2
 dump = False
+skip_broadcast = False
 best_http_proxy = ''
 env_proxy = ''
 unicode = str
-timeout = 90
+broadcast_timeout = 90
+shoal_server_timeout = 30
 paths = config.paths
 
 def get_local_squid(q, t):
     PORT = 50000
     BROADCAST_ID = "fna349fn" #to make sure we don't confuse or get confused by other programs
 
     from socket import socket, AF_INET, SOCK_DGRAM
@@ -70,38 +73,44 @@
     """
         gets server and dump variables from command line arguments
     """
     global server
     global dump
     global frontier
     global numsquids
+    global skip_broadcast
 
     p = OptionParser()
     p.add_option("-s", "--server", action="store", type="string", dest="server",
                  help="Also needs string for specifying the shoal server to use. " +
                  "Takes precedence over the option in config file.")
     p.add_option("-d", "--dump", action="store_true", dest="dump",
                  help="Print closest proxies to terminal for debugging "+
                  "instead of executing a cvfms-talk command to update the active configuration.")
     p.add_option("-f", "--frontier", action="store_true", dest="frontier",
                  help="Outputs a string suitable for use as a frontier proxy eviroment variable" +
                  "instead of executing a cvfms-talk command to update the active configuration.")
     p.add_option("-n", "--squids", action="store", type="int", dest="numsquids",
                  help="Specifies the number of squids to retrieve" +
                  "from the shoal-server (default is 2).")
+    p.add_option("-k", "--skip-broadcast", action="store_true",  dest="skip_broadcast",
+                 help="Tells the shoal client to skip waiting for a local squid broadcast" +
+                 "signal to avoid a fruitless timeout.")
     (options, args) = p.parse_args()
 
     if options.server:
         server = options.server
     if options.dump:
         dump = True
     if options.frontier:
         frontier = True
     if options.numsquids:
         numsquids = options.numsquids
+    if options.skip_broadcast:
+        skip_broadcast = True
 
 def convertServerData(val):
     """
         converts val to digits if it's not already or else return None
     """
     if val.isdigit():
         return int(val)
@@ -309,33 +318,37 @@
     #this goes direct to avoid any bad configuration
     proxy_handler = UrlRequest.ProxyHandler({})
     opener = UrlRequest.build_opener(proxy_handler)
     if server[-1] == "/":
         server_url = server + "%s/" % (numsquids + 5)
     else:
         server_url = server + "/%s/" % (numsquids + 5)
-    f = opener.open(server_url, timeout=5)
+    f = opener.open(server_url, timeout=shoal_server_timeout)
     # data = json.loads(f.read())
     data = parseServerData(f.read())
     syslog.syslog(syslog.LOG_DEBUG, "Got data from %s" % server)
-except (UrlError, ValueError) as e:
+except (UrlError, ValueError, socket.timeout) as e:
     # This is where the client now exits if it can't reach shoal, might be worth
     # refactoring instead of injecting code here to reuse the proceeding code.
     #checkEnvVariable()
     #checkConfig()
     syslog.syslog(syslog.LOG_ERR, "Unable to reach shoal-server, reverting to defaults")
     #sys.exit(1)
+except Exception as ex:
+    syslog.syslog(syslog.LOG_ERR, "Encountered unknown exception during request to shoal-server:")
+    syslog.syslog(syslog.LOG_ERR, "%s" % ex)
+    syslog.syslog(syslog.LOG_ERR, "Continuing with defaults...")    
 
 
-if not frontier:
+if not frontier and not skip_broadcast:
     q = Queue()
-    p = Process(target=get_local_squid, args=(q,timeout))
+    p = Process(target=get_local_squid, args=(q,broadcast_timeout))
     p.start()
     try:
-       local_squid = q.get(block=True, timeout=timeout)
+       local_squid = q.get(block=True, timeout=broadcast_timeout)
     except Q.Empty:
        #continue
        #print("queue timeout !")
        pass
     p.join()
 
 # If the shoal_server was reachable
@@ -426,16 +439,26 @@
     syslog.syslog(syslog.LOG_INFO, "Setting %s as proxy" % cvmfs_http_proxy)
 
     syslog.syslog(syslog.LOG_DEBUG, "Executing 'cvmfs_talk proxy set %s'" % cvmfs_http_proxy)
     try:
         p = Popen(["cvmfs_talk", "proxy", "set", cvmfs_http_proxy], stdout=PIPE, stderr=PIPE)
         output, errors = p.communicate()
         if errors:
+            try:
+                errors = errors.decode()
+            except (UnicodeDecodeError, AttributeError):
+                pass
             syslog.syslog(syslog.LOG_ERR, errors)
         if output:
+            #in some versions output is returned as a byte string instead of a normal string
+            # this check will make sure it's an actual string before attempting to log it
+            try:
+                output = output.decode()
+            except (UnicodeDecodeError, AttributeError):
+                pass
             syslog.syslog(syslog.LOG_DEBUG, output)
         if p.returncode:
             syslog.syslog(
                 syslog.LOG_ERR,
                 "WARNING: CVMFS proxies may not have been set correctly for all repos")
             sys.exit(p.returncode)
         else:
```

### Comparing `shoal-client-1.0.2/PKG-INFO` & `shoal-client-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 Metadata-Version: 2.1
 Name: shoal-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A squid cache publishing and advertising tool designed to work in fast changing environments
 Home-page: http://github.com/hep-gc/shoal
 Author: Mike Chester, Colson Drimiel, Ian Gable, Alex Lam, Rob Prior, Ryan Taylor, Steve Traylen, Marcus Ebert, Da Meng
 Author-email: heprc-shoal@uvic.ca
 License: 'GPL3' or 'Apache 2'
-Description: # Shoal Client README
-        # Version: v1.0.1
-        
-        shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
-        and using cvmfs-talk to update the active proxy configuration.
-        
-        shoal-client is a simple python script typically configured to run with cron to check for new squids 
-        periodically. Before setting the cronjob in place make sure that shoal-client is
-        configured correctly (see Usage below).
-        
-        With the release of v0.6.4 the shoal-client now offers support for frontier. Running the shoal-client
-        with the --frontier or -f option will produce an output string instead of attempting to update the
-        proxies via cvmfs-talk. See Usage below for more information.
-        
-        
-        ## Installation
-        
-        **Note**: Requires Python 2.4+
-        
-        **Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
-        root permissions.
-        
-        ### Recommended Instalation Method: Use pip
-        
-        1. `pip install shoal-client`
-        2. Copy the configuration file to proper location
-            ```
-            # For python3
-            cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
-            
-            # For python2
-            cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
-            ````
-        3. Check settings in `shoal_client.conf` update as needed
-        
-            
-        ## Usage
-        
-        Confirm the that you configured shoal-client as expected by checking the output of `shoal-client --dump`
-        The output is a list of servers that will be set as proxies using cvmfs-talk. For example you will see 
-        something like the following:
-        
-            http://squid.example1.com:3128;http://squid.example2.com:3128;http://squid.example3.com:3128;http://squid.example4.com:3128;http://squid.example5.org:3128;DIRECT
-        
-        If the output looks resonable now set a crontab entry to run shoal say every 30 minutes:
-        
-            0,30 * * * * /usr/bin/shoal-client
-        
-        New in version 0.6.4 is the --frontier option that will produce an output string suitable for frontier.
-        Users will need to use a simple script that runs shoal-client and uses the output to set the proxies.
-        An example script can be found [here](https://github.com/hep-gc/shoal/blob/master/shoal-client/scripts/frontier_set.sh) in the shoal-client/scripts directory.
-        Example output when running `shoal-client --frontier`:
-        
-            (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
-        
-        ### Flags and Options
-        | Option | Description |
-        | --- | --- |
-        | -d or --dump | Print closest proxies to terminal for testing or debugging. |
-        | -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
-        | -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
-        | -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
-        
-        Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
-        
-             cvmfs_talk proxy info
-        
-        ## Other Installation Methods
-        
-        ### Using Pip
-        
-        1. `pip install shoal-client`
-        2. Copy the configuration file to proper location
-            ```
-            # For python3
-            cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
-            
-            # For python2
-            cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
-            ```
-        3. Check settings in `shoal_client.conf` update as needed
-        
-        ### Using Git
-        1. `git clone git://github.com/hep-gc/shoal.git`
-        2. `cd shoal/shoal-client/`
-        3. `python setup.py install`
-        4. Copy the configuration file to proper location `cp conf/shoal_client.conf /etc/shoal/`
-        5. Check settings in `shoal_client.conf` update as needed
-        
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Shoal Client README
+# Version: v1.0.1
+
+shoal-client will configure cvmfs to use the closest squid server to you by contacting the shoal server
+and using cvmfs-talk to update the active proxy configuration.
+
+shoal-client is a simple python script typically configured to run with cron to check for new squids 
+periodically. Before setting the cronjob in place make sure that shoal-client is
+configured correctly (see Usage below).
+
+With the release of v0.6.4 the shoal-client now offers support for frontier. Running the shoal-client
+with the --frontier or -f option will produce an output string instead of attempting to update the
+proxies via cvmfs-talk. See Usage below for more information.
+
+
+## Installation
+
+**Note**: Requires Python 2.4+
+
+**Note**: Shoal config files will be located either at `~/.shoal/` or `/etc/shoal/` if installed 
+root permissions.
+
+### Recommended Instalation Method: Use pip
+
+1. `pip install shoal-client`
+2. Copy the configuration file to proper location
+    ```
+    # For python3
+    cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
+    
+    # For python2
+    cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
+    ````
+3. Check settings in `shoal_client.conf` update as needed
+
+    
+## Usage
+
+Confirm the that you configured shoal-client as expected by checking the output of `shoal-client --dump`
+The output is a list of servers that will be set as proxies using cvmfs-talk. For example you will see 
+something like the following:
+
+    http://squid.example1.com:3128;http://squid.example2.com:3128;http://squid.example3.com:3128;http://squid.example4.com:3128;http://squid.example5.org:3128;DIRECT
+
+If the output looks resonable now set a crontab entry to run shoal say every 30 minutes:
+
+    0,30 * * * * /usr/bin/shoal-client
+
+New in version 0.6.4 is the --frontier option that will produce an output string suitable for frontier.
+Users will need to use a simple script that runs shoal-client and uses the output to set the proxies.
+An example script can be found [here](https://github.com/hep-gc/shoal/blob/master/shoal-client/scripts/frontier_set.sh) in the shoal-client/scripts directory.
+Example output when running `shoal-client --frontier`:
+
+    (serverurl=http://PresetServer.ca:3128)(proxyurl=http://PROXY.FROM.SHOAL.1:3128)(proxyurl=http://PROXY.FROM.SHOAL.2:3128)
+
+### Flags and Options
+| Option | Description |
+| --- | --- |
+| -d or --dump | Print closest proxies to terminal for testing or debugging. |
+| -s `hostname` or --server `hostname`| Specifies URL of the desired shoal-server to contact. Takes precedence over the option in config file. |
+| -n `int` or --squids `int` | Specifies the number of squids to retrieve from the shoal-server |
+| -f or --frontier| Outputs a string appropriate for use as the frontier proxy enviroment variable instead of using cvmfs-talk to update the active proxy configuration|
+
+Shoal client now uses the cvmfs_talk protocol. To view the list of returned squids issue:
+
+     cvmfs_talk proxy info
+
+## Other Installation Methods
+
+### Using Pip
+
+1. `pip install shoal-client`
+2. Copy the configuration file to proper location
+    ```
+    # For python3
+    cp /usr/local/share/shoal-client/shoal_client.conf /etc/shoal/
+    
+    # For python2
+    cp /usr/share/shoal-client/shoal_client.conf /etc/shoal/
+    ```
+3. Check settings in `shoal_client.conf` update as needed
+
+### Using Git
+1. `git clone git://github.com/hep-gc/shoal.git`
+2. `cd shoal/shoal-client/`
+3. `python setup.py install`
+4. Copy the configuration file to proper location `cp conf/shoal_client.conf /etc/shoal/`
+5. Check settings in `shoal_client.conf` update as needed
+
+
+
```

