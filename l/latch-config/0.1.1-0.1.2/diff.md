# Comparing `tmp/latch_config-0.1.1.tar.gz` & `tmp/latch_config-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_config-0.1.1.tar", max compression
+gzip compressed data, was "latch_config-0.1.2.tar", max compression
```

## Comparing `latch_config-0.1.1.tar` & `latch_config-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.1/LICENSE
--rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.1/README.md
--rw-r--r--   0        0        0     2081 2023-04-27 21:03:15.353972 latch_config-0.1.1/latch_config/config.py
--rw-r--r--   0        0        0      782 2023-04-27 21:03:33.072975 latch_config-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.1/setup.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.2/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.2/README.md
+-rw-r--r--   0        0        0     2238 2023-04-28 21:10:22.580571 latch_config-0.1.2/latch_config/config.py
+-rw-r--r--   0        0        0      782 2023-04-28 21:10:40.091123 latch_config-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.2/setup.py
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.2/PKG-INFO
```

### Comparing `latch_config-0.1.1/LICENSE` & `latch_config-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.1/latch_config/config.py` & `latch_config-0.1.2/latch_config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,19 @@
         env_name = ""
         if val is None:
             env_name = env_prefix + f.metadata.get("env", f.name)
             env_name = f.metadata.get("env_name_override", env_name)
 
             env_val = os.environ.get(env_name)
             if env_val is not None:
-                val = typ(env_val)
+                parser = f.metadata.get("parser")
+                if parser is not None:
+                    val = parser(env_val)
+                else:
+                    val = typ(env_val)
 
         if val is None:
             if f.default != MISSING:
                 val = f.default
             else:
                 raise RuntimeError(f"missing value for '{f.name}' (${env_name})")
```

### Comparing `latch_config-0.1.1/pyproject.toml` & `latch_config-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-config"
-version = "0.1.1"
+version = "0.1.2"
 description = "Shared config for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_config-0.1.1/setup.py` & `latch_config-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['latch_config']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'latch-config',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Shared config for latch python backend services',
     'long_description': '# python-config\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

