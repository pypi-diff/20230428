# Comparing `tmp/areas-0.1.8.tar.gz` & `tmp/areas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "areas-0.1.8.tar", max compression
+gzip compressed data, was "areas-0.1.9.tar", max compression
```

## Comparing `areas-0.1.8.tar` & `areas-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1091 2022-07-10 20:34:09.292968 areas-0.1.8/LICENSE
--rw-r--r--   0        0        0     8590 2023-04-05 15:11:22.994752 areas-0.1.8/README.md
--rw-r--r--   0        0        0       60 2022-09-03 17:56:00.424811 areas-0.1.8/areas/__init__.py
--rw-r--r--   0        0        0      357 2023-04-05 15:09:12.614604 areas-0.1.8/areas/config/architectures.py
--rw-r--r--   0        0        0      168 2022-09-03 17:56:00.425471 areas-0.1.8/areas/exception/__init__.py
--rw-r--r--   0        0        0      307 2022-09-03 17:56:00.425628 areas-0.1.8/areas/exception/compile_error.py
--rw-r--r--   0        0        0      162 2022-09-03 17:56:00.425742 areas-0.1.8/areas/exception/runtime_error.py
--rw-r--r--   0        0        0      100 2022-09-03 17:56:00.425867 areas-0.1.8/areas/exception/tool_file_error.py
--rw-r--r--   0        0        0     4165 2023-03-07 17:56:25.298171 areas-0.1.8/areas/main.py
--rw-r--r--   0        0        0      186 2022-09-03 17:56:00.426288 areas-0.1.8/areas/parameters/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-07 13:37:32.479679 areas-0.1.8/areas/parameters/array_parameter.py
--rw-r--r--   0        0        0      807 2023-04-07 13:37:21.737957 areas-0.1.8/areas/parameters/numeric_parameter.py
--rw-r--r--   0        0        0     1243 2023-04-07 13:37:29.419047 areas-0.1.8/areas/parameters/parameter.py
--rw-r--r--   0        0        0      774 2023-04-07 13:37:26.893885 areas-0.1.8/areas/parameters/string_parameter.py
--rw-r--r--   0        0        0      254 2022-09-03 17:56:00.427442 areas-0.1.8/areas/subroutines/__init__.py
--rw-r--r--   0        0        0     3736 2022-09-03 17:56:00.427779 areas-0.1.8/areas/subroutines/array_subroutine.py
--rw-r--r--   0        0        0     3997 2022-09-03 17:56:00.428127 areas-0.1.8/areas/subroutines/mixed_subroutine.py
--rw-r--r--   0        0        0     2103 2022-09-03 17:56:00.428360 areas-0.1.8/areas/subroutines/numeric_subroutine.py
--rw-r--r--   0        0        0     1773 2022-09-03 17:56:00.428562 areas-0.1.8/areas/subroutines/subroutine.py
--rw-r--r--   0        0        0     1356 2022-09-03 17:56:00.428979 areas-0.1.8/areas/subroutines/void_subroutine.py
--rw-r--r--   0        0        0     4587 2023-04-14 23:00:21.216832 areas-0.1.8/areas/test.py
--rw-r--r--   0        0        0    12405 2023-04-14 23:00:09.980564 areas-0.1.8/areas/tester.py
--rw-r--r--   0        0        0        0 2022-09-03 17:56:00.429619 areas-0.1.8/areas/util/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-07 22:04:30.099795 areas-0.1.8/areas/util/parse_errors.py
--rw-r--r--   0        0        0     3113 2023-04-07 12:58:14.476852 areas-0.1.8/areas/util/subroutine_integrity.py
--rw-r--r--   0        0        0      226 2022-09-03 17:56:00.430092 areas-0.1.8/areas/util/type_casting.py
--rw-r--r--   0        0        0      574 2023-04-14 23:12:27.685841 areas-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 areas-0.1.8/setup.py
--rw-r--r--   0        0        0     9031 1970-01-01 00:00:00.000000 areas-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-07-10 20:34:09.292968 areas-0.1.9/LICENSE
+-rw-r--r--   0        0        0     8590 2023-04-05 15:11:22.994752 areas-0.1.9/README.md
+-rw-r--r--   0        0        0       60 2022-09-03 17:56:00.424811 areas-0.1.9/areas/__init__.py
+-rw-r--r--   0        0        0      357 2023-04-05 15:09:12.614604 areas-0.1.9/areas/config/architectures.py
+-rw-r--r--   0        0        0      168 2022-09-03 17:56:00.425471 areas-0.1.9/areas/exception/__init__.py
+-rw-r--r--   0        0        0      307 2022-09-03 17:56:00.425628 areas-0.1.9/areas/exception/compile_error.py
+-rw-r--r--   0        0        0      162 2022-09-03 17:56:00.425742 areas-0.1.9/areas/exception/runtime_error.py
+-rw-r--r--   0        0        0      100 2022-09-03 17:56:00.425867 areas-0.1.9/areas/exception/tool_file_error.py
+-rw-r--r--   0        0        0     4165 2023-03-07 17:56:25.298171 areas-0.1.9/areas/main.py
+-rw-r--r--   0        0        0      186 2022-09-03 17:56:00.426288 areas-0.1.9/areas/parameters/__init__.py
+-rw-r--r--   0        0        0     1853 2023-04-07 13:37:32.479679 areas-0.1.9/areas/parameters/array_parameter.py
+-rw-r--r--   0        0        0      807 2023-04-07 13:37:21.737957 areas-0.1.9/areas/parameters/numeric_parameter.py
+-rw-r--r--   0        0        0     1243 2023-04-07 13:37:29.419047 areas-0.1.9/areas/parameters/parameter.py
+-rw-r--r--   0        0        0      774 2023-04-07 13:37:26.893885 areas-0.1.9/areas/parameters/string_parameter.py
+-rw-r--r--   0        0        0      254 2022-09-03 17:56:00.427442 areas-0.1.9/areas/subroutines/__init__.py
+-rw-r--r--   0        0        0     3736 2022-09-03 17:56:00.427779 areas-0.1.9/areas/subroutines/array_subroutine.py
+-rw-r--r--   0        0        0     3997 2022-09-03 17:56:00.428127 areas-0.1.9/areas/subroutines/mixed_subroutine.py
+-rw-r--r--   0        0        0     2103 2022-09-03 17:56:00.428360 areas-0.1.9/areas/subroutines/numeric_subroutine.py
+-rw-r--r--   0        0        0     1773 2022-09-03 17:56:00.428562 areas-0.1.9/areas/subroutines/subroutine.py
+-rw-r--r--   0        0        0     1356 2022-09-03 17:56:00.428979 areas-0.1.9/areas/subroutines/void_subroutine.py
+-rw-r--r--   0        0        0     4866 2023-04-28 21:55:29.314351 areas-0.1.9/areas/test.py
+-rw-r--r--   0        0        0    14750 2023-04-28 21:27:49.577288 areas-0.1.9/areas/tester.py
+-rw-r--r--   0        0        0        0 2022-09-03 17:56:00.429619 areas-0.1.9/areas/util/__init__.py
+-rw-r--r--   0        0        0     1281 2023-04-07 22:04:30.099795 areas-0.1.9/areas/util/parse_errors.py
+-rw-r--r--   0        0        0     3113 2023-04-07 12:58:14.476852 areas-0.1.9/areas/util/subroutine_integrity.py
+-rw-r--r--   0        0        0      226 2022-09-03 17:56:00.430092 areas-0.1.9/areas/util/type_casting.py
+-rw-r--r--   0        0        0      574 2023-04-28 21:58:57.011582 areas-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 areas-0.1.9/setup.py
+-rw-r--r--   0        0        0     9031 1970-01-01 00:00:00.000000 areas-0.1.9/PKG-INFO
```

### Comparing `areas-0.1.8/LICENSE` & `areas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/README.md` & `areas-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/main.py` & `areas-0.1.9/areas/main.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/parameters/array_parameter.py` & `areas-0.1.9/areas/parameters/array_parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/parameters/numeric_parameter.py` & `areas-0.1.9/areas/parameters/numeric_parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/parameters/parameter.py` & `areas-0.1.9/areas/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/parameters/string_parameter.py` & `areas-0.1.9/areas/parameters/string_parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/subroutines/array_subroutine.py` & `areas-0.1.9/areas/subroutines/array_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/subroutines/mixed_subroutine.py` & `areas-0.1.9/areas/subroutines/mixed_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/subroutines/numeric_subroutine.py` & `areas-0.1.9/areas/subroutines/numeric_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/subroutines/subroutine.py` & `areas-0.1.9/areas/subroutines/subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/subroutines/void_subroutine.py` & `areas-0.1.9/areas/subroutines/void_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/test.py` & `areas-0.1.9/areas/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,25 @@
 from areas.subroutines import MixedSubroutine as Mixed
 from areas.subroutines import NumericSubroutine as Numeric
 from areas.subroutines import VoidSubroutine as Void
 from areas.tester import Tester
 
 
 class Test:
