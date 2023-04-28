# Comparing `tmp/scrape_schema-0.1.0.tar.gz` & `tmp/scrape_schema-0.1.1.tar.gz`

## Comparing `scrape_schema-0.1.0.tar` & `scrape_schema-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/__init__.py
--rw-r--r--   0        0        0    21663 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/LICENSE
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/README.md
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/README.md
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/PKG-INFO
```

### Comparing `scrape_schema-0.1.0/scrape_schema/base.py` & `scrape_schema-0.1.1/scrape_schema/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 _stdout_handler.setFormatter(_formatter)
 logger.addHandler(_stdout_handler)
 
 T = TypeVar("T")
 MARKUP_TYPE: TypeAlias = Union[str, Any]
 
 
+def extract_fields(markup: MARKUP_TYPE, **fields: "BaseField") -> Dict[str, Any]:
+    return {key: field.extract(markup) for key, field in fields.items()}
+
+
 class ABCField(ABC):
     @abstractmethod
     def _parse(self, markup: MARKUP_TYPE) -> Any:
         ...
 
     @abstractmethod
     def _filter(self, value: T) -> bool:
```

### Comparing `scrape_schema-0.1.0/scrape_schema/callbacks/slax.py` & `scrape_schema-0.1.1/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/scrape_schema/callbacks/soup.py` & `scrape_schema-0.1.1/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/scrape_schema/fields/nested.py` & `scrape_schema-0.1.1/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/scrape_schema/fields/regex.py` & `scrape_schema-0.1.1/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/scrape_schema/fields/slax.py` & `scrape_schema-0.1.1/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/scrape_schema/fields/soup.py` & `scrape_schema-0.1.1/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/.gitignore` & `scrape_schema-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/LICENSE` & `scrape_schema-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/README.md` & `scrape_schema-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/pyproject.toml` & `scrape_schema-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.0/PKG-INFO` & `scrape_schema-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

