# Comparing `tmp/forest-python-0.6.1.tar.gz` & `tmp/forest-python-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forest-python-0.6.1.tar", last modified: Wed Jan 26 04:30:24 2022, max compression
+gzip compressed data, was "forest-python-0.6.3.tar", last modified: Wed Apr 26 05:29:22 2023, max compression
```

## Comparing `forest-python-0.6.1.tar` & `forest-python-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2022-01-26 04:30:24.842454 forest-python-0.6.1/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1067 2022-01-10 06:48:02.000000 forest-python-0.6.1/LICENSE
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1777 2022-01-26 04:30:24.842454 forest-python-0.6.1/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1421 2022-01-26 04:14:00.000000 forest-python-0.6.1/README.rst
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2022-01-26 04:30:24.842454 forest-python-0.6.1/forest/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2022-01-10 06:48:02.000000 forest-python-0.6.1/forest/__init__.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2022-01-26 04:30:24.842454 forest-python-0.6.1/forest/binary_trees/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2022-01-10 06:48:02.000000 forest-python-0.6.1/forest/binary_trees/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5852 2022-01-26 04:14:00.000000 forest-python-0.6.1/forest/binary_trees/atomic_trees.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    15612 2022-01-26 04:14:00.000000 forest-python-0.6.1/forest/binary_trees/avl_tree.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     9933 2022-01-26 04:14:00.000000 forest-python-0.6.1/forest/binary_trees/binary_search_tree.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    15673 2022-01-26 04:14:00.000000 forest-python-0.6.1/forest/binary_trees/double_threaded_binary_tree.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    22093 2022-01-26 04:14:00.000000 forest-python-0.6.1/forest/binary_trees/red_black_tree.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    25300 2022-01-26 04:14:00.000000 forest-python-0.6.1/forest/binary_trees/single_threaded_binary_trees.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    13712 2022-01-10 06:48:02.000000 forest-python-0.6.1/forest/binary_trees/traversal.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2712 2022-01-10 06:48:02.000000 forest-python-0.6.1/forest/metrics.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      364 2022-01-10 06:48:02.000000 forest-python-0.6.1/forest/tree_exceptions.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2022-01-26 04:30:24.842454 forest-python-0.6.1/forest_python.egg-info/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1777 2022-01-26 04:30:24.000000 forest-python-0.6.1/forest_python.egg-info/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      554 2022-01-26 04:30:24.000000 forest-python-0.6.1/forest_python.egg-info/SOURCES.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2022-01-26 04:30:24.000000 forest-python-0.6.1/forest_python.egg-info/dependency_links.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        7 2022-01-26 04:30:24.000000 forest-python-0.6.1/forest_python.egg-info/top_level.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2022-01-26 04:30:24.842454 forest-python-0.6.1/setup.cfg
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      749 2022-01-26 04:14:00.000000 forest-python-0.6.1/setup.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-26 05:29:22.382585 forest-python-0.6.3/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1067 2023-04-19 05:46:25.000000 forest-python-0.6.3/LICENSE
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1864 2023-04-26 05:29:22.382585 forest-python-0.6.3/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1421 2023-04-19 05:46:25.000000 forest-python-0.6.3/README.rst
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-26 05:29:22.372585 forest-python-0.6.3/forest/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-19 05:46:25.000000 forest-python-0.6.3/forest/__init__.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-26 05:29:22.372585 forest-python-0.6.3/forest/binary_trees/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-19 05:46:25.000000 forest-python-0.6.3/forest/binary_trees/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5852 2023-04-19 05:46:25.000000 forest-python-0.6.3/forest/binary_trees/atomic_trees.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    15610 2023-04-19 06:15:21.000000 forest-python-0.6.3/forest/binary_trees/avl_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     9932 2023-04-19 06:15:21.000000 forest-python-0.6.3/forest/binary_trees/binary_search_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    15663 2023-04-19 06:15:21.000000 forest-python-0.6.3/forest/binary_trees/double_threaded_binary_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    22093 2023-04-19 05:46:25.000000 forest-python-0.6.3/forest/binary_trees/red_black_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    25297 2023-04-19 06:15:21.000000 forest-python-0.6.3/forest/binary_trees/single_threaded_binary_trees.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)    13707 2023-04-19 06:15:21.000000 forest-python-0.6.3/forest/binary_trees/traversal.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2700 2023-04-19 05:46:25.000000 forest-python-0.6.3/forest/metrics.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      364 2023-04-19 05:46:25.000000 forest-python-0.6.3/forest/tree_exceptions.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-26 05:29:22.372585 forest-python-0.6.3/forest_python.egg-info/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1864 2023-04-26 05:29:22.000000 forest-python-0.6.3/forest_python.egg-info/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      803 2023-04-26 05:29:22.000000 forest-python-0.6.3/forest_python.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2023-04-26 05:29:22.000000 forest-python-0.6.3/forest_python.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       21 2023-04-26 05:29:22.000000 forest-python-0.6.3/forest_python.egg-info/top_level.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      568 2023-04-19 06:15:35.000000 forest-python-0.6.3/pyproject.toml
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2023-04-26 05:29:22.382585 forest-python-0.6.3/setup.cfg
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-26 05:29:22.372585 forest-python-0.6.3/tests/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     6816 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_atomic_trees.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     7840 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_avl_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2127 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_binary_search_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5151 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_double_threaded_binary_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1340 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_metrics.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     6689 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_red_black_tree.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     7546 2023-04-19 05:46:25.000000 forest-python-0.6.3/tests/test_single_threaded_binary_trees.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     4128 2023-04-19 06:15:21.000000 forest-python-0.6.3/tests/test_traversal.py
```

### Comparing `forest-python-0.6.1/LICENSE` & `forest-python-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forest-python-0.6.1/PKG-INFO` & `forest-python-0.6.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: forest-python
-Version: 0.6.1
-Summary: The Forest Project in Python
-Home-page: https://github.com/shunsvineyard/forest-python
-Author: Shun Huang
-Author-email: zsh@shunsvineyard.info
-License: MIT
-Keywords: tree data-structures
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Build the Forest in Python
 ==========================
 
 .. image:: https://github.com/shunsvineyard/forest-python/actions/workflows/testing.yml/badge.svg
     :target: https://github.com/shunsvineyard/forest-python/actions/workflows/testing.yml
 
 .. image:: https://github.com/shunsvineyard/forest-python/actions/workflows/linting.yml/badge.svg