-
-    def __init__(self, submission_file, subroutine_file=None, tests_file=None,
-                 subroutines=None, test_suite=None,
-                 timeout=1, float_threshold=1e-6, save_to_file=False):
+    def __init__(
+        self,
+        submission_file,
+        subroutine_file=None,
+        tests_file=None,
+        subroutines=None,
+        test_suite=None,
+        timeout=1,
+        float_threshold=1e-6,
+        save_to_file=False,
+    ):
         self.submission_file = submission_file
         self.subroutine_file = subroutine_file
         self.tests_file = tests_file
 
         # files always override manual definitions
         self.subroutines = subroutines
         self.test_suite = test_suite
@@ -33,85 +40,106 @@
         self.__read_files()
         self.__parse_inputs()
         self.__build_test_cases()
 
     def __parse_inputs(self):
         for key in self.subroutines:
             if key not in self.test_suite:
-                raise ToolFileError(
-                    f"Subroutine {key} is not in the test suite")
+                raise ToolFileError(f"Subroutine {key} is not in the test suite")
             else:
                 subroutine = self.subroutines[key]
                 test_suite = self.test_suite[key]
 
                 subroutine_integrity.parse_subroutine(subroutine, test_suite)
 
     def __load_file(self, file):
-        ext = file.split('.')[-1]
+        ext = file.split(".")[-1]
 
-        if ext == 'json':
+        if ext == "json":
             return json.load(open(file))
-        elif ext == 'yaml' or ext == 'yml':
+        elif ext == "yaml" or ext == "yml":
             return safe_load(open(file))
         else:
