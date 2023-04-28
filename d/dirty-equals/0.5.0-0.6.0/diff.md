# Comparing `tmp/dirty_equals-0.5.0.tar.gz` & `tmp/dirty_equals-0.6.0.tar.gz`

## Comparing `dirty_equals-0.5.0.tar` & `dirty_equals-0.6.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/.codecov.yml
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/Makefile
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/mkdocs.yml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/setup.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/.github/workflows/upload-previews.yml
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/__init__.py
--rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_base.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_boolean.py
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_datetime.py
--rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_dict.py
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_inspection.py
--rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_numeric.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_other.py
--rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_sequence.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_strings.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/py.typed
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/dirty_equals/version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/CNAME
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/index.md
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/internals.md
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/plugins.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/usage.md
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/img/dirty-equals-logo-base.svg
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/img/dirty-equals-logo-favicon.svg
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/img/favicon.png
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/img/logo-text.svg
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/img/logo-white.svg
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/boolean.md
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/custom.md
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/datetime.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/dict.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/inspection.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/numeric.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/other.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/sequence.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/docs/types/string.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/all.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/docs.in
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/docs.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/linting.in
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/linting.txt
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/pyproject.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/tests.in
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/requirements/tests.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/mypy_checks.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_base.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_boolean.py
--rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_datetime.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_dict.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_docs.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_inspection.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_list_tuple.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_numeric.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_other.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/tests/test_strings.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/LICENSE
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/README.md
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 dirty_equals-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/.codecov.yml
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/Makefile
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/.github/workflows/upload-previews.yml
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/__init__.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_base.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_boolean.py
+-rw-r--r--   0        0        0    11190 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_datetime.py
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_dict.py
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_inspection.py
+-rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_numeric.py
+-rw-r--r--   0        0        0    13021 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_other.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_sequence.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_strings.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/py.typed
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/dirty_equals/version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/CNAME
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/index.md
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/internals.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/plugins.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/usage.md
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/img/dirty-equals-logo-base.svg
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/img/dirty-equals-logo-favicon.svg
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/img/favicon.png
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/img/logo-text.svg
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/img/logo-white.svg
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/boolean.md
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/custom.md
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/datetime.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/dict.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/inspection.md
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/numeric.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/other.md
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/sequence.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/docs/types/string.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/all.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/docs.in
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/docs.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/linting.in
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/linting.txt
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/tests.in
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/requirements/tests.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/mypy_checks.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_base.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_boolean.py
+-rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_datetime.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_dict.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_docs.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_inspection.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_list_tuple.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_numeric.py
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_other.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/tests/test_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/README.md
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 dirty_equals-0.6.0/PKG-INFO
```

### Comparing `dirty_equals-0.5.0/Makefile` & `dirty_equals-0.6.0/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 .DEFAULT_GOAL := all
-isort = isort dirty_equals tests
-black = black dirty_equals tests
+sources = dirty_equals tests
 
 .PHONY: install
 install:
 	pip install -r requirements/all.txt
 	pre-commit install
 
 .PHONY: format
 format:
-	$(isort)
-	$(black)
+	black $(sources)
+	ruff --fix $(sources)
 
 .PHONY: lint
 lint:
-	flake8 --max-complexity 10 --max-line-length 120 --ignore E203,W503 dirty_equals tests
-	$(isort) --check-only --df
-	$(black) --check
+	ruff $(sources)
+	black $(sources) --check --diff
 
 .PHONY: test
 test:
 	coverage run -m pytest
 	python tests/mypy_checks.py
 
 .PHONY: testcov
```

### Comparing `dirty_equals-0.5.0/mkdocs.yml` & `dirty_equals-0.6.0/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -59,30 +59,37 @@
   - attr_list
   - md_in_html
   - pymdownx.emoji:
       emoji_index: !!python/name:materialx.emoji.twemoji
       emoji_generator: !!python/name:materialx.emoji.to_svg
 
 extra:
+  version:
+    provider: mike
   analytics:
     provider: google
     property: G-FLP20728CW
   social:
   - icon: fontawesome/brands/github-alt
     link: https://github.com/samuelcolvin/dirty-equals
   - icon: fontawesome/brands/twitter
     link: https://twitter.com/samuel_colvin
 
+watch:
+  - dirty_equals
+
 plugins:
+  - mike:
+      alias_type: symlink
+      canonical_version: latest
   - search
   - mkdocstrings:
-      watch: [dirty_equals]
       handlers:
         python:
-          rendering:
+          options:
             show_root_heading: true
             show_root_full_path: false
             show_source: false
             heading_level: 2
             merge_init_into_class: true
             show_signature_annotations: true
             separate_signature: true
```

### Comparing `dirty_equals-0.5.0/.github/workflows/ci.yml` & `dirty_equals-0.6.0/.github/workflows/ci.yml`

 * *Files 27% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 jobs:
   test:
     name: test ${{ matrix.python-version }} on ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu, macos]
-        python-version: ['3.7', '3.8', '3.9', '3.10']
-        # test 3.11-dev and pypy on ubuntu only to speed up CI, no reason why macos X pypy should fail separately
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        # test pypy on ubuntu only to speed up CI, no reason why macos X pypy should fail separately
         include:
           - os: 'ubuntu'
-            python-version: '3.11-dev'
-          - os: 'ubuntu'
             python-version: 'pypy-3.7'
           - os: 'ubuntu'
             python-version: 'pypy-3.8'
           - os: 'ubuntu'
             python-version: 'pypy-3.9'
 
     runs-on: ${{ matrix.os }}-latest
@@ -38,22 +36,15 @@
     - uses: actions/checkout@v3
 
     - name: set up python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
-    - uses: actions/cache@v3
-      id: cache
-      with:
-        path: ${{ env.pythonLocation }}
-        key: ${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('requirements/tests.txt') }}
-
     - run: pip install -r requirements/tests.txt -r requirements/pyproject.txt
-      if: steps.cache.outputs.cache-hit != 'true'
 
     - run: make test
 
     - run: coverage xml
 
     - uses: codecov/codecov-action@v3
       with:
@@ -66,22 +57,15 @@
     steps:
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
         python-version: '3.10'
 
-    - uses: actions/cache@v3
-      id: cache
-      with:
-        path: ${{ env.pythonLocation }}
-        key: ${{ env.pythonLocation }}-${{ hashFiles('requirements/linting.txt') }}-${{ hashFiles('pyproject.toml') }}
-
     - run: pip install -r requirements/linting.txt
-      if: steps.cache.outputs.cache-hit != 'true'
 
     - uses: pre-commit/action@v3.0.0
       with:
         extra_args: --all-files
 
   docs:
     runs-on: ubuntu-latest
@@ -94,68 +78,104 @@
         python-version: '3.10'
 
     - name: install
       run: pip install -r requirements/docs.txt
 
     - name: install mkdocs-material-insiders
       if: github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/tags/')
-      run: pip install https://files.scolvin.com/${MKDOCS_TOKEN}/mkdocs-material/mkdocs_material-8.2.8+insiders.4.12.0-py3-none-any.whl
+      run: pip install https://files.scolvin.com/${MKDOCS_TOKEN}/mkdocs-material/mkdocs_material-9.1.5+insiders.4.32.4-py3-none-any.whl
       env:
         MKDOCS_TOKEN: ${{ secrets.mkdocs_token }}
 
     - name: build site
       run: mkdocs build --strict
 
     - name: store docs site
       uses: actions/upload-artifact@v3
       with:
         name: docs
         path: site
 
-  deploy:
-    needs:
-      - test
-      - lint
-      - docs
-    if: "success() && startsWith(github.ref, 'refs/tags/')"
+  check:  # This job does nothing and is only used for the branch protection
+    if: always()
+    needs: [lint, test, docs]
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Decide whether the needed jobs succeeded or failed
+        uses: re-actors/alls-green@release/v1
+        id: all-green
+        with:
+          jobs: ${{ toJSON(needs) }}
+
+  publish_docs:
+    needs: [check]
+    if: "success() && (github.ref == 'refs/heads/main' || startsWith(github.ref, 'refs/tags/'))"
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - name: set up python
         uses: actions/setup-python@v4
         with:
           python-version: '3.9'
 
-      - name: get docs
-        uses: actions/download-artifact@v3
+      - name: install
+        run: pip install -r requirements/docs.txt
+
+      - name: install mkdocs-material-insiders
+        run: pip install https://files.scolvin.com/${MKDOCS_TOKEN}/mkdocs-material/mkdocs_material-9.1.5+insiders.4.32.4-py3-none-any.whl
+        env:
+          MKDOCS_TOKEN: ${{ secrets.mkdocs_token }}
+
+      - name: Set git credentials
+        run: |
+          git config --global user.name "${{ github.actor }}"
+          git config --global user.email "${{ github.actor }}@users.noreply.github.com"
+          git config --global pull.rebase true
+          git pull origin docs-site
+
+      - run: mike deploy -b docs-site dev --push
+        if: github.ref == 'refs/heads/main'
+
+      - name: check version
+        if: "startsWith(github.ref, 'refs/tags/')"
+        id: check-version
+        uses: samuelcolvin/check-python-version@v3.2
         with:
-          name: docs
-          path: site
+          version_file_path: 'dirty_equals/version.py'
+
+      - run: mike deploy -b docs-site ${{ steps.check-version.outputs.VERSION_MAJOR_MINOR }} latest --update-aliases --push
+        if: "startsWith(github.ref, 'refs/tags/') && !fromJSON(steps.check-version.outputs.IS_PRERELEASE)"
+
+  deploy:
+    needs: [check]
+    if: "success() && startsWith(github.ref, 'refs/tags/')"
+    runs-on: ubuntu-latest
+    environment: release
+
+    permissions:
+      id-token: write
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: set up python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
 
       - name: install
-        run: pip install -U twine build packaging
+        run: pip install -U build
 
       - name: check version
         id: check-version
-        run: python <(curl -Ls https://gist.githubusercontent.com/samuelcolvin/4e1ad439c5489e8d6478cdee3eb952ef/raw/check_version.py)
-        env:
-          VERSION_PATH: 'dirty_equals/version.py'
+        uses: samuelcolvin/check-python-version@v3.2
+        with:
+          version_file_path: 'dirty_equals/version.py'
 
       - name: build
         run: python -m build
 
-      - run: twine check dist/*
-
-      - name: upload to pypi
-        run: twine upload dist/*
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.pypi_token }}
-
-      - name: publish docs
-        uses: JamesIves/github-pages-deploy-action@v4
-        if: '!fromJSON(steps.check-version.outputs.IS_PRERELEASE)'
-        with:
-          branch: gh-pages
-          folder: site
+      - name: Upload package to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dirty_equals-0.5.0/.github/workflows/upload-previews.yml` & `dirty_equals-0.6.0/.github/workflows/upload-previews.yml`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/dirty_equals/__init__.py` & `dirty_equals-0.6.0/dirty_equals/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 from ._boolean import IsFalseLike, IsTrueLike
 from ._datetime import IsDate, IsDatetime, IsNow, IsToday
 from ._dict import IsDict, IsIgnoreDict, IsPartialDict, IsStrictDict
 from ._inspection import HasAttributes, HasName, HasRepr, IsInstance
 from ._numeric import (
     IsApprox,
     IsFloat,
+    IsFloatInf,
+    IsFloatInfNeg,
+    IsFloatInfPos,
+    IsFloatNan,
     IsInt,
     IsNegative,
     IsNegativeFloat,
     IsNegativeInt,
     IsNonNegative,
     IsNonPositive,
     IsNumber,
     IsNumeric,
     IsPositive,
     IsPositiveFloat,
     IsPositiveInt,
 )