@@ -53,9 +39,7 @@
 - Install from Github
 
 .. code-block:: bash
 
     git clone https://github.com/shunsvineyard/forest-python.git
     cd forest-python
     pip install -r requirements.txt
-
-
```

### Comparing `forest-python-0.6.1/README.rst` & `forest-python-0.6.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: forest-python
+Version: 0.6.3
+Summary: The Forest Project in Python
+Author-email: Shun Huang <shun@formosa1544.com>
+License: MIT License
+Project-URL: repository, https://github.com/burpeesDaily/forest-python
+Keywords: tree,data-structures
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Build the Forest in Python
 ==========================
 
 .. image:: https://github.com/shunsvineyard/forest-python/actions/workflows/testing.yml/badge.svg
     :target: https://github.com/shunsvineyard/forest-python/actions/workflows/testing.yml
 
 .. image:: https://github.com/shunsvineyard/forest-python/actions/workflows/linting.yml/badge.svg
```

### Comparing `forest-python-0.6.1/forest/binary_trees/atomic_trees.py` & `forest-python-0.6.3/forest/binary_trees/atomic_trees.py`

 * *Files identical despite different names*

### Comparing `forest-python-0.6.1/forest/binary_trees/avl_tree.py` & `forest-python-0.6.3/forest/binary_trees/avl_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
 
         Parameters
         ----------
         key: `Any`
             The key of the node to be deleted.
         """
         if self.root and (deleting_node := self._search(key=key)):
-
             # Case: no child
             if (deleting_node.left is None) and (deleting_node.right is None):
                 self._delete_no_child(deleting_node=deleting_node)
             # Case: Two children
             elif deleting_node.left and deleting_node.right:
                 replacing_node = self.get_leftmost(node=deleting_node.right)
                 # Replace the deleting node with the replacing node,
@@ -426,15 +425,14 @@
         else:
             deleting_node.parent.right = replacing_node
 
         if replacing_node:
             replacing_node.parent = deleting_node.parent
 
     def _delete_fixup(self, fixing_node: Node) -> None:
-
         while fixing_node:
             fixing_node.height = 1 + max(
                 self.get_height(fixing_node.left), self.get_height(fixing_node.right)
             )
 
             if self._get_balance_factor(fixing_node) > 1:
                 # Case Left-Left
```

### Comparing `forest-python-0.6.1/forest/binary_trees/binary_search_tree.py` & `forest-python-0.6.3/forest/binary_trees/binary_search_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 
         Parameters
         ----------
         key: `Any`
             The key of the node to be deleted.
         """
         if self.root and (deleting_node := self._search(key=key)):