-            raise ToolFileError(
-                'File extension not supported: {}'.format(ext))
+            raise ToolFileError("File extension not supported: {}".format(ext))
 
     def __read_files(self):
         try:
             if self.subroutine_file is not None:
                 self.subroutines = self.__load_file(self.subroutine_file)
 
             if self.tests_file is not None:
                 self.test_suite = self.__load_file(self.tests_file)
         except IOError as err:
             raise ToolFileError(
-                'Could not open: {}, please specify a valid file'.format(str(err)))
+                "Could not open: {}, please specify a valid file".format(str(err))
+            )
         except YAMLError as err:
             raise ToolFileError(
-                'Error parsing YAML files: ({}), please correct syntax'.format(str(err)))
+                "Error parsing YAML files: ({}), please correct syntax".format(str(err))
+            )
 
     def __build_subroutine(self, name, definition):
-        map_to_truth_value = ['array' in ret or ret ==
-                              'string' for ret in definition['return']]
-
-        architecture = definition['architecture'] if 'architecture' in definition else "arm"
+        map_to_truth_value = [
+            "array" in ret or ret == "string" for ret in definition["return"]
+        ]
+
+        architecture = (
+            definition["architecture"] if "architecture" in definition else "arm"
+        )
 
         if not len(map_to_truth_value):  # No returns - void subroutine
-            return Void(name, definition['params'], architecture)
+            return Void(name, definition["params"], architecture)
         elif all(map_to_truth_value):  # Only arrays and/or strings as return values
-            return Array(name, definition['params'], definition['return'], architecture)
+            return Array(name, definition["params"], definition["return"], architecture)
         elif not any(map_to_truth_value):  # Numeric output
-            return Numeric(name, definition['params'], definition['return'][0], architecture)
+            return Numeric(
+                name, definition["params"], definition["return"][0], architecture
+            )
         else:  # Mixed return
-            return Mixed(name, definition['params'], definition['return'][0], definition['return'][1:], architecture)
+            return Mixed(
+                name,
+                definition["params"],
+                definition["return"][0],
+                definition["return"][1:],
+                architecture,
+            )
 
     def __build_test_cases(self):
-        self.subroutine_objects = {name: self.__build_subroutine(
-            name, definition) for name, definition in self.subroutines.items()}
+        self.subroutine_objects = {
+            name: self.__build_subroutine(name, definition)
+            for name, definition in self.subroutines.items()
+        }
 
     def run(self):
         folder_prefix = str(datetime.now().microsecond)
 
-        grading_folder = f'tmp_{folder_prefix}_grading'
-        feedback_folder = f'tmp_{folder_prefix}_feedback'
+        grading_folder = f"tmp_{folder_prefix}_grading"
+        feedback_folder = f"tmp_{folder_prefix}_feedback"
 
         try:
-            tester = Tester(self.subroutine_objects, self.test_suite, grading_folder=grading_folder,
-                            feedback_folder=feedback_folder, float_threshold=self.float_threshold,
-                            timeout=self.timeout, save_to_file=self.save_to_file)
+            tester = Tester(
+                self.subroutine_objects,
+                self.test_suite,
+                grading_folder=grading_folder,
+                feedback_folder=feedback_folder,
+                float_threshold=self.float_threshold,
+                timeout=self.timeout,
+                save_to_file=self.save_to_file,
+            )
 
             submission = tester.grade_submission(self.submission_file)
 
             filename = match(
-                r'(?:.+\/)*(.*)?.*\.zip', self.submission_file, flags=IGNORECASE).group(1)
+                r"(?:.+\/)*(.*)?.*\.zip", self.submission_file, flags=IGNORECASE
+            ).group(1)
 
             return {
-                'submission_name': filename,
-                'subroutines': submission,
+                "submission_name": filename,
+                "subroutines": submission,
             }
         except Exception as err:
             raise err
         finally:
             import shutil
+
             shutil.rmtree(grading_folder, ignore_errors=True)
             shutil.rmtree(feedback_folder, ignore_errors=True)
```

### Comparing `areas-0.1.8/areas/tester.py` & `areas-0.1.9/areas/tester.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,199 +12,308 @@
 from areas.exception import *
 from areas.util.parse_errors import parse_compilation_errors
 
 
 class Tester:
     """Evaluator class that grades student's submissions based on test input/output comparison and optional code scoring"""
 
-    def __init__(self, subroutines, test_suite, cmd_line_args=None, grading_folder=None,
-                 feedback_folder=None, float_threshold=None, timeout=None, save_to_file=True):
-        self.temp_grading_folder = grading_folder or cmd_line_args['gfd']
-        self.feedback_folder = feedback_folder or cmd_line_args['ffd']
+    def __init__(
+        self,
+        subroutines,
+        test_suite,
+        cmd_line_args=None,
+        grading_folder=None,
+        feedback_folder=None,
+        float_threshold=None,
+        timeout=None,
+        save_to_file=True,
+    ):
+        self.temp_grading_folder = grading_folder or cmd_line_args["gfd"]
+        self.feedback_folder = feedback_folder or cmd_line_args["ffd"]
         self.subroutines = subroutines
-        self.float_threshold = float_threshold or cmd_line_args['fpre']
-        self.timeout = timeout or cmd_line_args['tout']
+        self.float_threshold = float_threshold or cmd_line_args["fpre"]
+        self.timeout = timeout or cmd_line_args["tout"]
         self.save_to_file = save_to_file
 
