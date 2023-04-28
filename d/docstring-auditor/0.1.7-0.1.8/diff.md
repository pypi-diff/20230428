# Comparing `tmp/docstring_auditor-0.1.7.tar.gz` & `tmp/docstring_auditor-0.1.8.tar.gz`

## Comparing `docstring_auditor-0.1.7.tar` & `docstring_auditor-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/Dockerfile
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/action.yml
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/image-latest.yml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/image-release.yml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/release.yml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/docstring_auditor/__init__.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/docstring_auditor/main.py
--rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/tests/test_critique.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/tests/test_extractor.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/tests/test_reporter.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/LICENSE
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/README.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 docstring_auditor-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.aidev
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/Dockerfile
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/action.yml
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/image-latest.yml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/image-release.yml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/docstring_auditor/__init__.py
+-rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/docstring_auditor/main.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_critique.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_exit_codes.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_extractor.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/tests/test_reporter.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/LICENSE
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/README.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 docstring_auditor-0.1.8/PKG-INFO
```

### Comparing `docstring_auditor-0.1.7/Dockerfile` & `docstring_auditor-0.1.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.7/action.yml` & `docstring_auditor-0.1.8/action.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.7/.github/workflows/image-latest.yml` & `docstring_auditor-0.1.8/.github/workflows/image-latest.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.7/.github/workflows/image-release.yml` & `docstring_auditor-0.1.8/.github/workflows/image-release.yml`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.7/.github/workflows/test.yml` & `docstring_auditor-0.1.8/.github/workflows/test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
         python-version: ['3.10']
+    env:
+      OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
@@ -38,8 +40,11 @@
     - name: Run tests
       run: hatch run dev:tests
 
     - name: Run type checking
       run: hatch run dev:lint-types
 
     - name: Run format checking
-      run: hatch run dev:lint-format
+      run: hatch run dev:lint-format
+
+    - name: Run self test
+      run: hatch run docstring-auditor
```

### Comparing `docstring_auditor-0.1.7/docstring_auditor/main.py` & `docstring_auditor-0.1.8/docstring_auditor/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import os
+import sys
 import click
 import ast
 import json
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Tuple
 import openai
 
 
 def extract_functions(file_path: str) -> List[Optional[str]]:
     """
     Extract functions from a Python file.
 
@@ -19,15 +20,15 @@
     Parameters
     ----------
     file_path : str
         The path to the .py file to extract functions from.
 
     Returns
     -------
-    List[str]
+    List[Optional[str]]
         A list of strings, where each string contains the entire code for a
         function, including the definition, docstring, and code.
 
     Examples
     --------
     >>> file_path = 'path/to/your/python_file.py'
     >>> functions = extract_functions(file_path)
@@ -49,38 +50,41 @@
         for func in tree.body
         if isinstance(func, ast.FunctionDef)
     ]
 
     return functions
 
 
-def ask_for_critique(function: str) -> Dict[str, str]:
+def ask_for_critique(function: str, model: str) -> Dict[str, str]:
     """
     Query OpenAI for a critique of the docstring for a function.
 
     Parameters
     ----------
     function : str
         A string containing the code and the docstring for the Python function.
         The input should be formatted as a single string, with the code and docstring combined.
+    model : str
+        The name of the OpenAI model to use for the query.
 
     Returns
     -------
-    response_dict : dict
+    response_dict : Dict[str, str]
         A dictionary containing the analysis of the docstring, including function name, errors, warnings, and the corrected docstring if needed.
     """
 
     DESIRED_DOCSTRING_STYLE = "numpydoc"
 
     PROMPT_SYSTEM = (
         "You are a coding assistant. "
         "You are detail orientated and precise. "
         "You have extensive knowledge of all coding languages and packages."
         "You will review the documentation for python functions that I provide."
         "The documentation you are helping to write is written for someone with very little coding experience."
+        "Do not provide errors or warnings about imports."
         "Please provide verbose descriptions and ensure no assumptions are made in the documentation."
     )
 
     PROMPT_QUERY = (
         "In the next message, I will provide you with the code for a Python function. "
         f"This will include the docstrings, which should be in the {DESIRED_DOCSTRING_STYLE} style.\n\n"
         "Does the docstring for the function describe the functionality provided by the code? "
@@ -104,153 +108,207 @@
         {
             "role": "assistant",
             "content": "Please provide the code for the Python function and its docstring so I can analyze it for you.",
         },
         {"role": "user", "content": function},
     ]
     response = openai.ChatCompletion.create(
-        model="gpt-4", temperature=0.1, messages=messages
+        model=model, temperature=0.0, messages=messages
     )
 
     response_str = response["choices"][0]["message"]["content"]
     response_dict = json.loads(response_str)
 
     return response_dict
 
 
-def report_concerns(response_dict: Dict[str, str]) -> bool:
+def report_concerns(response_dict: Dict[str, str]) -> Tuple[int, int]:
     """
     Inform the user of any concerns with the docstring.
 
     Parameters
     ----------
