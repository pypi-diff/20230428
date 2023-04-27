# Comparing `tmp/perpetuo-0.3.0.tar.gz` & `tmp/perpetuo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perpetuo-0.3.0.tar", last modified: Thu Apr 27 06:53:13 2023, max compression
+gzip compressed data, was "perpetuo-0.3.1.tar", last modified: Thu Apr 27 23:32:59 2023, max compression
```

## Comparing `perpetuo-0.3.0.tar` & `perpetuo-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    50192 2023-04-27 06:53:04.000000 perpetuo-0.3.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 06:53:04.000000 perpetuo-0.3.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 06:53:04.000000 perpetuo-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 06:53:04.000000 perpetuo-0.3.0/LICENSE.APACHE2
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 06:53:04.000000 perpetuo-0.3.0/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 06:53:04.000000 perpetuo-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 06:53:13.948888 perpetuo-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-27 06:53:04.000000 perpetuo-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 06:53:04.000000 perpetuo-0.3.0/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-27 06:53:04.000000 perpetuo-0.3.0/prep-manylinux-container.sh
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 06:53:04.000000 perpetuo-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.944888 perpetuo-0.3.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/python/perpetuo/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_perpetuo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/python/perpetuo/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/_tests/test_perpetuo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:04.000000 perpetuo-0.3.0/python/perpetuo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/python/perpetuo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 06:53:13.000000 perpetuo-0.3.0/python/perpetuo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:53:13.948888 perpetuo-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-27 06:53:04.000000 perpetuo-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:53:13.948888 perpetuo-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-27 06:53:04.000000 perpetuo-0.3.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-27 06:53:04.000000 perpetuo-0.3.0/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-27 06:53:04.000000 perpetuo-0.3.0/src/shmem.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:59.706192 perpetuo-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    49899 2023-04-27 23:32:49.000000 perpetuo-0.3.1/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 23:32:49.000000 perpetuo-0.3.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 23:32:49.000000 perpetuo-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 23:32:49.000000 perpetuo-0.3.1/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 23:32:49.000000 perpetuo-0.3.1/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 23:32:49.000000 perpetuo-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 23:32:59.706192 perpetuo-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-27 23:32:49.000000 perpetuo-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 23:32:49.000000 perpetuo-0.3.1/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-27 23:32:49.000000 perpetuo-0.3.1/prep-manylinux-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 23:32:49.000000 perpetuo-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:59.702192 perpetuo-0.3.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:59.706192 perpetuo-0.3.1/python/perpetuo/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 23:32:49.000000 perpetuo-0.3.1/python/perpetuo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 23:32:49.000000 perpetuo-0.3.1/python/perpetuo/_perpetuo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-27 23:32:49.000000 perpetuo-0.3.1/python/perpetuo/_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:59.706192 perpetuo-0.3.1/python/perpetuo/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:49.000000 perpetuo-0.3.1/python/perpetuo/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-27 23:32:49.000000 perpetuo-0.3.1/python/perpetuo/_tests/test_perpetuo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:49.000000 perpetuo-0.3.1/python/perpetuo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:59.706192 perpetuo-0.3.1/python/perpetuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-27 23:32:59.000000 perpetuo-0.3.1/python/perpetuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-27 23:32:59.000000 perpetuo-0.3.1/python/perpetuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:32:59.000000 perpetuo-0.3.1/python/perpetuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:32:59.000000 perpetuo-0.3.1/python/perpetuo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 23:32:59.000000 perpetuo-0.3.1/python/perpetuo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:32:59.706192 perpetuo-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-27 23:32:49.000000 perpetuo-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:32:59.706192 perpetuo-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-27 23:32:49.000000 perpetuo-0.3.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-27 23:32:49.000000 perpetuo-0.3.1/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-27 23:32:49.000000 perpetuo-0.3.1/src/shmem.rs
```

### Comparing `perpetuo-0.3.0/Cargo.lock` & `perpetuo-0.3.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -465,15 +465,15 @@
 
 [[package]]
 name = "ctrlc"
 version = "3.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbcf33c2a618cbe41ee43ae6e9f2e48368cd9f9db2896f10167d8d762679f639"
 dependencies = [
- "nix 0.26.2",
+ "nix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "cxx"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -994,26 +994,14 @@
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nix"
-version = "0.25.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f346ff70e7dbfd675fe90590b92d59ef2de15a8779ae305ebcbfd3f0caf59be4"
-dependencies = [
- "autocfg",
- "bitflags",
- "cfg-if",
- "libc",
-]
-
-[[package]]
-name = "nix"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
 dependencies = [
  "bitflags",
  "cfg-if",
  "libc",
@@ -1115,15 +1103,15 @@
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "perpetuo"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "anyhow",
  "bytemuck",
  "clap 4.2.4",
  "indoc 2.0.1",
  "libc",
  "memmap",
@@ -1408,27 +1396,26 @@
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "remoteprocess"
 version = "0.4.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3ed67d3fade907d519c2edd07329a8f16296a64f91b6f3c35570769cf6b25d"
+source = "git+https://github.com/njsmith/remoteprocess?branch=static-link#02c6f11ec5a1058fcdd4989ab9e63ea2df1a7be6"
 dependencies = [
  "addr2line",
  "goblin 0.6.1",
  "lazy_static",
  "libc",
  "libproc 0.12.0",
  "log",
  "mach",
  "mach_o_sys",
  "memmap",
- "nix 0.25.1",
+ "nix",
  "object",
  "proc-maps 0.3.1",
  "read-process-memory",
  "regex",
  "winapi",
 ]
```

### Comparing `perpetuo-0.3.0/Cargo.toml` & `perpetuo-0.3.1/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "perpetuo"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "perpetuo"
@@ -21,14 +21,17 @@
 memmap = "0.7.0"
 once_cell = "1.17.1"
 proc-maps = "0.3.0"
 py-spy = "0.3.14"
 pyo3 = { version = "0.18.3", features = ["extension-module", "abi3", "abi3-py39"] }
 remoteprocess = "0.4.11"
 
+[patch.crates-io]
+remoteprocess = { git = "https://github.com/njsmith/remoteprocess", branch = "static-link" }
+
 [build-dependencies]
 pyo3-build-config = "*"
 
 [target.'cfg(unix)'.dependencies]
 libc = "*"
 
 [target.'cfg(windows)'.dependencies]
```

### Comparing `perpetuo-0.3.0/LICENSE.APACHE2` & `perpetuo-0.3.1/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/LICENSE.MIT` & `perpetuo-0.3.1/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/PKG-INFO` & `perpetuo-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.3.0/README.md` & `perpetuo-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/prep-manylinux-container.sh` & `perpetuo-0.3.1/prep-manylinux-container.sh`

 * *Files 3% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # because our final binary is a PIE, so everything in it has to be PIC. So build our own
 # libunwind that we can force to use -fPIC.
 cd /
 curl -L https://github.com/libunwind/libunwind/archive/refs/tags/v1.6.2.tar.gz  -o libunwind.tar.gz
 tar xvf libunwind.tar.gz
 cd libunwind-*/
 autoreconf -i
-./configure CFLAGS="-fPIC"
+./configure CFLAGS="-fPIC" --enable-static
 make -j3
 make install
```

### Comparing `perpetuo-0.3.0/pyproject.toml` & `perpetuo-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 
 [project]
 name = "perpetuo"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   {name = "Nathaniel J. Smith", email = "njs@pobox.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT OR Apache-2.0"}
 description = "A stall tracker for Python's GIL and Trio tasks"
```

### Comparing `perpetuo-0.3.0/python/perpetuo/_setup.py` & `perpetuo-0.3.1/python/perpetuo/_setup.py`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/python/perpetuo/_tests/test_perpetuo.py` & `perpetuo-0.3.1/python/perpetuo/_tests/test_perpetuo.py`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/python/perpetuo.egg-info/PKG-INFO` & `perpetuo-0.3.1/python/perpetuo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.3.0/python/perpetuo.egg-info/SOURCES.txt` & `perpetuo-0.3.1/python/perpetuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/setup.py` & `perpetuo-0.3.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 from setuptools_rust import Binding, RustBin, RustExtension, Strip
 from wheel.bdist_wheel import bdist_wheel
 
 
 # https://github.com/joerick/python-abi3-package-sample/blob/main/setup.py
 class bdist_wheel_abi3(bdist_wheel):
     def get_tag(self):
@@ -24,11 +24,11 @@
             py_limited_api=True,
             # strip=Strip.Debug
         ),
         RustBin("perpetuo", strip=Strip.Debug),
     ],
     cmdclass={"bdist_wheel": bdist_wheel_abi3},
     package_dir={"": "python"},
-    packages=["perpetuo"],
+    packages=find_packages(where="python"),
     package_data={"perpetuo": ["py.typed", "__init__.pyi"]},
     zip_safe=False,
 )
```

### Comparing `perpetuo-0.3.0/src/lib.rs` & `perpetuo-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/src/main.rs` & `perpetuo-0.3.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `perpetuo-0.3.0/src/shmem.rs` & `perpetuo-0.3.1/src/shmem.rs`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
                     .process
                     .copy(current.metadata.name_ptr, current.metadata.name_len)?;
                 let name = String::from_utf8(name)?;
                 stalls.push(StallReport {
                     id,
                     name,
                     thread_hint: current.metadata.thread_hint,
-                    duration: now - snapshot.last_updated,
+                    duration: now.duration_since(snapshot.last_updated),
                 })
             } else {
                 snapshot.stall_tracker = current;
                 snapshot.last_updated = now;
             }
         }
         Ok(stalls)
```

