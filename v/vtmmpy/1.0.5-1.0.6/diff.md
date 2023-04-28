# Comparing `tmp/vtmmpy-1.0.5.tar.gz` & `tmp/vtmmpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtmmpy-1.0.5.tar", last modified: Thu Apr 20 11:07:55 2023, max compression
+gzip compressed data, was "vtmmpy-1.0.6.tar", last modified: Fri Apr 28 10:56:14 2023, max compression
```

## Comparing `vtmmpy-1.0.5.tar` & `vtmmpy-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 11:07:55.618233 vtmmpy-1.0.5/
--rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.5/LICENSE
--rw-rw-r--   0 tony      (1000) tony      (1000)     3693 2023-04-20 11:07:55.618233 vtmmpy-1.0.5/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     3218 2023-04-19 13:22:05.000000 vtmmpy-1.0.5/README.md
--rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.5/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-20 11:07:55.618233 vtmmpy-1.0.5/setup.cfg
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 11:07:55.618233 vtmmpy-1.0.5/src/
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 11:07:55.618233 vtmmpy-1.0.5/src/vtmmpy/
--rw-r--r--   0 tony      (1000) tony      (1000)     8551 2023-04-20 10:33:21.000000 vtmmpy-1.0.5/src/vtmmpy/__init__.py
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-20 11:07:55.618233 vtmmpy-1.0.5/src/vtmmpy.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3693 2023-04-20 11:07:55.000000 vtmmpy-1.0.5/src/vtmmpy.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-20 11:07:55.000000 vtmmpy-1.0.5/src/vtmmpy.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-20 11:07:55.000000 vtmmpy-1.0.5/src/vtmmpy.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-20 11:07:55.000000 vtmmpy-1.0.5/src/vtmmpy.egg-info/top_level.txt
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/
+-rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.6/LICENSE
+-rw-rw-r--   0 tony      (1000) tony      (1000)     4115 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)     3640 2023-04-28 10:46:41.000000 vtmmpy-1.0.6/README.md
+-rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.6/pyproject.toml
+-rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/setup.cfg
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/src/
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/src/vtmmpy/
+-rw-r--r--   0 tony      (1000) tony      (1000)     8697 2023-04-28 10:35:27.000000 vtmmpy-1.0.6/src/vtmmpy/__init__.py
+drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/src/vtmmpy.egg-info/
+-rw-r--r--   0 tony      (1000) tony      (1000)     4115 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/PKG-INFO
+-rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/top_level.txt
```

### Comparing `vtmmpy-1.0.5/LICENSE` & `vtmmpy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.5/PKG-INFO` & `vtmmpy-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtmmpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: A vectorized implementation of the transfer matrix method
 Home-page: https://github.com/AI-Tony/vtmmpy/tree/main
 Author: Tony
 Author-email: tk_87@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -55,16 +55,16 @@
 - l_scale (optional): input length scale, default is nanometers.
 - incident_medium (optional): incident medium, default is air.
 - transmitted_medium (optional): transmitted medium, default is air. 
 
 Add multilayer metamaterial designs with the ```addDesign()``` method. 
 
 ```
-materials = ["Ag", "SiO2", "Ag", "SiO2", "Ag"] 
-thicknesses = [15, 85, 15, 85, 15] 
+materials   = ["Ag", "SiO2", "Ag", "SiO2", "Ag", "SiO2"] 
+thicknesses = [15, 85, 15, 85, 15, 85] 
 
 tmm.addDesign(materials, thicknesses)
 ```
 
 - materials: list of materials 
 - thicknesses: list of the corresponding material thicknesses 
 
@@ -73,14 +73,24 @@
 Optionally call the ```summary()``` and/or ```designs()``` methods to view the data currently held by the instance.
 
 ```
 tmm.summary() 
 tmm.designs() 
 ```
 
+Additionally, the ```tmm.opticalProperties()``` method can be used to obtain a dictionary of optical properties of the materials entered in the frequency range specified.
+
+```
+props = tmm.opticalProperties()
+
+print(props.keys()) # output: dict_keys(['air', 'SiO2', 'Ag'])
+print(props["Ag"]["n"]) # ouput is the refractive index of Ag
+print(props["Ag"]["beta"]) # ouput is the propagation constant of Ag
+```
+
 Calculate the reflection/transmission coefficients by calling the appropriate method. You should specify wether you want the transverse magnetic/electric polarization by supplying the "TM" or "TE" flag, respectively.
 
 ```
 RTM = tmm.reflection("TM") 
 RTE = tmm.reflection("TE") 
 TTM = tmm.transmission("TM") 
 TTE = tmm.transmission("TE")
```

