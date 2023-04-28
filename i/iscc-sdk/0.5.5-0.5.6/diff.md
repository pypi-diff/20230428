# Comparing `tmp/iscc_sdk-0.5.5.tar.gz` & `tmp/iscc_sdk-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscc_sdk-0.5.5.tar", max compression
+gzip compressed data, was "iscc_sdk-0.5.6.tar", max compression
```

## Comparing `iscc_sdk-0.5.5.tar` & `iscc_sdk-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      866 2023-03-26 12:52:17.536881 iscc_sdk-0.5.5/iscc_sdk/__init__.py
--rw-r--r--   0        0        0     3859 2023-03-26 12:52:17.530881 iscc_sdk-0.5.5/iscc_sdk/audio.py
--rw-r--r--   0        0        0       99 2023-03-26 12:52:17.531881 iscc_sdk-0.5.5/iscc_sdk/compat.py
--rw-r--r--   0        0        0      897 2023-03-26 12:52:17.531881 iscc_sdk-0.5.5/iscc_sdk/docx_.py
--rw-r--r--   0        0        0     1491 2023-03-26 12:52:17.531881 iscc_sdk-0.5.5/iscc_sdk/epub.py
--rw-r--r--   0        0        0      166 2023-03-26 12:52:17.532882 iscc_sdk-0.5.5/iscc_sdk/exceptions.py
--rw-r--r--   0        0        0     8091 2023-03-26 12:52:17.532882 iscc_sdk-0.5.5/iscc_sdk/image.py
--rw-r--r--   0        0        0      683 2023-03-26 12:52:17.532882 iscc_sdk-0.5.5/iscc_sdk/install.py
--rw-r--r--   0        0        0     1274 2023-03-26 12:52:17.533881 iscc_sdk-0.5.5/iscc_sdk/ipfs.py
--rw-r--r--   0        0        0     6772 2023-03-26 12:52:17.533881 iscc_sdk-0.5.5/iscc_sdk/main.py
--rw-r--r--   0        0        0     9258 2023-03-26 12:52:17.533881 iscc_sdk-0.5.5/iscc_sdk/mediatype.py
--rw-r--r--   0        0        0     1898 2023-03-26 12:52:17.534881 iscc_sdk-0.5.5/iscc_sdk/metadata.py
--rw-r--r--   0        0        0     1905 2023-03-26 12:52:17.534881 iscc_sdk-0.5.5/iscc_sdk/monkeys.py
--rw-r--r--   0        0        0     3021 2023-03-26 12:52:17.534881 iscc_sdk-0.5.5/iscc_sdk/mp7.py
--rw-r--r--   0        0        0     2720 2023-03-26 12:52:17.534881 iscc_sdk-0.5.5/iscc_sdk/options.py
--rw-r--r--   0        0        0     2502 2023-03-26 12:52:17.535881 iscc_sdk-0.5.5/iscc_sdk/pdf.py
--rw-r--r--   0        0        0     5761 2023-03-26 12:52:17.535881 iscc_sdk-0.5.5/iscc_sdk/text.py
--rw-r--r--   0        0        0      684 2023-03-26 12:52:17.535881 iscc_sdk-0.5.5/iscc_sdk/thumbnail.py
--rw-r--r--   0        0        0    20755 2023-03-26 12:52:17.536881 iscc_sdk-0.5.5/iscc_sdk/tools.py
--rw-r--r--   0        0        0     5802 2023-03-26 12:52:17.536881 iscc_sdk-0.5.5/iscc_sdk/video.py
--rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.5/LICENSE
--rw-r--r--   0        0        0     3266 2023-03-26 12:52:17.475354 iscc_sdk-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3243 2023-03-26 12:52:17.475354 iscc_sdk-0.5.5/README.md
--rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 iscc_sdk-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      866 2023-04-28 18:57:50.903193 iscc_sdk-0.5.6/iscc_sdk/__init__.py
+-rw-r--r--   0        0        0     3859 2023-04-28 18:56:24.488929 iscc_sdk-0.5.6/iscc_sdk/audio.py
+-rw-r--r--   0        0        0       99 2023-04-28 18:56:24.488929 iscc_sdk-0.5.6/iscc_sdk/compat.py
+-rw-r--r--   0        0        0      897 2023-04-28 18:56:24.489929 iscc_sdk-0.5.6/iscc_sdk/docx_.py
+-rw-r--r--   0        0        0     1491 2023-04-28 18:56:24.489929 iscc_sdk-0.5.6/iscc_sdk/epub.py
+-rw-r--r--   0        0        0      166 2023-04-28 18:56:24.489929 iscc_sdk-0.5.6/iscc_sdk/exceptions.py
+-rw-r--r--   0        0        0     8091 2023-04-28 18:56:24.490929 iscc_sdk-0.5.6/iscc_sdk/image.py
+-rw-r--r--   0        0        0      683 2023-04-28 18:56:24.490929 iscc_sdk-0.5.6/iscc_sdk/install.py
+-rw-r--r--   0        0        0     1274 2023-04-28 18:56:24.490929 iscc_sdk-0.5.6/iscc_sdk/ipfs.py
+-rw-r--r--   0        0        0     6772 2023-04-28 18:56:24.491929 iscc_sdk-0.5.6/iscc_sdk/main.py
+-rw-r--r--   0        0        0     9258 2023-04-28 18:56:24.491929 iscc_sdk-0.5.6/iscc_sdk/mediatype.py
+-rw-r--r--   0        0        0     1898 2023-04-28 18:56:24.491929 iscc_sdk-0.5.6/iscc_sdk/metadata.py
+-rw-r--r--   0        0        0     1905 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/monkeys.py
+-rw-r--r--   0        0        0     3021 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/mp7.py
+-rw-r--r--   0        0        0     2720 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/options.py
+-rw-r--r--   0        0        0     2502 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/pdf.py
+-rw-r--r--   0        0        0     5761 2023-04-28 18:56:24.493929 iscc_sdk-0.5.6/iscc_sdk/text.py
+-rw-r--r--   0        0        0      684 2023-04-28 18:56:24.493929 iscc_sdk-0.5.6/iscc_sdk/thumbnail.py
+-rw-r--r--   0        0        0    21133 2023-04-28 18:57:50.904193 iscc_sdk-0.5.6/iscc_sdk/tools.py
+-rw-r--r--   0        0        0     5802 2023-04-28 18:56:24.494930 iscc_sdk-0.5.6/iscc_sdk/video.py
+-rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3259 2023-04-28 18:57:50.906193 iscc_sdk-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3392 2023-04-28 18:57:50.902194 iscc_sdk-0.5.6/README.md
+-rw-r--r--   0        0        0     6025 1970-01-01 00:00:00.000000 iscc_sdk-0.5.6/PKG-INFO
```

### Comparing `iscc_sdk-0.5.5/iscc_sdk/__init__.py` & `iscc_sdk-0.5.6/iscc_sdk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ISCC - Software Development Kit."""
 import os
 from platformdirs import PlatformDirs
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 APP_NAME = "iscc-sdk"
 APP_AUTHOR = "iscc"
 dirs = PlatformDirs(appname=APP_NAME, appauthor=APP_AUTHOR)
 os.makedirs(dirs.user_data_dir, exist_ok=True)
 os.environ["LOGURU_AUTOINIT"] = "False"
```

### Comparing `iscc_sdk-0.5.5/iscc_sdk/audio.py` & `iscc_sdk-0.5.6/iscc_sdk/audio.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/docx_.py` & `iscc_sdk-0.5.6/iscc_sdk/docx_.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/epub.py` & `iscc_sdk-0.5.6/iscc_sdk/epub.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/image.py` & `iscc_sdk-0.5.6/iscc_sdk/image.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/install.py` & `iscc_sdk-0.5.6/iscc_sdk/install.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/ipfs.py` & `iscc_sdk-0.5.6/iscc_sdk/ipfs.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/main.py` & `iscc_sdk-0.5.6/iscc_sdk/main.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/mediatype.py` & `iscc_sdk-0.5.6/iscc_sdk/mediatype.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/metadata.py` & `iscc_sdk-0.5.6/iscc_sdk/metadata.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/monkeys.py` & `iscc_sdk-0.5.6/iscc_sdk/monkeys.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/mp7.py` & `iscc_sdk-0.5.6/iscc_sdk/mp7.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/options.py` & `iscc_sdk-0.5.6/iscc_sdk/options.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/pdf.py` & `iscc_sdk-0.5.6/iscc_sdk/pdf.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/text.py` & `iscc_sdk-0.5.6/iscc_sdk/text.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/thumbnail.py` & `iscc_sdk-0.5.6/iscc_sdk/thumbnail.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/iscc_sdk/tools.py` & `iscc_sdk-0.5.6/iscc_sdk/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     "linux-64": "190977d9419daed8a555240b9c6ddf6a12940c5ff470647095ee6242e217de5c",
     "darwin-64": "afea164b0bc9b91e5205d126f96a21836a91ea2d24200e1b7612a7304ea3b4f1",
 }
 
 TIKA_VERSION = "2.6.0"
 TIKA_URL = f"{BASE_URL}/tika-app-{TIKA_VERSION}.jar"
 TIKA_CHECKSUM = "4e91e89461a67c6a28c401ab131288979e76d3edca7bbb0b2f4844dd3539358e"
+TIKA_INSTALL_ATTEMPTS = 0
 
 EXIV2_VERSION = "0.27.2"
 EXIV2_URLS = {
     "windows-64": f"{BASE_URL}/exiv2-{EXIV2_VERSION}-2017msvc64.zip",
     "linux-64": f"{BASE_URL}/exiv2-{EXIV2_VERSION}-Linux64.tar.gz",
     "darwin-64": f"{BASE_URL}/exiv2-{EXIV2_VERSION}-Darwin.tar.gz",
 }
@@ -535,19 +536,26 @@
     # Ensure JAVA is installed
     java_install()
 
     if tika_is_installed():
         log.debug("Tika is already installed")
         return tika_bin()
     else:
-        log.critical("installing tika")
-        path = tika_download()
-        st = os.stat(tika_bin())
-        os.chmod(tika_bin(), st.st_mode | stat.S_IEXEC)
-        return path
+        global TIKA_INSTALL_ATTEMPTS
+        if TIKA_INSTALL_ATTEMPTS == 0:
+            log.critical("Installing Tika")
+            path = tika_download()
+            st = os.stat(tika_bin())
+            os.chmod(tika_bin(), st.st_mode | stat.S_IEXEC)
+            TIKA_INSTALL_ATTEMPTS += 1
+            return path
+        else:
+            log.critical("Allready installed tika in this session not attemting a second time!")
+            log.critical("Check your environment (internet access / java setup)")
+            sys.exit(1)
 
 
 def tika_version_info():  # pragma: no cover
     # type: () -> str
     """
     Check tika-app version.
