# Comparing `tmp/cssfinder_backend_rust-0.1.0.tar.gz` & `tmp/cssfinder_backend_rust-0.1.1.tar.gz`

## Comparing `cssfinder_backend_rust-0.1.0.tar` & `cssfinder_backend_rust-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 cssfinder_backend_rust-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123       19 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.gitattributes
--rw-r--r--   0     1001      123     1219 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.github/workflows/code_quality.yaml
--rw-r--r--   0     1001      123     2880 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0     1001      123     4163 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.github/workflows/deploy_to_test_pypi.yml
--rw-r--r--   0     1001      123      679 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.gitignore
--rw-r--r--   0     1001      123     1381 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123       82 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.prettierignore
--rw-r--r--   0     1001      123      399 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.prettierrc
--rw-r--r--   0     1001      123      757 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.vscode/dictionary.txt
--rw-r--r--   0     1001      123     3733 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/.vscode/settings.json
--rw-r--r--   0     1001      123      339 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/CHANGELOG.md
--rw-r--r--   0     1001      123     1068 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/LICENSE.md
--rw-r--r--   0     1001      123      799 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/README.md
--rw-r--r--   0     1001      123     1490 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/main.py
--rw-r--r--   0     1001      123   206626 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/poetry.lock
--rw-r--r--   0     1001      123       61 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/poetry.toml
--rw-r--r--   0     1001      123     2291 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123       15 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/rustfmt.toml
--rw-r--r--   0     1001      123     1203 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/scripts/__init__.py
--rw-r--r--   0     1001      123     3870 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/scripts/release.py
--rw-r--r--   0     1001      123     1097 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/scripts/templates/MIT.md.jinja2
--rw-r--r--   0     1001      123     2320 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/scripts/version.py
--rw-r--r--   0     1001      123    13682 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123    16991 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/src/naive.rs
--rw-r--r--   0     1001      123     1726 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/src/shared.rs
--rw-r--r--   0     1001      123        0 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/test/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/test/test_python/__init__.py
--rw-r--r--   0     1001      123     7711 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/test/test_python/test_conform.py
--rw-r--r--   0     1001      123    15408 2023-04-19 22:55:57.000000 cssfinder_backend_rust-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 cssfinder_backend_rust-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 cssfinder_backend_rust-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123       19 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.gitattributes
+-rw-r--r--   0     1001      123     1219 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.github/workflows/code_quality.yaml
+-rw-r--r--   0     1001      123     2880 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0     1001      123     4163 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.github/workflows/deploy_to_test_pypi.yml
+-rw-r--r--   0     1001      123      679 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.gitignore
+-rw-r--r--   0     1001      123     1381 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123       82 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.prettierignore
+-rw-r--r--   0     1001      123      399 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.prettierrc
+-rw-r--r--   0     1001      123      757 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.vscode/dictionary.txt
+-rw-r--r--   0     1001      123     3733 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/.vscode/settings.json
+-rw-r--r--   0     1001      123     1247 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/CHANGELOG.md
+-rw-r--r--   0     1001      123     1068 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/LICENSE.md
+-rw-r--r--   0     1001      123      799 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/README.md
+-rw-r--r--   0     1001      123     1490 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/main.py
+-rw-r--r--   0     1001      123   206626 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/poetry.lock
+-rw-r--r--   0     1001      123       61 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/poetry.toml
+-rw-r--r--   0     1001      123     2291 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123       15 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/rustfmt.toml
+-rw-r--r--   0     1001      123     1203 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/scripts/__init__.py
+-rw-r--r--   0     1001      123     3995 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/scripts/release.py
+-rw-r--r--   0     1001      123     1097 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/scripts/templates/MIT.md.jinja2
+-rw-r--r--   0     1001      123     2320 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/scripts/version.py
+-rw-r--r--   0     1001      123    13791 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123    17163 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/src/naive.rs
+-rw-r--r--   0     1001      123     1726 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/src/shared.rs
+-rw-r--r--   0     1001      123        0 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/test/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/test/test_python/__init__.py
+-rw-r--r--   0     1001      123     7711 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/test/test_python/test_conform.py
+-rw-r--r--   0     1001      123    15408 2023-04-27 22:19:22.000000 cssfinder_backend_rust-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 cssfinder_backend_rust-0.1.1/PKG-INFO
```

### Comparing `cssfinder_backend_rust-0.1.0/Cargo.toml` & `cssfinder_backend_rust-0.1.1/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cssfinder-backend-rust"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 authors = ["Krzysztof Wisniewski <argmaster.world@gmail.com>"]
 description = "Implementation of CSSFinder backend using Rust."
 repository = "https://github.com/argmaster/cssfinder_backend_rust"
 readme = "README.md"
 license-file = "LICENSE.md"