### Comparing `vtmmpy-1.0.5/README.md` & `vtmmpy-1.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 - l_scale (optional): input length scale, default is nanometers.
 - incident_medium (optional): incident medium, default is air.
 - transmitted_medium (optional): transmitted medium, default is air. 
 
 Add multilayer metamaterial designs with the ```addDesign()``` method. 
 
 ```
-materials = ["Ag", "SiO2", "Ag", "SiO2", "Ag"] 
-thicknesses = [15, 85, 15, 85, 15] 
+materials   = ["Ag", "SiO2", "Ag", "SiO2", "Ag", "SiO2"] 
+thicknesses = [15, 85, 15, 85, 15, 85] 
 
 tmm.addDesign(materials, thicknesses)
 ```
 
 - materials: list of materials 
 - thicknesses: list of the corresponding material thicknesses 
 
@@ -59,14 +59,24 @@
 Optionally call the ```summary()``` and/or ```designs()``` methods to view the data currently held by the instance.
 
 ```
 tmm.summary() 
 tmm.designs() 
 ```
 
+Additionally, the ```tmm.opticalProperties()``` method can be used to obtain a dictionary of optical properties of the materials entered in the frequency range specified.
+
+```
+props = tmm.opticalProperties()
+
+print(props.keys()) # output: dict_keys(['air', 'SiO2', 'Ag'])
+print(props["Ag"]["n"]) # ouput is the refractive index of Ag
+print(props["Ag"]["beta"]) # ouput is the propagation constant of Ag
+```
+
 Calculate the reflection/transmission coefficients by calling the appropriate method. You should specify wether you want the transverse magnetic/electric polarization by supplying the "TM" or "TE" flag, respectively.
 
 ```
 RTM = tmm.reflection("TM") 
 RTE = tmm.reflection("TE") 
 TTM = tmm.transmission("TM") 
 TTE = tmm.transmission("TE")
```

### Comparing `vtmmpy-1.0.5/setup.cfg` & `vtmmpy-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vtmmpy
-version = 1.0.5
+version = 1.0.6
 author = Tony
 author_email = tk_87@hotmail.com
 description = A vectorized implementation of the transfer matrix method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AI-Tony/vtmmpy/tree/main
 project_urls =
```

### Comparing `vtmmpy-1.0.5/src/vtmmpy/__init__.py` & `vtmmpy-1.0.6/src/vtmmpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,42 +72,42 @@
             transmitted_medium="air"): 
 
         RefractiveIndex.__init__(self) 
         self.__theta = theta * np.pi/180 
         self.__freq = freq * f_scale 
         self.__f_scale = f_scale
         self.__l_scale = l_scale
-        self.__materialsProperties = {} 
+        self.__opticalProperties = {} 
         self.__incident_medium = incident_medium 
         self.__transmitted_medium = transmitted_medium 
 
     def reflection(self, polarization):
         if polarization == "TE":
             ni = 1 
             nt = 1 
         elif polarization == "TM":
-            ni = self.__materialsProperties[self.__incident_medium][0] 
-            nt = self.__materialsProperties[self.__transmitted_medium][0] 
-        bi = self.__materialsProperties[self.__incident_medium][1] 
-        bt = self.__materialsProperties[self.__transmitted_medium][1] 
+            ni = self.__opticalProperties[self.__incident_medium]["n"] 
+            nt = self.__opticalProperties[self.__transmitted_medium]["n"] 
+        bi = self.__opticalProperties[self.__incident_medium]["beta"] 
+        bt = self.__opticalProperties[self.__transmitted_medium]["beta"] 
         M  = self.__transferMatrix(polarization) 
         M  = self.__inverse(M) 
         r  = -(M[0,0,:,:,:]*bi*nt*nt - M[1,1,:,:,:]*bt*ni*ni + 1j*(M[1,0,:,:,:]*nt*nt*ni*ni + M[0,1,:,:,:]*bi*bt))/\
               (M[0,0,:,:,:]*bi*nt*nt + M[1,1,:,:,:]*bt*ni*ni - 1j*(M[1,0,:,:,:]*nt*nt*ni*ni - M[0,1,:,:,:]*bi*bt)) 
         return r
 
     def transmission(self, polarization):
         if polarization == "TE":
             ni = 1 
             nt = 1 
         elif polarization == "TM":
-            ni = self.__materialsProperties[self.__incident_medium][0] 
-            nt = self.__materialsProperties[self.__transmitted_medium][0] 
-        bi = self.__materialsProperties[self.__incident_medium][1] 
-        bt = self.__materialsProperties[self.__transmitted_medium][1] 
+            ni = self.__opticalProperties[self.__incident_medium]["n"] 
+            nt = self.__opticalProperties[self.__transmitted_medium]["n"] 
+        bi = self.__opticalProperties[self.__incident_medium]["beta"] 
+        bt = self.__opticalProperties[self.__transmitted_medium]["beta"] 
         M  = self.__transferMatrix(polarization) 
         M  = self.__inverse(M) 
         t  = -2*ni*nt*bi / (M[0,0,:,:,:]*bi*nt*nt + M[1,1,:,:,:]*bt*ni*ni - 1j*(M[1,0,:,:,:]*nt*nt*ni*ni - M[0,1,:,:,:]*bi*bt)) 
         return t
 
     def addDesign(self, materials, thicknesses): 
         materials = np.array(materials) 