-    response_dict : dict
+    response_dict : Dict[str, str]
         A dictionary containing the function name, error, warning, and solution.
 
     Returns
     -------
-    bool
-        Returns True if there are any concerns (errors or warnings), otherwise returns False.
+    Tuple[int, int]
+        Returns a tuple containing the count of errors and warnings found in the docstring.
     """
     function_name = response_dict["function"]
     error = response_dict["error"]
     warning = response_dict["warning"]
     solution = response_dict["solution"]
 
+    error_count = 0
+    warning_count = 0
+
     if not error and not warning:
         click.secho(
             f"No concerns found with the docstring for the function: {function_name}\n",
             fg="green",
         )
-        return False
     else:
         if error:
             click.secho(
                 f"An error was found in the function: {function_name}\n", fg="red"
             )
             click.secho(f"{error}\n", fg="red")
+            error_count += 1
         if warning:
             click.secho(
                 f"A warning was found in the function: {function_name}\n", fg="yellow"
             )
             click.secho(f"{warning}\n", fg="yellow")
+            warning_count += 1
         if solution:
             click.secho(f"A proposed solution to these concerns is:\n\n{solution}\n\n")
-        return True
+
+    return error_count, warning_count
 
 
-def process_file(file_path: str):
+def process_file(file_path: str, model: str) -> Tuple[int, int]:
     """
     Process a single Python file and analyze its functions' docstrings.
 
+    This function processes the given Python file, extracts the functions within it,
+    and analyzes their docstrings for errors and warnings.
+    It then returns the total number of errors and warnings found in the
+    docstrings of the functions in the given file.
+
     Parameters
     ----------
     file_path : str
         The path to the .py file to analyze the functions' docstrings.
+    model : str
+        The name of the OpenAI model to use for the analysis.
 
     Returns
     -------
-    None
-        The function does not return any value. It prints the critiques and suggestions for the docstrings in the given file.
+    Tuple[int, int]
+        A tuple containing the total number of errors and warnings found in the docstrings of the functions in the given file.
     """
     functions = extract_functions(file_path)
 
+    error_count = 0
+    warning_count = 0
+
     for idx, function in enumerate(functions):
         print(
             f"Processing function {idx + 1} of {len(functions)} in file {file_path}..."
         )
         assert isinstance(function, str)
-        critique = ask_for_critique(function)
-        report_concerns(critique)
+        critique = ask_for_critique(function, model)
+        errors, warnings = report_concerns(critique)
+        error_count += errors
+        warning_count += warnings
 
+    return error_count, warning_count
 
-def process_directory(directory_path: str, ignore_dirs: Optional[List[str]] = None):
+
+def process_directory(
+    directory_path: str, model: str, ignore_dirs: Optional[List[str]] = None
+) -> Tuple[int, int]:
     """
     Recursively process all .py files in a directory and its subdirectories, ignoring specified directories.
 
     Parameters
     ----------
     directory_path : str
         The path to the directory containing .py files to analyze the functions' docstrings.
-
+    model : str
+        The name of the OpenAI model to use for the docstring analysis.
     ignore_dirs : Optional[List[str]]
         A list of directory names to ignore while processing .py files. By default, it ignores the "tests" directory.
 
     Returns
     -------