-        self.template_files = [sr.build_c_file()
-                               for sr in self.subroutines.values()]
+        self.template_files = [sr.build_c_file() for sr in self.subroutines.values()]
 
-        self.test_outputs = [list(map(lambda test: test['outputs'], test_suite[name]))
-                             for name in self.subroutines.keys()]
-        self.test_inputs = [list(map(lambda test: test['inputs'], test_suite[name]))
-                            for name in self.subroutines.keys()]
-        self.test_weights = [list(map(lambda test: test['weight'], test_suite[name]))
-                             for name in self.subroutines.keys()]
+        self.test_outputs = [
+            list(map(lambda test: test["outputs"], test_suite[name]))
+            for name in self.subroutines.keys()
+        ]
+        self.test_inputs = [
+            list(map(lambda test: test["inputs"], test_suite[name]))
+            for name in self.subroutines.keys()
+        ]
+        self.test_weights = [
+            list(map(lambda test: test["weight"], test_suite[name]))
+            for name in self.subroutines.keys()
+        ]
 
         if os.path.exists(self.feedback_folder):
             delete_dir(self.feedback_folder)
 
         if self.save_to_file:
             os.mkdir(self.feedback_folder)
 
     def extract_submission_files(self, student_submission):
         """Extracts all relevant subroutine files from a submission in order to be graded"""
-        with unzip(student_submission, 'r') as zip_file:
+        with unzip(student_submission, "r") as zip_file:
             # Get a list of all subroutine file names from the zip
-            files = filter(lambda x: x is not None, map(lambda y: match(
-                r'(?:\w+/)*([\w\-]+\.s)', y), zip_file.namelist()))
+            files = filter(
+                lambda x: x is not None,
+                map(lambda y: match(r"(?:\w+/)*([\w\-]+\.s)", y), zip_file.namelist()),
+            )
             for file in files:
-                with open('{}/{}'.format(self.temp_grading_folder, file.group(1).lower()), mode='wb') as f:
+                with open(
+                    "{}/{}".format(self.temp_grading_folder, file.group(1).lower()),
+                    mode="wb",
+                ) as f:
                     f.write(zip_file.read(file.group(0)))
 
     def get_extra_assembly_to_include(self, subroutine):
         """Obtains a list of subroutines that are used in the given one so that they can be correctly included at compilation time"""
         try:
-            with open('{}/{}.s'.format(self.temp_grading_folder, subroutine.lower()), mode='rb') as f:
-                calls = list(filter(lambda x: x is not None, map(lambda y: search(
-                    rb'(bl|call)\s+([\w\-\_]+)', y.strip(), flags=IGNORECASE), f.readlines())))
+            with open(
+                "{}/{}.s".format(self.temp_grading_folder, subroutine.lower()),
+                mode="rb",
+            ) as f:
+                content = f.readlines()
+
+                calls = list(
+                    filter(
+                        lambda x: x is not None,
+                        map(
+                            lambda y: search(
+                                rb"(bl|call)\s+([\w\-\_]+)", y.strip(), flags=IGNORECASE
+                            ),
+                            content,
+                        ),
+                    )
+                )
 
                 # risc-v calls
-                riscv_calls = list(filter(lambda x: x is not None, map(lambda y: search(
-                    rb'jalr?\s+(?:[\w\-\_]+),\s+([\w\-\_]+)(,\s+\d)?', y.strip(), flags=IGNORECASE), f.readlines())))
-
-                calls = calls + riscv_calls
-
-                calls = set(map(lambda x: x.group(
-                    2).lower().decode('utf-8'), calls))
-
-                return [sr for sr in calls if os.path.exists('{}/{}.s'.format(self.temp_grading_folder, sr))]
+                jalr_calls = list(
+                    filter(
+                        lambda x: x is not None,
+                        map(
+                            lambda y: search(
+                                rb"jalr?\s+(?:.[\w\-\_]+),\s+(.[\w\-\_]+)(,\s+\d)?",
+                                y.strip(),
+                                flags=IGNORECASE,
+                            ),
+                            content,
+                        ),
+                    )
+                )
+
+                jal_calls = list(
+                    filter(
+                        lambda x: x is not None,
+                        map(
+                            lambda y: search(
+                                rb"jal\s+(.[\w\-\_]+)",
+                                y.strip(),
+                                flags=IGNORECASE,
+                            ),
+                            content,
+                        ),
+                    )
+                )
+
+                calls = set(map(lambda x: x.group(2).lower().decode("utf-8"), calls))
+                jalr_calls = set(
+                    map(lambda x: x.group(1).lower().decode("utf-8"), jalr_calls)
+                )
+                jal_calls = set(
+                    map(lambda x: x.group(1).lower().decode("utf-8"), jal_calls)
+                )
+
+                calls = set(list(calls) + list(jalr_calls) + list(jal_calls))
+
+                return [
+                    sr
+                    for sr in calls
+                    if os.path.exists("{}/{}.s".format(self.temp_grading_folder, sr))
+                ]
         except FileNotFoundError:
             return []
 
     def cleanup_files(self, files):
         for path in files:
-            file = open(path, 'r+', encoding='ISO-8859-1')
-            new_content = file.read().replace('system', 'blacklisted_word')
+            file = open(path, "r+", encoding="ISO-8859-1")
+            new_content = file.read().replace("system", "blacklisted_word")
             file.seek(0)
             file.write(new_content)
             file.truncate()
             file.close()
 