```

### Comparing `cssfinder_backend_rust-0.1.0/.github/workflows/code_quality.yaml` & `cssfinder_backend_rust-0.1.1/.github/workflows/code_quality.yaml`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/.github/workflows/deploy_to_pypi.yml` & `cssfinder_backend_rust-0.1.1/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/.github/workflows/deploy_to_test_pypi.yml` & `cssfinder_backend_rust-0.1.1/.github/workflows/deploy_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/.gitignore` & `cssfinder_backend_rust-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/.pre-commit-config.yaml` & `cssfinder_backend_rust-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/.vscode/dictionary.txt` & `cssfinder_backend_rust-0.1.1/.vscode/dictionary.txt`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/.vscode/settings.json` & `cssfinder_backend_rust-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/LICENSE.md` & `cssfinder_backend_rust-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/README.md` & `cssfinder_backend_rust-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/main.py` & `cssfinder_backend_rust-0.1.1/main.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/poetry.lock` & `cssfinder_backend_rust-0.1.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/pyproject.toml` & `cssfinder_backend_rust-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cssfinder-backend-rust-dev"
-version = "0.1.0"
+version = "0.1.1"
 description = "Development environment for Rust based implementation of CSSFinder backend. Use Maturin to build."
 authors = ["Krzysztof Wisniewski <argmaster.world@gmail.com>"]
 repository = "https://github.com/argmaster/cssfinder_backend_rust"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -37,15 +37,15 @@
     { cmd = "pre-commit run --all-files -v" },
 ]
 build = { cmd = "maturin build --release --out dist" }
 version = { script = "scripts.version:main" }
 
 [project]
 name = "cssfinder_backend_rust"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.8"
 authors = [
     { name = "Krzysztof Wisniewski", email = "argmaster.world@gmail.com" },
 ]
 description = "Implementation of CSSFinder backend using Rust."
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `cssfinder_backend_rust-0.1.0/scripts/__init__.py` & `cssfinder_backend_rust-0.1.1/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/scripts/release.py` & `cssfinder_backend_rust-0.1.1/scripts/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,19 @@
     subprocess.run(["git", "switch", "-c", f"release/{version}"])
     replace_version(
         PYPROJECT_PATH,
         r"version\s*=\s*\"(.*?)\"\n",
         f'version = "{version}"\n',
     )
     replace_version(
+        PYPROJECT_PATH,
+        r"version\s*=\s*\"(.*?)\"\n",
+        f'version = "{version}"\n',
+    )
+    replace_version(
         ROOT_DIR / "Cargo.toml",
         r"version\s*=\s*\"(.*?)\"\n",
         f'version = "{version}"\n',
     )
     replace_version(
         ROOT_DIR / "src" / "lib.rs",
         r"m.add(\"__version__\", \"0.1.0\")\?;",
```

### Comparing `cssfinder_backend_rust-0.1.0/scripts/templates/MIT.md.jinja2` & `cssfinder_backend_rust-0.1.1/scripts/templates/MIT.md.jinja2`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/scripts/version.py` & `cssfinder_backend_rust-0.1.1/scripts/version.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/src/lib.rs` & `cssfinder_backend_rust-0.1.1/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -375,26 +375,28 @@
             );
 
             NaiveRustBackendF32 { backend }
         }
 
         fn set_symmetries(
             &mut self,
-            symmetries: Vec<Vec<np::PyReadonlyArray2<Complex<f32>>>>,
+            symmetries: Vec<Vec<np::PyReadonlyArray2<Complex<f64>>>>,
         ) {
             use ndarray as nd;
 
             let symmetries_local = symmetries
                 .into_iter()
                 .map(|inner_vec| {
                     inner_vec
                         .into_iter()
                         .map(|pyarray| {
                             let array_ref = pyarray.as_array();
-                            let array: nd::Array2<Complex<f32>> = array_ref.to_owned();
+                            let array: nd::Array2<Complex<f32>> = array_ref.mapv(|x| {
+                                Complex::<f32>::new(x.re as f32, x.im as f32)
+                            });
                             array
                         })
                         .collect()
                 })
                 .collect();
             self.backend.set_symmetries(symmetries_local);
         }
```

### Comparing `cssfinder_backend_rust-0.1.0/src/naive.rs` & `cssfinder_backend_rust-0.1.1/src/naive.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 use std::any;
 use std::f64::consts::PI;
 use std::fmt;
 use std::ops::Sub;
 
 use ndarray as nd;
 use num::Complex;
-use num_traits::Float;
+use num_traits::{Float, Zero};
 use rand::Rng;
 
 use crate::shared::AlgoMode;
 
 pub fn product<T>(lhs: &nd::Array2<Complex<T>>, rhs: &nd::Array2<Complex<T>>) -> T
 where
     T: Float + std::fmt::Debug + rand_distr::uniform::SampleUniform + 'static,
@@ -138,14 +138,21 @@
     let mut output = state.to_owned();
 
     for row in symmetries {
         for symmetry in row {
             output = rotate(&output, symmetry) + output;
         }
     }
+
+    let mut trace = Complex::<T>::zero();
+    for i in 0..output.dim().0 {
+        trace = trace + output[[i, i]];
+    }
+
+    output = output.map(|x| *x / trace);
     output
 }
 
 //   ██████     ███████    ███████            ███    ███     ██████     ██████     ███████
 //   ██   ██    ██         ██                 ████  ████    ██    ██    ██   ██    ██
 //   ██   ██    █████      ███████            ██ ████ ██    ██    ██    ██   ██    █████
 //   ██   ██    ██              ██            ██  ██  ██    ██    ██    ██   ██    ██
```

### Comparing `cssfinder_backend_rust-0.1.0/src/shared.rs` & `cssfinder_backend_rust-0.1.1/src/shared.rs`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/test/test_python/test_conform.py` & `cssfinder_backend_rust-0.1.1/test/test_python/test_conform.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_rust-0.1.0/Cargo.lock` & `cssfinder_backend_rust-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -33,32 +33,32 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cssfinder-backend-rust"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "ndarray",
  "ndarray-rand",
  "num",
  "num-traits",
  "numpy",
  "pyo3",
  "rand",
  "rand_distr",
  "statrs",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -71,17 +71,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -93,17 +93,17 @@
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
@@ -297,75 +297,75 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
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
```

### Comparing `cssfinder_backend_rust-0.1.0/PKG-INFO` & `cssfinder_backend_rust-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssfinder_backend_rust
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 License-File: LICENSE.md
 Summary: Implementation of CSSFinder backend using Rust.
 Author: Krzysztof Wisniewski <argmaster.world@gmail.com>
```

