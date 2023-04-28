# Comparing `tmp/assignment-manager-0.1.4.tar.gz` & `tmp/assignment-manager-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assignment-manager-0.1.4.tar", last modified: Thu Apr 27 05:46:31 2023, max compression
+gzip compressed data, was "assignment-manager-0.1.5.tar", last modified: Fri Apr 28 16:05:10 2023, max compression
```

## Comparing `assignment-manager-0.1.4.tar` & `assignment-manager-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.4/LICENSE
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.4/README.md
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.4/pyproject.toml
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/setup.cfg
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-27 05:45:44.000000 assignment-manager-0.1.4/setup.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/src/
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/src/assignment_manager/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.4/src/assignment_manager/__init__.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     3954 2023-04-26 20:45:44.000000 assignment-manager-0.1.4/src/assignment_manager/assignments.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1811 2023-04-25 18:23:27.000000 assignment-manager-0.1.4/src/assignment_manager/data.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2440 2023-04-26 20:40:11.000000 assignment-manager-0.1.4/src/assignment_manager/io.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      989 2023-04-25 18:44:19.000000 assignment-manager-0.1.4/src/assignment_manager/main.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-27 05:46:31.018197 assignment-manager-0.1.4/src/assignment_manager.egg-info/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/entry_points.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/requires.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-27 05:46:31.000000 assignment-manager-0.1.4/src/assignment_manager.egg-info/top_level.txt
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.749641 assignment-manager-0.1.5/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.5/LICENSE
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-28 16:05:10.749641 assignment-manager-0.1.5/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.5/README.md
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      129 2023-04-26 20:40:07.000000 assignment-manager-0.1.5/pyproject.toml
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-28 16:05:10.749641 assignment-manager-0.1.5/setup.cfg
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-28 16:04:47.000000 assignment-manager-0.1.5/setup.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.745641 assignment-manager-0.1.5/src/
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.745641 assignment-manager-0.1.5/src/assignment_manager/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.5/src/assignment_manager/__init__.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     5177 2023-04-28 16:03:33.000000 assignment-manager-0.1.5/src/assignment_manager/assignments.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1817 2023-04-28 15:55:50.000000 assignment-manager-0.1.5/src/assignment_manager/data.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2461 2023-04-28 09:11:02.000000 assignment-manager-0.1.5/src/assignment_manager/io.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1013 2023-04-28 09:09:32.000000 assignment-manager-0.1.5/src/assignment_manager/main.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-28 16:05:10.745641 assignment-manager-0.1.5/src/assignment_manager.egg-info/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/requires.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-28 16:05:10.000000 assignment-manager-0.1.5/src/assignment_manager.egg-info/top_level.txt
```

### Comparing `assignment-manager-0.1.4/LICENSE` & `assignment-manager-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.4/PKG-INFO` & `assignment-manager-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.4
+Version: 0.1.5
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `assignment-manager-0.1.4/setup.py` & `assignment-manager-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="assignment-manager",
-    version="0.1.4",
+    version="0.1.5",
     description=("Manage reoccuring assignments and tasks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PraxTube/assignment-manager",
     author="Prax",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `assignment-manager-0.1.4/src/assignment_manager/assignments.py` & `assignment-manager-0.1.5/src/assignment_manager/assignments.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,41 +16,77 @@
     current_date = datetime.today()
     for i, d in enumerate(assignment_data):
         if datetime.strptime(d[1], "%d.%m.%Y") >= current_date:
             return i
     return len(assignment_data) - 1
 
 
-def show_all_assignments():
+def sort_data(row_data, sort_index, ascending=True):
+    if sort_index < 0 or sort_index >= len(row_data):
+        raise ValueError(
+            "The given index must be in range of the row_data",
+            sort_index,
+            row_data,
+        )
+
+    row_data.sort(key=lambda x: x[sort_index], reverse=not ascending)
+
+
+def get_table_rows():
     data = load_data()
-    table_headers = ["Name", "Start", "Deadline", "Progress"]
     table_rows = []
     for key in data:
         cycle = _find_next_deadline(data[key])
-        deadline = "{} ({})".format(
-            data[key][cycle][1],
-            (
-                datetime.strptime(data[key][cycle][1], "%d.%m.%Y")
-                - datetime.today()
-            ).days,
-        )
+        remaing_days = (
+            datetime.strptime(data[key][cycle][1], "%d.%m.%Y")
+            - datetime.today()
+        ).days
         table_rows.append(
             [
                 key,
-                data[key][cycle][0],
-                deadline,
-                Progress(data[key][cycle][2]).name,
+                datetime.strptime(data[key][cycle][0], "%d.%m.%Y"),
+                datetime.strptime(data[key][cycle][1], "%d.%m.%Y"),
+                Progress(data[key][cycle][2]),
+                remaing_days,
             ]
         )