-    def compile_and_run(self, subroutine, template_file, inp, output_file, architecture="arm"):
+    def compile_and_run(
+        self, subroutine, template_file, inp, output_file, architecture="arm"
+    ):
         """Compiles and runs, with the generated C template files, the student's submission files.
-        Returns a boolean tuple with information of a successful (or not) compilation and a successful (or not) test run"""
+        Returns a boolean tuple with information of a successful (or not) compilation and a successful (or not) test run
+        """
 
-        compiler = ARCHITECTURES[architecture]['compiler']
-        emulator = ARCHITECTURES[architecture]['emulator']
+        compiler = ARCHITECTURES[architecture]["compiler"]
+        emulator = ARCHITECTURES[architecture]["emulator"]
 
         sr = self.subroutines[subroutine]
         sr_non_int_outputs = sr.get_nr_outputs()
 
         # Rearrange parameter-input pair order for format due to possible parameters that are output and, therefore, declared first
         sorted_param_list = list(zip(sr.parameters, inp))
-        sorted_param_list = sorted_param_list[-sr_non_int_outputs:] + \
-            sorted_param_list[:-sr_non_int_outputs]
+        sorted_param_list = (
+            sorted_param_list[-sr_non_int_outputs:]
+            + sorted_param_list[:-sr_non_int_outputs]
+        )
 
         # Build C file from template
-        open('{}.c'.format(output_file), 'w').write(
-            template_file.format(*[param.get_literal_representation(inp_literal) for param, inp_literal in sorted_param_list]))
+        open("{}.c".format(output_file), "w").write(
+            template_file.format(
+                *[
+                    param.get_literal_representation(inp_literal)
+                    for param, inp_literal in sorted_param_list
+                ]
+            )
+        )
 
         compilation_files = list(
-            map(lambda x: "{}/{}.s".format(self.temp_grading_folder, x.lower()),
-                [subroutine, *self.get_extra_assembly_to_include(subroutine)])
+            map(
+                lambda x: "{}/{}.s".format(self.temp_grading_folder, x.lower()),
+                [subroutine, *self.get_extra_assembly_to_include(subroutine)],
+            )
         )
 
         try:
             self.cleanup_files(compilation_files)  # temporary fix
         except Exception as e:
             pass
 
         # Compile student code alongside generated C file
-        compilation_process = subprocess.Popen('{} -o {} {}.c {} -static'.format(
-            compiler,
-            output_file,
-            output_file,
-            ' '.join(compilation_files)
-        ).split(' '), stderr=subprocess.PIPE)
+        compilation_process = subprocess.Popen(
+            "{} -o {} {}.c {} -static".format(
+                compiler, output_file, output_file, " ".join(compilation_files)
+            ).split(" "),
+            stderr=subprocess.PIPE,
+        )
         compilation_process.wait()
         (_, stderr) = compilation_process.communicate()
 
         # Throw compilation error
-        if compilation_process.returncode != 0:  # If it doesn't even compile, not worth checking any further
+        if (
+            compilation_process.returncode != 0
+        ):  # If it doesn't even compile, not worth checking any further
             raise CompileError(stderr)
 
         # Execute and redirect output to temporary .txt file
-        real_output_file = '{}.txt'.format(output_file)
-        execution_process = subprocess.Popen('timeout {} {} {}'.format(self.timeout, emulator, output_file), stdout=open(
-            real_output_file, mode='w', encoding='utf-8'), stderr=subprocess.PIPE, shell=True)
+        real_output_file = "{}.txt".format(output_file)
+        execution_process = subprocess.Popen(
+            "timeout {} {} {}".format(self.timeout, emulator, output_file),
+            stdout=open(real_output_file, mode="w", encoding="utf-8"),
+            stderr=subprocess.PIPE,
+            shell=True,
+        )
         execution_process.wait()
         (_, stderr) = execution_process.communicate()
 
         if execution_process.returncode != 0:
-            if execution_process.returncode == 124:  # Return code when timeout had to kill the process
+            if (
+                execution_process.returncode == 124
+            ):  # Return code when timeout had to kill the process
                 raise RuntimeError(
-                    'Failed to run: process took longer than {}s limit'.format(self.timeout))
+                    "Failed to run: process took longer than {}s limit".format(
+                        self.timeout
+                    )
+                )
             else:  # Other reason, but not running properly
                 first_index = str(stderr).find('"') + 1
                 last_index = str(stderr).rfind('"')
 
-                message = str(stderr)[
-                    first_index:last_index].strip()
+                message = str(stderr)[first_index:last_index].strip()
 
-                raise RuntimeError(
-                    'Failed to run: {}\n'.format(message))
+                raise RuntimeError("Failed to run: {}\n".format(message))
 
-    def compare_test_call_output(self, subroutine, output_file, expected_outputs, given_inputs):
+    def compare_test_call_output(
+        self, subroutine, output_file, expected_outputs, given_inputs
+    ):
         """Compares expected to real outputs, calculating student's score on it"""
         # Read real outputs
-        real_outputs = list(map(lambda x: x.decode(
-            'utf-8', 'backslashreplace').strip(), open('{}.txt'.format(output_file), 'rb').readlines()))
+        real_outputs = list(
+            map(
+                lambda x: x.decode("utf-8", "backslashreplace").strip(),
+                open("{}.txt".format(output_file), "rb").readlines(),
+            )
+        )
 
         # Should return outputs and result (expected if necessary)
 