-    None
-        The function does not return any value. It prints the critiques and suggestions for the docstrings in the .py files.
+    Tuple[int, int]
+        A tuple containing the total number of errors and warnings found in the docstrings of the .py files.
     """
     if ignore_dirs is None:
         ignore_dirs = ["tests"]
 
+    error_count = 0
+    warning_count = 0
+
     for root, dirs, files in os.walk(directory_path):
         dirs[:] = [d for d in dirs if d not in ignore_dirs]
 
         for file in files:
             if file.endswith(".py"):
                 file_path = os.path.join(root, file)
-                process_file(file_path)
+                errors, warnings = process_file(file_path, model)
+                error_count += errors
+                warning_count += warnings
+
+    return error_count, warning_count
 
 
 @click.command(name="DocstringAuditor")
 @click.argument("path", type=click.Path(exists=True, readable=True), default=__file__)
 @click.option(
     "--ignore-dirs",
     type=click.STRING,
     multiple=True,
     default=["tests"],
     help="A list of directory names to ignore while processing .py files. Separate multiple directories with a space.",
 )
-def docstring_auditor(path: str, ignore_dirs: List[str]):
+@click.option(
+    "--error-on-warnings",
+    is_flag=True,
+    default=False,
+    help="If true, warnings will be treated as errors and included in the exit code count.",
+)
+@click.option(
+    "--model",
+    type=click.STRING,
+    default="gpt-4",
+    help="The OpenAI model to use for docstring analysis. Default is 'gpt-4'.",
+)
+def docstring_auditor(path: str, ignore_dirs: List[str], error_on_warnings: bool, model: str):
     """
     Analyze Python functions' docstrings in a given file or directory and provide critiques and suggestions for improvement.
 
     This program reads a Python file or directory, extracts the functions and their docstrings,
     and then analyzes the docstrings for errors, warnings,
     and possible improvements. The critiques and suggestions are then displayed to the user.
 
     Parameters
     ----------
     path : str
         The path to the .py file or directory to analyze the functions' docstrings.
-
     ignore_dirs : List[str]
         A list of directory names to ignore while processing .py files.