-from ._other import FunctionCheck, IsIP, IsJson, IsUUID
+from ._other import FunctionCheck, IsHash, IsIP, IsJson, IsUrl, IsUUID
 from ._sequence import Contains, HasLen, IsList, IsListOrTuple, IsTuple
 from ._strings import IsAnyStr, IsBytes, IsStr
 from .version import VERSION
 
 __all__ = (
     # base
     'DirtyEquals',
@@ -57,23 +61,29 @@
     'IsNonNegative',
     'IsInt',
     'IsPositiveInt',
     'IsNegativeInt',
     'IsFloat',
     'IsPositiveFloat',
     'IsNegativeFloat',
+    'IsFloatInf',
+    'IsFloatInfNeg',
+    'IsFloatInfPos',
+    'IsFloatNan',
     # inspection
     'HasAttributes',
     'HasName',
     'HasRepr',
     'IsInstance',
     # other
     'FunctionCheck',
     'IsJson',
     'IsUUID',
+    'IsUrl',
+    'IsHash',
     'IsIP',
     # strings
     'IsStr',
     'IsBytes',
     'IsAnyStr',
     # version
     '__version__',
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_base.py` & `dirty_equals-0.6.0/dirty_equals/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         ```py title=".values"
         from dirty_equals import IsStr
 
         token_is_str = IsStr(regex=r't-.+')
         assert 't-123' == token_is_str
 
         print(token_is_str.value)
-        #> 't-123'
+        #> t-123
         ```
         """
         if self._was_equal:
             return self._other
         else:
             raise AttributeError('value is not available until __eq__ has been called')
 
@@ -216,15 +216,15 @@
     def __init__(self, expected_value: Any, *more_expected_values: Any):
         """
         Args:
             expected_value: Expected value for equals to return true.
             *more_expected_values: More expected values for equals to return true.
 
         ```py title="IsOneOf"
-        from dirty_equals import IsOneOf, Contains
+        from dirty_equals import Contains, IsOneOf
 
         assert 1 == IsOneOf(1, 2, 3)
         assert 4 != IsOneOf(1, 2, 3)
         # check that a list either contain 1 or is empty
         assert [1, 2, 3] == Contains(1) | IsOneOf([])
         assert [] == Contains(1) | IsOneOf([])
         ```
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_boolean.py` & `dirty_equals-0.6.0/dirty_equals/_boolean.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/dirty_equals/_datetime.py` & `dirty_equals-0.6.0/dirty_equals/_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,18 @@
             iso_string: whether to allow iso formatted strings in comparison
             format_string: if provided, `format_string` is used with `datetime.strptime` to parse strings
             enforce_tz: whether timezone should be enforced in comparison, see below for more details
 
         Examples of basic usage:
 
         ```py title="IsDatetime"
-        from dirty_equals import IsDatetime
         from datetime import datetime
 
+        from dirty_equals import IsDatetime
+
         y2k = datetime(2000, 1, 1)
         assert datetime(2000, 1, 1) == IsDatetime(approx=y2k)
         # Note: this requires the system timezone to be UTC
         assert 946684800.123 == IsDatetime(approx=y2k, unix_number=True)
         assert datetime(2000, 1, 1, 0, 0, 9) == IsDatetime(approx=y2k, delta=10)
         assert '2000-01-01T00:00' == IsDatetime(approx=y2k, iso_string=True)
 
@@ -140,17 +141,18 @@
             iso_string: whether to allow iso formatted strings in comparison
             format_string: if provided, `format_string` is used with `datetime.strptime` to parse strings
             enforce_tz: whether timezone should be enforced in comparison, see below for more details
             tz: either a `pytz.timezone`, a `datetime.timezone` or a string which will be passed to `pytz.timezone`,
                 if provided now will be converted to this timezone.
 
         ```py title="IsNow"
-        from dirty_equals import IsNow
         from datetime import datetime, timezone
 
+        from dirty_equals import IsNow
+
         now = datetime.now()
         assert now == IsNow
         assert now.timestamp() == IsNow(unix_number=True)
         assert now.timestamp() != IsNow
         assert now.isoformat() == IsNow(iso_string=True)
         assert now.isoformat() != IsNow
 
@@ -181,15 +183,14 @@
     def _get_now(self) -> datetime:
         if self.tz is None:
             return datetime.now()
         else:
             return datetime.utcnow().replace(tzinfo=timezone.utc).astimezone(self.tz)
 
     def prepare(self, other: Any) -> datetime:
-
         # update approx for every comparing, to check if other value is dirty equal
         # to current moment of time
         self.approx = self._get_now()
 
         return super().prepare(other)
 
 
@@ -208,15 +209,14 @@
         gt: Optional[date] = None,
         lt: Optional[date] = None,
         ge: Optional[date] = None,
         le: Optional[date] = None,
         iso_string: bool = False,
         format_string: Optional[str] = None,
     ):
-
         """
         Args:
             approx: A value to approximately compare to.
             delta: The allowable different when comparing to the value to now, if omitted 2 seconds is used,
                 ints and floats are assumed to represent seconds and converted to `timedelta`s.
             gt: Value which the compared value should be greater than (after).
             lt: Value which the compared value should be less than (before).
@@ -224,17 +224,18 @@
             le: Value which the compared value should be less than (before) or equal to.
             iso_string: whether to allow iso formatted strings in comparison
             format_string: if provided, `format_string` is used with `datetime.strptime` to parse strings
 
         Examples of basic usage:
 
         ```py title="IsDate"
-        from dirty_equals import IsDate
         from datetime import date
 
+        from dirty_equals import IsDate
+
         y2k = date(2000, 1, 1)
         assert date(2000, 1, 1) == IsDate(approx=y2k)
         assert '2000-01-01' == IsDate(approx=y2k, iso_string=True)
 
         assert date(2000, 1, 2) == IsDate(gt=y2k)
         assert date(1999, 1, 2) != IsDate(gt=y2k)
         ```
@@ -282,17 +283,18 @@
         format_string: Optional[str] = None,
     ):
         """
         Args:
             iso_string: whether to allow iso formatted strings in comparison
             format_string: if provided, `format_string` is used with `datetime.strptime` to parse strings
         ```py title="IsToday"
-        from dirty_equals import IsToday
         from datetime import date, timedelta
 
+        from dirty_equals import IsToday
+
         today = date.today()
         assert today == IsToday
         assert today.isoformat() == IsToday(iso_string=True)
         assert today.isoformat() != IsToday
         assert today + timedelta(days=1) != IsToday
         assert today.strftime('%Y/%m/%d') == IsToday(format_string='%Y/%m/%d')
         assert today.strftime('%Y/%m/%d') != IsToday()
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_dict.py` & `dirty_equals-0.6.0/dirty_equals/_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Container, Dict, Optional, Union, overload
+from typing import Any, Callable, Container, Dict, overload
 
 from ._base import DirtyEquals, DirtyEqualsMeta
 from ._utils import get_dict_arg
 
 NotGiven = object()
 
 
@@ -13,22 +13,22 @@
     Base class for comparing dictionaries. By default, `IsDict` isn't particularly useful on its own
     (it behaves pretty much like a normal `dict`), but it can be subclassed
     (see [`IsPartialDict`][dirty_equals.IsPartialDict] and [`IsStrictDict`][dirty_equals.IsStrictDict]) or modified
     with `.settings(...)` to powerful things.
     """
 
     @overload
-    def __init__(self, expected: Dict[Any, Any]):
+    def __init__(self, expected: dict[Any, Any]):
         ...
 
     @overload
     def __init__(self, **expected: Any):
         ...
 
-    def __init__(self, *expected_args: Dict[Any, Any], **expected_kwargs: Any):
+    def __init__(self, *expected_args: dict[Any, Any], **expected_kwargs: Any):
         """
         Can be created from either keyword arguments or an existing dictionary (same as `dict()`).
 
         `IsDict` is not particularly useful on its own, but it can be subclassed or modified with
         [`.settings(...)`][dirty_equals.IsDict.settings] to facilitate powerful comparison of dictionaries.
 
         ```py title="IsDict"