-        converted_output = self.subroutines[subroutine].convert_outputs(
-            real_outputs)
+        converted_output = self.subroutines[subroutine].convert_outputs(real_outputs)
 
         # Actual comparison
-        if not self.subroutines[subroutine].compare_outputs(expected_outputs, real_outputs, self.float_threshold):
-            return (False, {
-                'output': list(map(lambda x: repr(x).replace("'", ""), real_outputs)),
-                'expected': expected_outputs,
-                'passed': False
-            })
-
-        return (True, {
-            'output': list(map(lambda x: repr(x).replace("'", ""), real_outputs)),
-            'passed': True
-        })
+        if not self.subroutines[subroutine].compare_outputs(
+            expected_outputs, real_outputs, self.float_threshold
+        ):
+            return (
+                False,
+                {
+                    "output": list(
+                        map(lambda x: repr(x).replace("'", ""), real_outputs)
+                    ),
+                    "expected": expected_outputs,
+                    "passed": False,
+                },
+            )
+
+        return (
+            True,
+            {
+                "output": list(map(lambda x: repr(x).replace("'", ""), real_outputs)),
+                "passed": True,
+            },
+        )
 
     def grade_submission(self, student_submission):
         """Grades a student's submission by comparing each real output to expected output, writing feedback in failing cases if applicable and final grade to grades csv"""
         # Reset temporary grading folder if for some reason it already exists
         if os.path.exists(self.temp_grading_folder):
             delete_dir(self.temp_grading_folder)
         os.mkdir(self.temp_grading_folder)
 
         # Extract all assembly files to grading directory
         self.extract_submission_files(student_submission)
 
         filename = match(
-            r'(?:.+\/)*(.*)?.*\.zip', student_submission, flags=IGNORECASE).group(1)
+            r"(?:.+\/)*(.*)?.*\.zip", student_submission, flags=IGNORECASE
+        ).group(1)
 
         if self.save_to_file:
             feedback_file = open(
-                '{}/{}.json'.format(self.feedback_folder, filename), 'w')
+                "{}/{}.json".format(self.feedback_folder, filename), "w"
+            )
 
         subroutine_list = []
 
-        for subroutine, template_file, inputs, outputs, weights in zip(self.subroutines.keys(), self.template_files, self.test_inputs, self.test_outputs, self.test_weights):
+        for subroutine, template_file, inputs, outputs, weights in zip(
+            self.subroutines.keys(),
+            self.template_files,
+            self.test_inputs,
+            self.test_outputs,
+            self.test_weights,
+        ):
             # set default compiler as arm
             architecture = self.subroutines[subroutine].architecture or "arm"
 
             # Subroutine output file template
-            output_file = '{}/{}'.format(self.temp_grading_folder,
-                                         subroutine.lower())
+            output_file = "{}/{}".format(self.temp_grading_folder, subroutine.lower())
 
             passed = 0
 
             # Creating subroutine object
-            subroutine_object = {
-                'name': subroutine
-            }
+            subroutine_object = {"name": subroutine}
 
             compiled = True
             compile_output = None
 
             all_tests_passed = True
 
             tests_list = []
@@ -214,71 +323,77 @@
 
             for inp, out, weight in zip(inputs, outputs, weights):
                 # Try to compile and run submission for a specific input case
                 # If it fails, grade with zero and move to next subroutine
 
                 test_object = {}
 
-                test_object['weight'] = weight
+                test_object["weight"] = weight
 
                 try:
                     self.compile_and_run(
-                        subroutine, template_file, inp, output_file, architecture)
+                        subroutine, template_file, inp, output_file, architecture
+                    )
                 except CompileError as compile_error:
                     compile_output = str(compile_error)
                     compiled = False
                     break
 
                 except RuntimeError as runtime_error:
                     all_tests_passed = False
 
-                    test_object['run'] = False
-                    test_object['error'] = str(runtime_error)
-                    test_object['input'] = inp
+                    test_object["run"] = False
+                    test_object["error"] = str(runtime_error)
+                    test_object["input"] = inp
 
                     tests_list.append(test_object)
                     continue
 
-                test_object['run'] = True
+                test_object["run"] = True
 
                 (test_passed, test_compare_object) = self.compare_test_call_output(
-                    subroutine, output_file, out, inp)
+                    subroutine, output_file, out, inp
+                )
 
                 if test_passed:
                     passed = passed + 1
 
                     score = score + int(float(weight) * 1000000)
                 else:
                     all_tests_passed = False
 
-                test_object['input'] = inp
+                test_object["input"] = inp
                 test_object.update(test_compare_object)
                 tests_list.append(test_object)
 
-            subroutine_object['compiled'] = compiled
+            subroutine_object["compiled"] = compiled
 
             if not compiled:
-                subroutine_object['compile_output'] = compile_output
+                subroutine_object["compile_output"] = compile_output
 
                 compilation_warnings, compilation_errors = parse_compilation_errors(
-                    compile_output)
+                    compile_output
+                )
 
