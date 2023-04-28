# Comparing `tmp/cev_metrics-0.1.0.tar.gz` & `tmp/cev_metrics-0.1.1.tar.gz`

## Comparing `cev_metrics-0.1.0.tar` & `cev_metrics-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cev_metrics-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     2817 2023-04-28 17:15:29.000000 cev_metrics-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0      501       20      152 2023-04-28 16:54:20.000000 cev_metrics-0.1.0/.gitignore
--rw-r--r--   0      501       20       63 2023-04-04 00:30:55.000000 cev_metrics-0.1.0/README.md
--rw-r--r--   0      501       20     1696 2023-04-07 15:55:57.000000 cev_metrics-0.1.0/ozette.py
--rw-r--r--   0      501       20      439 2023-04-28 16:46:28.000000 cev_metrics-0.1.0/pyproject.toml
--rw-r--r--   0      501       20      362 2023-04-28 17:09:19.000000 cev_metrics-0.1.0/python/cev_metrics/__init__.py
--rw-r--r--   0      501       20     1647 2023-04-28 17:08:50.000000 cev_metrics-0.1.0/python/cev_metrics/_rust.py
--rw-r--r--   0      501       20    15314 2023-04-28 15:16:16.000000 cev_metrics-0.1.0/python/cev_metrics/py.py
--rw-r--r--   0      501       20      454 2023-04-07 17:12:13.000000 cev_metrics-0.1.0/results.md
--rw-r--r--   0      501       20    12891 2023-04-28 16:58:04.000000 cev_metrics-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     3056 2023-04-09 01:52:00.000000 cev_metrics-0.1.0/src/step_function.rs
--rwxr-xr-x   0      501       20      538 2023-04-28 17:09:32.000000 cev_metrics-0.1.0/x.py
--rw-r--r--   0      501       20    13105 2023-04-07 15:25:24.000000 cev_metrics-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 cev_metrics-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cev_metrics-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2845 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      152 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/.gitignore
+-rw-r--r--   0     1001      123       63 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/README.md
+-rw-r--r--   0     1001      123       10 2023-04-28 17:38:04.000000 cev_metrics-0.1.1/dist/cev_metrics-0.1.1.tar.gz
+-rw-r--r--   0     1001      123      439 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123      362 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/python/cev_metrics/__init__.py
+-rw-r--r--   0     1001      123     1647 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/python/cev_metrics/_rust.py
+-rw-r--r--   0     1001      123    15314 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/python/cev_metrics/py.py
+-rw-r--r--   0     1001      123    12891 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     3056 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/src/step_function.rs
+-rwxr-xr-x   0     1001      123      492 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/x.py
+-rw-r--r--   0     1001      123    13105 2023-04-28 17:38:03.000000 cev_metrics-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 cev_metrics-0.1.1/PKG-INFO
```

### Comparing `cev_metrics-0.1.0/.github/workflows/ci.yml` & `cev_metrics-0.1.1/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -105,15 +105,16 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
+    # needs: [linux, windows, macos, sdist]
+    needs: [macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `cev_metrics-0.1.0/python/cev_metrics/_rust.py` & `cev_metrics-0.1.1/python/cev_metrics/_rust.py`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.0/python/cev_metrics/py.py` & `cev_metrics-0.1.1/python/cev_metrics/py.py`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.0/src/lib.rs` & `cev_metrics-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.0/src/step_function.rs` & `cev_metrics-0.1.1/src/step_function.rs`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.0/Cargo.lock` & `cev_metrics-0.1.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cev-metrics"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "delaunator",
  "numpy",
  "petgraph",
  "pyo3",
  "rayon",
 ]
@@ -29,17 +29,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -124,33 +124,33 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "bb99c395ae250e1bf9133673f03ca9f97b7e71b705436bf8f089453445d1e9fe"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
@@ -263,75 +263,75 @@
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -413,17 +413,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
```