```

### Comparing `iscc_sdk-0.5.5/iscc_sdk/video.py` & `iscc_sdk-0.5.6/iscc_sdk/video.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/LICENSE` & `iscc_sdk-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.5/pyproject.toml` & `iscc_sdk-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscc-sdk"
-version = "0.5.5"
+version = "0.5.6"
 description = "SDK for creating ISCCs (International Standard Content Codes)"
 authors = ["Titusz <tp@py7.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://sdk.iscc.codes"
 repository = "https://github.com/iscc/iscc-sdk"
 keywords=["iscc", "identifier", "media", "content", "hash", "blockchain", "similarity"]
@@ -84,9 +84,9 @@
 format-md = { cmd = "mdformat --wrap 100 README.md", help = "Markdown formating with mdformat" }
 lf = { cmd = "poetry run python -m devtools.lf", help = "Convert line endings to lf"}
 test = { cmd = "poetry run pytest --cov=iscc_sdk --cov-fail-under=100", help = "Run tests with coverage" }
 sec = { cmd = "poetry run bandit -r iscc_sdk -q", help = "Security check with bandit" }
 all = ["format-md", "docs", "lf", "black", "test"]
 
 [build-system]
-requires = ["poetry>=1.4.0", "Cython"]
+requires = ["poetry", "Cython"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iscc_sdk-0.5.5/README.md` & `iscc_sdk-0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,31 @@
 
 Use the Python package manager [pip](https://pip.pypa.io/en/stable/) to install `iscc-sdk`.
 
 ```bash
 pip install iscc-sdk
 ```
 
+## Getting Started
+
+Create an ISCC-CODE for a media file:
+
+```python
+import iscc_sdk as idk
+
+print(idk.code_iscc("/path/to/mediafile.jpg"))
+```
+
 ## Documentation
 
 <https://sdk.iscc.codes>
 
 ## Troubleshooting
 
-On Linux and MacOS might need to install taglib as a prerequisite. On Ubuntu, Mint and other
+On Linux and MacOS you might need to install taglib as a prerequisite. On Ubuntu, Mint and other
 Debian-Based distributions do:
 
 ```shell
 sudo apt install libtag1-dev
 ```
 
 On a Mac, use HomeBrew:
```

### Comparing `iscc_sdk-0.5.5/PKG-INFO` & `iscc_sdk-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iscc-sdk
-Version: 0.5.5
+Version: 0.5.6
 Summary: SDK for creating ISCCs (International Standard Content Codes)
 Home-page: https://sdk.iscc.codes
 License: Apache-2.0
 Keywords: iscc,identifier,media,content,hash,blockchain,similarity
 Author: Titusz
 Author-email: tp@py7.de
 Requires-Python: >=3.8,<4.0
@@ -99,21 +99,31 @@
 
 Use the Python package manager [pip](https://pip.pypa.io/en/stable/) to install `iscc-sdk`.
 
 ```bash
 pip install iscc-sdk
 ```
 
+## Getting Started
+
+Create an ISCC-CODE for a media file:
+
+```python
+import iscc_sdk as idk
+
+print(idk.code_iscc("/path/to/mediafile.jpg"))
+```
+
 ## Documentation
 
 <https://sdk.iscc.codes>
 
 ## Troubleshooting
 
-On Linux and MacOS might need to install taglib as a prerequisite. On Ubuntu, Mint and other
+On Linux and MacOS you might need to install taglib as a prerequisite. On Ubuntu, Mint and other
 Debian-Based distributions do:
 
 ```shell
 sudo apt install libtag1-dev
 ```
 
 On a Mac, use HomeBrew:
```