-
             # Case 1: no child or Case 2a: only one right child
             if deleting_node.left is None:
                 self._transplant(
                     deleting_node=deleting_node, replacing_node=deleting_node.right
                 )
 
             # Case 2b: only one left left child
```

### Comparing `forest-python-0.6.1/forest/binary_trees/double_threaded_binary_tree.py` & `forest-python-0.6.3/forest/binary_trees/double_threaded_binary_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,14 @@
         `DuplicateKeyError`
             Raised if the key to be insted has existed in the tree.
         """
         node = Node(key=key, data=data)
         if self.root is None:
             self.root = node
         else:
-
             temp = self.root
 
             while temp:
                 # Move to left subtree
                 if node.key < temp.key:
                     if temp.left_thread is False and temp.left:
                         temp = temp.left
@@ -182,38 +181,35 @@
 
         Parameters
         ----------
         key: `Any`
             The key of the node to be deleted.
         """
         if self.root and (deleting_node := self._search(key=key)):
-
             # Case 1: no child
             if (deleting_node.left_thread or deleting_node.left is None) and (
                 deleting_node.right_thread or deleting_node.right is None
             ):
                 self._transplant(deleting_node=deleting_node, replacing_node=None)
 
             # Case 2a: only one right child
             elif (
                 deleting_node.left_thread or deleting_node.left is None
             ) and deleting_node.right_thread is False:
-
                 successor = self.get_successor(node=deleting_node)
                 if successor:
                     successor.left = deleting_node.left
                 self._transplant(
                     deleting_node=deleting_node, replacing_node=deleting_node.right
                 )
 
             # Case 2b: only one left child,
             elif (
                 deleting_node.right_thread or deleting_node.right is None
             ) and deleting_node.left_thread is False:
-
                 predecessor = self.get_predecessor(node=deleting_node)
                 if predecessor:
                     predecessor.right = deleting_node.right
                 self._transplant(
                     deleting_node=deleting_node, replacing_node=deleting_node.left
                 )
 
@@ -439,41 +435,35 @@
             if self.root:
                 self.root.left_thread = False
                 self.root.right_thread = False
         elif deleting_node == deleting_node.parent.left:
             deleting_node.parent.left = replacing_node
 
             if replacing_node:
-
                 if deleting_node.left_thread:
-
                     if replacing_node.left_thread:
                         replacing_node.left = deleting_node.left
 
                 if deleting_node.right_thread:
-
                     if replacing_node.right_thread:
                         replacing_node.right = replacing_node.right
 
             else:
                 deleting_node.parent.left = deleting_node.left
                 deleting_node.parent.left_thread = True
 
         else:  # deleting_node == deleting_node.parent.right
             deleting_node.parent.right = replacing_node
 
             if replacing_node:
-
                 if deleting_node.left_thread:
-
                     if replacing_node.left_thread:
                         replacing_node.left = deleting_node.left
 
                 if deleting_node.right_thread:
-
                     if replacing_node.right_thread:
                         replacing_node.right = replacing_node.right
 
             else:
                 deleting_node.parent.right = deleting_node.right
                 deleting_node.parent.right_thread = True
```

### Comparing `forest-python-0.6.1/forest/binary_trees/red_black_tree.py` & `forest-python-0.6.3/forest/binary_trees/red_black_tree.py`

 * *Files identical despite different names*

### Comparing `forest-python-0.6.1/forest/binary_trees/single_threaded_binary_trees.py` & `forest-python-0.6.3/forest/binary_trees/single_threaded_binary_trees.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         `Optional[Node]`
             The node found by the given key.
         If the key does not exist, return `None`.
         """
         return self._search(key=key)
 
     def _search(self, key: Any) -> Optional[Node]:
-
         current = self.root
         while current:
             if key == current.key:
                 return current
             elif key < current.key:
                 current = current.left
             else:  # key > current.key
@@ -171,15 +170,14 @@
 
         Parameters
         ----------
         key: `Any`
             The key of the node to be deleted.
         """
         if self.root and (deleting_node := self._search(key=key)):
-
             # Case 1: no child
             if deleting_node.left is None and (
                 deleting_node.right is None or deleting_node.is_thread
             ):
                 self._transplant(deleting_node=deleting_node, replacing_node=None)
 
             # Case 2a: only one left child