+    return table_rows
+
+
+def show_all_assignments(sort):
+    table_headers = ["Name", "Start", "Deadline", "Progress", "Days"]
+    table_rows = get_table_rows()
+
+    if sort:
+        sort_index = table_headers.index(
+            io.list_prompt(table_headers, "Which to sort by?")
+        )
+        ascending = io.binary_prompt("Sort ascending?")
+    else:
+        sort_index = 4
+        ascending = True
+
+    table_headers[sort_index] += " ▼" if ascending else " ▲"
+    sort_data(table_rows, sort_index, ascending)
+
+    for i in range(len(table_rows)):
+        table_rows[i] = [
+            table_rows[i][0],
+            table_rows[i][1].strftime("%d.%m.%Y"),
+            table_rows[i][2].strftime("%d.%m.%Y"),
+            table_rows[i][3].name,
+            str(table_rows[i][4]),
+        ]
+
     io.print_table(table_headers, table_rows)
 
 
 def show_specific_assignment():
     data = load_data()
-    name = io.course_response(data.keys())
+    name = io.list_prompt(data.keys(), "Which course do you want to update?")
 
     table_headers = ["Start", "Deadline", "Progress"]
     table_rows = []
     for data_entry in data[name]:
         table_rows.append(
             [data_entry[0], data_entry[1], Progress(data_entry[2]).name]
         )
@@ -85,41 +121,43 @@
     progress = generate_dates(params[1], params[2], params[3], params[4])
     data[params[0]] = progress
     write_data(data)
 
 
 def update_assignment():
     data = load_data()
-    name = io.course_response(data.keys())
+    name = io.list_prompt(data.keys(), "Which course do you want to update?")
 
     cycle_choices = [d for d in data[name]]
     progress_choices = [p.name for p in Progress]
     cycle, progress = io.update_assignment_response(
         cycle_choices, progress_choices
     )
 
     data[name][cycle][2] = progress
     write_data(data)
 
 
 def rename_assignment():
     data = load_data()
-    old_name = io.course_response(data.keys())
+    old_name = io.list_prompt(
+        data.keys(), "Which course do you want to update?"
+    )
     new_name = io.rename_assignment_response()
 
     if new_name in data:
         raise ValueError("The name already exists!", new_name, data.keys())
 
     data[new_name] = data.pop(old_name)
     write_data(data)
 
 
 def remove_assignment():
     data = load_data()
-    name = io.course_response(data.keys())
+    name = io.list_prompt(data.keys(), "Which course do you want to update?")
 
     confirmation_msg = (
         "This will delete [bold]ALL[/bold] data for "
         "the course: [bold]{}[/bold]\n".format(name)
     )
 
     if not io.confirmation_prompt(confirmation_msg):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `assignment-manager-0.1.4/src/assignment_manager/data.py` & `assignment-manager-0.1.5/src/assignment_manager/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 from pathlib import Path
 import json
-from enum import Enum
+from enum import IntEnum
 
 
-class Progress(Enum):
+class Progress(IntEnum):
     NOT_STARTED = 0
     JUST_STARTED = 1
     IN_PROGRESS = 2
     ALMOST_DONE = 3
     DONE = 4
```

### Comparing `assignment-manager-0.1.4/src/assignment_manager/io.py` & `assignment-manager-0.1.5/src/assignment_manager/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,15 @@
     print(table)
 
 
 def confirmation_prompt(msg=""):
     if msg != "":
         print(msg)
 
-    question = [
-        inquirer.List(
-            "confirmation",
-            message="Are you sure you want to continue?",
-            choices=["Yes", "No"],
-        )
-    ]
-    if inquirer.prompt(question)["confirmation"] == "Yes":
+    if binary_prompt("Are you sure you want to continue?"):
         return True
     print("[bold]Aborting...[/bold]")
     return False
 
 
 def add_assignment_response():
     questions = [
@@ -50,23 +43,36 @@
         answers["start_date"],
         answers["end_date"],
         int(answers["torus"]),
         int(answers["amount"]),
     )
 
 
-def course_response(course_choices):
-    question_course = [
+def binary_prompt(msg):
+    question = [
+        inquirer.List(
+            "answer",
+            message=msg,
+            choices=["Yes", "No"],
+        )
+    ]
+    if inquirer.prompt(question)["answer"] == "Yes":
+        return True
+    return False
+
+
+def list_prompt(choices, msg):
+    question = [
         inquirer.List(
-            "name",
-            message="Which course do you want to update?",
-            choices=course_choices,
+            "answer",
+            message=msg,
+            choices=choices,
         ),
     ]
-    return inquirer.prompt(question_course)["name"]
+    return inquirer.prompt(question)["answer"]
 
 
 def update_assignment_response(cycle_choices, progress_choices):
     questions = [
         inquirer.List(
             "cycle",
             message="Which cycle do you want to update?",
```

### Comparing `assignment-manager-0.1.4/src/assignment_manager/main.py` & `assignment-manager-0.1.5/src/assignment_manager/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 @app.command()
 def add():
     assignments.add_assignment()
 
 
 @app.command()
-def show(one: bool = False):
+def show(one: bool = False, sort: bool = False):
     if one:
         assignments.show_specific_assignment()
     else:
-        assignments.show_all_assignments()
+        assignments.show_all_assignments(sort)
 
 
 @app.command()
 def update():
     assignments.update_assignment()
```

### Comparing `assignment-manager-0.1.4/src/assignment_manager.egg-info/PKG-INFO` & `assignment-manager-0.1.5/src/assignment_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.4
+Version: 0.1.5
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