+    error_on_warnings : bool
+        If true, warnings will be treated as errors and included in the exit code count.
+    model : str
+        The OpenAI model to use for docstring analysis. Default is 'gpt-4'.
 
     Returns
     -------
     None
         The function does not return any value. It prints the critiques and suggestions for the docstrings in the given file or directory.
     """
     if os.path.isfile(path):
-        process_file(path)
+        error_count, warning_count = process_file(path, model)
     elif os.path.isdir(path):
-        process_directory(path, ignore_dirs)
+        error_count, warning_count = process_directory(path, model, ignore_dirs)
     else:
-        click.secho(
-            "Invalid path. Please provide a valid file or directory path.", fg="red"
+        error_text = "Invalid path. Please provide a valid file or directory path."
+        click.secho(error_text, fg="red")
+        sys.exit(error_text)
+
+    if error_count > 0 or (error_on_warnings and warning_count > 0):
+        error_text = (
+            f"Auditor identified {error_count} errors and {warning_count} warnings."
         )
+        click.secho(error_text, fg="red")
+        sys.exit(error_count + (warning_count if error_on_warnings else 0))
+    else:
+        click.secho("No errors found.", fg="green")
+        sys.exit(0)
 
 
 if __name__ == "__main__":
     docstring_auditor()
```

### Comparing `docstring_auditor-0.1.7/tests/test_critique.py` & `docstring_auditor-0.1.8/tests/test_critique.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 def test_ask_for_critique(openai_mock):
     function = (
         "def test_function():\n"
         '    """This is a test function."""\n'
         "    return 'successful'\n"
     )
 
-    response_dict = ask_for_critique(function)
+    response_dict = ask_for_critique(function, model="gpt-4")
     assert response_dict["function"].startswith("test_function_")
 
     current_test_id = (
         openai_mock.param.__name__
     )  # Access the current mock function's name
     if "no_errors_warnings" in current_test_id:
         assert response_dict["error"] == ""
```

### Comparing `docstring_auditor-0.1.7/tests/test_extractor.py` & `docstring_auditor-0.1.8/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.7/tests/test_reporter.py` & `docstring_auditor-0.1.8/tests/test_reporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     response_dict = {
         "function": "test_function",
         "error": "",
         "warning": "",
         "solution": "",
     }
     result = report_concerns(response_dict)
-    assert result is False
+    assert result == (0, 0)
     assert len(captured_output) == 1
     assert "No concerns found" in captured_output[0]
 
 
 def test_report_concerns_error_only(monkeypatch):
     captured_output = []
 
@@ -34,15 +34,15 @@
     response_dict = {
         "function": "test_function",
         "error": "An error occurred.",
         "warning": "",
         "solution": "Updated docstring.",
     }
     result = report_concerns(response_dict)
-    assert result is True
+    assert result == (1, 0)
     assert len(captured_output) == 3
     assert "An error was found" in captured_output[0]
     assert "An error occurred." in captured_output[1]
     assert "Updated docstring.\n\n" in captured_output[2]
 
 
 def test_report_concerns_warning_only(monkeypatch):
@@ -56,15 +56,15 @@
     response_dict = {
         "function": "test_function",
         "error": "",
         "warning": "A warning occurred.",
         "solution": "",
     }
     result = report_concerns(response_dict)
-    assert result is True
+    assert result == (0, 1)
     assert len(captured_output) == 2
     assert "A warning was found" in captured_output[0]
     assert "A warning occurred." in captured_output[1]
 
 
 def test_report_concerns_error_and_warning(monkeypatch):
     captured_output = []
@@ -78,14 +78,14 @@
         "function": "test_function",
         "error": "An error occurred.",
         "warning": "A warning occurred.",
         "solution": "Updated docstring.",
     }
     result = report_concerns(response_dict)
     print(captured_output)
-    assert result is True
+    assert result == (1, 1)
     assert len(captured_output) == 5
     assert "An error was found" in captured_output[0]
     assert "An error occurred." in captured_output[1]
     assert "A warning was found" in captured_output[2]
     assert "A warning occurred." in captured_output[3]
     assert "Updated docstring.\n\n" in captured_output[4]
```

### Comparing `docstring_auditor-0.1.7/.gitignore` & `docstring_auditor-0.1.8/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -159,8 +159,9 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 .python-version
 
 package-lock.json
 package.json
-
+***.draft
+***.DS_Store
```

### Comparing `docstring_auditor-0.1.7/LICENSE` & `docstring_auditor-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring_auditor-0.1.7/README.md` & `docstring_auditor-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Docstring Auditor
 
+[![PyPI version](https://badge.fury.io/py/docstring-auditor.svg)](https://badge.fury.io/py/docstring-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
 [![tests](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml)
-[![Release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
+[![release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
+
 
 Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation.
 Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings,
 ensuring they align with your code's true purpose. Accessible to both experts and novices,
 Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings.
 Say hello to better code documentation!
```

### Comparing `docstring_auditor-0.1.7/pyproject.toml` & `docstring_auditor-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "docstring-auditor"
-version = "0.1.7"
+version = "0.1.8"
 authors = [{name = "Rob Luke", email = "rob.luke@ae.studio"}]
 description = "A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement"
 readme = "README.md"
 keywords = ["docstring", "auditor", "openai", "gpt"]
 url = "https://github.com/agencyenterprise/docstring-auditor"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `docstring_auditor-0.1.7/PKG-INFO` & `docstring_auditor-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstring-auditor
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool to analyze Python functions' docstrings and provide critiques and suggestions for improvement
 Author-email: Rob Luke <rob.luke@ae.studio>
 License-File: LICENSE
 Keywords: auditor,docstring,gpt,openai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Docstring Auditor
 
+[![PyPI version](https://badge.fury.io/py/docstring-auditor.svg)](https://badge.fury.io/py/docstring-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docstring-auditor)
 [![tests](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/test.yml)
-[![Release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
+[![release](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml/badge.svg)](https://github.com/agencyenterprise/docstring-auditor/actions/workflows/release.yml)
+
 
 Meet _Docstring Auditor_, your go-to solution for maintaining precise and up-to-date Python code documentation.
 Tired of misleading or outdated docstrings? Docstring Auditor harnesses the power of large language models to analyze and critique your docstrings,
 ensuring they align with your code's true purpose. Accessible to both experts and novices,
 Docstring Auditor is your ultimate companion for clear, concise, and informative docstrings.
 Say hello to better code documentation!
```

