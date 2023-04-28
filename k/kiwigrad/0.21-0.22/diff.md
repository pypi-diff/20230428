# Comparing `tmp/kiwigrad-0.21.tar.gz` & `tmp/kiwigrad-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.21.tar", last modified: Thu Apr 27 13:49:51 2023, max compression
+gzip compressed data, was "kiwigrad-0.22.tar", last modified: Thu Apr 27 21:25:06 2023, max compression
```

## Comparing `kiwigrad-0.21.tar` & `kiwigrad-0.22.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.890771 kiwigrad-0.21/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.21/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.21/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3178 2023-04-27 13:49:51.888813 kiwigrad-0.21/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1320 2023-04-20 21:05:52.000000 kiwigrad-0.21/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.878316 kiwigrad-0.21/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      324 2023-04-27 13:43:36.000000 kiwigrad-0.21/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8659 2023-04-27 13:36:32.000000 kiwigrad-0.21/kiwigrad/engine.c
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.21/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.21/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.21/kiwigrad/layers.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.21/kiwigrad/neurons.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.21/kiwigrad/nn.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.21/kiwigrad/skeleton.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.884191 kiwigrad-0.21/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3178 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      376 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-27 13:47:47.000000 kiwigrad-0.21/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-27 13:49:51.891179 kiwigrad-0.21/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-04-27 13:39:57.000000 kiwigrad-0.21/setup.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.886318 kiwigrad-0.21/test/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1353 2023-04-19 21:20:17.000000 kiwigrad-0.21/test/test.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 21:25:06.609819 kiwigrad-0.22/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.22/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.22/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2176 2023-04-27 21:25:06.609534 kiwigrad-0.22/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1700 2023-04-27 14:59:17.000000 kiwigrad-0.22/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 21:25:06.606511 kiwigrad-0.22/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      253 2023-04-27 20:26:18.000000 kiwigrad-0.22/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9302 2023-04-27 21:24:37.000000 kiwigrad-0.22/kiwigrad/engine.c
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.22/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.22/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.22/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.22/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.22/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 21:25:06.608309 kiwigrad-0.22/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2176 2023-04-27 21:25:06.000000 kiwigrad-0.22/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      312 2023-04-27 21:25:06.000000 kiwigrad-0.22/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-27 21:25:06.000000 kiwigrad-0.22/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-27 21:25:06.000000 kiwigrad-0.22/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-27 21:25:06.609971 kiwigrad-0.22/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-04-27 20:23:13.000000 kiwigrad-0.22/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 21:25:06.608791 kiwigrad-0.22/test/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      618 2023-04-27 14:12:42.000000 kiwigrad-0.22/test/test.py
```

### Comparing `kiwigrad-0.21/LICENSE` & `kiwigrad-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.21/kiwigrad/engine.c` & `kiwigrad-0.22/kiwigrad/engine.c`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,22 @@
 relu_backward(PyObject *self) {
   Value *child = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
   child->grad += (((Value *)self)->data > 0) * ((Value *)self)->grad;
   Py_RETURN_NONE;
 }
 
 static PyObject *
+sigmoid_backward(PyObject *self) {
+  Value *child = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
+  double x = ((Value *)self)->data;
+  child->grad += (x * (1 - x)) * ((Value *)self)->grad;
+  Py_RETURN_NONE;
+}
+
+static PyObject *
 add_backward(PyObject *self) {
   Value *child_1 = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 0));
   Value *child_2 = ((Value *)PyTuple_GetItem(((Value *)self)->prev, 1));
   
   child_1->grad += ((Value *)self)->grad;
   child_2->grad += ((Value *)self)->grad;
   Py_RETURN_NONE;
@@ -146,15 +154,16 @@
 }
 
 typedef PyObject * (*BackwardFunction)(PyObject *);
 static BackwardFunction backward_methods[] = {
    &add_backward,
    &mul_backward,
    &pow_backward,
-   &relu_backward
+   &relu_backward,
+   &sigmoid_backward
   };
 
 static PyObject * Value_relu(PyObject *self) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   if (((Value *)self)->data < 0.0) {
     value->data = 0.0;
   } else {
@@ -162,14 +171,26 @@
   }
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
   value->func_idx = 3;
   return (PyObject *)value;
 }
 
+static PyObject * Value_sigmoid(PyObject *self) {
+  Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
+  double x = ((Value *)self)->data;
+  double t = 1 / (1 + exp(-x));
+  value->data = t;
+  value->grad = 0.0;
+  value->prev = PyTuple_Pack(1, self);
+  value->func_idx = 4;
+  return (PyObject *)value;
+}
+
+
 static void list_append(List *list, PyObject *value) {
   Node *node = malloc(sizeof(Node));
   node->value = ((Value *)value);
   node->next = NULL;
   if (!(list->head)) {
     node->prev = NULL;
     list->head = node;
@@ -218,14 +239,15 @@
     node = node->prev;
   }
   Py_RETURN_NONE;
 }
 
 static PyMethodDef Value_methods[] = {
     {"relu", (PyCFunction)Value_relu, METH_NOARGS, "ReLU"},
+    {"sigmoid", (PyCFunction)Value_sigmoid, METH_NOARGS, "Sigmoid"},
     // {"_backward", (PyCFunction)_backward, METH_NOARGS, "Backward"}, // DEBUG
     {"backward", (PyCFunction)backward, METH_NOARGS, "Backward"},
     {NULL}  /* Sentinel */
 };
 
 static PyMemberDef Value_members[] = {
    {"data", T_DOUBLE, offsetof(Value, data), 0, "Data"},
```

### Comparing `kiwigrad-0.21/kiwigrad/engine.py` & `kiwigrad-0.22/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.21/kiwigrad/layers.py` & `kiwigrad-0.22/kiwigrad/layers.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.21/kiwigrad/neurons.py` & `kiwigrad-0.22/kiwigrad/neurons.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.21/kiwigrad/nn.py` & `kiwigrad-0.22/kiwigrad/nn.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.21/setup.py` & `kiwigrad-0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools.extension import Extension
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='kiwigrad',
-      version='0.21',
+      version='0.22',
       description='Mini deep learning framework',
       author='Marco Salvalaggio',
       author_email='mar.salvalaggio@gmail.com',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/marcosalvalaggio/kiwigrad',
```

