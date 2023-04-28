# Comparing `tmp/front-0.1.89.tar.gz` & `tmp/front-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "front-0.1.89.tar", last modified: Fri Apr 28 12:46:49 2023, max compression
+gzip compressed data, was "front-0.1.9.tar", last modified: Fri Feb 18 02:01:54 2022, max compression
```

## Comparing `front-0.1.89.tar` & `front-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.624485 front-0.1.89/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 12:45:55.000000 front-0.1.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-04-28 12:46:49.624485 front-0.1.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-04-28 12:45:55.000000 front-0.1.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.620485 front-0.1.89/front/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 12:45:56.000000 front-0.1.89/front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-28 12:45:56.000000 front-0.1.89/front/app_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-28 12:45:56.000000 front-0.1.89/front/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    37248 2023-04-28 12:45:56.000000 front-0.1.89/front/crude.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-04-28 12:45:56.000000 front-0.1.89/front/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-28 12:45:56.000000 front-0.1.89/front/data_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.620485 front-0.1.89/front/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 12:45:56.000000 front-0.1.89/front/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-28 12:45:56.000000 front-0.1.89/front/elements/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 12:45:56.000000 front-0.1.89/front/elements/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 12:45:56.000000 front-0.1.89/front/elements/tree_maker_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.620485 front-0.1.89/front/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/kaggle_front.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/pos_key_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/simple_ml_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/tw_data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-28 12:45:56.000000 front-0.1.89/front/examples/wordle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-28 12:45:56.000000 front-0.1.89/front/py2pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.624485 front-0.1.89/front/scrap/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 12:45:56.000000 front-0.1.89/front/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-28 12:45:56.000000 front-0.1.89/front/scrap/binder_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-28 12:45:56.000000 front-0.1.89/front/scrap/binder_proposal_no_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-28 12:45:56.000000 front-0.1.89/front/scrap/state_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 12:45:56.000000 front-0.1.89/front/scrap/tw_simple_new_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-28 12:45:56.000000 front-0.1.89/front/spec_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-04-28 12:45:56.000000 front-0.1.89/front/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.624485 front-0.1.89/front/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/app_identity_pydantic_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/app_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_crude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_crudify_based_on_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_py2pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/test_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-28 12:45:56.000000 front-0.1.89/front/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-28 12:45:56.000000 front-0.1.89/front/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 12:45:56.000000 front-0.1.89/front/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-04-28 12:45:56.000000 front-0.1.89/front/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:46:49.620485 front-0.1.89/front.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-04-28 12:46:49.000000 front-0.1.89/front.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 12:46:49.000000 front-0.1.89/front.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:49.000000 front-0.1.89/front.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:46:49.000000 front-0.1.89/front.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 12:46:49.000000 front-0.1.89/front.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 12:46:49.000000 front-0.1.89/front.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 12:46:49.624485 front-0.1.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 12:45:56.000000 front-0.1.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-18 02:01:29.000000 front-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-02-18 02:01:54.493507 front-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2022-02-18 02:01:29.000000 front-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-02-18 02:01:53.000000 front-0.1.9/front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-02-18 02:01:53.000000 front-0.1.9/front/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16485 2022-02-18 02:01:53.000000 front-0.1.9/front/crude.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:29.000000 front-0.1.9/front/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/issues.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3762 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/kaggle_front.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/pos_key_args.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/tw_data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-02-18 02:01:53.000000 front-0.1.9/front/py2pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/scrap/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-18 02:01:29.000000 front-0.1.9/front/scrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/app_identity_pydantic_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/app_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-02-18 02:01:53.000000 front-0.1.9/front/tests/test_combos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-02-18 02:01:53.000000 front-0.1.9/front/tests/test_crude.py
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/test_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/test_py2pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-02-18 02:01:53.000000 front-0.1.9/front/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-02-18 02:01:54.493507 front-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-02-18 02:01:29.000000 front-0.1.9/setup.py
```

### Comparing `front-0.1.89/LICENSE` & `front-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/__init__.py` & `front-0.1.9/front/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,26 +31,7 @@
     from streamlitfront import session_state
     from streamlitfront import base
     from streamlitfront import util
     from streamlitfront import *
     from warnings import warn
 
     warn('Moved to seperate streamlitfront package', DeprecationWarning)
-
-from .app_maker import AppMaker
-from .spec_maker_base import (
-    SpecMakerBase,
-    APP_KEY,
-    OBJ_KEY,
-    RENDERING_KEY,
-    NAME_KEY,
-)
-from .elements import (
-    ElementTreeMaker,
-    ELEMENT_KEY,
-    FrontComponentBase,
-    FrontContainerBase,
-    FrontElementBase,
-    DEFAULT_INPUT_KEY,
-)
-from .crude import Crudifier, prepare_for_crude_dispatch
-from .data_binding import BoundData, Binder
```

### Comparing `front-0.1.89/front/base.py` & `front-0.1.9/front/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # for prepare_for_crude_dispatch
     param_to_mall_map=(),
     mall=None,
     output_store=None,
     save_name_param: str = 'save_name',
     include_stores_attribute: bool = False,
     # for setting defaults
-    defaults: Optional[Mapping] = None,
+    defaults: Optional[Mapping] = None
 ):
     param_to_mall_map = keys_to_values_if_non_mapping_iterable(param_to_mall_map)
 
     from i2 import Sig
 
     wrapped_func = func  # to seed the following sequence of wrapping
 
