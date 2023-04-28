# Comparing `tmp/popcornnotify-0.1.4.tar.gz` & `tmp/popcornnotify-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/popcornnotify-0.1.4.tar", last modified: Wed Dec 20 23:02:06 2017, max compression
+gzip compressed data, was "popcornnotify-0.2.1.tar", last modified: Fri Apr 28 18:14:58 2023, max compression
```

## Comparing `popcornnotify-0.1.4.tar` & `popcornnotify-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/
--rw-r--r--   0 jstrauss   (501) staff       (20)     1309 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/PKG-INFO
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify/
--rw-r--r--   0 jstrauss   (501) staff       (20)       87 2017-12-20 23:01:49.000000 popcornnotify-0.1.4/popcornnotify/__init__.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     2151 2017-12-20 20:43:33.000000 popcornnotify-0.1.4/popcornnotify/notify.py
--rw-r--r--   0 jstrauss   (501) staff       (20)     1460 2017-12-20 20:44:50.000000 popcornnotify-0.1.4/popcornnotify/notify_cli.py
-drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/
--rw-r--r--   0 jstrauss   (501) staff       (20)     1309 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/PKG-INFO
--rw-r--r--   0 jstrauss   (501) staff       (20)      353 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/SOURCES.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)       57 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/entry_points.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)       47 2017-12-20 21:16:07.000000 popcornnotify-0.1.4/popcornnotify.egg-info/pbr.json
--rw-r--r--   0 jstrauss   (501) staff       (20)        9 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/requires.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)       14 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/top_level.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)        1 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/popcornnotify.egg-info/dependency_links.txt
--rw-r--r--   0 jstrauss   (501) staff       (20)     1055 2017-12-20 23:01:49.000000 popcornnotify-0.1.4/setup.py
--rw-r--r--   0 jstrauss   (501) staff       (20)       59 2017-12-20 23:02:06.000000 popcornnotify-0.1.4/setup.cfg
--rw-r--r--   0 jstrauss   (501) staff       (20)      566 2017-10-11 19:35:31.000000 popcornnotify-0.1.4/README.rst
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2023-04-28 18:14:58.474026 popcornnotify-0.2.1/
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1264 2023-04-28 18:14:58.473541 popcornnotify-0.2.1/PKG-INFO
+-rw-r--r--   0 jstrauss   (501) staff       (20)      498 2022-12-26 02:28:49.000000 popcornnotify-0.2.1/README.md
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2023-04-28 18:14:58.465304 popcornnotify-0.2.1/popcornnotify/
+-rw-r--r--   0 jstrauss   (501) staff       (20)      115 2023-04-28 18:14:50.000000 popcornnotify-0.2.1/popcornnotify/__init__.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1965 2022-12-26 02:25:36.000000 popcornnotify-0.2.1/popcornnotify/notify.py
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1468 2022-12-26 20:59:07.000000 popcornnotify-0.2.1/popcornnotify/notify_cli.py
+drwxr-xr-x   0 jstrauss   (501) staff       (20)        0 2023-04-28 18:14:58.473000 popcornnotify-0.2.1/popcornnotify.egg-info/
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1264 2023-04-28 18:14:58.000000 popcornnotify-0.2.1/popcornnotify.egg-info/PKG-INFO
+-rw-r--r--   0 jstrauss   (501) staff       (20)      352 2023-04-28 18:14:58.000000 popcornnotify-0.2.1/popcornnotify.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)        1 2023-04-28 18:14:58.000000 popcornnotify-0.2.1/popcornnotify.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)       56 2023-04-28 18:14:58.000000 popcornnotify-0.2.1/popcornnotify.egg-info/entry_points.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)       47 2017-12-20 21:16:07.000000 popcornnotify-0.2.1/popcornnotify.egg-info/pbr.json
+-rw-r--r--   0 jstrauss   (501) staff       (20)        9 2023-04-28 18:14:58.000000 popcornnotify-0.2.1/popcornnotify.egg-info/requires.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)       14 2023-04-28 18:14:58.000000 popcornnotify-0.2.1/popcornnotify.egg-info/top_level.txt
+-rw-r--r--   0 jstrauss   (501) staff       (20)       38 2023-04-28 18:14:58.474221 popcornnotify-0.2.1/setup.cfg
+-rw-r--r--   0 jstrauss   (501) staff       (20)     1260 2023-04-28 18:14:45.000000 popcornnotify-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `popcornnotify-0.1.4/PKG-INFO` & `popcornnotify-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: popcornnotify
-Version: 0.1.4
+Version: 0.2.1
 Summary: Send simple emails and text messages from one API
 Home-page: https://popcornnotify.com
-Author: Abe
-Author-email: abe@popcornnotify.com
+Author: Jason Strauss
+Author-email: jason@popcornnotify.com
 License: MIT
-Description: The Popcorn Notify Python Client
-        ================================
-        
-        This the  Python client library for `Popcorn Notify <https://www.PopcornNotify.com>`_.
-        Popcorn Notify is a simple non-blocking API to send emails or text messages 
-        from within your code.
-        
-        ---
-        
-        ::
-        
-            from popcornnotify import notify
-        
-            notify('contact@popcornnotify.com', 'A new user signed up!', subject="Server Message")
-        
-            notify('5555555555', 'Long script has finished running.')
-        
-            notify(['contact@popcornnotify.com','support@popcornnotify.com','5555555555'], 'The server is on fire.')
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Telephony
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+
+# The Popcorn Notify Python Client
+
+This the  Python client library for [Popcorn Notify](https://www.PopcornNotify.com>).
+Popcorn Notify is a simple non-blocking API to send emails or text messages.
+
+```python
+from popcornnotify import notify
+
+notify('5555555555', 'Long script has finished running.')
+notify('contact@popcornnotify.com', 'A new user signed up!', subject="Server Message")
+notify(['contact@popcornnotify.com','support@popcornnotify.com','5555555555'], 'The server is on fire.')
+```
```

### Comparing `popcornnotify-0.1.4/popcornnotify/notify.py` & `popcornnotify-0.2.1/popcornnotify/notify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 PopcornNotify Python Client
 
-An API for sending simple emails and text messages from your code
+An API for sending simple emails and text messages from your code.
 """
 
 import os
 import requests
 import threading
 
 
 def notify(recipients=None, message=None, subject=None, api_key=None, verbose=False):
     try:
         notify_thread = threading.Thread(target=nonblocked_notify, args=(recipients, message, subject, api_key, verbose))
         notify_thread.start()
 
     except:
-        # print "There was an issue with Popcorn Notify"
+        # print("There was an issue with Popcorn Notify")
         pass
 
 
 def nonblocked_notify(recipients=None, message=None, subject=None, api_key=None, verbose=False):
     if not api_key:
         api_key = os.environ['POPCORNNOTIFY_API_KEY']
 
@@ -40,15 +40,15 @@
         self.message = message
         self.subject = subject
         self.verbose = verbose
 
         is_debug = os.environ.get('POPCORNNOTIFY_SEND', 'true').lower()
         if is_debug in ['f', 'false', '0']:
             if self.verbose:
-                print "Not sending Popcorn Notify. $POPCORNNOTIFY_SEND is set to false."
+                print("Not sending Popcorn Notify. $POPCORNNOTIFY_SEND is set to false.")
             return
 
         self.post_to_server()
 
     def post_to_server(self):
         popcorn_notify_params = {
             'api_key': self.api_key,
@@ -59,15 +59,12 @@
             # 'version': notify.VERSION
         }
 
         url = 'https://popcornnotify.com/notify'
         r = requests.post(url, json=popcorn_notify_params)
         if r.status_code == 200:
             if self.verbose:
-                print "Sent"
+                print("Sent")
             pass
         else:
             if self.verbose:
-                print r.text
-            pass
-            # print "Popcorn Notify: There was an issue connecting to the Popcorn Notify Server"
-            # print r.content  # this should be a good job or maybe an error
+                print(r.text)
```

### Comparing `popcornnotify-0.1.4/popcornnotify/notify_cli.py` & `popcornnotify-0.2.1/popcornnotify/notify_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import argparse
 import sys
-from notify import notify
+from popcornnotify.notify import notify
 
 def cli(*args, **kwargs):
     example_text = '''examples:
-	
+
 	notify 5555555555 "Hello World"
 
 	echo "Hello World" | notify 5555555555,team@popcornnotify.com -s "An Informative Subject Line"
 
 	./script.sh && echo "Script done at $(date)" | notify 555...,team@popcornnotify.com
 	'''
 
     parser = argparse.ArgumentParser(
 		prog='notify',
-		description='Send simple emails and text messages from one API', 
+		description='Send simple emails and text messages from one API',
 		epilog=example_text,
 		formatter_class=argparse.RawDescriptionHelpFormatter)
 
     # parser = argparse.ArgumentParser()
     parser.add_argument('recipients', help='Phone numbers or emails to notify, comma separated')
     parser.add_argument('message', help='Message to send', nargs='?')
     parser.add_argument('-s', '--subject', help='Email subject line')
@@ -33,9 +33,9 @@
         p_message = sys.stdin.read()
     else:
         parser.error("too few arguments")
 
     verbose = True
     if args.quiet:
         verbose = False
-    
+
     notify(recipients=args.recipients, message=p_message, subject=args.subject, api_key=args.api_key, verbose=verbose)
```

### Comparing `popcornnotify-0.1.4/popcornnotify.egg-info/PKG-INFO` & `popcornnotify-0.2.1/popcornnotify.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: popcornnotify
-Version: 0.1.4
+Version: 0.2.1
 Summary: Send simple emails and text messages from one API
 Home-page: https://popcornnotify.com
-Author: Abe
-Author-email: abe@popcornnotify.com
+Author: Jason Strauss
+Author-email: jason@popcornnotify.com
 License: MIT
-Description: The Popcorn Notify Python Client
-        ================================
-        
-        This the  Python client library for `Popcorn Notify <https://www.PopcornNotify.com>`_.
-        Popcorn Notify is a simple non-blocking API to send emails or text messages 
-        from within your code.
-        
-        ---
-        
-        ::
-        
-            from popcornnotify import notify
-        
-            notify('contact@popcornnotify.com', 'A new user signed up!', subject="Server Message")
-        
-            notify('5555555555', 'Long script has finished running.')
-        
-            notify(['contact@popcornnotify.com','support@popcornnotify.com','5555555555'], 'The server is on fire.')
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Telephony
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+
+# The Popcorn Notify Python Client
+
+This the  Python client library for [Popcorn Notify](https://www.PopcornNotify.com>).
+Popcorn Notify is a simple non-blocking API to send emails or text messages.
+
+```python
+from popcornnotify import notify
+
+notify('5555555555', 'Long script has finished running.')
+notify('contact@popcornnotify.com', 'A new user signed up!', subject="Server Message")
+notify(['contact@popcornnotify.com','support@popcornnotify.com','5555555555'], 'The server is on fire.')
+```
```

### Comparing `popcornnotify-0.1.4/setup.py` & `popcornnotify-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
-with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='popcornnotify',
-    version='0.1.4',
+    version='0.2.1',
     description='Send simple emails and text messages from one API',
     long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://popcornnotify.com',
-    author='Abe',
-    author_email='abe@popcornnotify.com',
+    author='Jason Strauss',
+    author_email='jason@popcornnotify.com',
     license='MIT',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
 
         'Intended Audience :: Developers',
+        'Intended Audience :: System Administrators',
 
+        'Topic :: Communications :: Chat',
         'Topic :: Communications :: Email',
         'Topic :: Communications :: Telephony',
         'Topic :: Software Development :: Libraries :: Python Modules',
 
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
     ],
     packages=['popcornnotify', ],
     install_requires=['requests'],
     entry_points={
         'console_scripts':[
             'notify = popcornnotify.notify_cli:cli',
         ]
```

