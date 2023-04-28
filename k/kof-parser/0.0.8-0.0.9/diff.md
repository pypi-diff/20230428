# Comparing `tmp/kof-parser-0.0.8.tar.gz` & `tmp/kof-parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kof-parser-0.0.8.tar", max compression
+gzip compressed data, was "kof-parser-0.0.9.tar", max compression
```

## Comparing `kof-parser-0.0.8.tar` & `kof-parser-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4205 2022-08-27 19:03:55.487119 kof-parser-0.0.8/README.md
--rw-r--r--   0        0        0     1142 2022-08-27 19:03:55.487119 kof-parser-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5675 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/KoordSys.csv
--rw-r--r--   0        0        0      124 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/__init__.py
--rw-r--r--   0        0        0      387 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/enums.py
--rw-r--r--   0        0        0     1063 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/kof.py
--rw-r--r--   0        0        0      340 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/model.py
--rw-r--r--   0        0        0    10468 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/parser.py
--rw-r--r--   0        0        0     4192 2022-08-27 19:03:55.487119 kof-parser-0.0.8/src/kof_parser/writer.py
--rw-r--r--   0        0        0     5027 2022-08-27 19:04:06.613051 kof-parser-0.0.8/setup.py
--rw-r--r--   0        0        0     5009 2022-08-27 19:04:06.613684 kof-parser-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-10-04 16:08:47.701157 kof-parser-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4198 2022-10-04 16:08:47.701157 kof-parser-0.0.9/README.md
+-rw-r--r--   0        0        0     1198 2022-10-04 16:08:47.705157 kof-parser-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5675 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/KoordSys.csv
+-rw-r--r--   0        0        0      124 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/__init__.py
+-rw-r--r--   0        0        0      387 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/enums.py
+-rw-r--r--   0        0        0     1063 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/kof.py
+-rw-r--r--   0        0        0      340 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/model.py
+-rw-r--r--   0        0        0    10512 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/parser.py
+-rw-r--r--   0        0        0     4192 2022-10-04 16:08:47.705157 kof-parser-0.0.9/src/kof_parser/writer.py
+-rw-r--r--   0        0        0     5069 2022-10-04 16:08:58.520410 kof-parser-0.0.9/setup.py
+-rw-r--r--   0        0        0     5059 2022-10-04 16:08:58.520957 kof-parser-0.0.9/PKG-INFO
```

### Comparing `kof-parser-0.0.8/README.md` & `kof-parser-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# NGI KOF Parser
+# KOF Parser
 
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![security: safety](https://img.shields.io/badge/security-safety-yellow.svg)](https://github.com/pyupio/safety)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 
 
-
-Python package for parsing KOF files.
+Python package for parsing and generating KOF files.
 
 References:
 
 NORWEGIAN GEOTECHNICAL SOCIETY
 - [NGF - VEILEDNING FOR
 SYMBOLER OG DEFINISJONER I GEOTEKNIKK](http://ngf.no/wp-content/uploads/2015/03/2_NGF-ny-melding-2-endelig-utgave-2011-12-04-med-topp-og-bunntekst-Alt-3.pdf)
 - [Norkart KOF specification](http://www.anleggsdata.no/wp-content/uploads/2018/04/KOF-BESKRIVELSE-Oppdatert2005.pdf)
 
 Latest releases see [CHANGES.md](https://github.com/norwegian-geotechnical-institute/kof-parser/blob/main/CHANGES.md)
 
 # Installation (end user) 
 
 ```bash
-
 pip install kof-parser
-
 ```
 
 ## Basic usage
 
 ### Read a kof file
 
 ```python
@@ -53,14 +50,16 @@
 # name='SMPLOC6' methods=['PZ'] point_easting=112901.11 point_northing=1217069.56 point_z=0.0 srid=5110
 # name='SMPLOC7' methods=['PZ'] point_easting=1217069.56 point_northing=112901.11 point_z=0.0 srid=5110
 
 ```
 
 ### Write a kof file
 
+To write a KOF file you need to build up a model of locations and methods.
+
 ```python
 from kof_parser import KOFWriter
 from kof_parser import Location
 
 kof_writer = KOFWriter()
 
 srid = 5110
@@ -83,20 +82,14 @@
 # 05 SMPLOC1             1217083.640  112892.810  1.000                
 # 05 SMPLOC2    2418     1217079.460  112893.150  2.000                
 # 05 SMPLOC3    2407     1217073.010  112891.880  0.000                
 ```
 
 # Getting Started developing
 
-1. Software dependencies
-
-2. Clone this repository
-
-3. Install
-
 ## Software dependencies
 
 Before you start, install:
 
    - Python 3.9 or higher
    - Poetry
    - black code formatter
@@ -116,15 +109,14 @@
     poetry install
 
 
 # Build and Test
 
 Run in the project root folder: 
 
-    poetry install
     poetry run pytest 
 
 Build the package wheel: 
 
     poetry build
 
 # Contribute
```

### Comparing `kof-parser-0.0.8/pyproject.toml` & `kof-parser-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,35 +11,35 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "kof-parser"
-version = "0.0.8"
+version = "0.0.9"
 description = "A KOF file parser. Follows Norkart's KOF 2.0 specification from 2005."
 license = "MIT"
-authors = ["Jostein Leira <jostein@leira.net>", "Magnus Mariero <magnus@neate.no>"]
+authors = ["Magnus Mariero <magnus@neate.no>", "Jostein Leira <jostein@leira.net>"]
 maintainers = ["Jostein Leira <jostein@leira.net>", "Magnus Mariero <magnus@neate.no>"]
 readme = "README.md"
-homepage = "https://ngi.no"
+homepage = "https://github.com/norwegian-geotechnical-institute/kof-parser"
 repository = "https://github.com/norwegian-geotechnical-institute/kof-parser"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 packages = [
     { include = "kof_parser", from="src" },
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pydantic = "^1.9.0"
+python = ">=3.9,<3.11"
+pydantic = "^1.10.2"
 coordinate-projector = "^0.0.4"
 cchardet = "^2.1.7"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `kof-parser-0.0.8/src/kof_parser/KoordSys.csv` & `kof-parser-0.0.9/src/kof_parser/KoordSys.csv`

 * *Files identical despite different names*

### Comparing `kof-parser-0.0.8/src/kof_parser/kof.py` & `kof-parser-0.0.9/src/kof_parser/kof.py`

 * *Files identical despite different names*

### Comparing `kof-parser-0.0.8/src/kof_parser/parser.py` & `kof-parser-0.0.9/src/kof_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         template_coordinate_block: str = "-05 PPPPPPPPPP KKKKKKKK XXXXXXXX.XXX YYYYYYY.YYY ZZZZ.ZZZ Bk MMMMMMM"
         parsed_line = line[0 : len(template_coordinate_block)]
 
         resolved_location.name = parsed_line[4:15].strip()
         resolved_location.srid = result_srid
         resolved_location.point_easting = float(parsed_line[24:37].strip())
         resolved_location.point_northing = float(parsed_line[37:49].strip())
-        resolved_location.point_z = float(parsed_line[49:58].strip())
+        resolved_location.point_z = float(parsed_line[49:58].strip()) if parsed_line[49:58].strip() else None
         new_method = self.tema_code_to_method(parsed_line[15:24].strip())
         if resolved_location.methods is not None:
             resolved_location.methods += [new_method] if new_method is not None else []
 
         return resolved_location
 
     def map_line_to_administrative_block(self, line: str, result_srid: int, file_srid: Optional[int]) -> None:
@@ -142,16 +142,16 @@
         finally:
             if close_file:
                 f.close()
 
     def _read_kof(
         self, file: BytesIO, result_srid: int, file_srid: Optional[int], swap_easting_northing: Optional[bool] = False
     ) -> List[Location]:
-        locations: Dict[str, Location] = {}
-        resolved_locations: List[Location] = []
+        locations: dict[str, Location] = dict()
+        resolved_locations: list[Location] = []
         if file_srid:
             self.file_srid = file_srid
         else:
             self.file_srid = result_srid
 
         self.encoding = self.detect_char_set_from_file(file)
         wrapper = TextIOWrapper(file, encoding=self.encoding)
```

### Comparing `kof-parser-0.0.8/src/kof_parser/writer.py` & `kof-parser-0.0.9/src/kof_parser/writer.py`

 * *Files identical despite different names*

### Comparing `kof-parser-0.0.8/setup.py` & `kof-parser-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cchardet>=2.1.7,<3.0.0',
  'coordinate-projector>=0.0.4,<0.0.5',
- 'pydantic>=1.9.0,<2.0.0']
+ 'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'kof-parser',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': "A KOF file parser. Follows Norkart's KOF 2.0 specification from 2005.",
-    'long_description': "# NGI KOF Parser\n\n[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)\n[![security: safety](https://img.shields.io/badge/security-safety-yellow.svg)](https://github.com/pyupio/safety)\n[![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)\n\n\n\nPython package for parsing KOF files.\n\nReferences:\n\nNORWEGIAN GEOTECHNICAL SOCIETY\n- [NGF - VEILEDNING FOR\nSYMBOLER OG DEFINISJONER I GEOTEKNIKK](http://ngf.no/wp-content/uploads/2015/03/2_NGF-ny-melding-2-endelig-utgave-2011-12-04-med-topp-og-bunntekst-Alt-3.pdf)\n- [Norkart KOF specification](http://www.anleggsdata.no/wp-content/uploads/2018/04/KOF-BESKRIVELSE-Oppdatert2005.pdf)\n\nLatest releases see [CHANGES.md](https://github.com/norwegian-geotechnical-institute/kof-parser/blob/main/CHANGES.md)\n\n# Installation (end user) \n\n```bash\n\npip install kof-parser\n\n```\n\n## Basic usage\n\n### Read a kof file\n\n```python\nfrom kof_parser import KOFParser\n\nparser = KOFParser()\n\n# ETRS89/NTM10:\nsrid = 5110\n\nlocations = parser.parse('tests/data/test.kof', result_srid=srid, file_srid=srid)\n\nfor location in locations:\n    print(location)\n\n# Output:\n# name='SMPLOC1' methods=[] point_easting=112892.81 point_northing=1217083.64 point_z=1.0 srid=5110\n# name='SMPLOC2' methods=['TOT'] point_easting=112893.15 point_northing=1217079.46 point_z=2.0 srid=5110\n# name='SMPLOC3' methods=['CPT'] point_easting=112891.88 point_northing=1217073.01 point_z=0.0 srid=5110\n# name='SMPLOC4' methods=['RP'] point_easting=112891.9 point_northing=1217067.54 point_z=0.0 srid=5110\n# name='SMPLOC5' methods=['SA'] point_easting=112902.92 point_northing=1217074.73 point_z=0.0 srid=5110\n# name='SMPLOC6' methods=['PZ'] point_easting=112901.11 point_northing=1217069.56 point_z=0.0 srid=5110\n# name='SMPLOC7' methods=['PZ'] point_easting=1217069.56 point_northing=112901.11 point_z=0.0 srid=5110\n\n```\n\n### Write a kof file\n\n```python\nfrom kof_parser import KOFWriter\nfrom kof_parser import Location\n\nkof_writer = KOFWriter()\n\nsrid = 5110\nlocations = [Location(name='SMPLOC1', point_easting=112892.81, point_northing=1217083.64, point_z=1.0),\n             Location(name='SMPLOC2', point_easting=112893.15, point_northing=1217079.46, point_z=2.0, methods=['TOT']),\n             Location(name='SMPLOC3', point_easting=112891.88, point_northing=1217073.01, point_z=0.0, methods=['CPT'])]\n\nkof_string = kof_writer.writeKOF(\n    project_id='project_id', project_name='cool-name', locations=locations, srid=srid\n)\n\nprint(kof_string)\n# Output:\n# 00 KOF Export from NGI's KOF parser\n# 00 Project: project_id. Name: cool-name\n# 00 Spatial Reference ID (SRID): 5110\n# 00 Export date (UTC): 2022-08-22 13:49:44.394607\n# 00 Oppdrag      Dato     Ver K.sys   Komm $21100000000 Observer    \n# 01 cool-name    22082022   1     210      $11100000000             \n# 05 SMPLOC1             1217083.640  112892.810  1.000                \n# 05 SMPLOC2    2418     1217079.460  112893.150  2.000                \n# 05 SMPLOC3    2407     1217073.010  112891.880  0.000                \n```\n\n# Getting Started developing\n\n1. Software dependencies\n\n2. Clone this repository\n\n3. Install\n\n## Software dependencies\n\nBefore you start, install:\n\n   - Python 3.9 or higher\n   - Poetry\n   - black code formatter\n   \n## Clone this repository\n\nUse git to clone this repository.\n\n## Install\n\nThere are several combinations of how to set up a local development environment.\n\nWe use Poetry for dependency management. See [Install poetry](https://python-poetry.org/docs/) if needed.\n\nThen, from the project root folder run:\n\n    poetry install\n\n\n# Build and Test\n\nRun in the project root folder: \n\n    poetry install\n    poetry run pytest \n\nBuild the package wheel: \n\n    poetry build\n\n# Contribute\n\nPlease start by adding an issue before submitting any pull requests.",
-    'author': 'Jostein Leira',
-    'author_email': 'jostein@leira.net',
+    'long_description': "# KOF Parser\n\n[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)\n[![security: safety](https://img.shields.io/badge/security-safety-yellow.svg)](https://github.com/pyupio/safety)\n[![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)\n\n\nPython package for parsing and generating KOF files.\n\nReferences:\n\nNORWEGIAN GEOTECHNICAL SOCIETY\n- [NGF - VEILEDNING FOR\nSYMBOLER OG DEFINISJONER I GEOTEKNIKK](http://ngf.no/wp-content/uploads/2015/03/2_NGF-ny-melding-2-endelig-utgave-2011-12-04-med-topp-og-bunntekst-Alt-3.pdf)\n- [Norkart KOF specification](http://www.anleggsdata.no/wp-content/uploads/2018/04/KOF-BESKRIVELSE-Oppdatert2005.pdf)\n\nLatest releases see [CHANGES.md](https://github.com/norwegian-geotechnical-institute/kof-parser/blob/main/CHANGES.md)\n\n# Installation (end user) \n\n```bash\npip install kof-parser\n```\n\n## Basic usage\n\n### Read a kof file\n\n```python\nfrom kof_parser import KOFParser\n\nparser = KOFParser()\n\n# ETRS89/NTM10:\nsrid = 5110\n\nlocations = parser.parse('tests/data/test.kof', result_srid=srid, file_srid=srid)\n\nfor location in locations:\n    print(location)\n\n# Output:\n# name='SMPLOC1' methods=[] point_easting=112892.81 point_northing=1217083.64 point_z=1.0 srid=5110\n# name='SMPLOC2' methods=['TOT'] point_easting=112893.15 point_northing=1217079.46 point_z=2.0 srid=5110\n# name='SMPLOC3' methods=['CPT'] point_easting=112891.88 point_northing=1217073.01 point_z=0.0 srid=5110\n# name='SMPLOC4' methods=['RP'] point_easting=112891.9 point_northing=1217067.54 point_z=0.0 srid=5110\n# name='SMPLOC5' methods=['SA'] point_easting=112902.92 point_northing=1217074.73 point_z=0.0 srid=5110\n# name='SMPLOC6' methods=['PZ'] point_easting=112901.11 point_northing=1217069.56 point_z=0.0 srid=5110\n# name='SMPLOC7' methods=['PZ'] point_easting=1217069.56 point_northing=112901.11 point_z=0.0 srid=5110\n\n```\n\n### Write a kof file\n\nTo write a KOF file you need to build up a model of locations and methods.\n\n```python\nfrom kof_parser import KOFWriter\nfrom kof_parser import Location\n\nkof_writer = KOFWriter()\n\nsrid = 5110\nlocations = [Location(name='SMPLOC1', point_easting=112892.81, point_northing=1217083.64, point_z=1.0),\n             Location(name='SMPLOC2', point_easting=112893.15, point_northing=1217079.46, point_z=2.0, methods=['TOT']),\n             Location(name='SMPLOC3', point_easting=112891.88, point_northing=1217073.01, point_z=0.0, methods=['CPT'])]\n\nkof_string = kof_writer.writeKOF(\n    project_id='project_id', project_name='cool-name', locations=locations, srid=srid\n)\n\nprint(kof_string)\n# Output:\n# 00 KOF Export from NGI's KOF parser\n# 00 Project: project_id. Name: cool-name\n# 00 Spatial Reference ID (SRID): 5110\n# 00 Export date (UTC): 2022-08-22 13:49:44.394607\n# 00 Oppdrag      Dato     Ver K.sys   Komm $21100000000 Observer    \n# 01 cool-name    22082022   1     210      $11100000000             \n# 05 SMPLOC1             1217083.640  112892.810  1.000                \n# 05 SMPLOC2    2418     1217079.460  112893.150  2.000                \n# 05 SMPLOC3    2407     1217073.010  112891.880  0.000                \n```\n\n# Getting Started developing\n\n## Software dependencies\n\nBefore you start, install:\n\n   - Python 3.9 or higher\n   - Poetry\n   - black code formatter\n   \n## Clone this repository\n\nUse git to clone this repository.\n\n## Install\n\nThere are several combinations of how to set up a local development environment.\n\nWe use Poetry for dependency management. See [Install poetry](https://python-poetry.org/docs/) if needed.\n\nThen, from the project root folder run:\n\n    poetry install\n\n\n# Build and Test\n\nRun in the project root folder: \n\n    poetry run pytest \n\nBuild the package wheel: \n\n    poetry build\n\n# Contribute\n\nPlease start by adding an issue before submitting any pull requests.",
+    'author': 'Magnus Mariero',
+    'author_email': 'magnus@neate.no',
     'maintainer': 'Jostein Leira',
     'maintainer_email': 'jostein@leira.net',
-    'url': 'https://ngi.no',
+    'url': 'https://github.com/norwegian-geotechnical-institute/kof-parser',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.9,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `kof-parser-0.0.8/PKG-INFO` & `kof-parser-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 Metadata-Version: 2.1
 Name: kof-parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: A KOF file parser. Follows Norkart's KOF 2.0 specification from 2005.
-Home-page: https://ngi.no
+Home-page: https://github.com/norwegian-geotechnical-institute/kof-parser
 License: MIT
-Author: Jostein Leira
-Author-email: jostein@leira.net
+Author: Magnus Mariero
+Author-email: magnus@neate.no
 Maintainer: Jostein Leira
 Maintainer-email: jostein@leira.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: cchardet (>=2.1.7,<3.0.0)
 Requires-Dist: coordinate-projector (>=0.0.4,<0.0.5)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Project-URL: Repository, https://github.com/norwegian-geotechnical-institute/kof-parser
 Description-Content-Type: text/markdown
 
-# NGI KOF Parser
+# KOF Parser
 
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![security: safety](https://img.shields.io/badge/security-safety-yellow.svg)](https://github.com/pyupio/safety)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 
 
-
-Python package for parsing KOF files.
+Python package for parsing and generating KOF files.
 
 References:
 
 NORWEGIAN GEOTECHNICAL SOCIETY
 - [NGF - VEILEDNING FOR
 SYMBOLER OG DEFINISJONER I GEOTEKNIKK](http://ngf.no/wp-content/uploads/2015/03/2_NGF-ny-melding-2-endelig-utgave-2011-12-04-med-topp-og-bunntekst-Alt-3.pdf)
 - [Norkart KOF specification](http://www.anleggsdata.no/wp-content/uploads/2018/04/KOF-BESKRIVELSE-Oppdatert2005.pdf)
 
 Latest releases see [CHANGES.md](https://github.com/norwegian-geotechnical-institute/kof-parser/blob/main/CHANGES.md)
 
 # Installation (end user) 
 
 ```bash
-
 pip install kof-parser
-
 ```
 
 ## Basic usage
 
 ### Read a kof file
 
 ```python
@@ -77,14 +74,16 @@
 # name='SMPLOC6' methods=['PZ'] point_easting=112901.11 point_northing=1217069.56 point_z=0.0 srid=5110
 # name='SMPLOC7' methods=['PZ'] point_easting=1217069.56 point_northing=112901.11 point_z=0.0 srid=5110
 
 ```
 
 ### Write a kof file
 
+To write a KOF file you need to build up a model of locations and methods.
+
 ```python
 from kof_parser import KOFWriter
 from kof_parser import Location
 
 kof_writer = KOFWriter()
 
 srid = 5110
@@ -107,20 +106,14 @@
 # 05 SMPLOC1             1217083.640  112892.810  1.000                
 # 05 SMPLOC2    2418     1217079.460  112893.150  2.000                
 # 05 SMPLOC3    2407     1217073.010  112891.880  0.000                
 ```
 
 # Getting Started developing
 
-1. Software dependencies
-
-2. Clone this repository
-
-3. Install
-
 ## Software dependencies
 
 Before you start, install:
 
    - Python 3.9 or higher
    - Poetry
    - black code formatter
@@ -140,15 +133,14 @@
     poetry install
 
 
 # Build and Test
 
 Run in the project root folder: 
 
-    poetry install
     poetry run pytest 
 
 Build the package wheel: 
 
     poetry build
 
 # Contribute
```

