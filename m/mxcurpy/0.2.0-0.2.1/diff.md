# Comparing `tmp/mxcurpy-0.2.0.tar.gz` & `tmp/mxcurpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcurpy-0.2.0.tar", max compression
+gzip compressed data, was "mxcurpy-0.2.1.tar", max compression
```

## Comparing `mxcurpy-0.2.0.tar` & `mxcurpy-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-03-31 05:07:49.031007 mxcurpy-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2484 2023-04-13 04:40:53.781448 mxcurpy-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-04-01 15:47:37.320336 mxcurpy-0.2.0/mxcurpy/__init__.py
--rw-r--r--   0        0        0     3928 2023-04-05 05:46:27.033002 mxcurpy-0.2.0/mxcurpy/curp.py
--rw-r--r--   0        0        0     2464 2023-04-12 05:28:21.336927 mxcurpy-0.2.0/mxcurpy/non_convenient_words.py
--rw-r--r--   0        0        0     5162 2023-04-13 04:08:37.738603 mxcurpy-0.2.0/mxcurpy/rfc.py
--rw-r--r--   0        0        0     1684 2023-04-02 20:23:30.022770 mxcurpy-0.2.0/mxcurpy/states.py
--rw-r--r--   0        0        0     1645 2023-04-13 04:07:38.049352 mxcurpy-0.2.0/mxcurpy/utils.py
--rw-r--r--   0        0        0      472 2023-04-13 04:17:57.018820 mxcurpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3181 2023-04-13 04:41:40.938459 mxcurpy-0.2.0/setup.py
--rw-r--r--   0        0        0     3175 2023-04-13 04:41:40.938655 mxcurpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-31 05:07:49.031007 mxcurpy-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2655 2023-04-28 05:20:18.556733 mxcurpy-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-01 15:47:37.320336 mxcurpy-0.2.1/mxcurpy/__init__.py
+-rw-r--r--   0        0        0     3928 2023-04-05 05:46:27.033002 mxcurpy-0.2.1/mxcurpy/curp.py
+-rw-r--r--   0        0        0     2464 2023-04-12 05:28:21.336927 mxcurpy-0.2.1/mxcurpy/non_convenient_words.py
+-rw-r--r--   0        0        0     5162 2023-04-13 04:08:37.738603 mxcurpy-0.2.1/mxcurpy/rfc.py
+-rw-r--r--   0        0        0     1684 2023-04-02 20:23:30.022770 mxcurpy-0.2.1/mxcurpy/states.py
+-rw-r--r--   0        0        0     1645 2023-04-13 04:07:38.049352 mxcurpy-0.2.1/mxcurpy/utils.py
+-rw-r--r--   0        0        0      472 2023-04-28 05:22:29.990147 mxcurpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3351 2023-04-28 05:23:19.227773 mxcurpy-0.2.1/setup.py
+-rw-r--r--   0        0        0     3346 2023-04-28 05:23:19.227992 mxcurpy-0.2.1/PKG-INFO
```

### Comparing `mxcurpy-0.2.0/LICENSE.txt` & `mxcurpy-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.2.0/README.md` & `mxcurpy-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # MXCurpy
 
 Generación de Clave Única de Registro de Población y el Registro Federal de Contibuyentes de México en Python.
 
 Documentos en los que está basado este paquete:
 
 **CURP**: [INSTRUCTIVO NORMATIVO PARA LA ASIGNACIÓN DE LA CLAVE ÚNICA DE REGISTRO DE
-POBLACIÓN](/docs/dof18102021.pdf)
+POBLACIÓN](https://github.com/hectorip/mxcurpy/blob/master/docs/dof18102021.pdf)
 
-**RFC**: [Instructivo RFC-2006](/docs/RFC-2006.pdf). Este es un instructivo antiguo, del 2006, ya que no he encontrado documentos más recientes públicos, pero estoy investigando si hay algún documento normativo que se pueda conseguir. Digamos que el método oficial para conseguir el RFC es siempre preguntándole al Sistema de Administración Tributaria (SAT), también según los documentos oficiales.
+**RFC**: [Instructivo RFC-2006](https://github.com/hectorip/mxcurpy/blob/master/docs/RFC-2006.pdf). Este es un instructivo antiguo, del 2006, ya que no he encontrado documentos más recientes públicos, pero estoy investigando si hay algún documento normativo que se pueda conseguir. Digamos que el método oficial para conseguir el RFC es siempre preguntándole al Sistema de Administración Tributaria (SAT), también según los documentos oficiales. Si tienes algún documento oficial más reciente, por favor, házmelo saber.
 
 ## Estado actual del proyecto
 
 Se puede generar tanto CURP como RFC, pero no se ha probado mucho, por lo que no se puede garantizar que funcione en todos los casos.
 
 ## Uso
 
@@ -46,15 +46,15 @@
 
 ## Limitaciones
 
 Aquí describimos algunas limitaciones que tenemos y que probablemente no se arreglen en un futuro cercano (ni lejano).
 
 ### CURP
 
-Los dod últimos carácteres al final de la CURP oficial son generados por la entidad de gobierno encargada de asignación de las curps al momento de genrarla, con el objetivo de
+Los dos últimos carácteres al final de la CURP oficial son generados por la entidad de gobierno encargada de asignación de las curps al momento de generarla, con el objetivo de
 evitar duplicados, por lo que no podemos generarlos con seguridad, por eso estos dos carácteres siempre serán `00`.
 
 ## Lista de estados válidos
 
 Estados:
 
 * "AGUASCALIENTES"
@@ -92,8 +92,8 @@
 * "YUCATAN"
 * "ZACATECAS"
 * "NACIDO EN EL EXTRANJERO"
 * "NE"
 
 ## LICENCIA
 
-MIT
+MIT
```

### Comparing `mxcurpy-0.2.0/mxcurpy/curp.py` & `mxcurpy-0.2.1/mxcurpy/curp.py`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.2.0/mxcurpy/non_convenient_words.py` & `mxcurpy-0.2.1/mxcurpy/non_convenient_words.py`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.2.0/mxcurpy/rfc.py` & `mxcurpy-0.2.1/mxcurpy/rfc.py`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.2.0/mxcurpy/states.py` & `mxcurpy-0.2.1/mxcurpy/states.py`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.2.0/mxcurpy/utils.py` & `mxcurpy-0.2.1/mxcurpy/utils.py`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.2.0/setup.py` & `mxcurpy-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['mxcurpy']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mxcurpy',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Compute CURP and RFC for Mexican Citizens',
-    'long_description': '# MXCurpy\n\nGeneración de Clave Única de Registro de Población y el Registro Federal de Contibuyentes de México en Python.\n\nDocumentos en los que está basado este paquete:\n\n**CURP**: [INSTRUCTIVO NORMATIVO PARA LA ASIGNACIÓN DE LA CLAVE ÚNICA DE REGISTRO DE\nPOBLACIÓN](/docs/dof18102021.pdf)\n\n**RFC**: [Instructivo RFC-2006](/docs/RFC-2006.pdf). Este es un instructivo antiguo, del 2006, ya que no he encontrado documentos más recientes públicos, pero estoy investigando si hay algún documento normativo que se pueda conseguir. Digamos que el método oficial para conseguir el RFC es siempre preguntándole al Sistema de Administración Tributaria (SAT), también según los documentos oficiales.\n\n## Estado actual del proyecto\n\nSe puede generar tanto CURP como RFC, pero no se ha probado mucho, por lo que no se puede garantizar que funcione en todos los casos.\n\n## Uso\n\nGeneración de CURP:\n\n```python\nfrom mxcurpy.curp import curp\n\nmy_curp = curp(names="Juan José", lastname="Martínez", second_lastname="Pérez", birth_date="12-08-1989", birth_state="Durango", sex="h")\n\n# MAPJ890812HDGRRN00\n\n```\n\nGeneración de RFC:\n\n```python\nfrom mxcurpy.rfc import rfc\n\nmy_rfc = rfc(\n                "Emma",\n                "Gómez",\n                "Díaz",\n                "31-12-1956"\n            )\n# GODE561231GR8\n```\n\n## Casos excepcionales\n\nSi la persona es nacida en el extranjero, mandar la cadena `"NACIDO EN EL EXTRANJERO"` como estado de nacimiento.\n\n## Limitaciones\n\nAquí describimos algunas limitaciones que tenemos y que probablemente no se arreglen en un futuro cercano (ni lejano).\n\n### CURP\n\nLos dod últimos carácteres al final de la CURP oficial son generados por la entidad de gobierno encargada de asignación de las curps al momento de genrarla, con el objetivo de\nevitar duplicados, por lo que no podemos generarlos con seguridad, por eso estos dos carácteres siempre serán `00`.\n\n## Lista de estados válidos\n\nEstados:\n\n* "AGUASCALIENTES"\n* "BAJA CALIFORNIA"\n* "BAJA CALIFORNIA SUR"\n* "CAMPECHE"\n* "COAHUILA"\n* "COLIMA"\n* "CHIAPAS"\n* "CHIHUAHUA"\n* "DISTRITO FEDERAL"\n* "CDMX"\n* "CIUDAD DE MEXICO"\n* "DURANGO"\n* "GUANAJUATO"\n* "GUERRERO"\n* "HIDALGO"\n* "JALISCO"\n* "MEXICO"\n* "MICHOACAN"\n* "MORELOS"\n* "NAYARIT"\n* "NUEVO LEON"\n* "OAXACA"\n* "PUEBLA"\n* "QUERETARO"\n* "QUINTANA ROO"\n* "SAN LUIS POTOSI"\n* "SINALOA"\n* "SONORA"\n* "TABASCO"\n* "TAMAULIPAS"\n* "TLAXCALA"\n* "VERACRUZ"\n* "YUCATAN"\n* "ZACATECAS"\n* "NACIDO EN EL EXTRANJERO"\n* "NE"\n\n## LICENCIA\n\nMIT\n',
+    'long_description': '# MXCurpy\n\nGeneración de Clave Única de Registro de Población y el Registro Federal de Contibuyentes de México en Python.\n\nDocumentos en los que está basado este paquete:\n\n**CURP**: [INSTRUCTIVO NORMATIVO PARA LA ASIGNACIÓN DE LA CLAVE ÚNICA DE REGISTRO DE\nPOBLACIÓN](https://github.com/hectorip/mxcurpy/blob/master/docs/dof18102021.pdf)\n\n**RFC**: [Instructivo RFC-2006](https://github.com/hectorip/mxcurpy/blob/master/docs/RFC-2006.pdf). Este es un instructivo antiguo, del 2006, ya que no he encontrado documentos más recientes públicos, pero estoy investigando si hay algún documento normativo que se pueda conseguir. Digamos que el método oficial para conseguir el RFC es siempre preguntándole al Sistema de Administración Tributaria (SAT), también según los documentos oficiales. Si tienes algún documento oficial más reciente, por favor, házmelo saber.\n\n## Estado actual del proyecto\n\nSe puede generar tanto CURP como RFC, pero no se ha probado mucho, por lo que no se puede garantizar que funcione en todos los casos.\n\n## Uso\n\nGeneración de CURP:\n\n```python\nfrom mxcurpy.curp import curp\n\nmy_curp = curp(names="Juan José", lastname="Martínez", second_lastname="Pérez", birth_date="12-08-1989", birth_state="Durango", sex="h")\n\n# MAPJ890812HDGRRN00\n\n```\n\nGeneración de RFC:\n\n```python\nfrom mxcurpy.rfc import rfc\n\nmy_rfc = rfc(\n                "Emma",\n                "Gómez",\n                "Díaz",\n                "31-12-1956"\n            )\n# GODE561231GR8\n```\n\n## Casos excepcionales\n\nSi la persona es nacida en el extranjero, mandar la cadena `"NACIDO EN EL EXTRANJERO"` como estado de nacimiento.\n\n## Limitaciones\n\nAquí describimos algunas limitaciones que tenemos y que probablemente no se arreglen en un futuro cercano (ni lejano).\n\n### CURP\n\nLos dos últimos carácteres al final de la CURP oficial son generados por la entidad de gobierno encargada de asignación de las curps al momento de generarla, con el objetivo de\nevitar duplicados, por lo que no podemos generarlos con seguridad, por eso estos dos carácteres siempre serán `00`.\n\n## Lista de estados válidos\n\nEstados:\n\n* "AGUASCALIENTES"\n* "BAJA CALIFORNIA"\n* "BAJA CALIFORNIA SUR"\n* "CAMPECHE"\n* "COAHUILA"\n* "COLIMA"\n* "CHIAPAS"\n* "CHIHUAHUA"\n* "DISTRITO FEDERAL"\n* "CDMX"\n* "CIUDAD DE MEXICO"\n* "DURANGO"\n* "GUANAJUATO"\n* "GUERRERO"\n* "HIDALGO"\n* "JALISCO"\n* "MEXICO"\n* "MICHOACAN"\n* "MORELOS"\n* "NAYARIT"\n* "NUEVO LEON"\n* "OAXACA"\n* "PUEBLA"\n* "QUERETARO"\n* "QUINTANA ROO"\n* "SAN LUIS POTOSI"\n* "SINALOA"\n* "SONORA"\n* "TABASCO"\n* "TAMAULIPAS"\n* "TLAXCALA"\n* "VERACRUZ"\n* "YUCATAN"\n* "ZACATECAS"\n* "NACIDO EN EL EXTRANJERO"\n* "NE"\n\n## LICENCIA\n\nMIT',
     'author': 'Héctor Iván Patricio Moreno',
     'author_email': 'hectorivanpatriciomoreno@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/hectorip/mxcurpy',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mxcurpy-0.2.0/PKG-INFO` & `mxcurpy-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcurpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Compute CURP and RFC for Mexican Citizens
 Home-page: https://github.com/hectorip/mxcurpy
 License: MIT
 Keywords: curp,mexico
 Author: Héctor Iván Patricio Moreno
 Author-email: hectorivanpatriciomoreno@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -20,17 +20,17 @@
 # MXCurpy
 
 Generación de Clave Única de Registro de Población y el Registro Federal de Contibuyentes de México en Python.
 
 Documentos en los que está basado este paquete:
 
 **CURP**: [INSTRUCTIVO NORMATIVO PARA LA ASIGNACIÓN DE LA CLAVE ÚNICA DE REGISTRO DE
-POBLACIÓN](/docs/dof18102021.pdf)
+POBLACIÓN](https://github.com/hectorip/mxcurpy/blob/master/docs/dof18102021.pdf)
 
-**RFC**: [Instructivo RFC-2006](/docs/RFC-2006.pdf). Este es un instructivo antiguo, del 2006, ya que no he encontrado documentos más recientes públicos, pero estoy investigando si hay algún documento normativo que se pueda conseguir. Digamos que el método oficial para conseguir el RFC es siempre preguntándole al Sistema de Administración Tributaria (SAT), también según los documentos oficiales.
+**RFC**: [Instructivo RFC-2006](https://github.com/hectorip/mxcurpy/blob/master/docs/RFC-2006.pdf). Este es un instructivo antiguo, del 2006, ya que no he encontrado documentos más recientes públicos, pero estoy investigando si hay algún documento normativo que se pueda conseguir. Digamos que el método oficial para conseguir el RFC es siempre preguntándole al Sistema de Administración Tributaria (SAT), también según los documentos oficiales. Si tienes algún documento oficial más reciente, por favor, házmelo saber.
 
 ## Estado actual del proyecto
 
 Se puede generar tanto CURP como RFC, pero no se ha probado mucho, por lo que no se puede garantizar que funcione en todos los casos.
 
 ## Uso
 
@@ -65,15 +65,15 @@
 
 ## Limitaciones
 
 Aquí describimos algunas limitaciones que tenemos y que probablemente no se arreglen en un futuro cercano (ni lejano).
 
 ### CURP
 
-Los dod últimos carácteres al final de la CURP oficial son generados por la entidad de gobierno encargada de asignación de las curps al momento de genrarla, con el objetivo de
+Los dos últimos carácteres al final de la CURP oficial son generados por la entidad de gobierno encargada de asignación de las curps al momento de generarla, con el objetivo de
 evitar duplicados, por lo que no podemos generarlos con seguridad, por eso estos dos carácteres siempre serán `00`.
 
 ## Lista de estados válidos
 
 Estados:
 
 * "AGUASCALIENTES"
@@ -112,8 +112,7 @@
 * "ZACATECAS"
 * "NACIDO EN EL EXTRANJERO"
 * "NE"
 
 ## LICENCIA
 
 MIT
-
```

