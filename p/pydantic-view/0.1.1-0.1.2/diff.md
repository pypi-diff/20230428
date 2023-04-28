# Comparing `tmp/pydantic_view-0.1.1.tar.gz` & `tmp/pydantic_view-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.1.1.tar", max compression
+gzip compressed data, was "pydantic_view-0.1.2.tar", max compression
```

## Comparing `pydantic_view-0.1.1.tar` & `pydantic_view-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.1.1/LICENSE
--rw-r--r--   0        0        0     5299 2023-04-22 18:45:42.000000 pydantic_view-0.1.1/README.md
--rw-r--r--   0        0        0      126 2023-04-22 18:42:38.000000 pydantic_view-0.1.1/pydantic_view/__init__.py
--rw-r--r--   0        0        0     2995 2023-04-22 18:26:01.000000 pydantic_view-0.1.1/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      872 2023-04-22 18:42:38.000000 pydantic_view-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6219 1970-01-01 00:00:00.000000 pydantic_view-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5625 2023-04-28 19:14:58.000000 pydantic_view-0.1.2/README.md
+-rw-r--r--   0        0        0      142 2023-04-28 16:02:37.000000 pydantic_view-0.1.2/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     4842 2023-04-28 19:02:19.000000 pydantic_view-0.1.2/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      872 2023-04-28 19:19:55.000000 pydantic_view-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 pydantic_view-0.1.2/PKG-INFO
```

### Comparing `pydantic_view-0.1.1/LICENSE` & `pydantic_view-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.1.1/README.md` & `pydantic_view-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -26,52 +26,63 @@
    ...:     password: str
    ...:     address: str
    ...: 
 
 In [2]: user = User(id=0, username="human", password="iamaman", address="Earth")
    ...: user.Out()
    ...: 
-Out[2]: Out(id=0, username='human', address='Earth')
+Out[2]: UserOut(id=0, username='human', address='Earth')
 
 In [3]: User.Update(id=0, username="human", password="iamasuperman", address="Earth")
    ...: 
-Out[3]: Update(id=0, username='human', password='iamasuperman', address='Earth')
+Out[3]: UserUpdate(id=0, username='human', password='iamasuperman', address='Earth')
 
 In [4]: User.Patch(id=0, address="Mars")
    ...: 
-Out[4]: Patch(id=0, username=None, password=None, address='Mars')
+Out[4]: UserPatch(id=0, username=None, password=None, address='Mars')
 ```
 
 
 ### FastAPI example
 
 ```python
 from typing import List
 
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 from pydantic import BaseModel, Field
 
-from pydantic_view import view
+from pydantic_view import view, view_validator
 
 
 @view("Out", exclude=["secret"])
-@view("Create", exclude=["id"])
+@view("Create", exclude=["id"], config={"extra": "forbid"})
 @view("Update", exclude=["id"])
 @view("UpdateMany")
 @view("Patch", exclude=["id"], optional=["name", "secret"])
 @view("PatchMany", optional=["name", "secret"])
 class Group(BaseModel):
     id: int
     name: str
     secret: str = None
 
+    @view_validator(["Create", "Update", "UpdateMany", "Patch", "PatchMany"], "name", allow_reuse=True)
+    def validate_name(cls, v):
+        if v == "admin":
+            raise ValueError("Invalid name")
+        return v
+
 
 @view("Out", exclude=["password"], recursive=True)
-@view("Create", exclude=["id"], optional_ex={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])})
+@view(
+    "Create",
+    exclude=["id"],
+    optional_ex={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
+    config={"extra": "forbid"},
+)
 @view("Update", exclude=["id"])
 @view("UpdateMany")
 @view("Patch", exclude=["id"], optional=["username", "password", "groups"])
 @view("PatchMany", optional=["username", "password", "groups"])
 class User(BaseModel):
     id: int
     username: str
```

### Comparing `pydantic_view-0.1.1/pyproject.toml` & `pydantic_view-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.1.1"
+version = "0.1.2"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.1.1/PKG-INFO` & `pydantic_view-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.1.1
+Version: 0.1.2
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -50,52 +50,63 @@
    ...:     password: str
    ...:     address: str
    ...: 
 
 In [2]: user = User(id=0, username="human", password="iamaman", address="Earth")
    ...: user.Out()
    ...: 
-Out[2]: Out(id=0, username='human', address='Earth')
+Out[2]: UserOut(id=0, username='human', address='Earth')
 
 In [3]: User.Update(id=0, username="human", password="iamasuperman", address="Earth")
    ...: 
-Out[3]: Update(id=0, username='human', password='iamasuperman', address='Earth')
+Out[3]: UserUpdate(id=0, username='human', password='iamasuperman', address='Earth')
 
 In [4]: User.Patch(id=0, address="Mars")
    ...: 
-Out[4]: Patch(id=0, username=None, password=None, address='Mars')
+Out[4]: UserPatch(id=0, username=None, password=None, address='Mars')
 ```
 
 
 ### FastAPI example
 
 ```python
 from typing import List
 
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 from pydantic import BaseModel, Field
 
-from pydantic_view import view
+from pydantic_view import view, view_validator
 
 
 @view("Out", exclude=["secret"])
-@view("Create", exclude=["id"])
+@view("Create", exclude=["id"], config={"extra": "forbid"})
 @view("Update", exclude=["id"])
 @view("UpdateMany")
 @view("Patch", exclude=["id"], optional=["name", "secret"])
 @view("PatchMany", optional=["name", "secret"])
 class Group(BaseModel):
     id: int
     name: str
     secret: str = None
 
+    @view_validator(["Create", "Update", "UpdateMany", "Patch", "PatchMany"], "name", allow_reuse=True)
+    def validate_name(cls, v):
+        if v == "admin":
+            raise ValueError("Invalid name")
+        return v
+
 
 @view("Out", exclude=["password"], recursive=True)
-@view("Create", exclude=["id"], optional_ex={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])})
+@view(
+    "Create",
+    exclude=["id"],
+    optional_ex={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
+    config={"extra": "forbid"},
+)
 @view("Update", exclude=["id"])
 @view("UpdateMany")
 @view("Patch", exclude=["id"], optional=["username", "password", "groups"])
 @view("PatchMany", optional=["username", "password", "groups"])
 class User(BaseModel):
     id: int
     username: str
```

