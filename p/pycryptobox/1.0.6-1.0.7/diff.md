# Comparing `tmp/pycryptobox-1.0.6.tar.gz` & `tmp/pycryptobox-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycryptobox-1.0.6.tar", last modified: Mon Mar 27 11:08:37 2023, max compression
+gzip compressed data, was "dist\pycryptobox-1.0.7.tar", last modified: Fri Apr 28 06:14:49 2023, max compression
```

## Comparing `pycryptobox-1.0.6.tar` & `pycryptobox-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 11:08:37.966317 pycryptobox-1.0.6/
--rw-rw-rw-   0        0        0       54 2023-03-27 10:40:02.000000 pycryptobox-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2568 2023-03-27 11:08:37.966317 pycryptobox-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1708 2023-03-27 11:02:06.000000 pycryptobox-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 11:08:37.957051 pycryptobox-1.0.6/pycryptobox/
--rw-rw-rw-   0        0        0      157 2023-03-27 10:40:02.000000 pycryptobox-1.0.6/pycryptobox/__init__.py
--rw-rw-rw-   0        0        0       62 2023-03-27 07:28:21.000000 pycryptobox-1.0.6/pycryptobox/config.ini
--rw-rw-rw-   0        0        0     3118 2023-03-27 10:40:02.000000 pycryptobox-1.0.6/pycryptobox/decryption.py
--rw-rw-rw-   0        0        0     3143 2023-03-27 10:46:30.000000 pycryptobox-1.0.6/pycryptobox/encryption.py
-drwxrwxrwx   0        0        0        0 2023-03-27 11:08:37.965184 pycryptobox-1.0.6/pycryptobox.egg-info/
--rw-rw-rw-   0        0        0     2568 2023-03-27 11:08:37.000000 pycryptobox-1.0.6/pycryptobox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-03-27 11:08:37.000000 pycryptobox-1.0.6/pycryptobox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 11:08:37.000000 pycryptobox-1.0.6/pycryptobox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2023-03-27 11:08:37.000000 pycryptobox-1.0.6/pycryptobox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-03-27 11:08:37.000000 pycryptobox-1.0.6/pycryptobox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-27 11:08:37.000000 pycryptobox-1.0.6/pycryptobox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 11:08:37.967322 pycryptobox-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1662 2023-03-27 10:49:02.000000 pycryptobox-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 06:14:49.952376 pycryptobox-1.0.7/
+-rw-rw-rw-   0        0        0       54 2023-03-27 10:40:02.000000 pycryptobox-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2568 2023-04-28 06:14:49.948850 pycryptobox-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1708 2023-04-28 06:01:51.000000 pycryptobox-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 06:14:49.930664 pycryptobox-1.0.7/pycryptobox/
+-rw-rw-rw-   0        0        0      157 2023-04-28 06:05:47.000000 pycryptobox-1.0.7/pycryptobox/__init__.py
+-rw-rw-rw-   0        0        0       62 2023-03-27 07:28:21.000000 pycryptobox-1.0.7/pycryptobox/config.ini
+-rw-rw-rw-   0        0        0     3118 2023-03-27 11:17:07.000000 pycryptobox-1.0.7/pycryptobox/decryption.py
+-rw-rw-rw-   0        0        0     3141 2023-03-27 11:40:38.000000 pycryptobox-1.0.7/pycryptobox/encryption.py
+drwxrwxrwx   0        0        0        0 2023-04-28 06:14:49.946855 pycryptobox-1.0.7/pycryptobox.egg-info/
+-rw-rw-rw-   0        0        0     2568 2023-04-28 06:14:49.000000 pycryptobox-1.0.7/pycryptobox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-04-28 06:14:49.000000 pycryptobox-1.0.7/pycryptobox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 06:14:49.000000 pycryptobox-1.0.7/pycryptobox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2023-04-28 06:14:49.000000 pycryptobox-1.0.7/pycryptobox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-28 06:14:49.000000 pycryptobox-1.0.7/pycryptobox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-28 06:14:49.000000 pycryptobox-1.0.7/pycryptobox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 06:14:49.954370 pycryptobox-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2023-04-28 06:01:15.000000 pycryptobox-1.0.7/setup.py
```

### Comparing `pycryptobox-1.0.6/PKG-INFO` & `pycryptobox-1.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycryptobox
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for encrypting and decrypting files
 Home-page: https://github.com/LpCodes/pycryptobox
 Author: https://github.com/LpCodes
 Keywords: encryption decryption file-security cryptography
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Archiving :: Compression
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/pycryptobox.svg)](https://badge.fury.io/py/pycryptobox) [![Downloads](https://static.pepy.tech/personalized-badge/pycryptobox?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycryptobox)[![Publish Package](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml)
+[![PyPI version](https://badge.fury.io/py/pycryptobox.svg)](https://badge.fury.io/py/pycryptobox) [![Downloads](https://static.pepy.tech/personalized-badge/pycryptobox?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycryptobox)[![Publish Package](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml)
 
 # pyCryptobox
 
 pyCryptoBox is a Python package that allows you to encrypt and decrypt files and folders using the Fernet symmetric encryption algorithm.
 
 ## Installation
```

### Comparing `pycryptobox-1.0.6/README.md` & `pycryptobox-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PyPI version](https://badge.fury.io/py/pycryptobox.svg)](https://badge.fury.io/py/pycryptobox) [![Downloads](https://static.pepy.tech/personalized-badge/pycryptobox?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycryptobox)[![Publish Package](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml)
+[![PyPI version](https://badge.fury.io/py/pycryptobox.svg)](https://badge.fury.io/py/pycryptobox) [![Downloads](https://static.pepy.tech/personalized-badge/pycryptobox?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycryptobox)[![Publish Package](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml)
 
 # pyCryptobox
 
 pyCryptoBox is a Python package that allows you to encrypt and decrypt files and folders using the Fernet symmetric encryption algorithm.
 
 ## Installation
```

### Comparing `pycryptobox-1.0.6/pycryptobox/decryption.py` & `pycryptobox-1.0.7/pycryptobox/decryption.py`

 * *Files identical despite different names*

### Comparing `pycryptobox-1.0.6/pycryptobox/encryption.py` & `pycryptobox-1.0.7/pycryptobox/encryption.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,7 @@
     with open(file_path + '.enc', 'wb') as f:
         f.write(encrypted_contents)
 
     # Remove the original unencrypted file
     os.remove(file_path)
 
     print(f"{file_path} ssuccessfully encrypted")
-
```

### Comparing `pycryptobox-1.0.6/pycryptobox.egg-info/PKG-INFO` & `pycryptobox-1.0.7/pycryptobox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycryptobox
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for encrypting and decrypting files
 Home-page: https://github.com/LpCodes/pycryptobox
 Author: https://github.com/LpCodes
 Keywords: encryption decryption file-security cryptography
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Archiving :: Compression
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/pycryptobox.svg)](https://badge.fury.io/py/pycryptobox) [![Downloads](https://static.pepy.tech/personalized-badge/pycryptobox?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycryptobox)[![Publish Package](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml)
+[![PyPI version](https://badge.fury.io/py/pycryptobox.svg)](https://badge.fury.io/py/pycryptobox) [![Downloads](https://static.pepy.tech/personalized-badge/pycryptobox?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycryptobox)[![Publish Package](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LpCodes/pycryptobox/actions/workflows/python-publish.yml)
 
 # pyCryptobox
 
 pyCryptoBox is a Python package that allows you to encrypt and decrypt files and folders using the Fernet symmetric encryption algorithm.
 
 ## Installation
```

### Comparing `pycryptobox-1.0.6/setup.py` & `pycryptobox-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages, Extension
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pycryptobox",
-    version="1.0.6",
+    version="1.0.7",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "encode-encrypt-dir = pycryptobox.encryption:encrypt_dir",
             "encrypt-file = pycryptobox.encryption:encrpt_file",
             "decode-decrypt-dir = pycryptobox.decryption:decrypt_dir",
             "decrypt-file = pycryptobox.decryption:decrypt_file",
```