-                subroutine_object['compilation_errors'] = {
-                    'warnings': compilation_warnings,
-                    'errors': compilation_errors
+                subroutine_object["compilation_errors"] = {
+                    "warnings": compilation_warnings,
+                    "errors": compilation_errors,
                 }
 
-            subroutine_object['ok'] = compiled and all_tests_passed
-            subroutine_object['passed_count'] = passed
-            subroutine_object['test_count'] = len(outputs)
-            subroutine_object['score'] = float(score / 1000000)
-            subroutine_object['tests'] = tests_list
+            subroutine_object["ok"] = compiled and all_tests_passed
+            subroutine_object["passed_count"] = passed
+            subroutine_object["test_count"] = len(outputs)
+            subroutine_object["score"] = float(score / 1000000)
+            subroutine_object["tests"] = tests_list
 
             subroutine_list.append(subroutine_object)
 
         if self.save_to_file:
-            json.dump({'submission_name': filename,
-                       'subroutines': subroutine_list}, feedback_file, indent=4)
+            json.dump(
+                {"submission_name": filename, "subroutines": subroutine_list},
+                feedback_file,
+                indent=4,
+            )
         # Remove temporary auxiliary folder and write final scores
         # delete_dir(self.temp_grading_folder)
 
         return subroutine_list
```

### Comparing `areas-0.1.8/areas/util/parse_errors.py` & `areas-0.1.9/areas/util/parse_errors.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/areas/util/subroutine_integrity.py` & `areas-0.1.9/areas/util/subroutine_integrity.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.8/pyproject.toml` & `areas-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "areas"
-version = "0.1.8"
+version = "0.1.9"
 description = "ARM64 and RISC-V (extensible) assessment system"
 authors = ["Luis Tavares <luistavares10@outlook.pt>"]
 repository = "https://github.com/luist18/areasear"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "areas"}]
