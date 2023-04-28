# Comparing `tmp/django_object_safety-0.3.1.tar.gz` & `tmp/django_object_safety-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-0.3.1.tar", max compression
+gzip compressed data, was "django_object_safety-0.4.0.tar", max compression
```

## Comparing `django_object_safety-0.3.1.tar` & `django_object_safety-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/LICENSE
--rw-r--r--   0        0        0      129 2023-04-22 18:09:42.813595 django_object_safety-0.3.1/README.md
--rw-r--r--   0        0        0      687 2023-04-23 18:56:13.893644 django_object_safety-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.3.1/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.3.1/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.3.1/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.3.1/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.3.1/safety/models.py
--rw-r--r--   0        0        0    12348 2023-04-23 15:01:19.966432 django_object_safety-0.3.1/safety/shortcuts.py
--rw-r--r--   0        0        0     6153 2023-04-23 14:45:56.136510 django_object_safety-0.3.1/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.3.1/safety/views.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 django_object_safety-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-28 19:59:26.762471 django_object_safety-0.4.0/README.md
+-rw-r--r--   0        0        0      687 2023-04-28 20:01:00.526700 django_object_safety-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.4.0/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.4.0/safety/models.py
+-rw-r--r--   0        0        0    17385 2023-04-28 19:59:47.702527 django_object_safety-0.4.0/safety/shortcuts.py
+-rw-r--r--   0        0        0     9475 2023-04-28 19:59:48.890530 django_object_safety-0.4.0/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.4.0/safety/views.py
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 django_object_safety-0.4.0/PKG-INFO
```

### Comparing `django_object_safety-0.3.1/LICENSE` & `django_object_safety-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/pyproject.toml` & `django_object_safety-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "0.3.1"
+version = "0.4.0"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
```

### Comparing `django_object_safety-0.3.1/safety/migrations/0001_initial.py` & `django_object_safety-0.4.0/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-0.4.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-0.4.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-0.4.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-0.4.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/safety/models.py` & `django_object_safety-0.4.0/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.3.1/safety/shortcuts.py` & `django_object_safety-0.4.0/safety/shortcuts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import itertools
+from functools import reduce
+from operator import concat
+
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Permission, Group
 from django.contrib.contenttypes.models import ContentType
 
 from safety.models import ObjectPermission, ObjectGroup
 
@@ -152,17 +156,22 @@
 
     if obj is None:
         if content_type is None:
             raise ValueError("Content type must be provided if obj is None.")
 
         permission = Permission.objects.get(codename=perm, content_type=content_type)
 