@@ -38,27 +38,27 @@
         assert {1: 2, 3: 4} == IsDict({1: 2, 3: 4})
         ```
         """
         self.expected_values = get_dict_arg('IsDict', expected_args, expected_kwargs)
 
         self.strict = False
         self.partial = False
-        self.ignore: Union[None, Container[Any], Callable[[Any], bool]] = None
+        self.ignore: None | Container[Any] | Callable[[Any], bool] = None
         self._post_init()
         super().__init__()
 
     def _post_init(self) -> None:
         pass
 
     def settings(
         self,
         *,
-        strict: Optional[bool] = None,
-        partial: Optional[bool] = None,
-        ignore: Union[None, Container[Any], Callable[[Any], bool]] = NotGiven,  # type: ignore[assignment]
+        strict: bool | None = None,
+        partial: bool | None = None,
+        ignore: None | Container[Any] | Callable[[Any], bool] = NotGiven,  # type: ignore[assignment]
     ) -> IsDict:
         """
         Allows you to customise the behaviour of `IsDict`, technically a new `IsDict` is required to allow chaining.
 
         Args:
             strict (bool): If `True`, the order of key/value pairs must match.
             partial (bool): If `True`, only keys include in the wrapped dict are checked.
@@ -66,22 +66,26 @@
                 Can be either a `Container` (e.g. `set` or `list`) of values to ignore, or a function that takes a
                 value and should return `True` if the value should be ignored.
 
         ```py title="IsDict.settings(...)"
         from dirty_equals import IsDict
 
         assert {'a': 1, 'b': 2, 'c': None} != IsDict(a=1, b=2)
-        assert {'a': 1, 'b': 2, 'c': None} == IsDict(a=1, b=2).settings(partial=True) #(1)!
+        assert {'a': 1, 'b': 2, 'c': None} == IsDict(a=1, b=2).settings(partial=True)  # (1)!
 
         assert {'b': 2, 'a': 1} == IsDict(a=1, b=2)
-        assert {'b': 2, 'a': 1} != IsDict(a=1, b=2).settings(strict=True) #(2)!
+        assert {'b': 2, 'a': 1} != IsDict(a=1, b=2).settings(strict=True)  # (2)!
 
         # combining partial and strict
-        assert {'a': 1, 'b': None, 'c': 3} == IsDict(a=1, c=3).settings(strict=True, partial=True)
-        assert {'b': None, 'c': 3, 'a': 1} != IsDict(a=1, c=3).settings(strict=True, partial=True)
+        assert {'a': 1, 'b': None, 'c': 3} == IsDict(a=1, c=3).settings(
+            strict=True, partial=True
+        )
+        assert {'b': None, 'c': 3, 'a': 1} != IsDict(a=1, c=3).settings(
+            strict=True, partial=True
+        )
         ```
 
         1. This is the same as [`IsPartialDict(a=1, b=2)`][dirty_equals.IsPartialDict]
         2. This is the same as [`IsStrictDict(a=1, b=2)`][dirty_equals.IsStrictDict]
         """
         new_cls = self.__class__(self.expected_values)
         new_cls.__dict__ = self.__dict__.copy()
@@ -93,15 +97,15 @@
             new_cls.ignore = ignore
 
         if new_cls.partial and new_cls.ignore:
             raise TypeError('partial and ignore cannot be used together')
 
         return new_cls
 
-    def equals(self, other: Dict[Any, Any]) -> bool:
+    def equals(self, other: dict[Any, Any]) -> bool:
         if not isinstance(other, dict):
             return False
 
         expected = self.expected_values
         if self.partial:
             other = {k: v for k, v in other.items() if k in expected}
 
@@ -113,15 +117,15 @@
             return False
 
         if self.strict and list(other.keys()) != list(expected.keys()):
             return False
 
         return True
 
-    def _filter_dict(self, d: Dict[Any, Any]) -> Dict[Any, Any]:
+    def _filter_dict(self, d: dict[Any, Any]) -> dict[Any, Any]:
         return {k: v for k, v in d.items() if not self._ignore_value(v)}
 
     def _ignore_value(self, v: Any) -> bool:
         # `isinstance(v, (DirtyEquals, DirtyEqualsMeta))` seems to always return `True` on pypy, no idea why
         if type(v) in (DirtyEquals, DirtyEqualsMeta):
             return False
         elif callable(self.ignore):
@@ -184,15 +188,15 @@
     `.settings(...)` can be used to customise the behaviour of `IsIgnoreDict`, in particular changing which
     values are ignored.
 
     ```py title="IsIgnoreDict"
     from dirty_equals import IsIgnoreDict
 
     assert {'a': 1, 'b': 2, 'c': None} == IsIgnoreDict(a=1, b=2)