```

### Comparing `areas-0.1.8/setup.py` & `areas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ['PyYAML>=6.0,<7.0', 'Unidecode>=1.3.4,<2.0.0', 'pytest>=7.2.0,<8.0.0']
 
 entry_points = \
 {'console_scripts': ['test = scripts:test']}
 
 setup_kwargs = {
     'name': 'areas',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'ARM64 and RISC-V (extensible) assessment system',
     'long_description': '# areas<!-- omit in toc -->\n\n[![GitHub license](https://img.shields.io/github/license/luist18/areas?color=blue)](https://github.com/luist18/areas/blob/main/LICENSE)\n\n**A**RM64 and **R**ISC-V (**e**xtensible) **A**ssessment **S**ystem.\n\n*areas* is originally a fork from [João Damas\'](https://github.com/cyrilico) [Automatic Observation and (grade) Calculation for (subroutine) Operations tool](https://github.com/cyrilico/aoco-code-correction). It is a tool to automate student\'s grading in the assignments done during the Microprocessor and Personal Computers course unit.\n\n## Differences with the original tool<!-- omit in toc -->\n\nTo ease the communication between the backend server and the tool the output demanded changes. Output `.txt` and `.csv` files are now combined in a more complete `.json` file. Structure of the `.zip` input file is simplified. Unsupported data types such as long and double are now supported. A new input parameter - weight - is introduced.\n\n---\n\n## Table of contents<!-- omit in toc -->\n\n- [1. Installation](#1-installation)\n- [2. Developing](#2-developing)\n- [3. Running](#3-running)\n- [4. Usage](#4-usage)\n- [5. File syntax and structure](#5-file-syntax-and-structure)\n  - [5.1. Available data types](#51-available-data-types)\n    - [5.1.1. Primitive data types](#511-primitive-data-types)\n    - [5.1.2. Array data types](#512-array-data-types)\n  - [5.2. subroutines.yaml](#52-subroutinesyaml)\n  - [5.3. tests.yaml](#53-testsyaml)\n  - [5.4. submission.zip](#54-submissionzip)\n- [6. Results](#6-results)\n\n## 1. Installation\n\nUsing Docker:\n\n```bash\ndocker pull luist188/areas\n```\n\n## 2. Developing\n\nTo develop the tool you must setup a Docker development environment to ease the dependencies installation and setup an isolated environment.\n\n1. Build the Docker development image:\n\n   ```bash\n   docker build -f Dockerfile.dev -t areas .\n   ```\n\n2. Run the image with the shared folder:\n\n   ```bash\n   docker run -it -v $(pwd):/usr/app areas\n   ```\n\nNote: if you are running MacOS with the M1 (or superior) chip you must add `--platform linux/x86_64` to `docker build` and `docker run`.\n\n## 3. Running\n\n1. Place the input files inside any directory.\n2. Run the image with a shared volume pointing to the input directory: `docker run -v input:destination -it luist188/areas` (you can learn more about `docker run` usage [here](https://docs.docker.com/engine/reference/run/))\n3. Run the alias command (assure you are using `/bin/bash`) `areas` or run `python main.py` in the tool\'s source.\n\n## 4. Usage\n\n```console\n$ areas [-h] -sr SR -t T -sm SM [SM ...] [-gfd GFD] [-ffd FFD] [-grf GRF] [-tout TOUT] [-fpre FPRE]\n\n$ areas [args]\n\nOptions:\n  --help, -h                Show help                                         [boolean]\n  -sr <subroutines.yaml>    .yaml file containing subroutine declaration      [required] [string]\n  -t <tests.yaml>           .yaml file containing the test cases              [required] [string]\n  -sm <submission.zip...>   .zip files containing user submission             [required] [string array]\n  -gfd <directory>          path to the directory to store temporary files\n    (e.g., compiled binaries)                                                 [default:grading] [string]\n  -ffd <directory>          path to the directory to store the grading for\n    each submission                                                           [default:feedback] [string]\n  -tout <timeout>           float timeout value                               [default:2.0] [float]\n  -fpre <precision>         floating point threshold for comparing floating\n    points in test cases                                                      [default:1e-6] [float]\n```\n\n## 5. File syntax and structure\n\n### 5.1. Available data types\n\n#### 5.1.1. Primitive data types\n\n- `int`\n- `long`\n- `float`\n- `double`\n- `char`\n- `chari` (char represented as an unsgined intenger - similar to char but has to be used when printed characters are not ASCII characters)\n\n#### 5.1.2. Array data types\n\n- `char*/string`\n- `array int`\n- `array long`\n- `array float`\n- `array double`\n- `array char`\n- `array chari`\n\n### 5.2. subroutines.yaml\n\nThe input file for the subroutine declaration has to follow a specific structure and syntax described as follows:\n\n```yaml\nfoo: \n  params: \n    - int\n    - array char\n    - array int\n    - array int\n  return: \n    - int\n    - array int\n\nbar: \n  params: \n    - long\n  return: \n    - long\n```\n\nEach subroutine has an optional parameter to define the subroutine architecture, the syntax is as follows:\n\n```yaml\nfoo: \n  architecture: arm\n  params: \n    - int\n    - array char\n    - array int\n    - array int\n  return: \n    - int\n    - array int\n```\n\nBy default, if the architecture parameter is omitted, the system will assume ARM64 as the subroutine architecture. The available architectures are the following:\n\n- `arm` - ARM64 architecture\n- `riscv` - RISC-V architecture\n\nThe subroutine name has to match the `.s` to test and is case insensitive. Thus, the subroutine `foo` or `bar` is going to check any `.s` file that matches its name case insensitive. All subroutines must contain an array of parameters, `params`, and an array of returns, `return`.\n\n### 5.3. tests.yaml\n\nThe input file for the test cases declaration has to follow a specific structure and syntax described as follows:\n\n```yaml\nbar:\n  - inputs:\n    - 6\n    outputs: \n    - 36\n    weight: 0.5\n  - inputs:\n    - 5\n    outputs: \n    - 25\n    weight: 0.5\n```\n\nThe root declaration of a test case must match the name declared in the `subroutines.yaml` file. Test cases have an array of inputs that has a list of outputs and a test weight. The sum of the test weights must be 1.0.\n\n### 5.4. submission.zip\n\nThe submission `zip` file must contain a `.s` file in its root. For example, for the subroutine `foo` and `bar` the `zip` structure should be as follows:\n\n```tree\nsubmission.zip\n├── foo.s\n└── bar.s\n```\n\n## 6. Results\n\nFor each submission file a `.json` file is created in the feedback directory with the same name of the `.zip` file. The file contains all information about compilation status and test cases. In addition, a simplified version of the result of all submissions is created in a `result.json`. The content of the files look as follows:\n\nFile **submission.json**\n\n```json\n[\n    {\n        "name": "foo",\n        "compiled": true,\n        "ok": true,\n        "passed_count": 2,\n        "test_count": 2,\n        "score": 1,\n        "tests": [\n            {\n                "weight": 1,\n                "run": true,\n                "input": [\n                    6,\n                    ["-", "+", "+", "-", "-", "+"],\n                    [1, 2, 3, 0, 1, -25],\n                    [13, 2, 8, 4, 5, 25]\n                ],\n                "output": [\n                    "0",\n                    ["12", "4", "11", "4", "4", "0"]\n                ],\n                "passed": true\n            }\n        ]\n    },\n    {\n        "name": "bar",\n        "compiled": true,\n        "ok": true,\n        "passed_count": 2,\n        "test_count": 2,\n        "score": 1,\n        "tests": [\n            {\n                "weight": 0.5,\n                "run": true,\n                "input": [\n                    6\n                ],\n                "output": [\n                    "36"\n                ],\n                "passed": true\n            },\n            {\n                "weight": 0.5,\n                "run": true,\n                "input": [\n                    5\n                ],\n                "output": [\n                    "25"\n                ],\n                "passed": true\n            }\n        ]\n    }\n]\n```\n\nFile **result.json**\n\n```json\n[\n    {\n        "submission_name": "submission",\n        "subroutines": [\n            {\n                "name": "foo",\n                "score": 0\n            },\n            {\n                "name": "bar",\n                "score": 0.5\n            }\n        ]\n    },\n    {\n        "submission_name": "submission2",\n        "subroutines": [\n            {\n                "name": "foo",\n                "score": 1\n            },\n            {\n                "name": "bar",\n                "score": 1\n            }\n        ]\n    }\n]\n```\n\n## License<!-- omit in toc -->\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Luis Tavares',
     'author_email': 'luistavares10@outlook.pt',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luist18/areasear',
```

### Comparing `areas-0.1.8/PKG-INFO` & `areas-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: areas
-Version: 0.1.8
+Version: 0.1.9
 Summary: ARM64 and RISC-V (extensible) assessment system
 Home-page: https://github.com/luist18/areasear
 License: MIT
 Author: Luis Tavares
 Author-email: luistavares10@outlook.pt
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