@@ -563,15 +561,14 @@
 
         Parameters
         ----------
         key: `Any`
             The key of the node to be deleted.
         """
         if self.root and (deleting_node := self._search(key=key)):
-
             # Case 1: no child
             if deleting_node.right is None and (
                 deleting_node.left is None or deleting_node.is_thread
             ):
                 self._transplant(deleting_node=deleting_node, replacing_node=None)
 
             # Case 2a: only one left child
```

### Comparing `forest-python-0.6.1/forest/binary_trees/traversal.py` & `forest-python-0.6.3/forest/binary_trees/traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,26 +254,24 @@
     stack = []
     if root.right:
         stack.append(root.right)
     stack.append(root)
     current = root.left
 
     while True:
-
         if current:
             if current.right:
                 stack.append(current.right)
                 stack.append(current)
                 current = current.left
                 continue
             stack.append(current)
             current = current.left
 
         else:  # current is None
-
             if len(stack) > 0:
                 current = stack.pop()
 
                 if current.right is None:
                     yield (current.key, current.data)
                     current = None
                     continue
@@ -306,26 +304,24 @@
     stack = []
     if root.left:
         stack.append(root.left)
     stack.append(root)
     current = root.right
 
     while True:
-
         if current:
             if current.left:
                 stack.append(current.left)
                 stack.append(current)
                 current = current.right
                 continue
             stack.append(current)
             current = current.right
 
         else:  # current is None
-
             if len(stack) > 0:
                 current = stack.pop()
 
                 if current.left is None:
                     yield (current.key, current.data)
                     current = None
                     continue
@@ -383,15 +379,14 @@
     stack = []
     if root.right:
         stack.append(root.right)
     stack.append(root)
     current = root.left
 
     while True:
-
         if current:
             if current.right:
                 stack.append(current.right)
                 stack.append(current)
                 current = current.left
                 continue
             else:  # current.right is None
```

### Comparing `forest-python-0.6.1/forest/metrics.py` & `forest-python-0.6.3/forest/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Licensed under MIT License.
 # See LICENSE in the project root for license information.
 
 """Metrics model to measure tree performance."""
 
 import numpy as np
 
-from typing import Dict, List, Union
+from typing import Union
 
 
 class Counter:
     """An incrementing and decrementing counter metric."""
 
     def __init__(self) -> None:
         self._count = 0
@@ -41,27 +41,27 @@
         return self._count
 
 
 class Histogram:
     """A metric which calculates the distribution of a value."""
 
     def __init__(self) -> None:
-        self._values: List[int] = list()
+        self._values: list[int] = list()
 
     def update(self, value: int) -> None:
         """Add a recorded value.
 
         Parameters
         ----------
         value: `int`
             value to be updated
         """
         self._values.append(value)
 
-    def report(self) -> Dict:
+    def report(self) -> dict:
         """Return the histogram report."""
         array = np.array(self._values)
         return {
             "min": array.min(),
             "max": array.max(),
             "medium": np.median(array),
             "mean": array.mean(),
@@ -78,15 +78,15 @@
 """Alias for the supported metric types."""
 
 
 class MetricRegistry:
     """A registry for metric instances."""
 
     def __init__(self) -> None:
-        self._registry: Dict[str, MetricType] = dict()
+        self._registry: dict[str, MetricType] = dict()
 
     def register(self, name: str, metric: MetricType) -> None:
         """Given a metric, register it under the given name.
 
         Parameters
         ----------
         name: `str`
```

### Comparing `forest-python-0.6.1/forest_python.egg-info/PKG-INFO` & `forest-python-0.6.3/forest_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: forest-python
-Version: 0.6.1
+Version: 0.6.3
 Summary: The Forest Project in Python
-Home-page: https://github.com/shunsvineyard/forest-python
-Author: Shun Huang
-Author-email: zsh@shunsvineyard.info
-License: MIT
-Keywords: tree data-structures
-Platform: UNKNOWN
+Author-email: Shun Huang <shun@formosa1544.com>
+License: MIT License
+Project-URL: repository, https://github.com/burpeesDaily/forest-python
+Keywords: tree,data-structures
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Build the Forest in Python
 ==========================
 
@@ -53,9 +53,7 @@
 - Install from Github
 
 .. code-block:: bash
 
     git clone https://github.com/shunsvineyard/forest-python.git
     cd forest-python
     pip install -r requirements.txt
-
-
```

