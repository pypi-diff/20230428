# Comparing `tmp/tupa123-1.4.3.tar.gz` & `tmp/tupa123-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.3.tar", last modified: Fri Apr 28 13:12:28 2023, max compression
+gzip compressed data, was "tupa123-1.4.4.tar", last modified: Fri Apr 28 13:57:47 2023, max compression
```

## Comparing `tupa123-1.4.3.tar` & `tupa123-1.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:12:28.723513 tupa123-1.4.3/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-04-28 13:12:28.722521 tupa123-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 13:12:28.723513 tupa123-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-28 13:11:49.000000 tupa123-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:12:28.711545 tupa123-1.4.3/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.3/tupa123/__init__.py
--rw-rw-rw-   0        0        0    69895 2023-04-28 13:08:09.000000 tupa123-1.4.3/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:12:28.720526 tupa123-1.4.3/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-04-28 13:12:28.000000 tupa123-1.4.3/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-28 13:12:28.000000 tupa123-1.4.3/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:12:28.000000 tupa123-1.4.3/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-28 13:12:28.000000 tupa123-1.4.3/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-28 13:12:28.000000 tupa123-1.4.3/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 13:57:47.453017 tupa123-1.4.4/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-04-28 13:57:47.453017 tupa123-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 13:57:47.453017 tupa123-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-28 13:57:02.000000 tupa123-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:57:47.443014 tupa123-1.4.4/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.4/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    72511 2023-04-28 13:53:17.000000 tupa123-1.4.4/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:57:47.453017 tupa123-1.4.4/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.3/LICENSE.txt` & `tupa123-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.3/PKG-INFO` & `tupa123-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.3
+Version: 1.4.4
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.3/README.md` & `tupa123-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.3/setup.py` & `tupa123-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.3',
+    version='1.4.4',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.3/tupa123/tupa123.py` & `tupa123-1.4.4/tupa123/tupa123.py`

 * *Files 3% similar despite different names*

```diff
@@ -891,15 +891,27 @@
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
 
             net02 = np.load(nomepasta + "net.npy")            
             net01 = self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9
             if (net01 != net02):
                 input('Neural network saves this different from configured network')
                 exit()
-                        
+
+            net03 = np.load(nomepasta + "netati.npy")            
+            net04 = self.fa2c + self.fa3c*1e3 + self.fa4c*1e6
+            if (net03 != net04):
+                input('Activation functions saves this different from configured network')
+                exit()
+
+            net05 = np.load(nomepasta + "norm.npy")            
+            net06 = self.norma + self.normout*1e3
+            if (net05 != net06):
+                input('Normalization saves this different from configured network')
+                exit()
+
             P12 = np.load(nomepasta + "P12.npy")
             P23 = np.load(nomepasta + "P23.npy")            
             P34 = np.load(nomepasta + "P34.npy")             
             B2 = np.load(nomepasta + "B2.npy")
             B3 = np.load(nomepasta + "B3.npy")
             B4 = np.load(nomepasta + "B4.npy")  
 
@@ -1117,14 +1129,17 @@
             B2 = B2m*1
             B3 = B3m*1
             B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
         np.save(nomepasta + "net.npy", self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9)
+        np.save(nomepasta + "netati.npy", self.fa2c + self.fa3c*1e3 + self.fa4c*1e6)
+        np.save(nomepasta + "norm.npy", self.norma + self.normout*1e3)
+        
         np.save(nomepasta + "P12.npy", P12)
         np.save(nomepasta + "P23.npy", P23)
         np.save(nomepasta + "P34.npy", P34)
         np.save(nomepasta + "B2.npy", B2)
         np.save(nomepasta + "B3.npy", B3)
         np.save(nomepasta + "B4.npy", B4)
 
@@ -1204,14 +1219,26 @@
 
             net02 = np.load(nomepasta + "net.npy")            
             net01 = self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9
             if (net01 != net02):
                 input('Neural network saves this different from configured network')
                 exit()
 
