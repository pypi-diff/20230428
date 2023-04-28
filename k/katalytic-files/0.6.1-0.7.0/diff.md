# Comparing `tmp/katalytic-files-0.6.1.tar.gz` & `tmp/katalytic-files-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.6.1.tar", last modified: Sun Apr 16 11:20:02 2023, max compression
+gzip compressed data, was "katalytic-files-0.7.0.tar", last modified: Fri Apr 28 11:58:56 2023, max compression
```

## Comparing `katalytic-files-0.6.1.tar` & `katalytic-files-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.gitignore
--rw-r--r--   0        0        0      841 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      542 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/.travis.yml
--rw-r--r--   0        0        0     1040 2023-04-16 11:19:58.263116 katalytic-files-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     2031 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/README.md
--rw-r--r--   0        0        0     1608 2023-04-16 11:19:57.838904 katalytic-files-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/pytest.sh
--rw-r--r--   0        0        0     3107 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/scripts/venv.sh
--rw-r--r--   0        0        0    12492 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/src/katalytic/files.py
--rw-r--r--   0        0        0    42174 2023-04-16 11:19:20.132061 katalytic-files-0.6.1/tests/test_files.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 katalytic-files-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic-files-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-files-0.7.0/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:14:43.739675 katalytic-files-0.7.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1669 2023-04-28 11:58:39.506842 katalytic-files-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic-files-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2031 2023-04-14 19:03:52.346854 katalytic-files-0.7.0/README.md
+-rw-r--r--   0        0        0     1552 2023-04-28 11:58:39.506842 katalytic-files-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    16089 2023-04-28 11:44:29.824284 katalytic-files-0.7.0/src/katalytic/files.py
+-rw-r--r--   0        0        0    44993 2023-04-28 11:43:36.576283 katalytic-files-0.7.0/tests/test_files.py
+-rw-r--r--   0        0        0     3209 1970-01-01 00:00:00.000000 katalytic-files-0.7.0/PKG-INFO
```

### Comparing `katalytic-files-0.6.1/.gitignore` & `katalytic-files-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.1/CHANGELOG.md` & `katalytic-files-0.7.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 0.7.0 (2023-04-28)
+### feat
+- [[`1cb4276`](https://gitlab.com/katalytic/katalytic-files/commit/1cb4276ed44ff52b8aa33cdf65a358acee213712)] add load_csv() and save_csv()
+- [[`d8c554c`](https://gitlab.com/katalytic/katalytic-files/commit/d8c554c8d993b1693b6e264a19c47a9352db9475)] add universal functions: load() and save()
+- [[`7ee6498`](https://gitlab.com/katalytic/katalytic-files/commit/7ee6498a7eb7db0192d5dcfe94ce564d25e51082)] **load_csv:** convert empty strings to None
+- [[`47bd254`](https://gitlab.com/katalytic/katalytic-files/commit/47bd254fe9fead96b08d75af0f2d878d51bc59c7)] **load/save:** lowercase the extension
+
+
 ## 0.6.1 (2023-04-16)
 ### Fix
 * Test the new token ([`f2838d7`](https://github.com/katalytic/katalytic-files/commit/f2838d7ca49a27e8bbf718fab5d55b64868cf734))
 * Test the new token ([`43d505a`](https://github.com/katalytic/katalytic-files/commit/43d505aab96beaa6807188d72aece63de7d9f812))
 
 
 ## 0.6.0 (2023-04-15)
```

### Comparing `katalytic-files-0.6.1/LICENSE.txt` & `katalytic-files-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.1/README.md` & `katalytic-files-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.6.1/pyproject.toml` & `katalytic-files-0.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.6.1"
+version = "0.7.0"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -26,14 +26,15 @@
     "automation",
     "filesystem"
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
+    "katalytic-data>=0.4.0",
     "katalytic-pkg>=0.2.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
@@ -56,13 +57,9 @@
 [testenv]
 extras = dev
 deps = -e .
 
 commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
 """
 
-[tool.semantic_release]
-version_variable = "pyproject.toml:version"
-branch = "main"
-
 [tool.flit.module]
 name = "katalytic.files"
```

### Comparing `katalytic-files-0.6.1/src/katalytic/files.py` & `katalytic-files-0.7.0/src/katalytic/files.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,108 @@
 import collections
 import copy
+import csv
 import itertools
 import json
 import re
 import shutil
 import tempfile
 
 from pathlib import Path
 
-from katalytic.pkg import get_version
+from katalytic.data import as_list_of_dicts, as_list_of_lists, sort_dict_by_keys
+from katalytic.pkg import get_version, get_functions_in_group, mark
 
 __version__, __version_info__ = get_version(__name__)
 
 
-def load_text(path, *, encoding='utf-8', **kwargs):
-    with open(path, encoding=encoding) as f:
-        return f.read()
-
-
-def save_text(data, path, *, encoding='utf-8'):
-    with open(path, 'w', encoding=encoding) as f:
-        return f.write(data)
+@mark('load::csv')
+def load_csv(path, *, encoding='utf-8', **kwargs):
+    with open(path, 'r', encoding=encoding) as f:
+        dialect = csv.Sniffer().sniff(f.read(1024))
+        f.seek(0)
+
+        reader = csv.reader(f, dialect)
+        header = next(reader)
+        data = [dict(zip(header, row)) for row in reader]
+
+    for col in header:
+        t = _guess_type(col, data)
+
+        for i, row in enumerate(data):
+            if row[col] in ('None', ''):
+                data[i][col] = None
+
+        if t == 'bool':
+            for i, row in enumerate(data):
+                if row[col] == 'True':
+                    data[i][col] = True
+                elif row[col] == 'False':
+                    data[i][col] = False
+        elif t == 'float':
+            for i, row in enumerate(data):
+                if row[col] is not None:
+                    data[i][col] = float(row[col])
+        elif t == 'int':
+            for i, row in enumerate(data):
+                if row[col] is not None:
+                    data[i][col] = int(row[col])
+
+    return data
+
+
+def _guess_type(col, data):
+    is_float = True
+    is_int = True
+    is_bool = True
+
+    for i, row in enumerate(data):
+        v = row[col]
+        if v in ('None', ''):
+            continue
+
+        if v in ('True', 'False'):
+            is_float = False
+            is_int = False
+            continue
+        else:
+            is_bool = False
+
+        if '.' not in v:
+            is_float = False
+
+        v = v.replace('.', '')
+        if not v.isdigit():
+            is_int = False
+            break
+
+    if is_bool:
+        return 'bool'
+    elif is_float:
+        return 'float'
+    elif is_int:
+        return 'int'
+    else:
+        return 'str'
+
+
+@mark('save::csv')
+def save_csv(data, path, *, encoding='utf-8', **kwargs):
+    data = as_list_of_lists(data)
+    with open(path, 'w', newline='', encoding=encoding) as f:
+        csv.writer(f, quoting=csv.QUOTE_ALL).writerows(data)
 
 
+@mark('load::json')
 def load_json(path, *, encoding='utf-8', **kwargs):
     with open(path, encoding=encoding) as f:
         return json.load(f, **kwargs)
 
 
+@mark('save::json')
 def save_json(data, path, *, encoding='utf-8', indent=4, **kwargs):
     if isinstance(indent, float) and indent.is_integer():
         indent = int(indent)
     elif not isinstance(indent, int):
         raise TypeError(f'<indent> expects a positive integer. Got {indent!r}')
     elif isinstance(indent, bool):
         raise TypeError(f'<indent> expects a positive integer. Got {indent!r}')
@@ -39,14 +110,72 @@
         raise ValueError(f'<indent> expects a positive integer. Got {indent!r}')
 
     sort_keys = kwargs.pop('sort_keys', True)
     with open(path, 'w', encoding=encoding) as f:
         json.dump(data, f, indent=indent, sort_keys=sort_keys, **kwargs)
 
 
+@mark('load::txt')
+def load_text(path, *, encoding='utf-8', **kwargs):
+    with open(path, encoding=encoding) as f:
+        return f.read()
+
+
+@mark('save::txt')
+def save_text(data, path, *, encoding='utf-8'):
+    with open(path, 'w', encoding=encoding) as f:
+        return f.write(data)
+
+
+def _find_grouped_functions(group):
+    loaders = {}
+    for func_name, f, groups in get_functions_in_group(group):
+        for g in groups:
+            ext = g.rpartition('::')[2]
+            loaders[ext] = f
+
+    # sort the dict with the most specific extension at the beginning
+    # this makes it easier to pick ".tar.gz" over ".gz"
+    return sort_dict_by_keys(loaders, key=len, reverse=True)
+
+
+def _setup_load():
+    # optimization: call _find_grouped_functions() in the outer function,
+    # so it doesn't have to be called every time load() is called
+    funcs = _find_grouped_functions('load::*')
+
+    def load(path, *, encoding='utf-8', **kwargs):
+        for ext, f in funcs.items():
+            if path.lower().endswith(f'.{ext}'):
+                return f(path, encoding=encoding, **kwargs)
+
+        raise RuntimeError(f'No load function found for {path!r}')
+
+    return load
+
+
+def _setup_save():
+    # optimization: call _find_grouped_functions() in the outer function,
+    # so it doesn't have to be called every time save() is called
+    funcs = _find_grouped_functions('save::*')
+
+    def save(data, path, *, encoding='utf-8', **kwargs):
+        for ext, f in funcs.items():
+            if path.lower().endswith(f'.{ext}'):
+                return f(data, path, encoding=encoding, **kwargs)
+
+        raise RuntimeError(f'No save function found for {path!r}')
+
+    return save
+
+
+load = _setup_load()
+save = _setup_save()
+
+
 def clear_dir(path, *, create_missing=True):
     """This function is not named "empty_dir" to avoid confusing it with "is_dir_empty"."""
     if not isinstance(create_missing, bool):
         raise TypeError(f'<create_missing> expects False or True. Got {type(create_missing)}')
 
     path = Path(path)
     delete_dir(path, missing_ok=True, non_empty_dir=True)
```

### Comparing `katalytic-files-0.6.1/tests/test_files.py` & `katalytic-files-0.7.0/tests/test_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,43 @@
 import collections
+import copy
 import shutil
 import tempfile
 from pathlib import Path
 
 import pytest
 
-from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, load_json, load_text, make_dir, move_dir, move_file, save_json, save_text
+from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, load, load_csv, load_json, load_text, make_dir, move_dir, move_file, save, save_csv, save_json, save_text
+
+
+def _create_seq_of_seq():
+    return [
+        ['a', 'b', 'c', 'd', 'e'],
+        [1, 'x', True, -1.5, True],
+        [2, None, False, 0.0, 'z'],
+        [None, 'y', '', None, 'w'],
+    ]
+
+
+def _create_seq_of_dicts():
+    return [
+        {'a': 1, 'b': 'x', 'c': True, 'd': -1.5, 'e': True},
+        {'a': 2, 'b': None, 'c': False, 'd': 0.0, 'e': 'z'},
+        {'a': None, 'b': 'y', 'c': '', 'd': None, 'e': 'w'},
+    ]
+
+
+def _create_dict_of_seq():
+    return {
+        'a': [1, 2, None],
+        'b': ['x', None, 'y'],
+        'c': [True, False, ''],
+        'd': [-1.5, 0.0, None],
+        'e': [True, 'z', 'w'],
+    }
 
 
 class TestGroup_save_and_load:
     class Test_json:
         def test_indent_0(self):
             data = self.create_json_data()
             path = _setup_path()
@@ -72,14 +100,86 @@
     class Test_text:
         def test_basic(self):
             data = 'some text\nwith newlines'
             path = _setup_path()
             save_text(data, path)
             assert load_text(path) == data
 
+    class Test_csv:
+        @pytest.mark.parametrize('data', [
+            _create_seq_of_seq(),
+            _create_seq_of_dicts(),
+            _create_dict_of_seq(),
+        ])
+        def test_basic(self, data):
+            expected = _create_seq_of_dicts()
+            expected[0]['e'] = str(expected[0]['e'])
+            expected[2]['c'] = None
+
+            path = _setup_path()
+            save_csv(data, path)
+            assert load_csv(path) == expected
+
+    class Test_universal_load_and_save:
+        def test_unknown(self):
+            with pytest.raises(RuntimeError):
+                load('data.unknown')
+
+            with pytest.raises(RuntimeError):
+                save('', 'data.unknown')
+
+        def test_txt(self):
+            data = 'Hello, World!\nThis is not a drill'
+            path = _setup_path('{}.txt')
+            save(data, path)
+
+            assert load(path) == load_text(path) == data
+
+        def test_csv(self):
+            data = _create_seq_of_dicts()
+            path = _setup_path('{}.CSV')
+            save(data, path)
+
+            expected_csv = copy.deepcopy(data)
+            expected_csv[0]['e'] = str(expected_csv[0]['e'])
+            expected_csv[2]['c'] = None
+
+            expected_text = '\n'.join([
+                '"a","b","c","d","e"',
+                '"1","x","True","-1.5","True"',
+                '"2","","False","0.0","z"',
+                '"","y","","","w"',
+            ])
+
+            assert load(path) == expected_csv
+            assert load_text(path).strip() == expected_text
+
+        def test_json(self):
+            data = {
+                'a': 1,
+                'b': [2, True, None, {}],
+            }
+            path = _setup_path('{}.json')
+            save(data, path)
+
+            expected_text = '\n'.join([
+                '{',
+                '    "a": 1,',
+                '    "b": [',
+                '        2,',
+                '        true,',
+                '        null,',
+                '        {}',
+                '    ]',
+                '}',
+            ])
+
+            assert load(path) == data
+            assert load_text(path).strip() == expected_text
+
 
 class TestGroup_copy:
     class Test_copy_dir:
         def test_dest_is_dir(self):
             src = Path(_setup_tree('{}_src'))
 
             dest = Path(get_unique_path('{}_dest'))
```

### Comparing `katalytic-files-0.6.1/PKG-INFO` & `katalytic-files-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.6.1
+Version: 0.7.0
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
+Requires-Dist: katalytic-data>=0.4.0
 Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-files.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-files.git
 Provides-Extra: dev
```