-        entity.user_permissions.add(
-            permission
-        )
+        if isinstance(entity, get_user_model()):
+            entity.user_permissions.add(
+                permission
+            )
+        elif isinstance(entity, Group):
+            entity.permissions.add(
+                permission
+            )
         return True
 
     permission = Permission.objects.get(codename=perm, content_type=ContentType.objects.get_for_model(obj))
 
     if isinstance(entity, get_user_model()):
         get_object_permission_model(obj).objects.get_or_create(permission=permission, to_id=entity.id,
                                                                to_ct=ContentType.objects.get_for_model(entity),
@@ -220,14 +229,145 @@
     if not group_obj_perm.exists():
         return False
 
     group_obj_perm.delete()
     return True
 
 
+def get_perms(entity, obj=None) -> list[str]:
+    """
+    Get the permissions for a user or group.
+
+    Args:
+        entity: The user or group to get the permissions for.
+        obj: The object to get the permissions on.
+    """
+
+    if obj is None:
+        return [perm.codename for perm in
+                (entity.user_permissions.all() if isinstance(entity, get_user_model()) else entity.permissions.all())]
+
+    return [perm.permission.codename for perm in get_object_permission_model(obj).objects.filter(
+        to_id=entity.id,
+        to_ct=ContentType.objects.get_for_model(entity),
+        object_id=obj.id,
+        object_ct=ContentType.objects.get_for_model(obj)
+    )]
+
+
+def get_gross_perms(entity, obj=None) -> list[str]:
+    """
+    Get the permissions for a user or group, including permissions from groups.
+
+    Args:
+        entity: The user or group to get the permissions for.
+        obj: The object to get the permissions on.
+    """
+
+    if obj is None:
+        return get_perms(entity) + list(
+            reduce(concat,
+                   [[permission.codename for permission in group.permissions] for group in entity.groups]
+                   )
+        )
+
+    return get_perms(entity, obj) + [perm.permission.codename for perm in get_object_group_model(obj).objects.filter(
+        users__in=[entity],
+        object=obj,
+    )]
+
+
+def get_users_with_perms(perms, obj=None, content_type=None, with_group_users=True) -> \
+        list[get_user_model()]:
+    """
+    Get all users that have the specified permission(s).
+
+    Args:
+        perms: A list of permissions to check.
+        obj: The object to check the permissions on.
+        with_group_users: Include users in groups that have the permission in the result.
+        content_type (ContentType): The ContentType of the object.
+
+    Returns:
+        list[User]: A list of users that have the permission.
+    """
+
+    if not isinstance(perms, list):
+        perms = [perms]
+
+    if obj is None:
+        if content_type is None:
+            raise ValueError("Content type must be provided if obj is None.")
+
+        permissions = get_user_model().objects.filter(
+            user_permissions__codename__in=perms,
+            user_permissions__content_type=content_type,
+        ).distinct()
+
+        if with_group_users:
+            permissions = list(permissions) + list(get_user_model().objects.filter(
+                groups__permissions__codename__in=perms,
+                groups__permissions__content_type=content_type,
+            ).distinct())
+
+        return permissions
+
+    permissions = get_object_permission_model(obj).objects.filter(
+        permission__codename__in=perms,
+    )
+
+    users = list(
+        [permission.to for permission in permissions.filter(to_ct=ContentType.objects.get_for_model(get_user_model()))]
+    )
+
+    if with_group_users:
+        if obj is None:
+            groups = Group.objects.filter(groups__permissions__codename__in=perms)
+        else:
+            groups = get_object_group_model(obj).objects.filter(permissions__codename__in=perms, target_id=obj.id,
+                                                                target_ct=ContentType.objects.get_for_model(obj))
+        users += itertools.chain(*[list(group.users.all()) for group in groups])
+
+    return users
+
+
+def get_groups_with_perms(perms: list[str] | str, content_type: ContentType, obj=None) -> list[Group]:
+    """
+    Get all groups that have the specified permission(s).
+
+    Args:
+        perms (list[str] | str): Permission string(s) to check.
+        content_type (ContentType): The content type of the model that holds the permissions.
+        obj: The object, if checking for object permissions.
+
+    Returns:
+        list[Group]: A list of groups that have the permission.
+    """
+
+    if not isinstance(perms, list):
+        perms = [perms]
+
+    if obj is None and content_type is None:
+        raise ValueError("Content type must be provided if obj is None.")
+
+    if obj is None:
+        return list(Group.objects.filter(permissions__codename__in=perms, permissions__content_type=content_type))
+
+    ct = content_type if content_type else ContentType.objects.get_for_model(obj)
+
+    permissions = get_object_permission_model(obj).objects.filter(permission__codename__in=perms,
+                                                                  permission__content_type=ct,
+                                                                  object_ct=ct,
+                                                                  object_id=obj.id,
+                                                                  to_ct=ContentType.objects.get_for_model(Group),
+                                                                  ).distinct()
+
+    return [perm.to for perm in permissions]
+
+
 def retrieve_object_group(name: str, obj) -> ObjectGroup:
     """
     Get an object group.
 
     Args:
         name (string): The name of the group.
         obj: The object to get the group from.
```

### Comparing `django_object_safety-0.3.1/safety/tests.py` & `django_object_safety-0.4.0/safety/tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from django.contrib.auth.models import Group, Permission
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.test import TransactionTestCase
 from django_fake_model import models as f
 
 from safety.shortcuts import set_perm, has_perm, lift_perm, create_object_group, delete_object_group, \
-    add_user_to_object_group, remove_user_from_object_group
+    add_user_to_object_group, remove_user_from_object_group, get_users_with_perms, get_groups_with_perms, \
+    retrieve_object_group
 
 
 class FakePost(f.FakeModel):
     title = models.CharField(max_length=100)
     content = models.TextField()
 
     class Meta:
@@ -84,59 +85,126 @@
     def test_lift_permission(self):
         set_perm(self.users[0], "view_fakepost", self.posts[0])
 
         lift_perm(self.users[0], "view_fakepost", self.posts[0])
 
         self.assertFalse(has_perm([self.users[0]], "view_fakepost", self.posts[0]))
 
+    def test_get_users_with_perms(self):
+        set_perm(self.users[0], "view_fakepost", self.posts[0])
+        set_perm(self.users[1], "view_fakepost", self.posts[0])
+
+        self.assertQuerySetEqual(get_users_with_perms("view_fakepost", self.posts[0]), [self.users[0], self.users[1]])
+
+    def test_get_users_with_perms_global(self):
+        set_perm(self.users[0], "view_fakepost", content_type=self.fake_post_ct)
+        set_perm(self.users[1], "view_fakepost", content_type=self.fake_post_ct)
+
+        self.assertListEqual(get_users_with_perms("view_fakepost", content_type=self.fake_post_ct),
+                             [self.users[0], self.users[1]])
+
+    def test_get_users_with_group_perms(self):
+        create_object_group("editors", ["view_fakepost"], self.posts[0])
+        add_user_to_object_group(self.users[0], "editors", self.posts[0])
+
+        self.assertListEqual(get_users_with_perms("view_fakepost", self.posts[0], with_group_users=True),
+                             [self.users[0]])
+
+    def test_get_users_with_group_perms_global(self):
+        group = Group.objects.create(name="editors")
+        group.permissions.add(Permission.objects.get(codename="view_fakepost", content_type=self.fake_post_ct))
+        self.users[0].groups.add(group)
+        self.users[1].groups.add(group)
+
+        self.assertListEqual(get_users_with_perms("view_fakepost", content_type=self.fake_post_ct,
+                                                  with_group_users=True), [self.users[0], self.users[1]])
+
+    def test_get_users_with_group_perms_global_with_group_users(self):
+        create_object_group("editors", ["view_fakepost"], self.posts[0])
+        add_user_to_object_group(self.users[0], "editors", self.posts[0])
+
+        self.assertListEqual(get_users_with_perms("view_fakepost", self.posts[0], with_group_users=True),
+                             [self.users[0]])
+
+    def test_get_groups_with_perms(self):
+        set_perm(self.groups[0], "view_fakepost", self.posts[0])
+        set_perm(self.groups[1], "view_fakepost", self.posts[0])
+
+        self.assertListEqual(get_groups_with_perms("view_fakepost", self.fake_post_ct, self.posts[0]),
+                             [self.groups[0], self.groups[1]])
+
+    def test_get_groups_with_perms_global(self):
+        set_perm(self.groups[0], "view_fakepost", content_type=self.fake_post_ct)
+        set_perm(self.groups[1], "view_fakepost", content_type=self.fake_post_ct)
+
+        self.assertListEqual(
+            get_groups_with_perms("view_fakepost", content_type=self.fake_post_ct),
+            [self.groups[0], self.groups[1]])
+
 
 @FakePost.fake_me
-class TestPermissionGroup(TransactionTestCase):
+class TestObjectGroup(TransactionTestCase):
     def setUp(self):
         self.users = []
         self.users.append(get_user_model().objects.create_user(username="TestUser", password="TestPassword"))
         self.users.append(get_user_model().objects.create_user(username="TestUser2", password="TestPassword"))
 
         self.posts = []
         self.posts.append(FakePost.objects.create(title="TestPost", content="TestContent"))
         self.posts.append(FakePost.objects.create(title="TestPost2", content="TestContent2"))
 
         FakePost.set_django_objects()
 
         self.fake_post_ct = ContentType.objects.get_for_model(FakePost)
 
-    def test_create_permission_group(self):
+    def test_create_object_group(self):
         create_object_group("editors",
                             ["view_fakepost", "change_fakepost", "delete_fakepost"],
                             self.posts[0])
         add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
         self.assertTrue(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
 
-    def test_delete_permission_group(self):
+    def test_delete_object_group(self):
         create_object_group("editors",
                             ["view_fakepost", "change_fakepost", "delete_fakepost"],
                             self.posts[0])
 
         delete_object_group("editors", self.posts[0])
 
         self.assertFalse(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
 
-    def test_remove_user_from_permission_group(self):
+    def test_retrieve_object_group(self):
+        create_object_group("editors",
+                            ["view_fakepost", "change_fakepost", "delete_fakepost"],
+                            self.posts[0])
+
+        self.assertTrue(retrieve_object_group("editors", self.posts[0]))
+
+    def test_add_user_to_object_group(self):
+        create_object_group("editors",
+                            ["view_fakepost", "change_fakepost", "delete_fakepost"],
+                            self.posts[0])
+
+        add_user_to_object_group(self.users[0], "editors", self.posts[0])
+
+        self.assertTrue(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
+
+    def test_remove_user_from_object_group(self):
         create_object_group("editors",
                             ["view_fakepost", "change_fakepost", "delete_fakepost"],
                             self.posts[0])
 
         add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
         remove_user_from_object_group(self.users[0], "editors", self.posts[0])
 
         self.assertFalse(has_perm([self.users[0]], "change_fakepost", self.posts[0]))
 
-    def test_remove_permission_on_delete(self):
+    def test_remove_object_group_on_delete(self):
         create_object_group("editors",
                             ["view_fakepost", "change_fakepost", "delete_fakepost"],
                             self.posts[0])
 
         add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
         post = self.posts[0]
```

### Comparing `django_object_safety-0.3.1/PKG-INFO` & `django_object_safety-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 0.3.1
+Version: 0.4.0
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >3.7
 Classifier: License :: OSI Approved :: MIT License
```