-    assert {'a': 1, 'b': 2, 'c': None, 'c': 'ignore'} == (
+    assert {'a': 1, 'b': 2, 'c': 'ignore'} == (
         IsIgnoreDict(a=1, b=2).settings(ignore={None, 'ignore'})
     )
 
     def is_even(v: int) -> bool:
         return v % 2 == 0
 
     assert {'a': 1, 'b': 2, 'c': 3, 'd': 4} == (
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_inspection.py` & `dirty_equals-0.6.0/dirty_equals/_inspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
     def __init__(self, *expected_args: Dict[Any, Any], **expected_kwargs: Any):
         """
         Can be created from either keyword arguments or an existing dictionary (same as `dict()`).
 
         Example:
         ```py title="HasAttributes"
-        from dirty_equals import HasAttributes, IsInt, IsStr, AnyThing
+        from dirty_equals import AnyThing, HasAttributes, IsInt, IsStr
 
         class Foo:
             def __init__(self, a, b):
                 self.a = a
                 self.b = b
 
             def spam(self):
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_numeric.py` & `dirty_equals-0.6.0/dirty_equals/_numeric.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 from typing import Any, Optional, Tuple, Type, TypeVar, Union
 
 from ._base import DirtyEquals
 
 __all__ = (
@@ -36,23 +37,26 @@
 
     allowed_types: Union[Type[N], Tuple[type, ...]] = (int, float, Decimal, date, datetime)
     """It allows any of the types supported in its subclasses."""
 
     def __init__(
         self,
         *,
+        exactly: Optional[N] = None,
         approx: Optional[N] = None,
         delta: Optional[N] = None,
         gt: Optional[N] = None,
         lt: Optional[N] = None,
         ge: Optional[N] = None,
         le: Optional[N] = None,
     ):
         """
         Args:
+            exactly: A value to exactly compare to - useful when you want to make sure a value is an `int` or `float`,
+                while also checking its value.
             approx: A value to approximately compare to.
             delta: The allowable different when comparing to the value to `approx`,
                 if omitted `value / 100` is used except for datetimes where 2 seconds is used.
             gt: Value which the compared value should be greater than.
             lt: Value which the compared value should be less than.
             ge: Value which the compared value should be greater than or equal to.
             le: Value which the compared value should be less than or equal to.
@@ -60,33 +64,40 @@
         If not values are provided, only the type is checked.
 
         If `approx` is provided as well a `gt`, `lt`, `ge`, or `le`, a `TypeError` is raised.
 
         Example of direct usage:
 
         ```py title="IsNumeric"
-        from dirty_equals import IsNumeric
         from datetime import datetime
 
+        from dirty_equals import IsNumeric
+
         assert 1.0 == IsNumeric
         assert 4 == IsNumeric(gt=3)
         d = datetime(2020, 1, 1, 12, 0, 0)
         assert d == IsNumeric(approx=datetime(2020, 1, 1, 12, 0, 1))
         ```
         """
+        self.exactly: Optional[N] = exactly
+        if self.exactly is not None and (gt, lt, ge, le) != (None, None, None, None):
+            raise TypeError('"exactly" cannot be combined with "gt", "lt", "ge", or "le"')
+        if self.exactly is not None and approx is not None:
+            raise TypeError('"exactly" cannot be combined with "approx"')
         self.approx: Optional[N] = approx
-        self.delta: Optional[N] = delta
         if self.approx is not None and (gt, lt, ge, le) != (None, None, None, None):
             raise TypeError('"approx" cannot be combined with "gt", "lt", "ge", or "le"')
+        self.delta: Optional[N] = delta
         self.gt: Optional[N] = gt
         self.lt: Optional[N] = lt
         self.ge: Optional[N] = ge
         self.le: Optional[N] = le
-        self.has_bounds_checks = not all(f is None for f in (approx, delta, gt, lt, ge, le))
+        self.has_bounds_checks = not all(f is None for f in (exactly, approx, delta, gt, lt, ge, le))
         kwargs = {
+            'exactly': Omit if exactly is None else exactly,
             'approx': Omit if approx is None else approx,
             'delta': Omit if delta is None else delta,
             'gt': Omit if gt is None else gt,
             'lt': Omit if lt is None else lt,
             'ge': Omit if ge is None else ge,
             'le': Omit if le is None else le,
         }
@@ -105,15 +116,17 @@
 
         if self.has_bounds_checks:
             return self.bounds_checks(other)
         else:
             return True
 
     def bounds_checks(self, other: N) -> bool:
-        if self.approx is not None:
+        if self.exactly is not None:
+            return self.exactly == other
+        elif self.approx is not None:
             if self.delta is None:
                 if isinstance(other, date):
                     delta: Any = timedelta(seconds=2)
                 else:
                     delta = abs(other / 100)
             else:
                 delta = self.delta
@@ -175,14 +188,15 @@
 class IsPositive(IsNumber):
     """
     Check that a value is positive (`> 0`), can be an `int`, a `float` or a `Decimal`
     (or indeed any value which implements `__gt__` for `0`).
 
     ```py title="IsPositive"
     from decimal import Decimal
+
     from dirty_equals import IsPositive
 
     assert 1.0 == IsPositive
     assert 1 == IsPositive
     assert Decimal('3.14') == IsPositive
     assert 0 != IsPositive
     assert -1 != IsPositive
@@ -197,14 +211,15 @@
 class IsNegative(IsNumber):
     """
     Check that a value is negative (`< 0`), can be an `int`, a `float` or a `Decimal`
     (or indeed any value which implements `__lt__` for `0`).
 
     ```py title="IsNegative"
     from decimal import Decimal
+
     from dirty_equals import IsNegative
 
     assert -1.0 == IsNegative
     assert -1 == IsNegative
     assert Decimal('-3.14') == IsNegative
     assert 0 != IsNegative
     assert 1 != IsNegative
@@ -219,14 +234,15 @@
 class IsNonNegative(IsNumber):
     """
     Check that a value is positive or zero (`>= 0`), can be an `int`, a `float` or a `Decimal`
     (or indeed any value which implements `__ge__` for `0`).
 
     ```py title="IsNonNegative"
     from decimal import Decimal
+
     from dirty_equals import IsNonNegative
 
     assert 1.0 == IsNonNegative
     assert 1 == IsNonNegative
     assert Decimal('3.14') == IsNonNegative
     assert 0 == IsNonNegative
     assert -1 != IsNonNegative
@@ -242,14 +258,15 @@
 class IsNonPositive(IsNumber):
     """
     Check that a value is negative or zero (`<=0`), can be an `int`, a `float` or a `Decimal`
     (or indeed any value which implements `__le__` for `0`).
 
     ```py title="IsNonPositive"
     from decimal import Decimal
+
     from dirty_equals import IsNonPositive
 
     assert -1.0 == IsNonPositive
     assert -1 == IsNonPositive
     assert Decimal('-3.14') == IsNonPositive
     assert 0 == IsNonPositive
     assert 1 != IsNonPositive
@@ -273,14 +290,16 @@
     from dirty_equals import IsInt
 
     assert 1 == IsInt
     assert -2 == IsInt
     assert 1.0 != IsInt
     assert 'foobar' != IsInt
     assert True != IsInt
+    assert 1 == IsInt(exactly=1)
+    assert -2 != IsInt(exactly=1)
     ```
     """
 
     allowed_types = int
     """
     As the name suggests, only integers are allowed, booleans (`True` are `False`) are explicitly excluded although
     technically they are sub-types of `int`.
@@ -289,14 +308,15 @@
 
 class IsPositiveInt(IsInt):
     """
     Like [`IsPositive`][dirty_equals.IsPositive] but only for `int`s.
 
     ```py title="IsPositiveInt"
     from decimal import Decimal
+
     from dirty_equals import IsPositiveInt
 
     assert 1 == IsPositiveInt
     assert 1.0 != IsPositiveInt
     assert Decimal('3.14') != IsPositiveInt
     assert 0 != IsPositiveInt
     assert -1 != IsPositiveInt
@@ -310,14 +330,15 @@
 
 class IsNegativeInt(IsInt):
     """
     Like [`IsNegative`][dirty_equals.IsNegative] but only for `int`s.
 
     ```py title="IsNegativeInt"
     from decimal import Decimal
+
     from dirty_equals import IsNegativeInt
 
     assert -1 == IsNegativeInt
     assert -1.0 != IsNegativeInt
     assert Decimal('-3.14') != IsNegativeInt
     assert 0 != IsNegativeInt
     assert 1 != IsNegativeInt
@@ -336,14 +357,16 @@
     Inherits from [`IsNumeric`][dirty_equals.IsNumeric] and can therefore be initialised with any of its arguments.
 
     ```py title="IsFloat"
     from dirty_equals import IsFloat
 
     assert 1.0 == IsFloat
     assert 1 != IsFloat
+    assert 1.0 == IsFloat(exactly=1.0)
+    assert 1.001 != IsFloat(exactly=1.0)
     ```
     """
 
     allowed_types = float
     """
     As the name suggests, only floats are allowed.
     """
@@ -351,14 +374,15 @@
 
 class IsPositiveFloat(IsFloat):
     """
     Like [`IsPositive`][dirty_equals.IsPositive] but only for `float`s.
 
     ```py title="IsPositiveFloat"
     from decimal import Decimal
+
     from dirty_equals import IsPositiveFloat
 
     assert 1.0 == IsPositiveFloat
     assert 1 != IsPositiveFloat
     assert Decimal('3.14') != IsPositiveFloat
     assert 0.0 != IsPositiveFloat
     assert -1.0 != IsPositiveFloat
@@ -372,20 +396,108 @@
 
 class IsNegativeFloat(IsFloat):
     """
     Like [`IsNegative`](#isnegative) but only for `float`s.
 
     ```py title="IsNegativeFloat"
     from decimal import Decimal
+
     from dirty_equals import IsNegativeFloat
 
     assert -1.0 == IsNegativeFloat
     assert -1 != IsNegativeFloat
     assert Decimal('-3.14') != IsNegativeFloat
     assert 0.0 != IsNegativeFloat
     assert 1.0 != IsNegativeFloat
     ```
     """
 
     def __init__(self) -> None:
         super().__init__(lt=0)
         self._repr_kwargs = {}
+
+
+class IsFloatInf(IsFloat):
+    """
+    Checks that a value is float and infinite (positive or negative).
+
+    Inherits from [`IsFloat`][dirty_equals.IsFloat].
+
+    ```py title="IsFloatInf"
+    from dirty_equals import IsFloatInf
+
+    assert float('inf') == IsFloatInf
+    assert float('-inf') == IsFloatInf
+    assert 1.0 != IsFloatInf
+    ```
+    """
+
+    def equals(self, other: Any) -> bool:
+        other = self.prepare(other)
+        return math.isinf(other)
+
+
+class IsFloatInfPos(IsFloatInf):
+    """
+    Checks that a value is float and positive infinite.
+
+    Inherits from [`IsFloatInf`][dirty_equals.IsFloatInf].
+
+    ```py title="IsFloatInfPos"
+    from dirty_equals import IsFloatInfPos
+
+    assert float('inf') == IsFloatInfPos
+    assert -float('-inf') == IsFloatInfPos
+    assert -float('inf') != IsFloatInfPos
+    assert float('-inf') != IsFloatInfPos
+    ```
+    """
+
+    def __init__(self) -> None:
+        super().__init__(gt=0)
+        self._repr_kwargs = {}
+
+    def equals(self, other: Any) -> bool:
+        return self.bounds_checks(other) and super().equals(other)
+
+
+class IsFloatInfNeg(IsFloatInf):
+    """
+    Checks that a value is float and negative infinite.
+
+    Inherits from [`IsFloatInf`][dirty_equals.IsFloatInf].
+
+    ```py title="IsFloatInfNeg"
+    from dirty_equals import IsFloatInfNeg
+
+    assert -float('inf') == IsFloatInfNeg
+    assert float('-inf') == IsFloatInfNeg
+    assert float('inf') != IsFloatInfNeg
+    assert -float('-inf') != IsFloatInfNeg
+    ```
+    """
+
+    def __init__(self) -> None:
+        super().__init__(lt=0)
+        self._repr_kwargs = {}
+
+    def equals(self, other: Any) -> bool:
+        return self.bounds_checks(other) and super().equals(other)
+
+
+class IsFloatNan(IsFloat):
+    """
+    Checks that a value is float and nan (not a number).
+
+    Inherits from [`IsFloat`][dirty_equals.IsFloat].
+
+    ```py title="IsFloatNan"
+    from dirty_equals import IsFloatNan
+
+    assert float('nan') == IsFloatNan
+    assert 1.0 != IsFloatNan
+    ```
+    """
+
+    def equals(self, other: Any) -> bool:
+        other = self.prepare(other)
+        return math.isnan(other)
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_sequence.py` & `dirty_equals-0.6.0/dirty_equals/_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         Args:
             min_length: Expected length if `max_length` is not given, else minimum length.
             max_length: Expected maximum length, use an ellipsis `...` to indicate that there's no maximum.
 
         ```py title="HasLen"
         from dirty_equals import HasLen
 
-        assert [1, 2, 3] == HasLen(3) #(1)!
-        assert '123' == HasLen(3, ...) #(2)!
-        assert (1, 2, 3) == HasLen(3, 5) #(3)!
-        assert (1, 2, 3) == HasLen(0, ...) #(4)!
+        assert [1, 2, 3] == HasLen(3)  # (1)!
+        assert '123' == HasLen(3, ...)  # (2)!
+        assert (1, 2, 3) == HasLen(3, 5)  # (3)!
+        assert (1, 2, 3) == HasLen(0, ...)  # (4)!
         ```
 
         1. Length must be 3.
         2. Length must be 3 or higher.
         3. Length must be between 3 and 5 inclusive.
         4. Length is required but can take any value.
         """
@@ -121,36 +121,34 @@
         Args:
             positions (Dict[int, Any]): Instead of `*items`, a dictionary of positions and
                 values to check and be provided.
             length (Union[int, Tuple[int, Union[int, Any]]]): length constraints, int or tuple matching the arguments
                 of [`HasLen`][dirty_equals.HasLen].
 
         ```py title="IsListOrTuple"
-        from dirty_equals import IsListOrTuple, AnyThing
+        from dirty_equals import AnyThing, IsListOrTuple
 
         assert [1, 2, 3] == IsListOrTuple(1, 2, 3)
         assert (1, 3, 2) == IsListOrTuple(1, 2, 3, check_order=False)
         assert [{'a': 1}, {'a': 2}] == (
-            IsListOrTuple({'a': 2}, {'a': 1}, check_order=False) #(1)!
+            IsListOrTuple({'a': 2}, {'a': 1}, check_order=False)  # (1)!
         )
-        assert [1, 2, 3, 3] != IsListOrTuple(1, 2, 3, check_order=False) #(2)!
+        assert [1, 2, 3, 3] != IsListOrTuple(1, 2, 3, check_order=False)  # (2)!
 
-        assert [1, 2, 3, 4, 5] == IsListOrTuple(1, 2, 3, length=...) #(3)!
-        assert [1, 2, 3, 4, 5] != IsListOrTuple(1, 2, 3, length=(8, 10)) #(4)!
+        assert [1, 2, 3, 4, 5] == IsListOrTuple(1, 2, 3, length=...)  # (3)!
+        assert [1, 2, 3, 4, 5] != IsListOrTuple(1, 2, 3, length=(8, 10))  # (4)!
 
+        assert ['a', 'b', 'c', 'd'] == (IsListOrTuple(positions={2: 'c', 3: 'd'}))  # (5)!
         assert ['a', 'b', 'c', 'd'] == (
-            IsListOrTuple(positions={2: 'c', 3: 'd'}) #(5)!
-        )
-        assert ['a', 'b', 'c', 'd'] == (
-            IsListOrTuple(positions={2: 'c', 3: 'd'}, length=4) #(6)!
+            IsListOrTuple(positions={2: 'c', 3: 'd'}, length=4)  # (6)!
         )
 
-        assert [1, 2, 3, 4] == IsListOrTuple(3, check_order=False, length=(0, ...)) #(7)!
+        assert [1, 2, 3, 4] == IsListOrTuple(3, check_order=False, length=(0, ...))  # (7)!
 
-        assert [1, 2, 3] == IsListOrTuple(AnyThing, AnyThing, 3) #(8)!
+        assert [1, 2, 3] == IsListOrTuple(AnyThing, AnyThing, 3)  # (8)!
         ```
 
         1. Unlike using sets for comparison, we can do order-insensitive comparisons on objects that are not hashable.
         2. And we won't get caught out by duplicate values
         3. Here we're just checking the first 3 items, the compared list or tuple can be of any length
         4. Compared list is not long enough
         5. Compare using `positions`, here no length if enforced
@@ -180,15 +178,15 @@
         super().__init__(
             *items,
             positions=Omit if positions is None else positions,
             length=_length_repr(self.length),
             check_order=self.check_order and Omit,
         )
 
-    def equals(self, other: Any) -> bool:  # noqa: C901
+    def equals(self, other: Any) -> bool:
         if not isinstance(other, self.allowed_type):
             return False
 
         if not _length_correct(self.length, other):
             return False
 
         if self.check_order:
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_strings.py` & `dirty_equals-0.6.0/dirty_equals/_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ._base import DirtyEquals
 from ._utils import Omit, plain_repr
 
 try:
     from typing import Literal
 except ImportError:
-    from typing_extensions import Literal  # type: ignore[misc]
+    from typing_extensions import Literal  # type: ignore[assignment]
 
 T = TypeVar('T', str, bytes)
 
 __all__ = 'IsStr', 'IsBytes', 'IsAnyStr'
 
 
 class IsAnyStr(DirtyEquals[T]):
@@ -47,15 +47,15 @@
         ```py title="IsAnyStr"
         from dirty_equals import IsAnyStr
 
         assert 'foobar' == IsAnyStr()
         assert b'foobar' == IsAnyStr()
         assert 123 != IsAnyStr()
         assert 'foobar' == IsAnyStr(regex='foo...')
-        assert 'foobar' == IsAnyStr(regex=b'foo...') #(1)!
+        assert 'foobar' == IsAnyStr(regex=b'foo...')  # (1)!
 
         assert 'foobar' == IsAnyStr(min_length=6)
         assert 'foobar' != IsAnyStr(min_length=8)
 
         assert 'foobar' == IsAnyStr(case='lower')
         assert 'Foobar' != IsAnyStr(case='lower')
         ```
```

### Comparing `dirty_equals-0.5.0/dirty_equals/_utils.py` & `dirty_equals-0.6.0/dirty_equals/_utils.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/index.md` & `dirty_equals-0.6.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="/img/logo-text.svg" alt="dirty-equals">
+  <img src="./img/logo-text.svg" alt="dirty-equals">
 </p>
 <p align="center">
   <em>Doing dirty (but extremely useful) things with equals.</em>
 </p>
 <p align="center">
   <a href="https://github.com/samuelcolvin/dirty-equals/actions?query=event%3Apush+branch%3Amain+workflow%3ACI">
     <img src="https://github.com/samuelcolvin/dirty-equals/workflows/CI/badge.svg?event=push" alt="CI">
@@ -32,42 +32,42 @@
 *dirty-equals* can be used in whatever context you like, but it comes into its own when writing unit tests for
 applications where you're commonly checking the response to API calls and the contents of a database.
 
 ## Usage
 
 Here's a trivial example of what *dirty-equals* can do:
 
-```{.py title="Trival Usage" test="false"}
+```{.py title="Trival Usage" test="skip"}
 from dirty_equals import IsPositive
 
-assert 1 == IsPositive #(1)!
+assert 1 == IsPositive  # (1)!
 assert -2 == IsPositive  # this will fail! (2)
 ```
 
 1. This `assert` will pass since `1` is indeed positive, so the result of `1 == IsPositive` is `True`.
 2. This will fail (raise a `AssertionError`) since `-2` is not positive,
    so the result of `-2 == IsPositive` is `False`.
 
 **Not that interesting yet!**, but consider the following unit test code using **dirty-equals**:
 
-```py
-title="More Powerful Usage"
+```{.py title="More Powerful Usage" lint="skip"}
 from dirty_equals import IsJson, IsNow, IsPositiveInt, IsStr
 
+
 def test_user_endpoint(client: 'HttpClient', db_conn: 'Database'):
-   client.pust('/users/create/', data=...)
+    client.pust('/users/create/', data=...)
 
-   user_data = db_conn.fetchrow('select * from users')
-   assert user_data == {
-       'id': IsPositiveInt, #(1)!
-       'username': 'samuelcolvin', #(2)!
-       'avatar_file': IsStr(regex=r'/[a-z0-9\-]{10}/example\.png'), #(3)!
-       'settings_json': IsJson({'theme': 'dark', 'language': 'en'}), #(4)!
-       'created_ts': IsNow(delta=3), #(5)!
-   }
+    user_data = db_conn.fetchrow('select * from users')
+    assert user_data == {
+        'id': IsPositiveInt,  # (1)!
+        'username': 'samuelcolvin',  # (2)!
+        'avatar_file': IsStr(regex=r'/[a-z0-9\-]{10}/example\.png'),  # (3)!
+        'settings_json': IsJson({'theme': 'dark', 'language': 'en'}),  # (4)!
+        'created_ts': IsNow(delta=3),  # (5)!
+    }
 ```
 
 1. We don't actually care what the `id` is, just that it's present, it's an `int` and it's positive.
 2. We can use a normal key and value here since we know exactly what value `username` should have before we test it.
 3. `avatar_file` is a string, but we don't know all of the string before the `assert`,
    just the format (regex) it should match.
 4. `settings_json` is a `JSON` string, but it's simpler and more robust to confirm it represents a particular python
```

#### html2text {}

```diff
@@ -3,42 +3,42 @@
                   [CI] [Coverage] [pypi] [versions] [license]
 --- {{ version }} **dirty-equals** is a python library that (mis)uses the
 `__eq__` method to make python code (generally unit tests) more declarative and
 therefore easier to read and write. *dirty-equals* can be used in whatever
 context you like, but it comes into its own when writing unit tests for
 applications where you're commonly checking the response to API calls and the
 contents of a database. ## Usage Here's a trivial example of what *dirty-
-equals* can do: ```{.py title="Trival Usage" test="false"} from dirty_equals
-import IsPositive assert 1 == IsPositive #(1)! assert -2 == IsPositive # this
+equals* can do: ```{.py title="Trival Usage" test="skip"} from dirty_equals
+import IsPositive assert 1 == IsPositive # (1)! assert -2 == IsPositive # this
 will fail! (2) ``` 1. This `assert` will pass since `1` is indeed positive, so
 the result of `1 == IsPositive` is `True`. 2. This will fail (raise a
 `AssertionError`) since `-2` is not positive, so the result of `-2 ==
 IsPositive` is `False`. **Not that interesting yet!**, but consider the
-following unit test code using **dirty-equals**: ```py title="More Powerful
-Usage" from dirty_equals import IsJson, IsNow, IsPositiveInt, IsStr def
-test_user_endpoint(client: 'HttpClient', db_conn: 'Database'): client.pust('/
-users/create/', data=...) user_data = db_conn.fetchrow('select * from users')
-assert user_data == { 'id': IsPositiveInt, #(1)! 'username': 'samuelcolvin', #
-(2)! 'avatar_file': IsStr(regex=r'/[a-z0-9\-]{10}/example\.png'), #(3)!
-'settings_json': IsJson({'theme': 'dark', 'language': 'en'}), #(4)!
-'created_ts': IsNow(delta=3), #(5)! } ``` 1. We don't actually care what the
-`id` is, just that it's present, it's an `int` and it's positive. 2. We can use
-a normal key and value here since we know exactly what value `username` should
-have before we test it. 3. `avatar_file` is a string, but we don't know all of
-the string before the `assert`, just the format (regex) it should match. 4.
-`settings_json` is a `JSON` string, but it's simpler and more robust to confirm
-it represents a particular python object rather than compare strings. 5.
-`created_at` is a `datetime`, although we don't know (or care) about its exact
-value; since the user was just created we know it must be close to now. `delta`
-is optional, it defaults to 2 seconds. Without **dirty-equals**, you'd have to
-compare individual fields and/or modify some fields before comparison - the
-test would not be declarative or as clear. **dirty-equals** can do so much more
-than that, for example: * [`IsPartialDict`][dirty_equals.IsPartialDict] lets
-you compare a subset of a dictionary * [`IsStrictDict`]
-[dirty_equals.IsStrictDict] lets you confirm order in a dictionary * [`IsList`]
-[dirty_equals.IsList] and [`IsTuple`][dirty_equals.IsTuple] lets you compare
-partial lists and tuples, with or without order constraints * nesting any of
-these types inside any others * [`IsInstance`][dirty_equals.IsInstance] lets
-you simply confirm the type of an object * You can even use [boolean operators]
-(./usage.md#boolean-logic) `|` and `&` to combine multiple conditions * and
-much more... ## Installation Simply: ```bash pip install dirty-equals ```
-**dirty-equals** requires **Python 3.7+**.
+following unit test code using **dirty-equals**: ```{.py title="More Powerful
+Usage" lint="skip"} from dirty_equals import IsJson, IsNow, IsPositiveInt,
+IsStr def test_user_endpoint(client: 'HttpClient', db_conn: 'Database'):
+client.pust('/users/create/', data=...) user_data = db_conn.fetchrow('select *
+from users') assert user_data == { 'id': IsPositiveInt, # (1)! 'username':
+'samuelcolvin', # (2)! 'avatar_file': IsStr(regex=r'/[a-z0-9\-]{10}/
+example\.png'), # (3)! 'settings_json': IsJson({'theme': 'dark', 'language':
+'en'}), # (4)! 'created_ts': IsNow(delta=3), # (5)! } ``` 1. We don't actually
+care what the `id` is, just that it's present, it's an `int` and it's positive.
+2. We can use a normal key and value here since we know exactly what value
+`username` should have before we test it. 3. `avatar_file` is a string, but we
+don't know all of the string before the `assert`, just the format (regex) it
+should match. 4. `settings_json` is a `JSON` string, but it's simpler and more
+robust to confirm it represents a particular python object rather than compare
+strings. 5. `created_at` is a `datetime`, although we don't know (or care)
+about its exact value; since the user was just created we know it must be close
+to now. `delta` is optional, it defaults to 2 seconds. Without **dirty-
+equals**, you'd have to compare individual fields and/or modify some fields
+before comparison - the test would not be declarative or as clear. **dirty-
+equals** can do so much more than that, for example: * [`IsPartialDict`]
+[dirty_equals.IsPartialDict] lets you compare a subset of a dictionary *
+[`IsStrictDict`][dirty_equals.IsStrictDict] lets you confirm order in a
+dictionary * [`IsList`][dirty_equals.IsList] and [`IsTuple`]
+[dirty_equals.IsTuple] lets you compare partial lists and tuples, with or
+without order constraints * nesting any of these types inside any others *
+[`IsInstance`][dirty_equals.IsInstance] lets you simply confirm the type of an
+object * You can even use [boolean operators](./usage.md#boolean-logic) `|` and
+`&` to combine multiple conditions * and much more... ## Installation Simply:
+```bash pip install dirty-equals ``` **dirty-equals** requires **Python 3.7+**.
```

### Comparing `dirty_equals-0.5.0/docs/internals.md` & `dirty_equals-0.6.0/docs/internals.md`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/plugins.py` & `dirty_equals-0.6.0/docs/plugins.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,31 +11,15 @@
 except ImportError:
     pytest = None
 
 logger = logging.getLogger('mkdocs.test_examples')
 
 
 def on_pre_build(config: Config):
-    test_examples()
-
-
-def test_examples():
-    """
-    Run the examples tests.
-    """
-    try:
-        run_pytest = getattr('pytest', 'main')
-    except AttributeError:
-        logger.info('pytest not installed, skipping examples tests')
-    else:
-        logger.info('running examples tests...')
-        return_code = run_pytest(['-q', '-p', 'no:sugar', 'tests/test_docs.py'])
-        if return_code != 0:
-            logger.warning('examples tests failed')
-
+    pass
 
 def on_files(files: Files, config: Config) -> Files:
     return remove_files(files)
 
 
 def remove_files(files: Files) -> Files:
     to_remove = []
@@ -49,28 +33,25 @@
     for f in to_remove:
         files.remove(f)
 
     return files
 
 
 def on_page_markdown(markdown: str, page: Page, config: Config, files: Files) -> str:
-    markdown = reinstate_code_titles(markdown)
     return add_version(markdown, page)
 
 
-def reinstate_code_titles(markdown: str) -> str:
-    """
-    Fix titles in code blocks, see https://youtrack.jetbrains.com/issue/PY-53246.
-    """
-    return re.sub(r'^(```py)\s*\ntitle=', r'\1 title=', markdown, flags=re.M)
-
-
 def add_version(markdown: str, page: Page) -> str:
-    if page.abs_url == '/':
+    if page.file.src_uri == 'index.md':
         version_ref = os.getenv('GITHUB_REF')
-        if version_ref:
+        if version_ref and version_ref.startswith('refs/tags/'):
             version = re.sub('^refs/tags/', '', version_ref.lower())
-            version_str = f'Documentation for version: **{version}**'
+            url = f'https://github.com/samuelcolvin/dirty-equals/releases/tag/{version}'
+            version_str = f'Documentation for version: [{version}]({url})'
+        elif sha := os.getenv('GITHUB_SHA'):
+            sha = sha[:7]
+            url = f'https://github.com/samuelcolvin/dirty-equals/commit/{sha}'
+            version_str = f'Documentation for development version: [{sha}]({url})'
         else:
             version_str = 'Documentation for development version'
         markdown = re.sub(r'{{ *version *}}', version_str, markdown)
     return markdown
```

### Comparing `dirty_equals-0.5.0/docs/usage.md` & `dirty_equals-0.6.0/docs/usage.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 *dirty-equals* types can be combined based on either `&`
 (and, all checks must be `True` for the combined check to be `True`) or `|`
 (or, any check can be `True` for the combined check to be `True`).
 
 Types can also be inverted using the `~` operator, this is equivalent to using `!=` instead of `==`.
 
 Example:
-```py
-title="Boolean Combination of Types"
-from dirty_equals import HasLen, Contains
+```py title="Boolean Combination of Types"
+from dirty_equals import Contains, HasLen
 
-assert ['a', 'b', 'c'] == HasLen(3) & Contains('a') #(1)!
-assert ['a', 'b', 'c'] == HasLen(3) | Contains('z') #(2)!
+assert ['a', 'b', 'c'] == HasLen(3) & Contains('a')  # (1)!
+assert ['a', 'b', 'c'] == HasLen(3) | Contains('z')  # (2)!
 
 assert ['a', 'b', 'c'] != Contains('z')
 assert ['a', 'b', 'c'] == ~Contains('z')
 ```
 
 1. The object on the left has to both have length 3 **and** contain `"a"`
 2. The object on the left has to either have length 3 **or** contain `"z"`
@@ -29,16 +28,15 @@
 
 *dirty-equals* allows comparison with types regardless of whether they've been initialised.
 
 This saves users adding `()` in lots of places.
 
 Example:
 
-```py
-title="Initialised vs. Uninitialised"
+```py title="Initialised vs. Uninitialised"
 from dirty_equals import IsInt
 
 # these two cases are the same
 assert 1 == IsInt
 assert 1 == IsInt()
 ```
 
@@ -47,48 +45,47 @@
     cannot be used like this, comparisons will just return `False`.
 
 ## `__repr__` and pytest compatibility
 
 dirty-equals types have reasonable `__repr__` methods, which describe types and generally are a close match
 of how they would be created:
 
-```py
-title="__repr__"
-from dirty_equals import IsInt, IsApprox
+```py title="__repr__"
+from dirty_equals import IsApprox, IsInt
 
 assert repr(IsInt) == 'IsInt'
 assert repr(IsInt()) == 'IsInt()'
 assert repr(IsApprox(42)) == 'IsApprox(approx=42)'
 ```
 
 However the repr method of types changes when an equals (`==`) operation on them returns a `True`, in this case
 the `__repr__` method will return `repr(other)`.
 
-```py
-title="repr() after comparison"
+```py title="repr() after comparison"
 from dirty_equals import IsInt
 
 v = IsInt()
 assert 42 == v
 assert repr(v) == '42'
 ```
 
 This black magic is designed to make the output of pytest when asserts on large objects fail as simple as
 possible to read.
 
 Consider the following unit test:
 
-```py
-title="pytest error example"
+```py title="pytest error example"
 from datetime import datetime
-from dirty_equals import IsPositiveInt, IsNow
+
+from dirty_equals import IsNow, IsPositiveInt
+
 
 def test_partial_dict():
     api_response_data = {
-        'id': 1, #(1)!
+        'id': 1,  # (1)!
         'first_name': 'John',
         'last_name': 'Doe',
         'created_at': datetime.now().isoformat(),
         'phone': '+44 123456789',
     }
 
     assert api_response_data == {
```

### Comparing `dirty_equals-0.5.0/docs/img/dirty-equals-logo-base.svg` & `dirty_equals-0.6.0/docs/img/dirty-equals-logo-base.svg`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/img/dirty-equals-logo-favicon.svg` & `dirty_equals-0.6.0/docs/img/dirty-equals-logo-favicon.svg`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/img/favicon.png` & `dirty_equals-0.6.0/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/img/logo-text.svg` & `dirty_equals-0.6.0/docs/img/logo-text.svg`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/img/logo-white.svg` & `dirty_equals-0.6.0/docs/img/logo-white.svg`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/docs/types/custom.md` & `dirty_equals-0.6.0/docs/types/custom.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # Custom Types
 
 ::: dirty_equals._base.DirtyEquals
-    rendering:
+    options:
       merge_init_into_class: false
 
 ## Custom Type Example
 
 To demonstrate the use of custom types, we'll create a custom type that matches any even number.
 
 We won't inherit from [`IsNumeric`][dirty_equals.IsNumeric] in this case to keep the example simple.
 
-```py
-title="IsEven"
+```py title="IsEven"
 from decimal import Decimal
 from typing import Any, Union
-from dirty_equals import IsOneOf
-from dirty_equals import DirtyEquals
+
+from dirty_equals import DirtyEquals, IsOneOf
+
 
 class IsEven(DirtyEquals[Union[int, float, Decimal]]):
     def equals(self, other: Any) -> bool:
         return other % 2 == 0
 
+
 assert 2 == IsEven
 assert 3 != IsEven
 assert 'foobar' != IsEven
 assert 3 == IsEven | IsOneOf(3)
 ```
 
 There are a few advantages of inheriting from [`DirtyEquals`][dirty_equals.DirtyEquals] compared to just
```

### Comparing `dirty_equals-0.5.0/docs/types/datetime.md` & `dirty_equals-0.6.0/docs/types/datetime.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     * if the datetime wrapped by `IsDatetime` is timezone naive, the compared value can either be naive or have a
       timezone all that matters is the datetime values match.
     * if the datetime wrapped by `IsDatetime` has a timezone, the compared value needs to represent the same point in
       time - either way it must have a timezone.
 
 Example
 
-```py
-title="IsDatetime & timezones"
+```py title="IsDatetime & timezones"
 from datetime import datetime
 
-from dirty_equals import IsDatetime
 import pytz
 
+from dirty_equals import IsDatetime
+
 tz_london = pytz.timezone('Europe/London')
 new_year_london = tz_london.localize(datetime(2000, 1, 1))
 
 tz_nyc = pytz.timezone('America/New_York')
 new_year_eve_nyc = tz_nyc.localize(datetime(1999, 12, 31, 19, 0, 0))
 
 assert new_year_eve_nyc == IsDatetime(approx=new_year_london, enforce_tz=False)
```

### Comparing `dirty_equals-0.5.0/docs/types/numeric.md` & `dirty_equals-0.6.0/docs/types/numeric.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 # Numeric Types
 
 ::: dirty_equals.IsInt
-    rendering:
+    options:
       merge_init_into_class: false
       separate_signature: false
 
 ::: dirty_equals.IsFloat
-    rendering:
+    options:
       merge_init_into_class: false
       separate_signature: false
 
 ::: dirty_equals.IsPositive
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsNegative
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsNonNegative
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsNonPositive
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsPositiveInt
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsNegativeInt
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsPositiveFloat
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsNegativeFloat
-    rendering:
+    options:
+      merge_init_into_class: false
+
+::: dirty_equals.IsFloatInf
+    options:
+      merge_init_into_class: false
+
+::: dirty_equals.IsFloatInfPos
+    options:
+      merge_init_into_class: false
+
+::: dirty_equals.IsFloatInfNeg
+    options:
+      merge_init_into_class: false
+
+::: dirty_equals.IsFloatNan
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsApprox
 
 ::: dirty_equals.IsNumber
-    rendering:
+    options:
       merge_init_into_class: false
 
 ::: dirty_equals.IsNumeric
```

### Comparing `dirty_equals-0.5.0/requirements/docs.txt` & `dirty_equals-0.6.0/requirements/docs.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,115 @@
 #
 # This file is autogenerated by pip-compile with python 3.10
 # To update, run:
 #
 #    pip-compile --output-file=requirements/docs.txt requirements/docs.in
 #
-black==22.6.0
+black==23.3.0
     # via -r requirements/docs.in
+certifi==2022.12.7
+    # via requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via
     #   black
     #   mkdocs
+colorama==0.4.6
+    # via
+    #   griffe
+    #   mkdocs-material
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.22.0
+griffe==0.27.1
     # via mkdocstrings-python
-importlib-metadata==4.12.0
-    # via mkdocs
+idna==3.4
+    # via requests
+importlib-metadata==6.6.0
+    # via mike
+importlib-resources==5.12.0
+    # via mike
 jinja2==3.1.2
     # via
+    #   mike
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via
     #   jinja2
     #   mkdocstrings
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.3.1
+mike @ git+https://github.com/jimporter/mike.git
+    # via -r requirements/docs.in
+mkdocs==1.4.2
     # via
     #   -r requirements/docs.in
+    #   mike
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocs-simple-hooks
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-material==8.4.1
+mkdocs-material==9.1.8
     # via -r requirements/docs.in
-mkdocs-material-extensions==1.0.3
+mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 mkdocs-simple-hooks==0.1.5
     # via -r requirements/docs.in
-mkdocstrings[python]==0.19.0
+mkdocstrings[python]==0.21.2
     # via
     #   -r requirements/docs.in
     #   mkdocstrings-python
-mkdocstrings-python==0.7.1
+mkdocstrings-python==0.9.0
     # via mkdocstrings
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via black
-packaging==21.3
-    # via mkdocs
-pathspec==0.9.0
+packaging==23.1
+    # via
+    #   black
+    #   mkdocs
+pathspec==0.11.1
     # via black
-platformdirs==2.5.2
+platformdirs==3.4.0
     # via black
-pygments==2.13.0
+pygments==2.15.1
     # via mkdocs-material
-pymdown-extensions==9.5
+pymdown-extensions==9.11
     # via
     #   mkdocs-material
     #   mkdocstrings
-pyparsing==3.0.9
-    # via packaging
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
+    #   mike
     #   mkdocs
+    #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
+regex==2023.3.23
+    # via mkdocs-material
+requests==2.29.0
+    # via mkdocs-material
 six==1.16.0
     # via python-dateutil
 tomli==2.0.1
     # via black
-watchdog==2.1.9
+urllib3==1.26.15
+    # via requests
+verspec==0.1.0
+    # via mike
+watchdog==3.0.0
     # via mkdocs
-zipp==3.8.1
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `dirty_equals-0.5.0/requirements/linting.txt` & `dirty_equals-0.6.0/requirements/linting.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,57 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --output-file=requirements/linting.txt requirements/linting.in
 #
-black==22.6.0
+black==23.3.0
     # via -r requirements/linting.in
 cfgv==3.3.1
     # via pre-commit
 click==8.1.3
     # via black
-colorama==0.4.5
-    # via isort
 distlib==0.3.6
     # via virtualenv
-filelock==3.8.0
+filelock==3.12.0
     # via virtualenv
-flake8==5.0.4
-    # via
-    #   -r requirements/linting.in
-    #   flake8-quotes
-flake8-quotes==3.3.1
-    # via -r requirements/linting.in
-identify==2.5.3
+identify==2.5.23
     # via pre-commit
-isort[colors]==5.10.1
-    # via -r requirements/linting.in
-mccabe==0.7.0
-    # via flake8
-mypy==0.971
+mypy==1.2.0
     # via -r requirements/linting.in
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
-pathspec==0.9.0
+packaging==23.1
     # via black
-platformdirs==2.5.2
+pathspec==0.11.1
+    # via black
+platformdirs==3.4.0
     # via
     #   black
     #   virtualenv
-pre-commit==2.20.0
+pre-commit==3.2.2
+    # via -r requirements/linting.in
+pydantic==1.10.7
     # via -r requirements/linting.in
-pycodestyle==2.9.1
-    # via
-    #   -r requirements/linting.in
-    #   flake8
-pyflakes==2.5.0
-    # via
-    #   -r requirements/linting.in
-    #   flake8
 pyyaml==6.0
     # via pre-commit
-toml==0.10.2
-    # via pre-commit
+ruff==0.0.263
+    # via -r requirements/linting.in
 tomli==2.0.1
     # via
     #   black
     #   mypy
-types-pytz==2022.2.1.0
+types-pytz==2023.3.0.0
     # via -r requirements/linting.in
-typing-extensions==4.3.0
-    # via mypy
-virtualenv==20.16.4
+typing-extensions==4.5.0
+    # via
+    #   mypy
+    #   pydantic
+virtualenv==20.22.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `dirty_equals-0.5.0/tests/test_base.py` & `dirty_equals-0.6.0/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import platform
 
+import packaging.version
 import pytest
 
 from dirty_equals import Contains, IsApprox, IsInt, IsNegative, IsOneOf, IsPositive, IsStr
+from dirty_equals.version import VERSION
 
 
 def test_or():
     assert 'foo' == IsStr | IsInt
     assert 1 == IsStr | IsInt
     assert -1 == IsStr | IsNegative | IsPositive
 
@@ -132,7 +134,11 @@
         ([1, 2, 3], Contains(1) | IsOneOf([])),
         ([], Contains(1) | IsOneOf([])),
         ([2], ~(Contains(1) | IsOneOf([]))),
     ],
 )
 def test_is_one_of(value, dirty):
     assert value == dirty
+
+
+def test_version():
+    packaging.version.parse(VERSION)
```

### Comparing `dirty_equals-0.5.0/tests/test_boolean.py` & `dirty_equals-0.6.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/tests/test_datetime.py` & `dirty_equals-0.6.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/tests/test_dict.py` & `dirty_equals-0.6.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/tests/test_inspection.py` & `dirty_equals-0.6.0/tests/test_inspection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import platform
+import sys
+
 import pytest
 
 from dirty_equals import AnyThing, HasAttributes, HasName, HasRepr, IsInstance, IsInt, IsStr
 
 
 class Foo:
     def __init__(self, a=1, b=2):
@@ -66,22 +69,28 @@
     ],
     ids=dirty_repr,
 )
 def test_has_name(value, dirty):
     assert value == dirty
 
 
+pypy38 = pytest.mark.skipif(
+    platform.python_implementation() == 'PyPy' and sys.version_info[:2] == (3, 8),
+    reason='pypy3.8 fails with this specific case 🤷',
+)
+
+
 @pytest.mark.parametrize(
     'value,dirty',
     [
         (Foo(1, 2), HasAttributes(a=1, b=2)),
         (Foo(1, 's'), HasAttributes(a=IsInt(), b=IsStr())),
         (Foo(1, 2), ~HasAttributes(a=IsInt(), b=IsStr())),
         (Foo(1, 2), ~HasAttributes(a=1, b=2, c=3)),
-        (Foo(1, 2), HasAttributes(a=1, b=2, spam=AnyThing)),
+        pytest.param(Foo(1, 2), HasAttributes(a=1, b=2, spam=AnyThing), marks=pypy38),
         (Foo(1, 2), ~HasAttributes(a=1, b=2, missing=AnyThing)),
     ],
     ids=dirty_repr,
 )
 def test_has_attributes(value, dirty):
     assert value == dirty
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dirty_equals-0.5.0/tests/test_list_tuple.py` & `dirty_equals-0.6.0/tests/test_list_tuple.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/tests/test_other.py` & `dirty_equals-0.6.0/tests/test_other.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import uuid
+from hashlib import md5, sha1, sha256
 from ipaddress import IPv4Address, IPv4Network, IPv6Address, IPv6Network
 
 import pytest
 
-from dirty_equals import FunctionCheck, IsIP, IsJson, IsUUID
+from dirty_equals import FunctionCheck, IsHash, IsIP, IsJson, IsUrl, IsUUID
 
 
 @pytest.mark.parametrize(
     'other,dirty',
     [
         (uuid.uuid4(), IsUUID()),
         (uuid.uuid4(), IsUUID),
@@ -179,7 +180,103 @@
         assert '123' == is_ip
     assert str(is_ip) == 'IsIP()'
 
 
 def test_ip_bad_netmask():
     with pytest.raises(TypeError, match='To check the netmask you must specify the IP version'):
         IsIP(netmask='255.255.255.0')
+
+
+@pytest.mark.parametrize(
+    'other,dirty',
+    [
+        ('f1e069787ECE74531d112559945c6871', IsHash('md5')),
+        ('40bd001563085fc35165329ea1FF5c5ecbdbbeef', IsHash('sha-1')),
+        ('a665a45920422f9d417e4867eFDC4fb8a04a1f3fff1fa07e998e86f7f7a27ae3', IsHash('sha-256')),
+        (b'f1e069787ECE74531d112559945c6871', IsHash('md5')),
+        (bytearray(b'f1e069787ECE74531d112559945c6871'), IsHash('md5')),
+    ],
+)
+def test_is_hash_true(other, dirty):
+    assert other == dirty
+
+
+@pytest.mark.parametrize(
+    'other,dirty',
+    [
+        ('foobar', IsHash('md5')),
+        (b'\x81 UnicodeDecodeError', IsHash('md5')),
+        ([1, 2, 3], IsHash('sha-1')),
+        ('f1e069787ECE74531d112559945c6871d', IsHash('md5')),
+        ('400bd001563085fc35165329ea1FF5c5ecbdbbeef', IsHash('sha-1')),
+        ('a665a45920422g9d417e4867eFDC4fb8a04a1f3fff1fa07e998e86f7f7a27ae3', IsHash('sha-256')),
+    ],
+)
+def test_is_hash_false(other, dirty):
+    assert other != dirty
+
+
+@pytest.mark.parametrize(
+    'hash_type',
+    ['md5', 'sha-1', 'sha-256'],
+)
+def test_is_hash_md5_false_repr(hash_type):
+    is_hash = IsHash(hash_type)
+    with pytest.raises(AssertionError):
+        assert '123' == is_hash
+    assert str(is_hash) == f"IsHash('{hash_type}')"
+
+
+@pytest.mark.parametrize(
+    'hash_func, hash_type',
+    [(md5, 'md5'), (sha1, 'sha-1'), (sha256, 'sha-256')],
+)
+def test_hashlib_hashes(hash_func, hash_type):
+    assert hash_func(b'dirty equals').hexdigest() == IsHash(hash_type)
+
+
+def test_wrong_hash_type():
+    with pytest.raises(ValueError, match='Hash type must be one of the following values: md5, sha-1, sha-256'):
+        assert '123' == IsHash('ntlm')
+
+
+@pytest.mark.parametrize(
+    'other,dirty',
+    [
+        ('https://example.com', IsUrl),
+        ('https://example.com', IsUrl(scheme='https')),
+        ('postgres://user:pass@localhost:5432/app', IsUrl(postgres_dsn=True)),
+    ],
+)
+def test_is_url_true(other, dirty):
+    assert other == dirty
+
+
+@pytest.mark.parametrize(
+    'other,dirty',
+    [
+        ('https://example.com', IsUrl(postgres_dsn=True)),
+        ('https://example.com', IsUrl(scheme='http')),
+        ('definitely not a url', IsUrl),
+        (42, IsUrl),
+        ('https://anotherexample.com', IsUrl(postgres_dsn=True)),
+    ],
+)
+def test_is_url_false(other, dirty):
+    assert other != dirty
+
+
+def test_is_url_invalid_kwargs():
+    with pytest.raises(
+        TypeError,
+        match='IsURL only checks these attributes: scheme, host, host_type, user, password, tld, port, path, query, '
+        'fragment',
+    ):
+        IsUrl(https=True)
+
+
+def test_is_url_too_many_url_types():
+    with pytest.raises(
+        ValueError,
+        match='You can only check against one Pydantic url type at a time',
+    ):
+        assert 'https://example.com' == IsUrl(any_url=True, http_url=True, postgres_dsn=True)
```

### Comparing `dirty_equals-0.5.0/tests/test_strings.py` & `dirty_equals-0.6.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/LICENSE` & `dirty_equals-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/README.md` & `dirty_equals-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dirty_equals-0.5.0/pyproject.toml` & `dirty_equals-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,32 +25,42 @@
     'Environment :: MacOS X',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
     'Typing :: Typed',
 ]
 requires-python = '>=3.7'
 dependencies = [
-    'typing-extensions>=4.0.1',
+    'typing-extensions>=4.0.1;python_version<"3.8"',
     'pytz>=2021.3',
 ]
+optional-dependencies = {pydantic = ['pydantic>=1.9.1'] }
 dynamic = ['version']
 
 [project.urls]
 Homepage = 'https://github.com/samuelcolvin/dirty-equals'
 Documentation = 'https://dirty-equals.helpmanual.io'
 Funding = 'https://github.com/sponsors/samuelcolvin'
 Source = 'https://github.com/samuelcolvin/dirty-equals'
 Changelog = 'https://github.com/samuelcolvin/dirty-equals/releases'
 
+[tool.ruff]
+line-length = 120
+extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
+flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
+mccabe = { max-complexity = 14 }
+isort = { known-first-party = ['tests'] }
+target-version = 'py37'
+
 [tool.pytest.ini_options]
 testpaths = "tests"
 filterwarnings = "error"
 
 [tool.coverage.run]
 source = ["dirty_equals"]
 branch = true
```

### Comparing `dirty_equals-0.5.0/PKG-INFO` & `dirty_equals-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirty-equals
-Version: 0.5.0
+Version: 0.6.0
 Summary: Doing dirty (but extremely useful) things with equals.
 Project-URL: Homepage, https://github.com/samuelcolvin/dirty-equals
 Project-URL: Documentation, https://dirty-equals.helpmanual.io
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/samuelcolvin/dirty-equals
 Project-URL: Changelog, https://github.com/samuelcolvin/dirty-equals/releases
 Author-email: Samuel Colvin <s@muelcolvin.com>
@@ -25,14 +25,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
@@ -42,20 +43,23 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: pytz>=2021.3
-Requires-Dist: typing-extensions>=4.0.1
+Requires-Dist: typing-extensions>=4.0.1; python_version < '3.8'
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=1.9.1; extra == 'pydantic'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://dirty-equals.helpmanual.io">
     <img src="https://dirty-equals.helpmanual.io/img/logo-text.svg" alt="dirty-equals">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dirty-equals Version: 0.5.0 Summary: Doing dirty
+Metadata-Version: 2.1 Name: dirty-equals Version: 0.6.0 Summary: Doing dirty
 (but extremely useful) things with equals. Project-URL: Homepage, https://
 github.com/samuelcolvin/dirty-equals Project-URL: Documentation, https://dirty-
 equals.helpmanual.io Project-URL: Funding, https://github.com/sponsors/
 samuelcolvin Project-URL: Source, https://github.com/samuelcolvin/dirty-equals
 Project-URL: Changelog, https://github.com/samuelcolvin/dirty-equals/releases
 Author-email: Samuel Colvin
 muelcolvin.com> License: The MIT License (MIT) Copyright (c) 2022 Samuel Colvin
@@ -15,29 +15,31 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Environment :: MacOS X
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+DEALINGS IN THE SOFTWARE. License-File: LICENSE Classifier: Development Status
+:: 4 - Beta Classifier: Environment :: Console Classifier: Environment :: MacOS
+X Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Classifier: Typing :: Typed Requires-Python: >=3.7 Requires-
-Dist: pytz>=2021.3 Requires-Dist: typing-extensions>=4.0.1 Description-Content-
-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed Requires-Python: >=3.7 Requires-Dist: pytz>=2021.3
+Requires-Dist: typing-extensions>=4.0.1; python_version < '3.8' Provides-Extra:
+pydantic Requires-Dist: pydantic>=1.9.1; extra == 'pydantic' Description-
+Content-Type: text/markdown
                                 [dirty-equals]
             Doing dirty (but extremely useful) things with equals.
                   [CI] [Coverage] [pypi] [versions] [license]
 --- **Documentation**: [dirty-equals.helpmanual.io](https://dirty-
 equals.helpmanual.io) **Source Code**: [github.com/samuelcolvin/dirty-equals]
 (https://github.com/samuelcolvin/dirty-equals) --- **dirty-equals** is a python
 library that (mis)uses the `__eq__` method to make python code (generally unit
```

