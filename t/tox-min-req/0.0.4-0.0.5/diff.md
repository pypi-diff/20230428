# Comparing `tmp/tox-min-req-0.0.4.tar.gz` & `tmp/tox-min-req-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-min-req-0.0.4.tar", last modified: Mon Mar 27 14:48:14 2023, max compression
+gzip compressed data, was "tox-min-req-0.0.5.tar", last modified: Thu Apr 27 20:38:53 2023, max compression
```

## Comparing `tox-min-req-0.0.4.tar` & `tox-min-req-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.841529 tox-min-req-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.825528 tox-min-req-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.829528 tox-min-req-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-27 14:48:14.841529 tox-min-req-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:48:14.841529 tox-min-req-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.829528 tox-min-req-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.829528 tox-min-req-0.0.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.825528 tox-min-req-0.0.4/tests/data/package_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.829528 tox-min-req-0.0.4/tests/data/package_data/sample_package/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/data/package_data/sample_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/data/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tests/test_parsing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.833529 tox-min-req-0.0.4/tox_min_req/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tox_min_req/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tox_min_req/_parse_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-27 14:47:51.000000 tox-min-req-0.0.4/tox_min_req/_tox_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:48:14.841529 tox-min-req-0.0.4/tox_min_req.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 14:48:14.000000 tox-min-req-0.0.4/tox_min_req.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.202313 tox-min-req-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.202313 tox-min-req-0.0.5/tests/data/package_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/tests/data/package_data/sample_package/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/data/package_data/sample_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/data/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tests/test_parsing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/tox_min_req/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tox_min_req/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tox_min_req/_parse_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-27 20:38:32.000000 tox-min-req-0.0.5/tox_min_req/_tox_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:38:53.206313 tox-min-req-0.0.5/tox_min_req.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 20:38:53.000000 tox-min-req-0.0.5/tox_min_req.egg-info/top_level.txt
```

### Comparing `tox-min-req-0.0.4/.github/workflows/test.yaml` & `tox-min-req-0.0.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `tox-min-req-0.0.4/.gitignore` & `tox-min-req-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tox-min-req-0.0.4/.pre-commit-config.yaml` & `tox-min-req-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tox-min-req-0.0.4/LICENSE.txt` & `tox-min-req-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tox-min-req-0.0.4/PKG-INFO` & `tox-min-req-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-min-req
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tox plugin to run tests with minimal requirements base on setup.cfg or pyproject.toml
 Author-email: Grzegorz Bokota <bokota+github@gmail.com>
 License: MIT
 Project-URL: Documentation, https://github.com/czaki/tox-min-req#readme
 Project-URL: Issues, https://github.com/czaki/tox-min-req/issues
 Project-URL: Source, https://github.com/czaki/tox-min-req
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tox-min-req-0.0.4/README.md` & `tox-min-req-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tox-min-req-0.0.4/pyproject.toml` & `tox-min-req-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-min-req-0.0.4/tests/test_integration.py` & `tox-min-req-0.0.5/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,7 +360,30 @@
             "test_file.py": test_file_template_six.format(six_version=target_six_version),
         },
         base=data_dir / "package_data",
     )
 
     result = project.run("run")
     result.assert_success()
+
+
+def test_reset_pip_constrains(
+    tox_project: ToxProjectCreator,
+    monkeypatch: pytest.MonkeyPatch,
+    data_dir: "Path",
+    tmp_path: "Path",
+) -> None:
+    env = f"{sys.version_info[0]}{sys.version_info[1]}"
+    monkeypatch.setenv("MIN_REQ", "1")
+    (tmp_path / "constraints.txt").write_text("six==1.14.0")
+    monkeypatch.setenv("PIP_CONSTRAINT", str(tmp_path / "constraints.txt"))
+    project = tox_project(
+        {
+            "tox.ini": TOX_INI_TEMPLATE.format(env=env, extras="setenv =\n    PIP_CONSTRAINT="),
+            "pyproject.toml": PYPROJECT_TOML_TEMPLATE,
+            "test_file.py": TEST_FILE_TEMPLATE.format(cmp="=="),
+        },
+        base=data_dir / "package_data",
+    )
+
+    result = project.run("run")
+    result.assert_success()
```

### Comparing `tox-min-req-0.0.4/tests/test_parsing_files.py` & `tox-min-req-0.0.5/tests/test_parsing_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,7 +64,8 @@
 
 def test_parse_single_requirement():
     p_ver, py_full_ver = "3.10", "3.10.1"
     assert parse_single_requirement("numpy==1.16.0", p_ver, py_full_ver) == {"numpy": "1.16.0"}
     assert parse_single_requirement("numpy>=1.16.0", p_ver, py_full_ver) == {"numpy": "1.16.0"}
     assert parse_single_requirement("numpy>=1.16.0 ; python_version < '3.8'", p_ver, py_full_ver) == {}
     assert parse_single_requirement("numpy[test]>=1.16.0", p_ver, py_full_ver) == {"numpy": "1.16.0"}
+    assert parse_single_requirement("numpy==1.16.0 # some text", p_ver, py_full_ver) == {"numpy": "1.16.0"}
```

### Comparing `tox-min-req-0.0.4/tox_min_req/_parse_dependencies.py` & `tox-min-req-0.0.5/tox_min_req/_parse_dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Parse single requirement line. It resolve requirement against current system and provided python version.
 
     :param line: line with requirement
     :param python_version: major.minor version of python
     :param python_full_version: major.minor.patch version of python
     :return: empty dict if the requirement is not valid or the requirement name and version
     """
-    req = Requirement(line)
+    req = Requirement(line.split("#", maxsplit=1)[0])
     if req.marker is not None and not req.marker.evaluate(
         {"python_version": python_version, "python_full_version": python_full_version},
     ):
         return {}
     version_li = [str(x).replace(">=", "").replace("==", "") for x in req.specifier if ">=" in str(x) or "==" in str(x)]
     if version_li:
         return {req.name: version_li[0]}
```

### Comparing `tox-min-req-0.0.4/tox_min_req/_tox_plugin.py` & `tox-min-req-0.0.5/tox_min_req/_tox_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         constrain_file = tox_env.env_tmp_dir / "constraints.txt"
 
     with constrain_file.open("w") as f:
         f.write("\n".join(f"{n}=={v}" for n, v in dependencies.items()))
         f.write("\n")
         f.write("\n".join(extra_lines))
 
-    if "PIP_CONSTRAINT" in tox_env.environment_variables:
+    if tox_env.environment_variables.get("PIP_CONSTRAINT", ""):
         tox_env.environment_variables["PIP_CONSTRAINT"] += f" {str(constrain_file)}"
     else:
         tox_env.environment_variables["PIP_CONSTRAINT"] = str(constrain_file)
 
     return constrain_file
```

### Comparing `tox-min-req-0.0.4/tox_min_req.egg-info/PKG-INFO` & `tox-min-req-0.0.5/tox_min_req.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-min-req
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tox plugin to run tests with minimal requirements base on setup.cfg or pyproject.toml
 Author-email: Grzegorz Bokota <bokota+github@gmail.com>
 License: MIT
 Project-URL: Documentation, https://github.com/czaki/tox-min-req#readme
 Project-URL: Issues, https://github.com/czaki/tox-min-req/issues
 Project-URL: Source, https://github.com/czaki/tox-min-req
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tox-min-req-0.0.4/tox_min_req.egg-info/SOURCES.txt` & `tox-min-req-0.0.5/tox_min_req.egg-info/SOURCES.txt`

 * *Files identical despite different names*

