# Comparing `tmp/QuantumIntelligence-0.0.4.tar.gz` & `tmp/QuantumIntelligence-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumIntelligence-0.0.4.tar", last modified: Fri Nov 25 12:41:12 2022, max compression
+gzip compressed data, was "QuantumIntelligence-0.0.5.tar", last modified: Fri Apr 28 05:21:39 2023, max compression
```

## Comparing `QuantumIntelligence-0.0.4.tar` & `QuantumIntelligence-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.384507 QuantumIntelligence-0.0.4/
--rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1763 2022-11-25 12:41:12.384507 QuantumIntelligence-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2022-11-25 12:41:12.384507 QuantumIntelligence-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     8844 2022-10-07 18:06:18.000000 QuantumIntelligence-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.357536 QuantumIntelligence-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.361419 QuantumIntelligence-0.0.4/src/QuantumIntelligence/
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.377521 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/
--rw-rw-rw-   0        0        0     1008 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
--rw-rw-rw-   0        0        0     7075 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/__init__.py
--rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
--rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
--rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.380839 QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/
--rw-rw-rw-   0        0        0    42657 2022-11-25 11:10:40.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/Circuit.py
--rw-rw-rw-   0        0        0     9710 2022-10-19 13:34:12.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/Gate.py
--rw-rw-rw-   0        0        0    14648 2022-10-19 14:04:31.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/Simulator.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.383498 QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/
--rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/MPSclass.py
--rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/TEBD.py
--rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/TNclass.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/__init__.py
--rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 12:41:12.365378 QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/
--rw-rw-rw-   0        0        0     1763 2022-11-25 12:41:12.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      977 2022-11-25 12:41:12.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-25 12:41:12.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-11-25 12:41:12.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-11-25 12:41:12.000000 QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.676466 QuantumIntelligence-0.0.5/
+-rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1763 2023-04-28 05:21:39.675391 QuantumIntelligence-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 05:21:39.676557 QuantumIntelligence-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     8844 2023-04-28 05:06:53.000000 QuantumIntelligence-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.647011 QuantumIntelligence-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.651836 QuantumIntelligence-0.0.5/src/QuantumIntelligence/
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.664937 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/
+-rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/__init__.py
+-rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
+-rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
+-rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.669432 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/
+-rw-rw-rw-   0        0        0    48902 2023-04-28 05:17:22.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Circuit.py
+-rw-rw-rw-   0        0        0     9960 2023-04-05 10:35:49.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Gate.py
+-rw-rw-rw-   0        0        0    18259 2023-04-28 05:17:22.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Simulator.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.674723 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/
+-rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/MPSclass.py
+-rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TEBD.py
+-rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TNclass.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.657170 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/top_level.txt
```

### Comparing `QuantumIntelligence-0.0.4/LICENSE` & `QuantumIntelligence-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/PKG-INFO` & `QuantumIntelligence-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.4
+Version: 0.0.5
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.4/README.md` & `QuantumIntelligence-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/setup.py` & `QuantumIntelligence-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="QuantumIntelligence",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.4",  # Required
+    version="0.0.5",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Developing quantum intelligence.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     s = open(path + file, 'wb')
     for ii in range(0, len(names)):
         tmp.pop(names[ii])
     pickle.dump(tmp, s)
     s.close()
 
 
