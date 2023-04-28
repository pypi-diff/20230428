# Comparing `tmp/tupa123-1.4.1.tar.gz` & `tmp/tupa123-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.1.tar", last modified: Thu Apr 27 11:23:22 2023, max compression
+gzip compressed data, was "tupa123-1.4.2.tar", last modified: Fri Apr 28 11:37:02 2023, max compression
```

## Comparing `tupa123-1.4.1.tar` & `tupa123-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:23:22.565594 tupa123-1.4.1/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-04-27 11:23:22.565594 tupa123-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 11:23:22.565594 tupa123-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-27 11:19:28.000000 tupa123-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:23:22.555559 tupa123-1.4.1/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.1/tupa123/__init__.py
--rw-rw-rw-   0        0        0       52 2023-04-27 11:22:32.000000 tupa123-1.4.1/tupa123/teste.py
--rw-rw-rw-   0        0        0    67989 2023-04-27 11:14:58.000000 tupa123-1.4.1/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:23:22.565594 tupa123-1.4.1/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-27 11:23:22.000000 tupa123-1.4.1/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 11:37:02.279296 tupa123-1.4.2/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-04-28 11:37:02.263645 tupa123-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 11:37:02.279296 tupa123-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-28 11:36:00.000000 tupa123-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:37:02.263645 tupa123-1.4.2/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.2/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    68140 2023-04-28 11:33:54.000000 tupa123-1.4.2/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:37:02.263645 tupa123-1.4.2/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-04-28 11:37:02.000000 tupa123-1.4.2/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-28 11:37:02.000000 tupa123-1.4.2/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 11:37:02.000000 tupa123-1.4.2/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-28 11:37:02.000000 tupa123-1.4.2/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 11:37:02.000000 tupa123-1.4.2/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.1/LICENSE.txt` & `tupa123-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.1/PKG-INFO` & `tupa123-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.1
+Version: 1.4.2
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.1/README.md` & `tupa123-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.1/setup.py` & `tupa123-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.1',
+    version='1.4.2',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.1/tupa123/tupa123.py` & `tupa123-1.4.2/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,15 @@
 
         if (self.norma>=3): 
             data = np.log(data + self.coef)
         normalized = data*1
         
         vetormax = np.max(data,0) 
         vetormin = np.min(data,0)
-        if self.shift>1:
+        if self.shift>1: #aplica o esticamento se tiver
             vetormax=np.where(vetormax < 0, vetormax*(1/self.shift), vetormax*self.shift)
             vetormin=np.where(vetormin < 0, vetormin*self.shift, vetormin*(1/self.shift))
 
         vetormed = (vetormax+vetormin)/2
         media = np.mean(data,0)
         desvio = np.std(data,0)        
                                     
@@ -911,20 +911,21 @@
             if (self.normout==1):
                 matY2 = self.Normalize(matY2,nomepasta + "vmax_out2.npy",nomepasta + "vmin_out2.npy",nomepasta + "media_out2.npy",nomepasta + "desvio_out2.npy")            
             #deleta os arquivos criados da validação cruzada que não sao uteis
             os.remove(nomepasta + "vmax_in2.npy")
             os.remove(nomepasta + "vmin_in2.npy")
             os.remove(nomepasta + "media_in2.npy")
             os.remove(nomepasta + "desvio_in2.npy")
-            os.remove(nomepasta + "vmax_out2.npy")
-            os.remove(nomepasta + "vmin_out2.npy")
-            os.remove(nomepasta + "media_out2.npy")
-            os.remove(nomepasta + "desvio_out2.npy")
-                      
-            
+            if (self.normout==1):
+                os.remove(nomepasta + "vmax_out2.npy")
+                os.remove(nomepasta + "vmin_out2.npy")
+                os.remove(nomepasta + "media_out2.npy")
+                os.remove(nomepasta + "desvio_out2.npy")
+ 
+
 
 
         #Processo de aprendizado------------------------------------------------------------
         
         VetorErro = [0]
         MenorErro = 999999999
         
@@ -1215,18 +1216,19 @@
             if (self.normout==1):
                 matY2 = self.Normalize(matY2,nomepasta + "vmax_out2.npy",nomepasta + "vmin_out2.npy",nomepasta + "media_out2.npy",nomepasta + "desvio_out2.npy")            
             #deleta os arquivos criados
             os.remove(nomepasta + "vmax_in2.npy")
             os.remove(nomepasta + "vmin_in2.npy")
             os.remove(nomepasta + "media_in2.npy")
             os.remove(nomepasta + "desvio_in2.npy")
-            os.remove(nomepasta + "vmax_out2.npy")
-            os.remove(nomepasta + "vmin_out2.npy")
-            os.remove(nomepasta + "media_out2.npy")
-            os.remove(nomepasta + "desvio_out2.npy")
+            if (self.normout==1):
+                os.remove(nomepasta + "vmax_out2.npy")
+                os.remove(nomepasta + "vmin_out2.npy")
+                os.remove(nomepasta + "media_out2.npy")
+                os.remove(nomepasta + "desvio_out2.npy")
 
 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
         VetorErro = [0]
@@ -1504,18 +1506,19 @@
             if (self.normout==1):
                 matY2 = self.Normalize(matY2,nomepasta + "vmax_out2.npy",nomepasta + "vmin_out2.npy",nomepasta + "media_out2.npy",nomepasta + "desvio_out2.npy")            
             #deleta os arquivos criados
             os.remove(nomepasta + "vmax_in2.npy")
             os.remove(nomepasta + "vmin_in2.npy")
             os.remove(nomepasta + "media_in2.npy")
             os.remove(nomepasta + "desvio_in2.npy")
-            os.remove(nomepasta + "vmax_out2.npy")
-            os.remove(nomepasta + "vmin_out2.npy")
-            os.remove(nomepasta + "media_out2.npy")
-            os.remove(nomepasta + "desvio_out2.npy")
+            if (self.normout==1):
+                os.remove(nomepasta + "vmax_out2.npy")
+                os.remove(nomepasta + "vmin_out2.npy")
+                os.remove(nomepasta + "media_out2.npy")
+                os.remove(nomepasta + "desvio_out2.npy")
 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
         VetorErro = [0]
         MenorErro = 999999999
```

### Comparing `tupa123-1.4.1/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.2/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.1
+Version: 1.4.2
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