@@ -42,15 +42,15 @@
         include_stores_attribute=include_stores_attribute,
     )
 
     # enum wrap
     wrapped_func = inject_enum_annotations(
         wrapped_func,
         extract_enum_value=True,
-        **{param: mall[mall_key] for param, mall_key in param_to_mall_map.items()},
+        **{param: mall[mall_key] for param, mall_key in param_to_mall_map.items()}
     )
 
     # insert defaults
     if defaults:
         # get only keys that are in wrapped_func signature as well as defaults
         wrapped_sig = Sig(wrapped_func)
         _defaults = wrapped_sig.kwargs_from_args_and_kwargs(
```

### Comparing `front-0.1.89/front/dag.py` & `front-0.1.9/front/crude.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,480 +1,451 @@
-"""Tools to dispatch dags
+"""
+Control complex python object through strings.
+Wrap functions so that the complex arguments can be specified through a string key
+that points to the actual python object (which is stored in a session's memory or
+persisted in some fashion).
+"""
 
-See below one of the dags that will often be used in this module's doctests:
+from typing import Any, Mapping, Optional, Callable, Union, Iterable
+from functools import partial
+from inspect import Parameter
+import os
 
->>> from meshed.makers import code_to_dag
->>> @code_to_dag
-... def dag():
-...     x = foo(a, b)
-...     y = bar(x, greeting)
-...     z = confuser(a, w=x)  # note the w=x to test non-trivial binding
->>> print(dag.dot_digraph_ascii())  # doctest: +SKIP
-
-.. code-block::
-     ┌──────────┐
-  ┌▶ │ confuser │ ◀──    a
-  │  └──────────┘
-  │    │                │
-  │    │                │
-  │    ▼                ▼
-  │                   ┌─────┐
-  │       z           │ foo │ ◀──  b
-  │                   └─────┘
-  │                     │
-  │                     │
-  │                     ▼
-  │
-  └──────────────────    x
-
-                        │
-                        │
-                        ▼
-                      ┌─────┐
-       greeting   ──▶ │ bar │
-                      └─────┘
-                        │
-                        │
-                        ▼
+import dill  # pip install dill
 
-                         y
+from i2 import Sig, double_up_as_factory
+from i2.wrapper import Ingress, wrap
+from dol import Files, wrap_kvs
+from dol.filesys import mk_tmp_dol_dir, ensure_dir
+
+
+KT = str
+VT = Any
+StoreType = Mapping[KT, VT]
+StoreName = KT
+Mall = Mapping[StoreName, StoreType]
+
+
+def auto_key(*args, **kwargs) -> KT:
+    """Make a str key from arguments.
+
+    >>> auto_key(1,2,c=3,d=4)
+    '1,2,c=3,d=4'
+    >>> auto_key(1,2)
+    '1,2'
+    >>> auto_key(c=3,d=4)
+    'c=3,d=4'
+    >>> auto_key()
+    ''
+    """
+    args_str = ','.join(map(str, args))
+    kwargs_str = ','.join(map(lambda kv: f'{kv[0]}={kv[1]}', kwargs.items()))
+    return ','.join(filter(None, [args_str, kwargs_str]))
 
 
+@wrap_kvs(data_of_obj=dill.dumps, obj_of_data=dill.loads)
+class DillFiles(Files):
+    """Serializes and deserializes with dill"""
 
-"""
-from collections import defaultdict
-from typing import Union, Iterable, Mapping, Any
-from functools import partial
-from itertools import chain
+    pass
 
-from operator import itemgetter
-from enum import Enum
-from dol import groupby
-from front.crude import prepare_for_crude_dispatch
 
-from meshed import DAG, FuncNode
-from meshed.base import ch_func_node_attrs
-from meshed.itools import parents, children
+def mk_mall_of_dill_stores(store_names=Iterable[StoreName], rootdir=None):
+    """Make a mall of DillFiles stores"""
+    rootdir = rootdir or mk_tmp_dol_dir('crude')
+    if isinstance(store_names, str):
+        store_names = store_names.split()
 
+    def name_and_rootdir():
+        for name in store_names:
+            root = os.path.join(rootdir, name)
+            ensure_dir(root)
+            yield name, root
 
-# TODO: Lot's of cleaning and simplification needed in this module!!!
-def simple_namer(name, *, prefix='', suffix=''):
-    return f'{prefix}{name}{suffix}'
+    return {name: DillFiles(root) for name, root in name_and_rootdir()}
 
 
-def crudify_func_nodes(
-    var_nodes: Union[str, Iterable[str]],
-    dag: DAG,
-    var_node_name_to_store_name=partial(simple_namer, suffix='_store'),
-    *,
-    mall: Union[Mapping[str, Mapping[str, Any]], None] = None,
-    include_stores_attribute: bool = False,
-    save_name_param: str = 'save_name',
-):
-    """Crudifies the given ``var_nodes`` in the ``dag``.
+# TODO: store_on_output: use i2.wrapper and possibly extend i2.wrapper to facilitate
+from functools import wraps
 
-    Crudifying a var node means crudifying it's ``FuncNode`` neighbors,
-    i.e. telling the function that outputs to the ``VarNode`` (if any) to save it's
-    output in a store and (additionally) return the key it saved it too instead of the
-    value itself, and telling any consumers of the var node to use that key as it's
-    argument instead, retrieving the value from said store.
 
-    >>> from meshed import DAG, FuncNode
-    >>> from inspect import signature
-    >>> def foo(a, b):  return a + b
-    >>> def bar(x, y):  return  x * y
-    >>> dag = DAG([
-    ...     FuncNode(foo, name='foo', out='foo_output'),
-    ...     FuncNode(bar, bind={'y': 'foo_output'})
-    ... ])
-
-    Let's crudify ``'foo_output'``. We don't need to specify a mall, since
-    ``crudify_func_nodes`` will make one for us.
-    But in order to get access to it, to see what the function is doing, let's define
-    a mall with a single store (a dictionary), named ``'foo_output_store'``
-    (note that the map between ``var_node`` string name and
-    store name is controlled by the ``var_node_name_to_store_name`` argument)
-
-    >>> store = dict()
-    >>> mall = {'foo_output_store': store}
-    >>> new_dag = crudify_func_nodes(['foo_output'], dag, mall=mall)
-
-    The ``new_dag`` will have the same global behavior:
-
-    >>> assert dag(2, 3, 4) == new_dag(2, 3, 4) == 20
-
-    Notice though, that the ``foo`` node will have an extra argument, ``save_name``,
-    which is the name of the store to save the output to:
-
-    >>> print(new_dag.synopsis_string())
-    a,b,save_name -> foo -> foo_output
-    foo_output,x -> bar_ -> bar
-
-    This difference will be reflected in the signature of the ``new_dag``:
-
-    >>> print(str(signature(dag)))
-    (a, b, x)
-    >>> print(str(signature(new_dag)))
-    (a, b, x, save_name: str = '')
-
-    Let's have a closer look at the functions that ``dag`` and ``new_dag`` are
-    using. The functions of the ``dag`` are the original functions we specified,
-    behaving normally:
-
-    >>> dag.func_nodes[0].func(2, 3)
-    5
-    >>> dag.func_nodes[1].func(4, 5)
-    20
-
-    But the first function of ``new_dag`` outputs ``'bar_last_output'`` instead of ``5``.
-
-    >>> new_dag.func_nodes[0].func(2, 3)
-    'bar_last_output'
-
-    Where did the ``5`` go? In the mall!
-
-    >>> mall
-    {'foo_output_store': {'bar_last_output': 5}}
-
-    So that ``5`` has been stored under the ``'bar_last_output'`` key.
-    Further, the second function's second argument will no longer work with numbers,
-    but with string keys, and use that same store to retrieve the value it needs for
-    the underlying function:
-
-    >>> new_dag.func_nodes[1].func(4, 'bar_last_output')
-    20
-
-    This ``'bar_last_output'`` was only the default value that is used if
-    ``save_name`` is not given. If we give it a different name, the value will be
-    stored under that name instead:
-
-    >>> new_dag.func_nodes[0].func(20, 22, save_name='my_save_name')
-    'my_save_name'
-    >>> mall
-    {'foo_output_store': {'bar_last_output': 5, 'my_save_name': 42}}
-
-
-    :param var_nodes: The ``VarNodes`` we want to crudify
-    :param dag: The dag that contains these var_nodes
-    :param var_node_name_to_store_name: The function to use to make a store for a given
-        var_node name. If you have an explicit mapping ``m`` for this, just use ``m.get``
-    :param mall: A ``mall`` (store of stores, i.e. mapping of mappings) whose keys are
-        store names, and values are the actual stores.
-    :param include_stores_attribute: Whether the crudified functions should have an
-        attribute containing a pointer to the stores involved
-    :param save_name_param: The name that the "save as" parameter should appear as.
+@double_up_as_factory
+def store_on_output(
+    func=None,
+    *,
+    store=None,
+    save_name_param='save_name',
+    add_store_to_func_attr='output_store',
+):
+    """Wrap func so it will have an extra save_name_param that can be used to
+    indicate whether to save the output of the function call to that key, in
+    that store
+
+    :param func:
+    :param store:
+    :param save_name_param: Name of the extra param
     :return:
     """
-    return DAG(
-        list(
-            _crudified_func_nodes(
-                var_nodes,
-                dag,
-                var_node_name_to_store_name,
-                mall=mall,
-                include_stores_attribute=include_stores_attribute,
-                save_name_param=save_name_param,
-            )
-        )
+    save_name_param_obj = Parameter(
+        name=save_name_param, kind=Parameter.KEYWORD_ONLY, default='', annotation=str,
     )
+    sig = Sig(func) + [save_name_param_obj]
+
+    if store is None:
+        store = dict()
+
+    @sig
+    @wraps(func)
+    def _func(*args, **kwargs):
+        kwargs = sig.kwargs_from_args_and_kwargs(args, kwargs, apply_defaults=True)
+        save_name = kwargs.pop(save_name_param)
+        args, kwargs = sig.args_and_kwargs_from_kwargs(kwargs)
+        output = func(*args, **kwargs)
+        if save_name:
+            store[save_name] = output
+        return output
+
+    if isinstance(add_store_to_func_attr, str):
+        setattr(_func, add_store_to_func_attr, store)
 
+    # _func.output_store = store  # redundant with above. Remove
 
-def crudify_funcs(
-    var_nodes: Union[str, Iterable[str]],
-    dag: DAG,  # TODO: Postelize. Accept func_nodes and funcs
-    var_node_name_to_store_name=partial(simple_namer, suffix='_store'),
+    return _func
+
+
+@double_up_as_factory
+def prepare_for_crude_dispatch(
+    func: Callable = None,
     *,
-    mall: Union[Mapping[str, Mapping[str, Any]], None] = None,
-    include_stores_attribute: bool = False,
+    param_to_mall_map: Optional[Iterable] = None,
+    mall: Optional[Mall] = None,
+    output_store: Optional[Union[Mapping, str]] = None,
     save_name_param: str = 'save_name',
+    include_stores_attribute: bool = False,
 ):
-    return list(_crudified_funcs(**locals()))
+    """
+    Wrap func into something that is ready for CRUDE dispatch.
+    It will be a function for whom specific arguments will be specified by strings,
+    via underlying stores containing the values.
+    We say that those arguments were crude-dispatched.
+
+    :param func: callable, the function to wrap
+    :param param_to_mall_map: dict, whose keys specify which params should be
+        crude-dispatched and whose values are the mall keys to the Mapping instances
+        (e.g. dict) that should be used for said param.
+        If a non-Mapping iterable is given, will take {name: name...} identity mapping
+        for names in that iterable.
+    :mall mall: A store of stores. A Mapping whose keys are what the values of
+        ``param_to_mall_map`` point to and whose values are mapping interfaces (called
+         "stores" of a storage backend (local or remote, persisted or in-memory).
+    :param output_store: a store used to record the output of the function
+    :param save_name_param: str, the argument name that should be used in the returned
+        functions to get the the key of ``output_store`` under which the output will be
+        saved.
+    :param include_stores_attribute: bool, whether to add an attribute to the function
+        containing the ``output_store``
+
+    :return: A function that outputs the same thing as ``func``, but (1) with some
+        parameters being changed so that on can specify some arguments
+        (those listed by ``param_to_mall_key_dict``)
+
+
+    >>> def func(a, b: float, c: int):
+    ...     return a + b * c
+    ...
+    >>> param_to_mall_map = dict(a='a', b='b_store')
+    >>>
+    >>> mall = dict(
+    ...     a = {'one': 1, 'two': 2},
+    ...     b_store = {'three': 3, 'four': 4},
+    ...     ununsed_store = {'to': 'illustrate'}
+    ... )
+    >>> crude_func = prepare_for_crude_dispatch(
+    ...     func, param_to_mall_map=param_to_mall_map, mall=mall
+    ... )
 
+    ``crude_func`` is like ``func``, but you enter your ``a`` and ``b`` inputs
+    via string keys that will look up the values you're pointing to in ``mall``
 
-class VarNodeRole(Enum):
-    """(Var)Node roles.
+    >>> assert crude_func('one', 'three', 10) == func(1, 3, 10) == 31
+    >>> crude_func('one', 'three', 10)
+    31
+    >>> func(1, 3, 10)
+    31
 
-    When a ``VarNode`` is used to source the arguments of a ``FuncNode``, it's playing
-    a ``VarNodeRole.argument`` role.
+    What's happening behind the scenes of ``crude_func`` is this.
+    Let's follow what happens for the ``b`` argument. Say the user says ``b='three'``...
 
-    When a ``VarNode`` is used to store the return value of a ``FuncNode``, it's playing
-    a ``VarNodeRole.return_value`` role.
+    - ``b`` is a key of ``param_to_mall_key_dict``, indicating that it should be "cruded"
 
-    Most ``VarNode``s play both roles during a ``DAG`` computation.
+    - ``param_to_mall_key_dict['b']`` is ``'b_store'``, so we know which mall key to use
 
-    """
+    - We retrieve ``mall['b_store']['three']``, which is ``3``, and call ``func`` with it
 
-    argument = 'argument'
-    return_value = 'return_value'
+    So this is equivalent to this:
 
+    >>> func(mall['a']['one'], mall['b_store']['three'], 10)
+    31
 
-def _get_returned_by_func_node(var_node: str, dag: DAG):
-    returned_by_func_node = parents(dag.graph, var_node)
-    if len(returned_by_func_node) > 1:
-        raise ValueError(
-            f"This var_node had more than one parent. That is shouldn't be possible: "
-            f'{var_node}'
-        )
-    return next(
-        iter(returned_by_func_node), None
-    )  # If None, it means it is NOT produced by a FuncNode, so is a root (input) node.
-
-
-def _validate_is_func_node(node, var_node, relationship):
-    if not isinstance(node, FuncNode):
-        raise ValueError(f'{relationship} ({node}) of {var_node=} must be a FuncNode')
-
-
-def _node_replacements_for_var_node_crudification(var_node: str, dag: DAG):
-    """Helper function that generates the (node_id, (VarNodeRole, var_node)) instructions
-    needed to crudify the input ``var_node`` in ``dag``.
-
-    In the ``dag`` below, the ``var_node`` named ``x`` is the output of ``foo``
-    and is used for the input of both ``bar`` (bound to the parameter of the same name)
-    and ``confuser`` (bound to the ``w`` parameter).
-
-    Therefore, as we "crudify" ``x`` we'll need to take care of all three cases:
-    We'll need to have ``foo`` crudify it's output and both ``bar`` and ``confuser``
-    crudify one of their params.
-
-    >>> from meshed.makers import code_to_dag
-    >>> @code_to_dag
-    ... def dag():
-    ...     x = foo(a, b)
-    ...     y = bar(x, greeting)
-    ...     z = confuser(a, w=x)  # note the w=x to test non-trivial binding
-    >>> assert sorted(
-    ...     _node_replacements_for_var_node_crudification('x', dag)
-    ... ) == (
-    ... [
-    ...     ('bar', (VarNodeRole.argument, 'x')),
-    ...     ('confuser', (VarNodeRole.argument, 'x')),
-    ...     ('foo', (VarNodeRole.return_value, 'x')),
-    ... ])
+    The signature of ``a`` and ``b`` also changed to be `str`:
 
-    """
-    if not var_node in dag.var_nodes:
-        raise ValueError(f"The {dag.name} dag doesn't have this var_node: {var_node}")
+    >>> from inspect import signature
+    >>> str(signature(crude_func))
+    '(a: str, b: str, c: int)'
 
-    returned_by_func_node = _get_returned_by_func_node(var_node, dag)
-    if returned_by_func_node is not None:
-        # If var_node is the output of a FuncNode
-        # ... make sure it is.
-        _validate_is_func_node(returned_by_func_node, var_node, 'Parent')
-        # yield a (func_node_name, 'return_value', var_node) triple
-        yield returned_by_func_node.name, (VarNodeRole.return_value, var_node)
-    # if returned_by_func_node is None, skip the above: var_node is a "root" node
-
-    # arg_of_func_nodes
-    for arg_of_func_node in children(dag.graph, var_node):
-        _validate_is_func_node(arg_of_func_node, var_node, 'Child')
-        yield arg_of_func_node.name, (VarNodeRole.argument, var_node)
-
-
-_no_more_elements = type('NoMoreElements', (), {})()
-
-
-def _get_first_if_any_and_asserting_unique(
-    iterable: Iterable,
-    default=_no_more_elements,
-    msg='Your iterator should have no more than one element',
-):
-    iterator = iter(iterable)
-    first_element = next(iterator, default)
-    assert next(iterator, _no_more_elements) == _no_more_elements, msg
-    return first_element
+    By default, the ``output_store`` argument is None, but if you specify a mapping
+    there (or a string key that appears in the ``mall`` you specified, pointing to
+    a mapping), then the function you'll get will have an extra argument.
+
+    >>> output_store = dict()
+    >>> crude_func = prepare_for_crude_dispatch(
+    ...     func,
+    ...     param_to_mall_map=param_to_mall_map,
+    ...     mall=mall,
+    ...     output_store=output_store
+    ... )
+    >>> str(signature(crude_func))
+    "(a: str, b: str, c: int, save_name: str = '')"
 
+    You now have this extra ``save_name`` param in your function.
+    (Note that you can change its name through the ``prepare_for_crude_dispatch``'s
+    ``save_name_param`` argument.)
+    The default for ``save_name`` is '', and if you don't specify a non-empty
+    string, nothing different will happen, but if you do specify a non-empty string,
+    the output of your function will be saved, in the ``output_store`` you specified,
+    using that ``save_name`` key you specified.
+
+    >>> crude_func('one', 'three', 10)
+    31
+    >>> output_store
+    {}
+    >>> crude_func('one', 'three', 10, save_name='save_here')
+    31
+    >>> output_store
+    {'save_here': 31}
 
-def group_kvs_into_dict(kvs):
-    return groupby(kvs, key=itemgetter(0), val=itemgetter(1))
+    """
+    ingress = None
 
+    store_for_param = {}
 
-# TODO: Skipping doctest because order not stable. Make it so
-# TODO: Perhaps we should use FuncNode.name (id) instead of FuncNode itself as key of
-#   dag.graph. We'd have less such problems then.
-def _func_nodes_arg_and_return_names_to_crude(
-    var_nodes: Union[str, Iterable[str]], dag: DAG,
-):
-    """Return a copy of a dag where ``var_nodes`` were crudified.
+    if param_to_mall_map is not None:
 
-    >>> from meshed import DAG
-    >>> from meshed.makers import code_to_dag
-    >>> @code_to_dag
-    ... def dag():
-    ...     x = foo(a, b)
-    ...     y = bar(x, greeting)
-    ...     z = confuser(a, w=x)  # note the w=x to test non-trivial binding
-    >>>
-    >>> # Showing but skipping (because can't get order to be stable (TODO: Make it so)
-    >>> sorted(
-    ... _func_nodes_arg_and_return_names_to_crude(['x', 'a'], dag)
-    ... )  # doctest: +SKIP
-    [
-        (FuncNode(a,x -> confuser -> z), ('x', 'a'), None),
-        (FuncNode(x,greeting -> bar -> y), ('x',), None),
-        (FuncNode(a,b -> foo -> x), ('a',), 'x')
-    ]
+        sig = Sig(func)
 
-    """
-    if isinstance(var_nodes, str):
-        var_nodes = var_nodes.split()
+        store_for_param = _mk_store_for_param(sig, param_to_mall_map, mall)
+
+        def kwargs_trans(outer_kw):
+            """
+            Let's say you have a function with three params: a, b, and c, whose arguments
+            should be ints. Let's say you want a and c to be cruded.
+            Then you need to specify a store for each one of these:
+
+            >>> store_for_param = {
+            ...     'a': {'one': 1, 'two': 2},
+            ...     'c': {'three': 3}
+            ... }
+
+            What kwargs_trans will with this store_for_param, is this:
+
+            >>> kwargs_trans({'a': 'one', 'b': 2, 'c': 'three'})
+            {'a': 1, 'b': 2, 'c': 3}
+            """
+            # outer_kw is going to be the new/wrapped/cruded interface of the function
+            # That is, the one that takes strings to specify arguments
+            # What we need to do now is transform the cruded argument values from strings
+            # to the values these strings are pointing to (via the store corresponding
+            # to that argument).
+            def get_values_from_stores():
+                # Note: only need to specify arguments that change
+                for param, store in store_for_param.items():
+                    # param's argument value is assumed to be a store_key
+                    store_key = outer_kw[param]
+                    # store_key points to the value the outer user wants the value for:
+                    # store is the store where to find it
+                    yield param, store[store_key]
+
+            return dict(get_values_from_stores())
+
+        ingress = Ingress(
+            inner_sig=sig,
+            kwargs_trans=kwargs_trans,
+            outer_sig=(
+                sig.ch_annotations(**{name: str for name in param_to_mall_map})
+                # + [save_name_param]
+            ),
+        )
 
-    get_node_replacements = partial(
-        _node_replacements_for_var_node_crudification, dag=dag
-    )
+    wrapped_f = wrap(func, ingress)
 
-    crude_modifications = group_kvs_into_dict(
-        chain.from_iterable(map(get_node_replacements, var_nodes))
-    )
+    if include_stores_attribute:
+        wrapped_f.store_for_param = store_for_param
 
-    for func_node in dag.func_nodes:
-        if modifications := crude_modifications.get(func_node.name, None):
-            grouped_modifications = group_kvs_into_dict(modifications)
-            argument_names = grouped_modifications.get(VarNodeRole.argument, [])
-            return_name = _get_first_if_any_and_asserting_unique(
-                iterable=grouped_modifications.get(VarNodeRole.return_value, []),
-                default=None,
-                msg=f"You shouldn't have more than one return_value in {func_node}",
-            )
-            yield func_node, tuple(argument_names), return_name
+    if output_store is not None:
+        output_store_name = 'output_store'
+        if isinstance(output_store, str):
+            # if output_store is a string, it should be the a key to store_for_param
+            output_store_name = output_store
+            output_store = mall[output_store_name]
         else:
-            yield func_node, (), None
+            # TODO: Assert MutableMapping, or just existence of __setitem__?
+            if not hasattr(output_store, '__setitem__'):
+                raise ValueError(f'Needs to have a __setitem__: {output_store}')
+        if output_store_name in store_for_param:
+            raise ValueError(
+                f'Name conflicts with existing param name: {output_store_name}'
+            )
 
+        wrapped_f = store_on_output(
+            wrapped_f, store=output_store, save_name_param=save_name_param,
+        )
+        wrapped_f.__name__ = wrapped_f.__name__ + '_w_output_storing'
 
-def _mk_param_to_mall_map_from_for_var_nodes(
-    var_nodes, bind, var_node_name_to_store_name
-):
-    """Generate (param, store_name) pairs.
+        if include_stores_attribute:
+            wrapped_f.output_store = output_store
 
-    >>> dict(
-    ...     _mk_param_to_mall_map_from_for_var_nodes(
-    ...         var_nodes=['a', 'c'],
-    ...         bind={'w': 'a', 'x': 'c', 'y': 'c', 'z': 'b'},
-    ...         var_node_name_to_store_name=lambda name: f"{name}_store"
-    ...     )
-    ... )
-    {'w': 'a_store', 'x': 'c_store', 'y': 'c_store'}
-    """
-    for param, var_node in bind.items():
-        if var_node in var_nodes:
-            yield param, var_node_name_to_store_name(var_node)
-
-
-def _return_save_name(*, save_name) -> str:
-    return save_name
-
-
-def _empty_name_callback():
-    raise RuntimeError(f'No save name was given')
-
-
-from i2.wrapper import rm_params
-from typing import Callable
-
-# TODO: Give control to ALL prepare_for_crude_dispatch arguments.
-#     param_to_mall_map: Optional[Union[dict, Iterable]] = None,
-#     mall: Optional[Mall] = None,
-#     include_stores_attribute: bool = False,
-#     output_store: Optional[Union[Mapping, str]] = None,
-#     # the arguments below only apply if output_store is given
-#     save_name_param: str = 'save_name',
-#     empty_name_callback: Callable[[], Any] = None,
-#     auto_namer: Callable[..., str] = None,
-#     output_trans: Callable[..., Any] = None,
-#     verbose: bool = True,
-def _crudified_func_nodes(
-    var_nodes: Union[str, Iterable[str]],
-    dag: DAG,
-    var_node_name_to_store_name=partial(simple_namer, suffix='_store'),
-    *,
-    mall: Union[Mapping[str, Mapping[str, Any]], None] = None,
-    include_stores_attribute: bool = False,
-    save_name_param: str = 'save_name',
-    auto_namer: Callable[[], Any] = None,
-    remove_save_name=False,  # TODO: should be False or not exist
-    store_factory=dict,
-):
-    if isinstance(var_nodes, str):
-        var_nodes = var_nodes.split()
-    # make a mall for all the var_names, giving them all empty dicts as stores
-    # if they are not there already.
-    if mall is None:
-        mall = defaultdict(dict)
-
-    # TODO: This overwrites the mall outside so user is surprised!
-    # mall = dict(
-    #     {var_node_name_to_store_name(var_name): dict() for var_name in var_nodes},
-    #     **mall,
-    # )
-    # Possible solution:
-    for var_name in var_nodes:
-        store_name_for_var_name = var_node_name_to_store_name(var_name)
-        if store_name_for_var_name not in mall:
-            # TODO: store_factory has no args here. Maybe we want to use
-            #  call_forgivingly to allow user to specify how to make store according to
-            #  var_name or store_name_for_var_name (or not)
-            #  Other possibility: store_factory is a function or mapping
-            mall[store_name_for_var_name] = store_factory()
-
-    if remove_save_name:
-        rm_save_name = partial(rm_params, params_to_remove=[save_name_param])
-    else:
-        rm_save_name = lambda x: x
-
-    for (
-        func_node,
-        argument_names,
-        return_name,
-    ) in _func_nodes_arg_and_return_names_to_crude(var_nodes, dag):
-        mk_param_mall_map = partial(
-            _mk_param_to_mall_map_from_for_var_nodes,
-            var_node_name_to_store_name=var_node_name_to_store_name,
+        # def egress(func_output):
+        #     store_for_param[output_store_name] = func_output
+        #     return func_output
+
+    return wrapped_f
+
+
+def _mk_store_for_param(sig, param_to_mall_key_dict=None, mall=None, verbose=True):
+    """Make a {param: store,...} dict from a {param: mall_key,...} dict, a sig and a
+    mall, validating stuff on the way."""
+    mall = mall or dict()
+    param_to_mall_key_dict = keys_to_values_if_non_mapping_iterable(
+        param_to_mall_key_dict
+    )
+    # mall_keys_that_are_also_params_but_not_param_to_mall_key_dict_keys
+    unmentioned_mall_keys = set(mall) & set(sig.names) - set(param_to_mall_key_dict)
+    if unmentioned_mall_keys and verbose:
+        from warnings import warn
+
+        warn(
+            f"Some of your mall keys were also func arg names, but you didn't mention "
+            f'them in param_to_mall_map, namely, these: {unmentioned_mall_keys}'
         )
-        if (argument_names, return_name) == ((), None):
-            yield func_node
-        else:
-            param_to_mall_map = (
-                dict(mk_param_mall_map(argument_names, func_node.bind)) or None
+    if param_to_mall_key_dict:
+        func_name_stub = ''
+        if sig.name:
+            func_name_stub = f'({sig.name})'
+        if isinstance(param_to_mall_key_dict, str):
+            param_to_mall_key_dict = param_to_mall_key_dict.split()
+        if not set(param_to_mall_key_dict).issubset(sig.names):
+            offenders = set(param_to_mall_key_dict) - set(sig.names)
+            raise ValueError(
+                'The param_to_mall_map should only contain keys that are '
+                f"parameters (i.e. 'argument names') of your function {func_name_stub}. "
+                f'Yet these param_to_mall_map keys were not argument names: '
+                f'{offenders}'
             )
-            output_store = (
-                var_node_name_to_store_name(return_name)
-                if return_name is not None
-                else None
+        if not set(param_to_mall_key_dict.values()).issubset(mall.keys()):
+            offenders = set(param_to_mall_key_dict.values()) - set(mall.keys())
+            keys = 'keys' if len(offenders) > 1 else 'key'
+            offenders = ', '.join(map(lambda x: f"'{x}'", offenders))
+
+            raise ValueError(
+                f'The {offenders} {keys} of your param_to_mall_map values were not '
+                f'in the mall. '
             )
+        # Note: store_for_param used to be the argument of prepare_for_crude_dispatch,
+        #   instead of the (param_to_mall_map, mall) pair which is overkill.
+        #   The reason for obliging the user to give this pair was because asking for
+        #   the user to be more explicit about the argname to store mapping would avoid
+        #   some bugs and make it possible to validate the request earlier on.
+        store_for_param = {
+            argname: mall[mall_key]
+            for argname, mall_key in param_to_mall_key_dict.items()
+        }
+        return store_for_param
+
+
+def keys_to_values_if_non_mapping_iterable(d: Iterable) -> Mapping:
+    if d is None:
+        return dict()
+    elif not isinstance(d, Mapping) and isinstance(d, Iterable):
+        d = {k: k for k in d}
+    return d
+
+
+# Note: This is not meant to actually be used in real apps, but be a drop in helper to
+#   talk to the mall (or rather "listen" since it's read-only) from a UI.
+def simple_mall_dispatch_core_func(
+    key: KT, action: str, store_name: StoreName, mall: Mall
+):
+    """Helper function to dispatch a mall
 
-            crudified_func = prepare_for_crude_dispatch(
-                func_node.func,
-                param_to_mall_map=param_to_mall_map,
-                output_store=output_store,
-                empty_name_callback=None,
-                auto_namer=lambda: f'{func_node.out}_last_output',
-                output_trans=_return_save_name,
-                mall=mall,
-                include_stores_attribute=include_stores_attribute,
-                save_name_param=save_name_param,
-            )
+    This function is only meant to be a helper to give a UI (GUI,
+    CLI...) mall-exploration capabilities. Namely:
 
-            yield ch_func_node_attrs(func_node, func=rm_save_name(crudified_func))
+    - ``list(mall)``: list the keys of a mall. This is achieved with args:
+        ``(key=None, action=None, store_name=None, mall=mall)``
+    - ``mall[store_name]``: get a store. Acheived by:
+        ``(key=None, action=None, store_name=store_name, mall=mall)``
+    - ``list(mall[store_name])``: list keys of a store (of the mall). Acheived by:
+        ``(key=None, action='list', store_name=store_name, mall=mall)``
+    - ``list(filter(key, mall[store_name]))``: list keys of a store (of the mall)
+        according to a substring filter. (only keys that have ``key`` as substring)
+        ``(key=key, action='list', store_name=store_name, mall=mall)``
+    - ``mall[store_name][key]``:  get the value/data of a store for ``key``
+        ``(key=key, action='get', store_name=store_name, mall=mall)``
+
+    :param key: The key
+    :param action: 'list' (to list keys of a store) or 'get' (to get the value of
+        ``key`` in the store (named ``store_name``)
+    :param store_name: Store name to look up in mall. If not given, the function will
+        output the mall keys (which are valid store names)
+    :param mall: dict of stores (Mapping interface to data)
+    :return:
 
+    >>> mall = {
+    ...     'english': {'one': 1, 'two': 2, 'three': 3},
+    ...     'french': {'un': 1, 'deux': 2},
+    ... }
 
-def _crudified_funcs(
-    var_nodes: Union[str, Iterable[str]],
-    dag: DAG,
-    var_node_name_to_store_name=partial(simple_namer, suffix='_store'),
-    *,
-    mall: Union[Mapping[str, Mapping[str, Any]], None] = None,
-    include_stores_attribute: bool = False,
-    save_name_param: str = 'save_name',
-):
-    kwargs = dict(locals(), remove_save_name=False)
-    func_nodes = _crudified_func_nodes(**kwargs)
-    yield from (fn.func for fn in func_nodes)
+    List the keys of a mall:
 
+    >>> simple_mall_dispatch_core_func(None, None, None, mall=mall)
+    ['english', 'french']
 
-def fnodes_to_var_node_crude_specs(fnodes):
-    for fnode in fnodes:
-        yield fnode.var, fnode.func, fnode.bind
+    Get a store
 
+    >>> simple_mall_dispatch_core_func(None, None, store_name='english', mall=mall)
+    {'one': 1, 'two': 2, 'three': 3}
 
-# empty_name_callback: Callable[[], Any] = None,
-# auto_namer: Callable[..., str] = None,
-# output_trans: Callable[..., Any] = None,
+    List keys of a store (of the mall):
+
+    >>> simple_mall_dispatch_core_func(
+    ...     None, action='list', store_name='english', mall=mall
+    ... )
+    ['one', 'two', 'three']
+
+    List keys of a store (of the mall) according to a substring filter:
+
+    >>> simple_mall_dispatch_core_func(
+    ...     'e', action='list', store_name='english', mall=mall
+    ... )
+    ['one', 'three']
+
+    >>> simple_mall_dispatch_core_func(
+    ...     'two', action='get', store_name='english', mall=mall
+    ... )
+    2
+
+
+    """
+    if not store_name:
+        # if store_name empty, list the store names (i.e. the mall keys)
+        return list(mall)
+    else:  # if not, get the store
+        store = mall[store_name]
+        if not action:
+            return store
+
+    key = key or ''
+    if action == 'list':
+        key = key.strip()  # to handle some invisible whitespace that would screw things
+        return list(filter(lambda k: key in k, store))
+    elif action == 'get':
+        return store[key]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `front-0.1.89/front/examples/experimentation.py` & `front-0.1.9/front/examples/experimentation.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/examples/issues.py` & `front-0.1.9/front/examples/issues.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/examples/kaggle_front.py` & `front-0.1.9/front/examples/kaggle_front.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/examples/pos_key_args.py` & `front-0.1.9/front/examples/pos_key_args.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/examples/simple.py` & `front-0.1.9/front/examples/simple.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/examples/tw_data_binding.py` & `front-0.1.9/front/examples/tw_data_binding.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/tests/test_combos.py` & `front-0.1.9/front/tests/test_combos.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         foo,
         param_to_mall_map={'a': 'a_store'},
         mall=mall,
         output_store=mall['saves'],
         include_stores_attribute=True,
     )
 
-    assert str(Sig(bar)) == "(a: Literal['one', 'two'], b, save_name: str = '')"
+    assert str(Sig(bar)) == "(a: str, b, save_name: str = '')"
     assert bar('two', 'mice', save_name='save_here') == 'micemice'
 
     assert bar.store_for_param == {'a': {'one': 1, 'two': 2}}
     assert bar.output_store == {'save_here': 'micemice'}
 
     # ------------ With prepare_for_dispatch (prepare_for_crude_dispatch + enum) ----------
```

### Comparing `front-0.1.89/front/tests/test_crude.py` & `front-0.1.9/front/tests/test_crude.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front/tests/test_py2pydantic.py` & `front-0.1.9/front/tests/test_py2pydantic.py`

 * *Files identical despite different names*

### Comparing `front-0.1.89/front.egg-info/SOURCES.txt` & `front-0.1.9/front.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,31 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 front/__init__.py
-front/app_maker.py
 front/base.py
 front/crude.py
-front/dag.py
-front/data_binding.py
 front/py2pydantic.py
-front/spec_maker_base.py
-front/state.py
-front/tools.py
-front/types.py
 front/util.py
 front.egg-info/PKG-INFO
 front.egg-info/SOURCES.txt
 front.egg-info/dependency_links.txt
 front.egg-info/not-zip-safe
 front.egg-info/requires.txt
 front.egg-info/top_level.txt
-front/elements/__init__.py
-front/elements/elements.py
-front/elements/implementation.py
-front/elements/tree_maker_base.py
 front/examples/__init__.py
 front/examples/data_binding.py
 front/examples/experimentation.py
 front/examples/issues.py
 front/examples/kaggle_front.py
 front/examples/pos_key_args.py
 front/examples/simple.py
-front/examples/simple_ml_1.py
 front/examples/tw_data_binding.py
-front/examples/wordle.py
 front/scrap/__init__.py
-front/scrap/binder_proposal.py
-front/scrap/binder_proposal_no_desc.py
-front/scrap/state_proposal.py
-front/scrap/tw_simple_new_arch.py
 front/tests/__init__.py
 front/tests/app_identity_pydantic_output.py
 front/tests/app_identity_write_output.py
 front/tests/test_combos.py
 front/tests/test_crude.py
-front/tests/test_crudify_based_on_names.py
 front/tests/test_identity_write_output.py
-front/tests/test_py2pydantic.py
-front/tests/test_state.py
-front/tests/test_use_case.py
-front/tests/util.py
+front/tests/test_py2pydantic.py
```

