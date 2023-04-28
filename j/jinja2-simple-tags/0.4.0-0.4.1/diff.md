# Comparing `tmp/jinja2-simple-tags-0.4.0.tar.gz` & `tmp/jinja2-simple-tags-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2-simple-tags-0.4.0.tar", last modified: Sat May 28 07:36:58 2022, max compression
+gzip compressed data, was "jinja2-simple-tags-0.4.1.tar", last modified: Thu Nov 24 08:40:08 2022, max compression
```

## Comparing `jinja2-simple-tags-0.4.0.tar` & `jinja2-simple-tags-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 07:36:58.802250 jinja2-simple-tags-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-28 07:36:48.000000 jinja2-simple-tags-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-05-28 07:36:48.000000 jinja2-simple-tags-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-28 07:36:48.000000 jinja2-simple-tags-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2022-05-28 07:36:58.802250 jinja2-simple-tags-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-05-28 07:36:48.000000 jinja2-simple-tags-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 07:36:58.802250 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2022-05-28 07:36:58.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-05-28 07:36:58.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 07:36:58.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 07:36:58.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-28 07:36:58.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-28 07:36:58.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-05-28 07:36:48.000000 jinja2-simple-tags-0.4.0/jinja2_simple_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-05-28 07:36:58.802250 jinja2-simple-tags-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-28 07:36:48.000000 jinja2-simple-tags-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:40:08.599356 jinja2-simple-tags-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      897 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2022-11-24 08:40:08.599356 jinja2-simple-tags-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:40:08.599356 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2022-11-24 08:40:08.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2022-11-24 08:40:08.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 08:40:08.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 08:40:08.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-24 08:40:08.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-24 08:40:08.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3814 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/jinja2_simple_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2022-11-24 08:40:08.599356 jinja2-simple-tags-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-24 08:40:01.000000 jinja2-simple-tags-0.4.1/setup.py
```

### Comparing `jinja2-simple-tags-0.4.0/LICENSE` & `jinja2-simple-tags-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2-simple-tags-0.4.0/PKG-INFO` & `jinja2-simple-tags-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-simple-tags
-Version: 0.4.0
+Version: 0.4.1
 Summary: Base classes for quick-and-easy template tag development
 Home-page: https://github.com/dldevinc/jinja2-simple-tags
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -17,56 +17,62 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jinja2-simple-tags
+
 Base classes for quick-and-easy template tag development
 
 [![PyPI](https://img.shields.io/pypi/v/jinja2-simple-tags.svg)](https://pypi.org/project/jinja2-simple-tags/)
 [![Build Status](https://travis-ci.com/dldevinc/jinja2-simple-tags.svg?branch=master)](https://travis-ci.org/dldevinc/jinja2-simple-tags)
 
 ## Compatibility
-* `python` >= 3.6
-* `Jinja2` >= 2.10
+
+-   `python` >= 3.6
+-   `Jinja2` >= 2.10
 
 ## Installation
+
 `pip install jinja2-simple-tags`
 
 ## Examples
 
 ### `StandaloneTag`
+
 ```python
 from django.utils.timezone import now
 from django.utils.formats import date_format
 from jinja2_simple_tags import StandaloneTag
 
 
 class NowExtension(StandaloneTag):
     tags = {"now"}
 
     def render(self, format_string='DATETIME_FORMAT'):
         return date_format(now(), format_string)
 ```
 
 Usage:
+
 ```jinja2
 {% now %}           {# 7th July 2020, 10:07 a.m. #}
 {% now "Y-m-d" %}   {# 2020-07-07 #}
 ```
 
-
 ### `ContainerTag`
+
 ```python
 from django.core.cache import cache
 from django.utils.encoding import force_str
 from django.core.cache.utils import make_template_fragment_key
 from jinja2_simple_tags import ContainerTag
 
 
@@ -83,23 +89,25 @@
         else:
             value = force_str(value)
 
         return value
 ```
 
 Usage:
+
 ```jinja2
 {% cache "footer", request.path, timeout=3600 %}
   <footer>
     ...
   </footer>
 {% endcache %}
 ```
 
 ### Context
+
 Current context is available through the `self.context`.
 
 ```python
 from django.urls import reverse
 from jinja2_simple_tags import StandaloneTag
 
 
@@ -109,18 +117,20 @@
     def render(self, name):
         request = self.context['request']
         url = reverse(name)
         return request.build_absolute_uri(url)
 ```
 
 ### Assignment
+
 Both `StandaloneTag` and `ContainerTag` comes with out-of-the-box
 support for assignment.
 
 Usage:
+
 ```jinja2
 {% now "Y-m-d" as today %}
 ...
 {{ today }}       {# 2020-07-07 #}
 ```
 
 ```jinja2
```

### Comparing `jinja2-simple-tags-0.4.0/README.md` & `jinja2-simple-tags-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # jinja2-simple-tags
+
 Base classes for quick-and-easy template tag development
 
 [![PyPI](https://img.shields.io/pypi/v/jinja2-simple-tags.svg)](https://pypi.org/project/jinja2-simple-tags/)
 [![Build Status](https://travis-ci.com/dldevinc/jinja2-simple-tags.svg?branch=master)](https://travis-ci.org/dldevinc/jinja2-simple-tags)
 
 ## Compatibility
-* `python` >= 3.6
-* `Jinja2` >= 2.10
+
+-   `python` >= 3.6
+-   `Jinja2` >= 2.10
 
 ## Installation
+
 `pip install jinja2-simple-tags`
 
 ## Examples
 
 ### `StandaloneTag`
+
 ```python
 from django.utils.timezone import now
 from django.utils.formats import date_format
 from jinja2_simple_tags import StandaloneTag
 
 
 class NowExtension(StandaloneTag):
     tags = {"now"}
 
     def render(self, format_string='DATETIME_FORMAT'):
         return date_format(now(), format_string)
 ```
 
 Usage:
+
 ```jinja2
 {% now %}           {# 7th July 2020, 10:07 a.m. #}
 {% now "Y-m-d" %}   {# 2020-07-07 #}
 ```
 
-
 ### `ContainerTag`
+
 ```python
 from django.core.cache import cache
 from django.utils.encoding import force_str
 from django.core.cache.utils import make_template_fragment_key
 from jinja2_simple_tags import ContainerTag
 
 
@@ -55,23 +60,25 @@
         else:
             value = force_str(value)
 
         return value
 ```
 
 Usage:
+
 ```jinja2
 {% cache "footer", request.path, timeout=3600 %}
   <footer>
     ...
   </footer>
 {% endcache %}
 ```
 
 ### Context
+
 Current context is available through the `self.context`.
 
 ```python
 from django.urls import reverse
 from jinja2_simple_tags import StandaloneTag
 
 
@@ -81,18 +88,20 @@
     def render(self, name):
         request = self.context['request']
         url = reverse(name)
         return request.build_absolute_uri(url)
 ```
 
 ### Assignment
+
 Both `StandaloneTag` and `ContainerTag` comes with out-of-the-box
 support for assignment.
 
 Usage:
+
 ```jinja2
 {% now "Y-m-d" as today %}
 ...
 {{ today }}       {# 2020-07-07 #}
 ```
 
 ```jinja2
```

### Comparing `jinja2-simple-tags-0.4.0/jinja2_simple_tags.egg-info/PKG-INFO` & `jinja2-simple-tags-0.4.1/jinja2_simple_tags.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-simple-tags
-Version: 0.4.0
+Version: 0.4.1
 Summary: Base classes for quick-and-easy template tag development
 Home-page: https://github.com/dldevinc/jinja2-simple-tags
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -17,56 +17,62 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jinja2-simple-tags
+
 Base classes for quick-and-easy template tag development
 
 [![PyPI](https://img.shields.io/pypi/v/jinja2-simple-tags.svg)](https://pypi.org/project/jinja2-simple-tags/)
 [![Build Status](https://travis-ci.com/dldevinc/jinja2-simple-tags.svg?branch=master)](https://travis-ci.org/dldevinc/jinja2-simple-tags)
 
 ## Compatibility
-* `python` >= 3.6
-* `Jinja2` >= 2.10
+
+-   `python` >= 3.6
+-   `Jinja2` >= 2.10
 
 ## Installation
+
 `pip install jinja2-simple-tags`
 
 ## Examples
 
 ### `StandaloneTag`
+
 ```python
 from django.utils.timezone import now
 from django.utils.formats import date_format
 from jinja2_simple_tags import StandaloneTag
 
 
 class NowExtension(StandaloneTag):
     tags = {"now"}
 
     def render(self, format_string='DATETIME_FORMAT'):
         return date_format(now(), format_string)
 ```
 
 Usage:
+
 ```jinja2
 {% now %}           {# 7th July 2020, 10:07 a.m. #}
 {% now "Y-m-d" %}   {# 2020-07-07 #}
 ```
 
-
 ### `ContainerTag`
+
 ```python
 from django.core.cache import cache
 from django.utils.encoding import force_str
 from django.core.cache.utils import make_template_fragment_key
 from jinja2_simple_tags import ContainerTag
 
 
@@ -83,23 +89,25 @@
         else:
             value = force_str(value)
 
         return value
 ```
 
 Usage:
+
 ```jinja2
 {% cache "footer", request.path, timeout=3600 %}
   <footer>
     ...
   </footer>
 {% endcache %}
 ```
 
 ### Context
+
 Current context is available through the `self.context`.
 
 ```python
 from django.urls import reverse
 from jinja2_simple_tags import StandaloneTag
 
 
@@ -109,18 +117,20 @@
     def render(self, name):
         request = self.context['request']
         url = reverse(name)
         return request.build_absolute_uri(url)
 ```
 
 ### Assignment
+
 Both `StandaloneTag` and `ContainerTag` comes with out-of-the-box
 support for assignment.
 
 Usage:
+
 ```jinja2
 {% now "Y-m-d" as today %}
 ...
 {{ today }}       {# 2020-07-07 #}
 ```
 
 ```jinja2
```

### Comparing `jinja2-simple-tags-0.4.0/jinja2_simple_tags.py` & `jinja2-simple-tags-0.4.1/jinja2_simple_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from jinja2 import nodes
 from jinja2.ext import Extension
 
 __all__ = ['StandaloneTag', 'ContainerTag']
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 
 
 class BaseTemplateTag(Extension):
     def __init__(self, environment):
         super().__init__(environment)
         self.template = None
         self.lineno = None
@@ -20,16 +20,16 @@
             nodes.Keyword('_template', nodes.Const(parser.name)),
             nodes.Keyword('_lineno', nodes.Const(lineno)),
             nodes.Keyword('_tag_name', nodes.Const(tag_name)),
         ]
         self.init_parser(parser)
         args, kwargs, target = self.parse_args(parser)
         kwargs.extend(additional_params)
-        block_call = self.call_method('render_wrapper', args, kwargs)
-        return self.output(parser, block_call, target, tag_name=tag_name, lineno=lineno)
+        call_node = self.call_method('render_wrapper', args, kwargs)
+        return self.output(parser, call_node, target, tag_name=tag_name, lineno=lineno)
 
     def init_parser(self, parser):
         parser.stream.skip(1)  # skip tag name
 
     def parse_args(self, parser):
         args = []
         kwargs = []
@@ -45,14 +45,18 @@
                         'Invalid assignment target', parser.stream.current.lineno
                     )
                 break
 
             if require_comma:
                 parser.stream.expect('comma')
 
+                # support for trailing comma
+                if parser.stream.current.type == 'block_end':
+                    break
+
             if (
                 parser.stream.current.type == 'name'
                 and parser.stream.look().type == 'assign'
             ):
                 key = parser.stream.current.value
                 parser.stream.skip(2)
                 value = parser.parse_expression()
@@ -62,38 +66,38 @@
                     parser.fail('Invalid argument syntax', parser.stream.current.lineno)
                 args.append(parser.parse_expression())
 
             require_comma = True
 
         return args, kwargs, target
 
-    def output(self, parser, block_call, target, tag_name, lineno):
+    def output(self, parser, call_node, target, tag_name, lineno):
         raise NotImplementedError
 
     def render_wrapper(self, *args, **kwargs):
         self.context = kwargs.pop('_context', None)
         self.template = kwargs.pop('_template', None)
         self.lineno = kwargs.pop('_lineno', None)
         self.tag_name = kwargs.pop('_tag_name', None)
         return self.render(*args, **kwargs)
 
     def render(self, *args, **kwargs):
         raise NotImplementedError
 
 
 class StandaloneTag(BaseTemplateTag):
-    def output(self, parser, block_call, target, tag_name, lineno):
+    def output(self, parser, call_node, target, tag_name, lineno):
         if target:
             target_node = nodes.Name(target, 'store', lineno=lineno)
-            return nodes.Assign(target_node, block_call, lineno=lineno)
-        call = nodes.MarkSafe(block_call, lineno=lineno)
+            return nodes.Assign(target_node, call_node, lineno=lineno)
+        call = nodes.MarkSafe(call_node, lineno=lineno)
         return nodes.Output([call], lineno=lineno)
 
 
 class ContainerTag(BaseTemplateTag):
-    def output(self, parser, block_call, target, tag_name, lineno):
+    def output(self, parser, call_node, target, tag_name, lineno):
         body = parser.parse_statements(['name:end%s' % tag_name], drop_needle=True)
-        call_block = nodes.CallBlock(block_call, [], [], body).set_lineno(lineno)
+        call_block = nodes.CallBlock(call_node, [], [], body).set_lineno(lineno)
         if target:
             target_node = nodes.Name(target, 'store', lineno=lineno)
             return nodes.AssignBlock(target_node, None, [call_block], lineno=lineno)
         return call_block
```

### Comparing `jinja2-simple-tags-0.4.0/setup.cfg` & `jinja2-simple-tags-0.4.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [bdist_wheel]
 universal = 1
 
 [options]
 zip_safe = false
```

