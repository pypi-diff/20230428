# Comparing `tmp/kidronekit-1.0.0.tar.gz` & `tmp/kidronekit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kidronekit-1.0.0.tar", last modified: Tue Apr 25 07:17:45 2023, max compression
+gzip compressed data, was "kidronekit-1.0.1.tar", last modified: Fri Apr 28 07:58:51 2023, max compression
```

## Comparing `kidronekit-1.0.0.tar` & `kidronekit-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rtr       (1000) rtr       (1000)        0 2023-04-25 07:17:45.777349 kidronekit-1.0.0/
--rw-rw-r--   0 rtr       (1000) rtr       (1000)    11357 2023-04-25 06:07:49.000000 kidronekit-1.0.0/LICENSE
--rw-rw-r--   0 rtr       (1000) rtr       (1000)     2805 2023-04-25 07:17:45.777349 kidronekit-1.0.0/PKG-INFO
--rw-rw-r--   0 rtr       (1000) rtr       (1000)     2113 2023-04-25 07:08:53.000000 kidronekit-1.0.0/README.md
-drwxrwxr-x   0 rtr       (1000) rtr       (1000)        0 2023-04-25 07:17:45.777349 kidronekit-1.0.0/kidronekit/
--rw-rw-r--   0 rtr       (1000) rtr       (1000)   126698 2023-04-25 07:04:23.000000 kidronekit-1.0.0/kidronekit/__init__.py
--rw-rw-r--   0 rtr       (1000) rtr       (1000)       51 2023-04-25 06:31:33.000000 kidronekit-1.0.0/kidronekit/lib.py
--rw-rw-r--   0 rtr       (1000) rtr       (1000)    11976 2023-04-25 06:31:30.000000 kidronekit-1.0.0/kidronekit/mavlink.py
--rw-rw-r--   0 rtr       (1000) rtr       (1000)      522 2022-06-15 22:33:02.000000 kidronekit-1.0.0/kidronekit/util.py
-drwxrwxr-x   0 rtr       (1000) rtr       (1000)        0 2023-04-25 07:17:45.777349 kidronekit-1.0.0/kidronekit.egg-info/
--rw-rw-r--   0 rtr       (1000) rtr       (1000)     2805 2023-04-25 07:17:45.000000 kidronekit-1.0.0/kidronekit.egg-info/PKG-INFO
--rw-rw-r--   0 rtr       (1000) rtr       (1000)      306 2023-04-25 07:17:45.000000 kidronekit-1.0.0/kidronekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rtr       (1000) rtr       (1000)        1 2023-04-25 07:17:45.000000 kidronekit-1.0.0/kidronekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rtr       (1000) rtr       (1000)       33 2023-04-25 07:17:45.000000 kidronekit-1.0.0/kidronekit.egg-info/requires.txt
--rw-rw-r--   0 rtr       (1000) rtr       (1000)       11 2023-04-25 07:17:45.000000 kidronekit-1.0.0/kidronekit.egg-info/top_level.txt
--rw-rw-r--   0 rtr       (1000) rtr       (1000)        1 2023-04-25 07:17:45.000000 kidronekit-1.0.0/kidronekit.egg-info/zip-safe
--rw-rw-r--   0 rtr       (1000) rtr       (1000)       38 2023-04-25 07:17:45.777349 kidronekit-1.0.0/setup.cfg
--rw-rw-r--   0 rtr       (1000) rtr       (1000)     1067 2023-04-25 06:34:52.000000 kidronekit-1.0.0/setup.py
+drwxrwxr-x   0 rtr       (1000) rtr       (1000)        0 2023-04-28 07:58:51.711997 kidronekit-1.0.1/
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)    11357 2023-04-25 06:07:49.000000 kidronekit-1.0.1/LICENSE
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)     2805 2023-04-28 07:58:51.711997 kidronekit-1.0.1/PKG-INFO
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)     2113 2023-04-25 07:08:53.000000 kidronekit-1.0.1/README.md
+drwxrwxr-x   0 rtr       (1000) rtr       (1000)        0 2023-04-28 07:58:51.707997 kidronekit-1.0.1/kidronekit/
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)   126990 2023-04-25 10:15:59.000000 kidronekit-1.0.1/kidronekit/__init__.py
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)       51 2023-04-25 06:31:33.000000 kidronekit-1.0.1/kidronekit/lib.py
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)    11976 2023-04-25 06:31:30.000000 kidronekit-1.0.1/kidronekit/mavlink.py
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)      522 2022-06-15 22:33:02.000000 kidronekit-1.0.1/kidronekit/util.py
+drwxrwxr-x   0 rtr       (1000) rtr       (1000)        0 2023-04-28 07:58:51.707997 kidronekit-1.0.1/kidronekit.egg-info/
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)     2805 2023-04-28 07:58:51.000000 kidronekit-1.0.1/kidronekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)      306 2023-04-28 07:58:51.000000 kidronekit-1.0.1/kidronekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)        1 2023-04-28 07:58:51.000000 kidronekit-1.0.1/kidronekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)       33 2023-04-28 07:58:51.000000 kidronekit-1.0.1/kidronekit.egg-info/requires.txt
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)       11 2023-04-28 07:58:51.000000 kidronekit-1.0.1/kidronekit.egg-info/top_level.txt
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)        1 2023-04-28 07:58:51.000000 kidronekit-1.0.1/kidronekit.egg-info/zip-safe
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)       38 2023-04-28 07:58:51.711997 kidronekit-1.0.1/setup.cfg
+-rw-rw-r--   0 rtr       (1000) rtr       (1000)     1067 2023-04-28 07:58:50.000000 kidronekit-1.0.1/setup.py
```

### Comparing `kidronekit-1.0.0/LICENSE` & `kidronekit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kidronekit-1.0.0/PKG-INFO` & `kidronekit-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidronekit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Premium extended version of dronekit.
 Home-page: https://github.com/kirinslab/kidronekit.git
 Author: 3D Robotics, Kirinlab
 Author-email: tim@3drobotics.com, kevinh@geeksville.com, haiquantran2897@gmail.com
 License: apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `kidronekit-1.0.0/README.md` & `kidronekit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kidronekit-1.0.0/kidronekit/__init__.py` & `kidronekit-1.0.1/kidronekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,20 @@
         """
 
         if self.north is not None and self.east is not None:
             if self.down is not None:
                 return math.sqrt(self.north**2 + self.east**2 + self.down**2)
             else:
                 return math.sqrt(self.north**2 + self.east**2)
+    
+    def distance_traveled(self):
+        """
+        Distance traveled, in meters.
+        """
+        pass
 
 
 class GPSInfo(object):
     """
     Standard information about GPS.
 
     If there is no GPS lock the parameters are set to ``None``.
@@ -2073,14 +2079,22 @@
 
         self.armed = True
 
         if wait:
             self.wait_for(lambda: self.armed, timeout=timeout,
                           errmsg='failed to arm vehicle')
 
+    def counter(self):
+        '''Return the time counter value.'''
+        pass
+
+    def time_in_air(self):
+        '''Return true if the vehicle is in air. (s)'''
+        pass
+
     def disarm(self, wait=True, timeout=None):
         '''Disarm the vehicle.
 
         If wait is True, wait for disarm operation to complete before
         returning.  If timeout is nonzero, raise a TimeouTerror if the
         vehicle has not disarmed after timeout seconds.
         '''
```

### Comparing `kidronekit-1.0.0/kidronekit/mavlink.py` & `kidronekit-1.0.1/kidronekit/mavlink.py`

 * *Files identical despite different names*

### Comparing `kidronekit-1.0.0/kidronekit/util.py` & `kidronekit-1.0.1/kidronekit/util.py`

 * *Files identical despite different names*

### Comparing `kidronekit-1.0.0/kidronekit.egg-info/PKG-INFO` & `kidronekit-1.0.1/kidronekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidronekit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Premium extended version of dronekit.
 Home-page: https://github.com/kirinslab/kidronekit.git
 Author: 3D Robotics, Kirinlab
 Author-email: tim@3drobotics.com, kevinh@geeksville.com, haiquantran2897@gmail.com
 License: apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `kidronekit-1.0.0/setup.py` & `kidronekit-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 import os
 
-version = '1.0.0'
+version = '1.0.1'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     LongDescription = f.read()
 
 setuptools.setup(
     name='kidronekit',
     zip_safe=True,
```