@@ -130,18 +130,19 @@
         self.w = 2*np.pi*self.__freq[:,None] * np.ones(self.__dims[1:]) 
         k0 = self.w / 3e8 
         kx = k0 * np.sin( self.__theta ) 
         material_set = set( self.__materials.flatten() )
         material_set.add( self.__incident_medium )
         material_set.add( self.__transmitted_medium ) 
         for mat in material_set:
-            if mat not in self.__materialsProperties.keys(): 
+            if mat not in self.__opticalProperties.keys(): 
                 n = self.index(mat) 
                 beta = np.sqrt( k0**2 * n**2 - kx**2 ) 
-                self.__materialsProperties["{}".format(mat)] = (n, beta) 
+                tmp_dict = { "n": n, "beta": beta} 
+                self.__opticalProperties["{}".format(mat)] = tmp_dict 
 
     def __transferMatrix(self, polarization):
         M            = np.zeros((2, 2, *self.__dims), dtype='cfloat') 
         M[0,0,:,:,:] = np.ones(self.__dims, dtype='cfloat') 
         M[1,1,:,:,:] = np.ones(self.__dims, dtype='cfloat') 
         for i in np.arange(self.__layers-1, -1, -1):
             m = self.__subMatrix( self.__materials[:,i], self.__thicknesses[:,i], polarization ) 
@@ -152,16 +153,16 @@
         d = thicknesses[:,None,None] * np.ones(self.__dims) 
         n    = np.empty(self.__dims, dtype="cfloat") 
         beta = np.empty(self.__dims, dtype="cfloat") 
         for i, mat in enumerate(materials): 
             if polarization == "TE":
                 n = 1
             elif polarization == "TM":
-                n[i,:,:] = self.__materialsProperties[ mat ][0] 
-            beta[i,:,:] = self.__materialsProperties[ mat ][1] 
+                n[i,:,:] = self.__opticalProperties[ mat ]["n"] 
+            beta[i,:,:] = self.__opticalProperties[ mat ]["beta"] 
         A =  np.cos( beta * d ) 
         B =  np.sin( beta * d ) * n * n / beta 
         C = -np.sin( beta * d ) * beta / (n * n) 
         D =  np.cos( beta * d )  
         return np.array( [ [A, B], [C, D] ], dtype='cfloat' ) 
 
     def __matmul(self, M, m):
@@ -192,7 +193,10 @@
     def designs(self):
         try:
             zipped = zip(self.__materials,self.__thicknesses) 
             for pair in zipped:
                 print(pair) 
         except:
             raise Exception("No designs found. Add designs with the addDesign() method.") 
+            
+    def opticalProperties(self):
+        return self.__opticalProperties
```

### Comparing `vtmmpy-1.0.5/src/vtmmpy.egg-info/PKG-INFO` & `vtmmpy-1.0.6/src/vtmmpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtmmpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: A vectorized implementation of the transfer matrix method
 Home-page: https://github.com/AI-Tony/vtmmpy/tree/main
 Author: Tony
 Author-email: tk_87@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -55,16 +55,16 @@
 - l_scale (optional): input length scale, default is nanometers.
 - incident_medium (optional): incident medium, default is air.
 - transmitted_medium (optional): transmitted medium, default is air. 
 
 Add multilayer metamaterial designs with the ```addDesign()``` method. 
 
 ```
-materials = ["Ag", "SiO2", "Ag", "SiO2", "Ag"] 
-thicknesses = [15, 85, 15, 85, 15] 
+materials   = ["Ag", "SiO2", "Ag", "SiO2", "Ag", "SiO2"] 
+thicknesses = [15, 85, 15, 85, 15, 85] 
 
 tmm.addDesign(materials, thicknesses)
 ```
 
 - materials: list of materials 
 - thicknesses: list of the corresponding material thicknesses 
 
@@ -73,14 +73,24 @@
 Optionally call the ```summary()``` and/or ```designs()``` methods to view the data currently held by the instance.
 
 ```
 tmm.summary() 
 tmm.designs() 
 ```
 
+Additionally, the ```tmm.opticalProperties()``` method can be used to obtain a dictionary of optical properties of the materials entered in the frequency range specified.
+
+```
+props = tmm.opticalProperties()
+
+print(props.keys()) # output: dict_keys(['air', 'SiO2', 'Ag'])
+print(props["Ag"]["n"]) # ouput is the refractive index of Ag
+print(props["Ag"]["beta"]) # ouput is the propagation constant of Ag
+```
+
 Calculate the reflection/transmission coefficients by calling the appropriate method. You should specify wether you want the transverse magnetic/electric polarization by supplying the "TM" or "TE" flag, respectively.
 
 ```
 RTM = tmm.reflection("TM") 
 RTE = tmm.reflection("TE") 
 TTM = tmm.transmission("TM") 
 TTE = tmm.transmission("TE")
```

