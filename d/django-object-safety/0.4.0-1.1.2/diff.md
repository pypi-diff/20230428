# Comparing `tmp/django_object_safety-0.4.0.tar.gz` & `tmp/django_object_safety-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-0.4.0.tar", max compression
+gzip compressed data, was "django_object_safety-1.1.2.tar", max compression
```

## Comparing `django_object_safety-0.4.0.tar` & `django_object_safety-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/LICENSE
--rw-r--r--   0        0        0      129 2023-04-28 19:59:26.762471 django_object_safety-0.4.0/README.md
--rw-r--r--   0        0        0      687 2023-04-28 20:01:00.526700 django_object_safety-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.4.0/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/models.py
--rw-r--r--   0        0        0    17385 2023-04-28 19:59:47.702527 django_object_safety-0.4.0/safety/shortcuts.py
--rw-r--r--   0        0        0     9475 2023-04-28 19:59:48.890530 django_object_safety-0.4.0/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/views.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 django_object_safety-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-28 21:32:04.641638 django_object_safety-1.1.2/README.md
+-rw-r--r--   0        0        0      698 2023-04-28 21:32:25.073621 django_object_safety-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.1.2/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.2/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.1.2/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.1.2/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-1.1.2/safety/models.py
+-rw-r--r--   0        0        0    18141 2023-04-28 21:32:07.033636 django_object_safety-1.1.2/safety/shortcuts.py
+-rw-r--r--   0        0        0     9846 2023-04-28 21:32:07.033636 django_object_safety-1.1.2/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.2/safety/views.py
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 django_object_safety-1.1.2/PKG-INFO
```

### Comparing `django_object_safety-0.4.0/LICENSE` & `django_object_safety-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/pyproject.toml` & `django_object_safety-1.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "0.4.0"
+version = "1.1.2"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
-homepage = "https://django-object-safety-docs.readthedocs.io/"
+homepage = "https://django-object-safety-docs.readthedocs.io/en/latest/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
 packages = [{ include = "safety" }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = ">3.7"
-django = ">3.2"
+python = "^3.10"
+django = "^4.2"
 
 [tool.poetry.group.dev.dependencies]
 build = "^0.10.0"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `django_object_safety-0.4.0/safety/migrations/0001_initial.py` & `django_object_safety-1.1.2/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-1.1.2/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-1.1.2/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-1.1.2/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-1.1.2/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/safety/models.py` & `django_object_safety-1.1.2/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.4.0/safety/shortcuts.py` & `django_object_safety-1.1.2/safety/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -360,14 +360,37 @@
                                                                   object_id=obj.id,
                                                                   to_ct=ContentType.objects.get_for_model(Group),
                                                                   ).distinct()
 
     return [perm.to for perm in permissions]
 
 
+def get_objects_for_entity(entity: get_user_model() | Group, permissions: list[str] | str, ct: ContentType) -> \
+        list[any]:
+    """
+    Get all objects that the user has the specified permissions on.
+    Args:
+        entity: The user that has access to the objects.
+        permissions (list[str]): The permissions required.
+        ct (ContentType): The content type of the objects.
+    """
+
+    if not isinstance(permissions, list):
+        permissions = [permissions]
+
+    perms = get_object_permission_model().objects.filter(
+        to_ct=ContentType.objects.get_for_model(entity),
+        to_id=entity.id,
+        permission__codename__in=permissions,
+        permission__content_type=ct,
+    )
+
+    return [perm.object for perm in perms]
+
+
 def retrieve_object_group(name: str, obj) -> ObjectGroup:
     """
     Get an object group.
 
     Args:
         name (string): The name of the group.
         obj: The object to get the group from.
```

### Comparing `django_object_safety-0.4.0/safety/tests.py` & `django_object_safety-1.1.2/safety/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.test import TransactionTestCase
 from django_fake_model import models as f
 
 from safety.shortcuts import set_perm, has_perm, lift_perm, create_object_group, delete_object_group, \
     add_user_to_object_group, remove_user_from_object_group, get_users_with_perms, get_groups_with_perms, \
-    retrieve_object_group
+    retrieve_object_group, get_objects_for_entity
 
 
 class FakePost(f.FakeModel):
     title = models.CharField(max_length=100)
     content = models.TextField()
 
     class Meta:
@@ -136,14 +136,22 @@
         set_perm(self.groups[0], "view_fakepost", content_type=self.fake_post_ct)
         set_perm(self.groups[1], "view_fakepost", content_type=self.fake_post_ct)
 
         self.assertListEqual(
             get_groups_with_perms("view_fakepost", content_type=self.fake_post_ct),
             [self.groups[0], self.groups[1]])
 
+    def test_get_objects_for_entity(self):
+        set_perm(self.users[0], "view_fakepost", self.posts[0])
+        set_perm(self.users[0], "view_fakepost", self.posts[1])
+
+        self.assertQuerySetEqual(
+            get_objects_for_entity(self.users[0], "view_fakepost", ct=ContentType.objects.get_for_model(FakePost)),
+            self.posts)
+
 
 @FakePost.fake_me
 class TestObjectGroup(TransactionTestCase):
     def setUp(self):
         self.users = []
         self.users.append(get_user_model().objects.create_user(username="TestUser", password="TestPassword"))
         self.users.append(get_user_model().objects.create_user(username="TestUser2", password="TestPassword"))
```

### Comparing `django_object_safety-0.4.0/PKG-INFO` & `django_object_safety-1.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 0.4.0
+Version: 1.1.2
 Summary: Adds object permissions to Django.
-Home-page: https://django-object-safety-docs.readthedocs.io/
+Home-page: https://django-object-safety-docs.readthedocs.io/en/latest/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
-Requires-Python: >3.7
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>3.2)
+Requires-Dist: django (>=4.2,<5.0)
 Project-URL: Repository, https://github.com/williammferreira/django-object-safety/
 Description-Content-Type: text/markdown
 
 ## Implements object permissions and groups in django
 
 View the documentation at http://django-object-safety-docs.readthedocs.io/
```