+            net03 = np.load(nomepasta + "netati.npy")            
+            net04 = self.fa2c + self.fa3c*1e3 + self.fa4c*1e6
+            if (net03 != net04):
+                input('Activation functions saves this different from configured network')
+                exit()
+
+            net05 = np.load(nomepasta + "norm.npy")            
+            net06 = self.norma + self.normout*1e3
+            if (net05 != net06):
+                input('Normalization saves this different from configured network')
+                exit()
+
             P12 = np.load(nomepasta + "P12.npy")
             P23 = np.load(nomepasta + "P23.npy")            
             P34 = np.load(nomepasta + "P34.npy")             
             B2 = np.load(nomepasta + "B2.npy")
             B3 = np.load(nomepasta + "B3.npy")
             B4 = np.load(nomepasta + "B4.npy")  
 
@@ -1383,14 +1410,17 @@
             B2 = B2m*1
             B3 = B3m*1
             B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
         np.save(nomepasta + "net.npy", self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9)
+        np.save(nomepasta + "netati.npy", self.fa2c + self.fa3c*1e3 + self.fa4c*1e6)
+        np.save(nomepasta + "norm.npy", self.norma + self.normout*1e3)
+        
         np.save(nomepasta + "P12.npy", P12)
         np.save(nomepasta + "P23.npy", P23)
         np.save(nomepasta + "P34.npy", P34)
         np.save(nomepasta + "B2.npy", B2)
         np.save(nomepasta + "B3.npy", B3)
         np.save(nomepasta + "B4.npy", B4)
 
@@ -1500,15 +1530,27 @@
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
 
             net02 = np.load(nomepasta + "net.npy")            
             net01 = self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9
             if (net01 != net02):
                 input('Neural network saves this different from configured network')
                 exit()
-                
+
+            net03 = np.load(nomepasta + "netati.npy")            
+            net04 = self.fa2c + self.fa3c*1e3 + self.fa4c*1e6
+            if (net03 != net04):
+                input('Activation functions saves this different from configured network')
+                exit()
+
+            net05 = np.load(nomepasta + "norm.npy")            
+            net06 = self.norma + self.normout*1e3
+            if (net05 != net06):
+                input('Normalization saves this different from configured network')
+                exit()
+
             P12 = np.load(nomepasta + "P12.npy")
             P23 = np.load(nomepasta + "P23.npy")            
             P34 = np.load(nomepasta + "P34.npy")             
             B2 = np.load(nomepasta + "B2.npy")
             B3 = np.load(nomepasta + "B3.npy")
             B4 = np.load(nomepasta + "B4.npy")  
 
@@ -1710,14 +1752,17 @@
             B2 = B2m*1
             B3 = B3m*1
             B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
         np.save(nomepasta + "net.npy", self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9)
+        np.save(nomepasta + "netati.npy", self.fa2c + self.fa3c*1e3 + self.fa4c*1e6)
+        np.save(nomepasta + "norm.npy", self.norma + self.normout*1e3)
+
         np.save(nomepasta + "P12.npy", P12)
         np.save(nomepasta + "P23.npy", P23)
         np.save(nomepasta + "P34.npy", P34)
         np.save(nomepasta + "B2.npy", B2)
         np.save(nomepasta + "B3.npy", B3)
         np.save(nomepasta + "B4.npy", B4)
 
@@ -1773,15 +1818,27 @@
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
 
             net02 = np.load(nomepasta + "net.npy")            
             net01 = self.nn1c + self.nn2c*1e3 + self.nn3c*1e6 + self.nn4c*1e9
             if (net01 != net02):
                 input('Neural network saves this different from configured network')
                 exit()
-            
+
+            net03 = np.load(nomepasta + "netati.npy")            
+            net04 = self.fa2c + self.fa3c*1e3 + self.fa4c*1e6
+            if (net03 != net04):
+                input('Activation functions saves this different from configured network')
+                exit()
+
+            net05 = np.load(nomepasta + "norm.npy")            
+            net06 = self.norma + self.normout*1e3
+            if (net05 != net06):
+                input('Normalization saves this different from configured network')
+                exit()
+
             P12 = np.load(nomepasta + "P12.npy")
             P23 = np.load(nomepasta + "P23.npy")            
             P34 = np.load(nomepasta + "P34.npy")             
             B2 = np.load(nomepasta + "B2.npy")
             B3 = np.load(nomepasta + "B3.npy")
             B4 = np.load(nomepasta + "B4.npy")
```

### Comparing `tupa123-1.4.3/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.4/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.3
+Version: 1.4.4
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