-# These are from BasicFunctions of Ran Shi_ju with some changes
+# These are from BasicFunctions of Ran Shi-ju with some changes
 
 
 def save_pr(path, file, data, names):
     """
     Save the data as a dict in a file located in the path
     :param path: the location of the saved file
     :param file: the name of the file
```

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/Circuit.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Circuit.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,39 +16,45 @@
 import numpy as np
 import torch as tc
 import stim
 import copy
 import pyzx as zx
 from QuantumIntelligence.QuantumSimulator import Gate
 from QuantumIntelligence.BasicFunSZZ import tensor_trick as tt
+from cirq.contrib.qasm_import import circuit_from_qasm
+from cirq.circuits.qasm_output import QasmUGate
 
 
 
 # [1, 0] is |0>, [0, 1] is |1>
 # do not use fake functions, it will be removed soon
 # please apply gate on position as list(range(?)) as much as possible, this will make it faster
 # please control gate on position as list(range(?, n_qubit)) as much as possible, this will make it faster
 
 class Circuit:
 
-    def __init__(self, n_qubit, device='cpu', dtype=tc.complex64, size=None):
+    def __init__(self, n_qubit, device='cpu', dtype=tc.complex64, size=None, qubit_position=None):
         self.n_qubit = n_qubit
         self.device = device
         self.dtype = dtype
         self.gate_list = list()
         self.position_list = list()
         self.control_list = list()
         self.barrier_index = list()
-        self.qubit_position = list()
         if size is None:
             # i think it will be a long time before we build a quantum computer with over 10^200 qubits
             self.size = (1, int(1e200))
         else:
             self.size = size
-        self.initialize_position()
+        if qubit_position is None:
+            self.qubit_position = list()
+            for ii in range(self.n_qubit):
+                self.qubit_position.append((ii // self.size[1], ii % self.size[1]))
+        else:
+            self.qubit_position = qubit_position
 
 
     @property
     def requires_grad(self):
         flag = list()
         for gg in self.gate_list:
             flag.append(gg.requires_grad)
@@ -61,21 +67,14 @@
                 gg.requires_grad = requires_grad
         else:
             for nn in range(len(self)):
                 self.gate_list[nn].requires_grad = requires_grad[nn]
 
     # core functions start
 
-    def initialize_position(self):
-        if len(self.qubit_position) !=0:
-            raise ValueError('there has been a qubit position')
-        for ii in range(self.n_qubit):
-            self.qubit_position.append((ii // self.size[1], ii % self.size[1]))
-
-
     def compose(self, circuit, position=None, control=None, inverse=False):
         if isinstance(circuit, Circuit):
             tmp_circuit = copy.deepcopy(circuit)
             if inverse:
                 tmp_circuit.inv()
             self.__extend(tmp_circuit, position=position, control=control)
         elif isinstance(circuit, Gate.Gate):
@@ -273,38 +272,57 @@
                         if nn in index_list_strict:
                             index_list_strict.remove(nn)
                     ii = ii + 1
         self.gate_list = new_gate_list
         self.position_list = new_position_list
         self.control_list = new_control_list
 
+    def map_qubits(self, qubit_map:dict):
+        for ii in range(len(self)):
+            self.position_list[ii] = [qubit_map[pp] for pp in self.position_list[ii]]
+            self.control_list[ii] = [qubit_map[pp] for pp in self.control_list[ii]]
+        self.qubit_position = [self.qubit_position[ii] for ii in qubit_map.keys()]
+
+    def using_qubits(self):
+        using_qubits = list()
+        for _, position, control in self:
+            using_qubits.extend(position)
+            using_qubits.extend(control)
+        using_qubits = sorted(list(set(using_qubits)))
+        return using_qubits
+
+    def map2usingQubits(self):
+        using_qubits = self.using_qubits()
+        map_dict = dict(zip(using_qubits, range(len(using_qubits))))
+        self.map_qubits(map_dict)
+        self.n_qubit = len(using_qubits)
+
     # core functions end
     # practical functions start
 
     # universal gate set from experiment
 
     def rx_gate(self, position, theta=np.pi, control=None):
-        tmp_gate = Gate.rx_gate(theta=theta, device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.rx_gate(theta=theta)
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def ry_gate(self, position, theta=np.pi, control=None):
-        tmp_gate = Gate.ry_gate(theta=theta, device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.ry_gate(theta=theta)
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def rz_gate(self, position, theta=np.pi, control=None):
-        tmp_gate = Gate.rz_gate(theta=theta, device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.rz_gate(theta=theta)
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def cz_gate(self, position):
-        tmp_gate = Gate.cz_gate(device=self.device, dtype=self.dtype)
-        for pp in position:
-            self.add_single_gate(tmp_gate, position=pp)
+        tmp_gate = Gate.cz_gate()
+        self.add_single_gate(tmp_gate, position=position)
 
     # decompose circuit to experimental gates
 
     def decompose2experimental_gate(self):
         # global phases are ignored
 
         old_gate_list = self.gate_list
@@ -457,16 +475,14 @@
                     walk_index = walk_index - 1
                 if walk_index <= 0:
                     self.pop(rxy_index)
                 if walk_index  == 0:
                     self.gate_list.insert(check_index + 1, Gate.r_gate(theta=walk_label[1], label=walk_label[0]))
                     self.position_list.insert(check_index + 1, [walk_position])
                     self.control_list.insert(check_index + 1, [])
-
-
             rxy_index = rxy_index - 1
         self.to(self.device).to(self.dtype)
             
     def cancel_xyz_surface_code_abandoned(self):
         walk_index = 0
         xyz_list = ['X', 'Y', 'Z']
         rxyz_list = ['RX', 'RY', 'RZ']
@@ -496,54 +512,58 @@
         for pp in position:
             if not isinstance(pp, list):
                 pp = [pp]
             self.add_single_gate(tmp_gate, position=pp, control=control)
 
 
     def x_gate(self, position, control=None):
-        tmp_gate = Gate.x_gate(device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.x_gate()
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def y_gate(self, position, control=None):
-        tmp_gate = Gate.y_gate(device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.y_gate()
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def z_gate(self, position, control=None):
-        tmp_gate = Gate.z_gate(device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.z_gate()
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def hadamard(self, position, control=None):
-        tmp_gate = Gate.hadamard(device=self.device, dtype=self.dtype)
+        tmp_gate = Gate.hadamard()
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def phase_shift(self, position, theta=tc.pi, control=None):
         for pp in position:
             tmp_gate = Gate.phase_shift(theta, device=self.device, dtype=self.dtype)
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def not_gate(self, position, control=None):
         for pp in position:
-            tmp_gate = Gate.not_gate(device=self.device, dtype=self.dtype)
+            tmp_gate = Gate.not_gate()
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def rand_gate(self, dim, position, control=None, requires_grad=False):
         tmp_gate = Gate.rand_gate(dim, device=self.device, dtype=self.dtype, requires_grad=requires_grad)
         self.add_single_gate(tmp_gate, position=position, control=control)
 
     def swap_gate(self, position, control=None):
         if len(position) != 2:
-            print('wrong use')
+            raise ValueError('wrong use')
         else:
-            tmp_gate = Gate.swap_gate(device=self.device, dtype=self.dtype)
+            tmp_gate = Gate.swap_gate()
             self.add_single_gate(tmp_gate, position=position, control=control)
 
+    def ccx_gate(self, position, control=None):
+        tmp_gate = Gate.ccx_gate()
+        self.add_single_gate(tmp_gate, position=position, control=control)
+
     def time_evolution(self, hamiltonian, time, position, control=None):
         tmp_gate = Gate.time_evolution(hamiltonian, time, device=self.device, dtype=self.dtype)
         self.add_single_gate(tmp_gate, position=position, control=control)
 
     def qft(self, position, control=None, inverse=False):
         if control is None:
             control = []
@@ -577,55 +597,77 @@
             n_f=None, control=None, inverse=False):
         tmp_circuit = qdc(self.n_qubit, unitary, position_phi, position_coin, position_f,
                           n_f, control, inverse, device=self.device, dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def to_qiskit(self):
         qiskit_circuit = qiskit.QuantumCircuit(self.n_qubit)
-        supported_label = ['CZ', 'CX', 'CY', 'H']
-        supported_label_c = ['X', 'Y', 'Z']
-        supported_label_r = ['RX', 'RY', 'RZ']
+        supported_label = ('CZ', 'CX', 'CY', 'H', 'SWAP', 'S', 'T', 'CCX')
+        supported_label_c = ('X', 'Y', 'Z', 'NOT')
+        supported_label_r = ('RX', 'RY', 'RZ')
+        supported_label_u = ('U3', 'U4')
         for ii in range(len(self)):
             old_label = self.gate_list[ii].label
             q_position = self.position_list[ii]
             c_position = self.control_list[ii]
             if old_label is None:
+                print(self.gate_list[ii].tensor)
                 raise ValueError('The ', str(ii), '-th gate does not have label.')
-
             if old_label in supported_label:
                 if len(c_position) > 0:
                     raise ValueError('Do not support control.', supported_label)
                 # not the swap between control and target qubit
                 if old_label == 'CX':
                     qiskit_circuit.cx(control_qubit=q_position[0], target_qubit=q_position[1])
                 elif old_label == 'CY':
                     qiskit_circuit.cy(control_qubit=q_position[0], target_qubit=q_position[1])
                 elif old_label == 'CZ':
                     qiskit_circuit.cz(control_qubit=q_position[0], target_qubit=q_position[1])
                 elif old_label == 'H':
                     qiskit_circuit.h(qubit=q_position)
+                elif old_label == 'SWAP':
+                    qiskit_circuit.cx(control_qubit=q_position[0], target_qubit=q_position[1])
+                    qiskit_circuit.cx(control_qubit=q_position[1], target_qubit=q_position[0])
+                    qiskit_circuit.cx(control_qubit=q_position[0], target_qubit=q_position[1])
+                elif old_label == 'CCX':
+                    qiskit_circuit.ccx(control_qubit1=q_position[0], control_qubit2=q_position[1],
+                                       target_qubit=q_position[2])
+                elif old_label == 'S':
+                    if self.gate_list[ii].inverse:
+                        qiskit_circuit.sdg(qubit=q_position)
+                    else:
+                        qiskit_circuit.s(qubit=q_position)
+                elif old_label == 'T':
+                    if self.gate_list[ii].inverse:
+                        qiskit_circuit.tdg(qubit=q_position)
+                    else:
+                        qiskit_circuit.t(qubit=q_position)
                 else:
                     raise ValueError('Please report this bug to deveploper. Error occurs in supported_label.')
             elif old_label in supported_label_c:
                 if len(c_position) == 0:
-                    if old_label == 'X':
+                    if old_label in ('X', 'NOT'):
                         qiskit_circuit.x(qubit=q_position)
                     elif old_label == 'Y':
                         qiskit_circuit.y(qubit=q_position)
                     elif old_label == 'Z':
                         qiskit_circuit.z(qubit=q_position)
                     else:
                         raise ValueError('Please report this bug to deveploper. Error occurs in supported_label_c.')
-                elif len(c_position) == 1:
-                    if old_label == 'X':
-                        qiskit_circuit.cx(control_qubit=c_position, target_qubit=q_position)
-                    elif old_label == 'Y':
-                        qiskit_circuit.cy(control_qubit=c_position, target_qubit=q_position)
+                elif len(c_position) < 5:
+                    # testing
+                    if old_label in ('X', 'NOT'):
+                        qiskit_circuit.mcx(control_qubits=c_position, target_qubit=q_position)
                     elif old_label == 'Z':
-                        qiskit_circuit.cz(control_qubit=c_position, target_qubit=q_position)
+                        if len(c_position) == 1:
+                            qiskit_circuit.cz(control_qubit=c_position, target_qubit=q_position)
+                        elif len(c_position) == 2:
+                            qiskit_circuit.ccz(control_qubits=c_position, target_qubit=q_position)
+                        else:
+                            raise ValueError('Do not multi support control.', supported_label_c)
                 else:
                     raise ValueError('Do not multi support control.', supported_label_c)
             elif old_label[0] in supported_label_r:
                 theta = old_label[1]
                 if self.gate_list[ii].inverse:
                     theta = -theta
                 if len(c_position) > 0:
@@ -635,18 +677,39 @@
                         qiskit_circuit.rx(theta=theta, qubit=q_position)
                     elif old_label[0] == 'RY':
                         qiskit_circuit.ry(theta=theta, qubit=q_position)
                     elif old_label[0] == 'RZ':
                         qiskit_circuit.rz(phi=theta, qubit=q_position)
                     else:
                         raise ValueError('Please report this bug to deveploper. Error occurs in supported_label_r.')
+            elif old_label[0] in supported_label_u:
+                theta = (old_label[1][0], old_label[1][1], old_label[1][2])
+                if self.gate_list[ii].inverse:
+                    theta = (-theta[0], - theta[2], - theta[1])
+                if len(c_position) > 1:
+                    raise ValueError('Do not support control.', supported_label_u)
+                if len(c_position) == 0:
+                    if old_label[0] in ('U3', 'U4'):
+                        qiskit_circuit.u(theta[0], theta[1], theta[2], qubit=q_position)
+                elif len(c_position) == 1:
+                    if old_label[0] in ('U3', 'U4'):
+                        if old_label[0] == 'U4':
+                            theta3 = old_label[1][3]
+                        else:
+                            theta3 = 0
+                        if self.gate_list[ii].inverse:
+                            theta3 = - theta3
+                        qiskit_circuit.cu(*theta, gamma=theta3, control_qubit=c_position, target_qubit=q_position)
+                    else:
+                        raise ValueError('tired')
             else:
                 raise ValueError('Do not support the label of', str(ii), 'th gate, which is', old_label)
         return qiskit_circuit
 
+
     def to_qasm(self):
         # this is achieved by qiskit
         qiskit_circuit = self.to_qiskit()
         qasm_circuit = qiskit_circuit.qasm()
         return qasm_circuit
 
     def from_qasm(self, qasm_circuit, replace=False):
@@ -657,16 +720,18 @@
 
     def from_qiskit(self, qiskit_circuit, replace=False):
         if replace:
             circuit = self
             circuit.clear()
         else:
             circuit = Circuit(self.n_qubit, self.device, self.dtype, size=self.size)
-        supported_name_no_params = ['x', 'y', 'z', 'h', 'cx', 'cy', 'cz']
+        supported_name_no_params = ['x', 'y', 'z', 'h', 'cx', 'cy', 'cz', 'ccx', 'swap']
+        supported_name_specific = ['sdg', 'tdg', 's', 't']
         supported_name_with_params = ['rx', 'ry', 'rz']
+        supported_name_with_complex_params = ['u3']
         qiskit_register = qiskit_circuit.qregs[0]
         for instruction in qiskit_circuit:
             operation = instruction.operation
             qubits = instruction.qubits
             name = operation.name
             position = []
             for qq in qubits:
@@ -676,38 +741,65 @@
             if name in supported_name_no_params:
                 circuit.labelled_gate(name=name.upper(), position=position)
             elif name in supported_name_with_params:
                 params = operation.params[0]
                 if not isinstance(params, float):
                     params = float(params)
                 circuit.labelled_gate(name=name.upper(), position=position, params=params)
+            elif name in supported_name_specific:
+                if name == 'sdg':
+                    circuit.append(Gate.s_gate(), position=position, inverse=True)
+                    # circuit.rz_gate(position=position, theta=-np.pi/2)
+                elif name == 'tdg':
+                    circuit.append(Gate.t_gate(), position=position, inverse=True)
+                    # circuit.rz_gate(position=position, theta=-np.pi/4)
+                elif name == 't':
+                    circuit.append(Gate.t_gate(), position=position)
+                    # circuit.rz_gate(position=position, theta=np.pi/4)
+                elif name == 's':
+                    circuit.append(Gate.s_gate(), position=position)
+                    # circuit.rz_gate(position=position, theta=np.pi/2)
+                else:
+                    raise ValueError('Please report this bug to deveploper. Error occurs in supported_name_specific.')
+            elif name in supported_name_with_complex_params:
+                if name == 'u3':
+                    params = tuple(float(ii) for ii in operation.params)
+                    circuit.append(Gate.u3(theta=params), position=position)
+                else:
+                    raise ValueError('Please report this bug to deveploper. Error occurs in supported_name_specific.')
             else:
                 raise ValueError('Does not support', name)
         if not replace:
             return circuit
 
+    def positive_theta(self):
+        for ii in range(len(self)):
+            old_label = self.gate_list[ii].label
+            if old_label[0] in ('RX', 'RY', 'RZ'):
+                while self.gate_list[ii].label[1] <= 0:
+                    self.gate_list[ii].label = (old_label[0], self.gate_list[ii].label[1] + 4*np.pi)
 
 
     def zx_optimize(self, replace=False):
+        self.positive_theta()
         qiskit_circuit = self.to_qiskit()
-        print(self.to_qasm())
         zx_circuit = zx.Circuit.from_qasm(self.to_qasm())
-
-        new_zx_circuit = zx.optimize.basic_optimization(zx_circuit, do_swaps=False)
+        # print(zx_circuit)
+        new_zx_circuit = zx.optimize.basic_optimization(zx_circuit.split_phase_gates(), do_swaps=False)
+        # new_zx_circuit = zx_circuit
         new_qasm_circuit = new_zx_circuit.to_qasm()
-        circuit = self.from_qasm(new_qasm_circuit, replace=replace)
+        new_qiskit_circuit = qiskit.QuantumCircuit.from_qasm_str(new_qasm_circuit)
+        new_qiskit_circuit = qiskit.transpile(new_qiskit_circuit,basis_gates=['cz', 'rx', 'rz'],optimization_level=3)
+        circuit = self.from_qiskit(new_qiskit_circuit, replace=True)
+        # circuit = self.from_qasm(new_qasm_circuit, replace=replace)
         if not replace:
             return circuit
 
-    def qiskit_transpile(self, basis_gates=None, optimization_level=3, replace=False):
-        if basis_gates is None:
-            basis_gates = ['cz', 'rx', 'ry', 'rz']
-        qiskit_circuit = qiskit.transpile(self.to_qiskit(),
-                                          basis_gates=basis_gates,
-                                          optimization_level=optimization_level)
+    def qiskit_transpile(self, replace=True, **kwargs):
+        qiskit_circuit = qiskit.transpile(self.to_qiskit(),**kwargs)
         circuit = self.from_qiskit(qiskit_circuit=qiskit_circuit, replace=replace)
         if not replace:
             return circuit
 
     def to_stim(self):
         stim_circuit = stim.Circuit()
         same_label_control0_list = ['CX', 'CY', 'CZ', 'H']
@@ -762,32 +854,48 @@
                     raise ValueError('Do not support theta/np.pi = ', str(old_label[1]/np.pi))
                 new_position = self.position_list[ii]
             else:
                 raise ValueError('Do not support the label of', str(ii), 'th gate, which is', old_label)
             stim_circuit.append(new_label, new_position)
         return stim_circuit
 
+
     def to_cirq(self):
-        self.decompose2experimental_gate()
-        supported_gates = {'CZ':cirq.CZ, 'RX':cirq.rx, 'RY':cirq.ry, 'RZ':cirq.rz}
+        supported_gates_C = {'CZ':cirq.CZ, 'CX':cirq.CX}
+        supported_gates_R = {'RX':cirq.rx, 'RY':cirq.ry, 'RZ':cirq.rz}
+        supported_gates_CC = {'CCX':cirq.CCX, }
+        supported_gates_U = {'U3':QasmUGate}
         cirq_citcuit = cirq.Circuit()
         for ii in range(len(self)):
             if len(self.control_list[ii]) > 0:
                 raise ValueError('does not support controlled gates')
             tmp_label = self.gate_list[ii].label
-            if tmp_label == 'CZ':
+            if tmp_label in supported_gates_C.keys():
                 position0 = self.qubit_position[self.position_list[ii][0]]
                 position1 = self.qubit_position[self.position_list[ii][1]]
                 qubit0 = cirq.GridQubit(position0[0], position0[1])
                 qubit1 = cirq.GridQubit(position1[0], position1[1])
-                cirq_citcuit.append(supported_gates[tmp_label](qubit0, qubit1))
-            elif tmp_label[0] in supported_gates.keys():
+                cirq_citcuit.append(supported_gates_C[tmp_label](qubit0, qubit1))
+            elif tmp_label in supported_gates_CC.keys():
                 position0 = self.qubit_position[self.position_list[ii][0]]
+                position1 = self.qubit_position[self.position_list[ii][1]]
+                position2 = self.qubit_position[self.position_list[ii][2]]
                 qubit0 = cirq.GridQubit(position0[0], position0[1])
-                cirq_citcuit.append(supported_gates[tmp_label[0]](tmp_label[1])(qubit0))
+                qubit1 = cirq.GridQubit(position1[0], position1[1])
+                qubit2 = cirq.GridQubit(position2[0], position2[1])
+                cirq_citcuit.append(supported_gates_CC[tmp_label](qubit0, qubit1, qubit2))
+            elif tmp_label[0] in supported_gates_R.keys():
+                position0 = self.qubit_position[self.position_list[ii][0]]
+                qubit0 = cirq.GridQubit(position0[0], position0[1])
+                cirq_citcuit.append(supported_gates_R[tmp_label[0]](tmp_label[1])(qubit0))
+            elif tmp_label[0] in supported_gates_U.keys():
+                position0 = self.qubit_position[self.position_list[ii][0]]
+                qubit0 = cirq.GridQubit(position0[0], position0[1])
+                theta, phi, lmda = tmp_label[1]
+                cirq_citcuit.append(supported_gates_U[tmp_label[0]](theta/np.pi, phi/np.pi, lmda/np.pi)(qubit0))
             else:
                 raise ValueError(tmp_label, 'is not supported')
         return cirq_citcuit
 
     def cirq_qubit_order(self):
         cirq_order_list = []
 
@@ -797,14 +905,17 @@
         return cirq_order
 
     def draw_circuit_cirq(self, save_path='./cirq.html'):
         cirq_circuit = self.to_cirq()
         c3d = cirq_web.Circuit3D(cirq_circuit)
         c3d.generate_html_file(file_name=save_path)
 
+    def qiskit_draw(self, **kwargs):
+        return self.to_qiskit().draw(**kwargs)
+
 
 
 
 def qft(n_qubit, position, control=None, inverse=False, device='cpu', dtype=tc.complex64):
     if control is None:
         control = []
     tmp_circuit = Circuit(n_qubit, device, dtype)
```

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/Gate.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Gate.py`

 * *Files 14% similar despite different names*

```diff
@@ -134,26 +134,51 @@
     def assign_tensor(self):
         # _labelled_gate_no_params = ('X', 'Y', 'Z', 'H', 'CX', 'CY', 'CZ')
         # _labelled_gate_with_params = ('RX', 'RY', 'RZ')
         if self.label is None:
             raise ValueError('label is None. Can not assign tensor data')
         if self.label in ('X', 'Y', 'Z'):
             self.tensor = get_pauli(name=self.label)
+        elif self.label == 'NOT':
+            self.tensor = _pauli_x
         elif self.label == 'H':
             self.tensor = tc.tensor([[1, 1], [1, -1]]) / np.sqrt(2)
-        elif self.label in ('CX', 'CY', 'CZ'):
-            self.tensor = tc.eye(4, dtype=tc.complex64)
-            self.tensor[2:, 2:] = get_pauli(name=self.label[1])
+        elif self.label == 'CX':
+            self.tensor =  tc.diag(tc.tensor([1, 1, 0, 0]))
+            self.tensor[2, 3] = 1
+            self.tensor[3, 2] = 1
+        elif self.label == 'CZ':
+            self.tensor =  tc.diag(tc.tensor([1, 1, 1, -1]))
+        elif self.label == 'SWAP':
+            self.tensor = tc.zeros(4, 4)
+            self.tensor[0, 0] = 1
+            self.tensor[1, 2] = 1
+            self.tensor[2, 1] = 1
+            self.tensor[3, 3] = 1
+        elif self.label == 'CCX':
+            self.tensor =  tc.diag(tc.tensor([1, 1, 1, 1, 1, 1, 0, 0]))
+            self.tensor[6, 7] = 1
+            self.tensor[7, 6] = 1
         elif self.label[0] in ('RX', 'RY', 'RZ'):
             theta = self.label[1]
-            if self.inverse:
-                theta = -theta
             self.tensor = tc.eye(2)*math.cos(theta/2) - 1j * np.sin(theta/2)*get_pauli(name=self.label[0][1])
+        elif self.label[0] in ('U3', 'U4'):
+            theta = self.label[1]
+            self.tensor = tc.tensor([[np.cos(theta[0]/2), -np.exp(1j*theta[2])*np.sin(theta[0]/2)],
+                      [np.exp(1j*theta[1])*np.sin(theta[0]/2), np.exp(1j*(theta[1] + theta[2]))*np.cos(theta[0]/2)]],)
+            if self.label[0] == 'U4':
+                self.tensor = np.exp(1j*theta[3])*self.tensor
+        elif self.label[0] in ('S'):
+            self.tensor = tc.tensor([[1, 0], [0, np.exp(1j*np.pi/2)]])
+        elif self.label[0] in ('T'):
+            self.tensor = tc.tensor([[1, 0], [0, np.exp(1j*np.pi/4)]])
         else:
             raise ValueError('The label', self.label, 'is not supported')
+        if self.inverse:
+            self.tensor = self.tensor.T.conj()
 
 
     # core function end
 
 # labelled gate
 
 def labelled_simple_gate(name, params=None):
@@ -162,92 +187,87 @@
     else:
         return Gate(unitary=None, label=(name, params))
 
 
 # Experimental univerisal gate set
 
 
-def rx_gate(theta=np.pi, device='cpu', dtype=tc.complex64):
+def rx_gate(theta=np.pi):
     # exp(-i*theta * x/2)
-    gate = tc.eye(2)*math.cos(theta/2) - 1j * np.sin(theta/2)*_pauli_x
-    return Gate(gate.to(device).to(dtype), label=('RX', theta))
+    return Gate(unitary=None, label=('RX', theta))
 
 
-def ry_gate(theta=np.pi, device='cpu', dtype=tc.complex64):
+def ry_gate(theta=np.pi):
     # exp(-i*theta * y/2)
-    gate = tc.eye(2)*math.cos(theta/2) - 1j * np.sin(theta/2)*_pauli_y
-    return Gate(gate.to(device).to(dtype), label=('RY', theta))
+    return Gate(unitary=None, label=('RY', theta))
 
 
-def rz_gate(theta=np.pi, device='cpu', dtype=tc.complex64):
+def rz_gate(theta=np.pi):
     # exp(-i*theta * z/2)
-    gate = tc.eye(2)*math.cos(theta/2) - 1j * np.sin(theta/2)*_pauli_z
-    return Gate(gate.to(device).to(dtype), label=('RZ', theta))
+    return Gate(unitary=None, label=('RZ', theta))
 
 def r_gate(theta=np.pi, label='RZ', device='cpu', dtype=tc.complex64):
-    if label == 'RZ':
-        return rz_gate(theta=theta, device=device, dtype=dtype)
-    elif label == 'RX':
-        return rx_gate(theta=theta, device=device, dtype=dtype)
-    elif label == 'RY':
-        return ry_gate(theta=theta, device=device, dtype=dtype)
+    if label in ('RZ', 'RX', 'RY'):
+        return Gate(unitary=None, label=(label, theta))
     else:
         raise ValueError('Label must be RX, RY or RZ.')
 
 
-def cz_gate(device='cpu', dtype=tc.complex64):
-    gate = tc.eye(2).kron(_pauli_z)
-    return Gate(gate.to(device).to(dtype), label='CZ')
-
-def cx_gate(device='cpu', dtype=tc.complex64):
-    gate = tc.eye(2).kron(_pauli_x)
-    return Gate(gate.to(device).to(dtype), label='CX')
-
-def cy_gate(device='cpu', dtype=tc.complex64):
-    gate = tc.eye(2).kron(_pauli_y)
-    return Gate(gate.to(device).to(dtype), label='CY')
+def cz_gate():
+    return Gate(unitary=None, label='CZ')
+
+def cx_gate():
+    return Gate(unitary=None, label='CX')
+
+def ccx_gate(device='cpu', dtype=tc.complex64):
+    return Gate(unitary=None, label='CCX')
 
 # practical gates with label
 
-def hadamard(device='cpu', dtype=tc.complex64):
-    gate = tc.tensor([[1, 1], [1, -1]], device=device, dtype=dtype) / np.sqrt(2)
-    return Gate(gate, label='H')
+def u3(theta:tuple):
+    return Gate(unitary=None, label=('U3', theta))
+
+def u4(theta:tuple, device='cpu', dtype=tc.complex64):
+    return Gate(unitary=None, label=('U4', theta))
+
+def hadamard():
+    return Gate(unitary=None, label='H')
 
 
 def phase_shift(theta, device='cpu', dtype=tc.complex64):
     gate = tc.eye(2, device=device, dtype=dtype)
     gate[1, 1] = tc.exp(tc.tensor(theta * 1j))
     return Gate(gate)
 
 
-def not_gate(device='cpu', dtype=tc.complex64):
+def not_gate():
     # this gate will be discarded
-    gate = tc.tensor([[0, 1], [1, 0]], device=device, dtype=dtype)
-    return Gate(gate, label='NOT')
+    return Gate(unitary=None, label='NOT')
+
+
+def x_gate():
+    return Gate(unitary=None, label='X')
 
 
-def x_gate(device='cpu', dtype=tc.complex64):
-    return Gate(_pauli_x.to(device).to(dtype), label='X')
+def y_gate():
+    return Gate(unitary=None, label='Y')
 
 
-def y_gate(device='cpu', dtype=tc.complex64):
-    return Gate(_pauli_y.to(device).to(dtype), label='Y')
+def z_gate():
+    return Gate(unitary=None, label='Z')
 
+def t_gate():
+    return Gate(unitary=None, label='T')
 
-def z_gate(device='cpu', dtype=tc.complex64):
-    return Gate(_pauli_z.to(device).to(dtype), label='Z')
+def s_gate():
+    return Gate(unitary=None, label='S')
 
 
-def swap_gate(device='cpu', dtype=tc.complex64):
-    gate = tc.zeros(4, 4, device=device, dtype=dtype)
-    gate[0, 0] = 1
-    gate[1, 2] = 1
-    gate[2, 1] = 1
-    gate[3, 3] = 1
-    return Gate(gate, label='SWAP')
+def swap_gate():
+    return Gate(unitary=None, label='SWAP')
 
 # gate without label
 
 
 def rand_gate(dim=2, device='cpu', dtype=tc.complex64, requires_grad=False):
     # Haar random gate
     tmp_tensor = tc.randn(dim, dim, device=device, dtype=dtype)
```

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/QuantumSimulator/Simulator.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,38 +17,41 @@
 import qiskit
 import qiskit_aer
 import stim
 import cirq
 import qsimcirq
 import torch as tc
 from QuantumIntelligence.QuantumSimulator.Circuit import Circuit
+from QuantumIntelligence.BasicFunSZZ.BasicClass import DefaultValuedDict as DVD
+from QuantumIntelligence.BasicFunSZZ import BasicFunctions_szz as bf
 
 
 # [1, 0] is |0>, [0, 1] is |1>
 # do not use fake functions, it will be removed soon
 # please apply gate on position as list(range(?)) as much as possible, this will make it faster
 # please control gate on position as list(range(?, n_qubit)) as much as possible, this will make it faster
 
 class SimulatorProcess:
     def __init__(self, n_qubit, device='cuda:0', dtype=tc.complex64,
-                 rand_seed=1, fast_mode=True, state_acc=1e-3, circuit_size=None, default_simulator='QI'):
+                 rand_seed=1, fast_mode=False, state_acc=1e-5,
+                 circuit_size=None, default_simulator='QI', qubit_position=None):
         self.n_qubit = n_qubit
         self.device = device
         self.dtype = dtype
         self.rand_seed = rand_seed
         self._state = None
         self.shape = (2,) * self.n_qubit
         self.default_simulator = default_simulator
         self.initialize_state()
         self.tmp_gate = None
         self.chi = 2 ** self.n_qubit
         self.fast_mode = fast_mode
         self.state_acc = state_acc
         self.circuit_size = circuit_size
-        self.circuit = Circuit(n_qubit, device=device, dtype=dtype, size=circuit_size)
+        self.circuit = Circuit(n_qubit, device=device, dtype=dtype, size=circuit_size, qubit_position=qubit_position)
 
     def initialize_state(self):
         self._state = tc.zeros(2 ** self.n_qubit, device=self.device, dtype=self.dtype)
         self._state[0] = 1
         self._state = self._state.view(self.shape)
 
     def simulate(self, clear_circuit=True, method=None, fast_mode=None, state_acc=None):
@@ -107,15 +110,15 @@
             gpu_options = qsimcirq.QSimOptions(use_gpu=False)
         self.circuit.regularize_all_position()
         cirq_circuit = self.circuit.to_cirq()
         cirq_order = self.circuit.cirq_qubit_order()
         qsim_simulator = qsimcirq.QSimSimulator(qsim_options=gpu_options)
         result = qsim_simulator.simulate(program=cirq_circuit, qubit_order=cirq_order,
                                          initial_state=self._state.to(tc.complex64).cpu().numpy().reshape(-1))
-        self._state = tc.from_numpy(result.final_state_vector).to(self.device).to(self.dtype)
+        self.state = tc.from_numpy(result.final_state_vector).to(self.device).to(self.dtype)
         if clear_circuit:
             self.circuit.clear()
 
     def qiskit_simulate(self, clear_circuit=True):
         self.circuit.regularize_all_position()
         if 'cuda' in self.device:
             device = 'GPU'
@@ -179,43 +182,46 @@
             tmp_state = self._state.new_empty(self._state.size())
             tmp_state[:, :, -1] = tmp_gate.mm(self._state[:, :, -1])
             tmp_state[:, :, :-1] = self._state[:, :, :-1]
             self._state = tmp_state
 
         self._state = self._state.view(self.shape).movedim(new_position, old_position)
 
-    def sampling(self, n_shots=1024, position=None, basis=None, if_print=True, rand_seed=None):
+    def sampling(self, n_shots=1024, position=None, basis=None, if_print=True, rand_seed=None, return_weight=False):
         if rand_seed is None:
             rand_seed = self.rand_seed
         if rand_seed is not None:
             random.seed(rand_seed)
         if basis is not None:
             tmp_state = self.change_measure_basis(position, basis)
         else:
             tmp_state = self._state.clone().detach()
         if position is None:
             position = list(range(self.n_qubit))
             weight = tc.abs(tmp_state.contiguous().view(-1)) ** 2
             m_p = len(position)
         else:
             m_p = len(position)
-            state_tmp = tmp_state.movedim(position, list(range(m_p))).contiguous().view(2 ** m_p, -1)
-            weight = tc.abs(tc.einsum('ab,ba->a', state_tmp, state_tmp.conj().t()))
+            tmp_state = tmp_state.movedim(position, list(range(m_p))).contiguous().view(2 ** m_p, -1)
+            weight = tc.abs(tc.einsum('ab,ba->a', tmp_state, tmp_state.conj().t()))
 
         population = list()
         for pp in range(2 ** m_p):
             element = bin(pp)[2:]
             element = (m_p - len(element)) * '0' + element
             population.append(element)
 
         res = Counter(random.choices(population, weight, k=n_shots))
         if if_print:
             for key in res.keys():
                 print(key, res[key])
-        return res
+        if return_weight:
+            return res, weight
+        else:
+            return res
 
     @staticmethod
     def count_sample(res, ss, position, if_print=True):
         new_res = dict()
         for key in res.keys():
             flag = True
             for pp in position:
@@ -239,16 +245,18 @@
             if basis[nn] == 'x':
                 tmp_state = tc.einsum('abc,bd->adc', tmp_state.reshape(2 ** pp, -1, 2 ** (self.n_qubit - pp - 1)), x_basis)
             elif basis[nn] == 'y':
                 tmp_state = tc.einsum('abc,bd->adc', tmp_state.reshape(2 ** pp, -1, 2 ** (self.n_qubit - pp - 1)), y_basis)
             tmp_state = tmp_state.view(self.shape).contiguous()
         return tmp_state
 
-    def collapse(self, position, basis=None):
+    def collapse(self, position=None, basis=None):
         m_p = len(position)
+        if position == None:
+            position = list(range(self.n_qubit))
         if basis is None:
             basis = '0' * m_p
         if m_p != len(basis):
             raise ValueError('error in extend, check position')
         index = int(basis, 2)
         new_position = list(range(-m_p, 0))
         tmp_state = self.state.movedim(position, new_position).reshape(-1, 2 ** m_p)
@@ -283,14 +291,15 @@
         self.circuit = circuit
         self.simulate()
         fidelity = tc.einsum('a,a->', backup_state.reshape(-1), self._state.reshape(-1).conj())
         self.circuit = backup_circuit
         self._state = backup_state
         return fidelity
 
+
 # This program only provides interfere to stim
 class SimulatorStabilizer:
     def __init__(self, n_qubit, device='cuda:0', dtype=tc.complex64,
                  rand_seed=1, state_acc=1e-3, circuit_size=None):
         self.n_qubit = n_qubit
         self.device = device
         self.dtype = dtype
@@ -303,27 +312,26 @@
 
     @property
     def stim_circuit(self):
         self._stim_circuit = self.circuit.to_stim()
         return self._stim_circuit
 
     @stim_circuit.setter
-    def stim_circuit(self, stim_circuit:stim.Circuit):
-        print('warning, you should not set the stim circuit. This figure needs to be fixed. Be carefull!!')
+    def stim_circuit(self, stim_circuit: stim.Circuit):
+        print('warning, you should not set the stim circuit. This feature needs to be fixed. Be careful!!')
         self._stim_circuit = stim_circuit
 
     def simulate(self, clear_circuit=True, force_mode=False):
         if force_mode:
             self.simulator.do(self._stim_circuit)
         else:
             self.simulator.do(self.stim_circuit)
         if clear_circuit:
             self.circuit.clear()
 
-
     def fake_measure_circuit(self, circuit: Circuit):
         pauli_string = stim.PauliString(self.n_qubit)
         pauli_list = []
         for ii in range(len(circuit)):
             tmp_str = pauli_string[circuit.position_list[ii][0]]
             if tmp_str == 0:
                 pauli_string[circuit.position_list[ii][0]] = circuit.gate_list[ii].label
@@ -331,7 +339,90 @@
                 pauli_list.append(pauli_string)
                 pauli_string = stim.PauliString(self.n_qubit)
                 assert pauli_string[circuit.position_list[ii][0]] == 0
                 pauli_string[circuit.position_list[ii][0]] = circuit.gate_list[ii].label
         for pau in pauli_list:
             pauli_string = pau * pauli_string
         return self.simulator.peek_observable_expectation(pauli_string)
+
+
+# temporary program
+class SimulatorSparse(SimulatorProcess):
+    def initialize_state(self):
+        self._state = DVD(default_value=0)
+        self._state[self.n_qubit*'0'] = 1
+
+    def simulate(self, clear_circuit=True):
+        print('this is a test progarm!!!!!!!!!!!!!!!!!')
+        self.circuit.regularize_all_position()
+        if len(self.circuit) > 0:
+            for ii in range(len(self.circuit)):
+                cc = self.circuit[ii]
+                if len(cc[2])>0:
+                    raise ValueError('Does not support controlled gate')
+                self.act_single_gate(gate=cc[0], position=cc[1])
+        if clear_circuit:
+            self.circuit.clear()
+
+    @property
+    def state(self):
+        return self._state
+
+    @state.setter
+    def state(self, state):
+        raise ValueError('not support')
+
+    def act_single_gate(self, gate, position, control=None, fast_mode=False):
+        new_state = DVD(default_value=0)
+        if len(position) == 1:
+            # single qubit gate
+            pp = position[0]
+            gmatrix = gate.tensor
+            for kk in self._state.keys():
+                new_state[kk]  = new_state[kk] + self._state[kk] * gmatrix[int(kk[pp]), int(kk[pp])]
+                kk1 = kk[:pp] + str(int(kk[pp]=='0')) + kk[pp+1:]
+                new_state[kk1]  = new_state[kk1] + self._state[kk] * gmatrix[1 - int(kk[pp]), int(kk[pp])]
+        elif len(position) == 2:
+            if not gate.label == 'CZ':
+                raise ValueError('Only CZ is supported as two-qubit gate')
+            pp0 = position[0]
+            pp1 = position[1]
+            for kk in self._state.keys():
+                if (kk[pp0]=='1') and (kk[pp1]=='1'):
+                    new_state[kk] = self._state[kk]
+                else:
+                    new_state[kk] = -self._state[kk]
+        else:
+            raise ValueError('Gate not supported')
+        pop_keys = []
+        for kk in new_state.keys():
+            if tc.abs(new_state[kk]) < 1e-8:
+                pop_keys.append(kk)
+        for kk in pop_keys:
+            new_state.pop(kk)
+        self._state = new_state
+
+    @staticmethod
+    def sampling(self, n_shots=1024, position=None, if_print=True, rand_seed=None, return_weight=False):
+        if rand_seed is None:
+            rand_seed = self.rand_seed
+        if rand_seed is not None:
+            random.seed(rand_seed)
+        m_p = len(position)
+        population = list()
+        weight = 2**m_p *[0]
+        for pp in range(2 ** m_p):
+            element = bin(pp)[2:]
+            element = (m_p - len(element)) * '0' + element
+            population.append(element)
+            for kk in self._state.keys():
+                pointer = {kk[position[ii]] == element[ii] for ii in range(m_p)}
+                if False not in pointer:
+                    weight[pp] = weight[pp] + tc.abs(self._state[kk])**2
+        res = Counter(random.choices(population, weight, k=n_shots))
+        if if_print:
+            for key in res.keys():
+                print(key, res[key])
+        if return_weight:
+            return res, weight
+        else:
+            return res
```

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/MPSclass.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/MPSclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/TEBD.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TEBD.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence/TEBD/TNclass.py` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TNclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/PKG-INFO` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.4
+Version: 0.0.5
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.4/src/QuantumIntelligence.egg-info/SOURCES.txt` & `QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

