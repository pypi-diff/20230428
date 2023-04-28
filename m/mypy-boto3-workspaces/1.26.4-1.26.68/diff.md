# Comparing `tmp/mypy-boto3-workspaces-1.26.4.tar.gz` & `tmp/mypy-boto3-workspaces-1.26.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.26.4.tar", last modified: Mon Nov  7 20:50:37 2022, max compression
+gzip compressed data, was "mypy-boto3-workspaces-1.26.68.tar", last modified: Thu Feb  9 20:26:51 2023, max compression
```

## Comparing `mypy-boto3-workspaces-1.26.4.tar` & `mypy-boto3-workspaces-1.26.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-workspaces-1.26.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21423 2022-11-07 20:50:37.092346 mypy-boto3-workspaces-1.26.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19976 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46561 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    46483 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12007 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12005 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10740 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10730 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    50313 2022-11-07 20:50:26.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    50276 2022-11-07 20:50:26.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21423 2022-11-07 20:50:36.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-07 20:50:36.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:36.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-07 20:50:36.000000 mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:37.092346 mypy-boto3-workspaces-1.26.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-11-07 20:50:25.000000 mypy-boto3-workspaces-1.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22019 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48049 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47969 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-02-09 20:26:38.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53904 2023-02-09 20:26:40.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53863 2023-02-09 20:26:39.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22019 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 20:26:51.000000 mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:51.606842 mypy-boto3-workspaces-1.26.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-09 20:26:37.000000 mypy-boto3-workspaces-1.26.68/setup.py
```

### Comparing `mypy-boto3-workspaces-1.26.4/LICENSE` & `mypy-boto3-workspaces-1.26.68/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.4/PKG-INFO` & `mypy-boto3-workspaces-1.26.68/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.26.4
-Summary: Type annotations for boto3.WorkSpaces 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.68
+Summary: Type annotations for boto3.WorkSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,21 +329,24 @@
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_workspaces.literals import (
     AccessPropertyValueType,
     ApplicationType,
     AssociationStatusType,
+    BundleTypeType,
+    CertificateBasedAuthStatusEnumType,
     ClientDeviceTypeType,
     ComputeType,
     ConnectionAliasStateType,
     ConnectionStateType,
     DedicatedTenancyModificationStateEnumType,
     DedicatedTenancySupportEnumType,
     DedicatedTenancySupportResultEnumType,
+    DeletableCertificateBasedAuthPropertyType,
     DeletableSamlPropertyType,
     DescribeAccountModificationsPaginatorName,
     DescribeIpGroupsPaginatorName,
     DescribeWorkspaceBundlesPaginatorName,
     DescribeWorkspaceDirectoriesPaginatorName,
     DescribeWorkspaceImagesPaginatorName,
     DescribeWorkspacesConnectionStatusPaginatorName,
@@ -353,16 +357,18 @@
     ModificationResourceEnumType,
     ModificationStateEnumType,
     OperatingSystemTypeType,
     ProtocolType,
     ReconnectEnumType,
     RunningModeType,
     SamlStatusEnumType,
+    StandbyWorkspaceRelationshipTypeType,
     TargetWorkspaceStateType,
     TenancyType,
+    WorkspaceBundleStateType,
     WorkspaceDirectoryStateType,
     WorkspaceDirectoryTypeType,
     WorkspaceImageIngestionProcessType,
     WorkspaceImageRequiredTenancyType,
     WorkspaceImageStateType,
     WorkspaceStateType,
     WorkSpacesServiceName,
@@ -387,21 +393,23 @@
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
+    PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
@@ -444,14 +452,15 @@
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
+    RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
@@ -467,14 +476,15 @@
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
     WorkspacesIpGroupTypeDef,
+    ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
@@ -482,14 +492,15 @@
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
     DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
+    StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
     WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
@@ -511,31 +522,34 @@
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
     WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
-    WorkspaceTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
+    WorkspaceTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
     DescribeIpGroupsResultTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
+    CreateStandbyWorkspacesRequestRequestTypeDef,
+    FailedCreateStandbyWorkspacesRequestTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
     CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
     DescribeWorkspaceImagesResultTypeDef,
+    CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
 
 
 def get_structure() -> AccountModificationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workspaces-1.26.4/README.md` & `mypy-boto3-workspaces-1.26.68/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,21 +297,24 @@
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_workspaces.literals import (
     AccessPropertyValueType,
     ApplicationType,
     AssociationStatusType,
+    BundleTypeType,
+    CertificateBasedAuthStatusEnumType,
     ClientDeviceTypeType,
     ComputeType,
     ConnectionAliasStateType,
     ConnectionStateType,
     DedicatedTenancyModificationStateEnumType,
     DedicatedTenancySupportEnumType,
     DedicatedTenancySupportResultEnumType,
+    DeletableCertificateBasedAuthPropertyType,
     DeletableSamlPropertyType,
     DescribeAccountModificationsPaginatorName,
     DescribeIpGroupsPaginatorName,
     DescribeWorkspaceBundlesPaginatorName,
     DescribeWorkspaceDirectoriesPaginatorName,
     DescribeWorkspaceImagesPaginatorName,
     DescribeWorkspacesConnectionStatusPaginatorName,
@@ -322,16 +325,18 @@
     ModificationResourceEnumType,
     ModificationStateEnumType,
     OperatingSystemTypeType,
     ProtocolType,
     ReconnectEnumType,
     RunningModeType,
     SamlStatusEnumType,
+    StandbyWorkspaceRelationshipTypeType,
     TargetWorkspaceStateType,
     TenancyType,
+    WorkspaceBundleStateType,
     WorkspaceDirectoryStateType,
     WorkspaceDirectoryTypeType,
     WorkspaceImageIngestionProcessType,
     WorkspaceImageRequiredTenancyType,
     WorkspaceImageStateType,
     WorkspaceStateType,
     WorkSpacesServiceName,
@@ -356,21 +361,23 @@
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
+    PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
@@ -413,14 +420,15 @@
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
+    RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
@@ -436,14 +444,15 @@
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
     WorkspacesIpGroupTypeDef,
+    ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
@@ -451,14 +460,15 @@
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
     DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
+    StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
     WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
@@ -480,31 +490,34 @@
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
     WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
-    WorkspaceTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
+    WorkspaceTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
     DescribeIpGroupsResultTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
+    CreateStandbyWorkspacesRequestRequestTypeDef,
+    FailedCreateStandbyWorkspacesRequestTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
     CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
     DescribeWorkspaceImagesResultTypeDef,
+    CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
 
 
 def get_structure() -> AccountModificationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/__init__.py` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/__init__.pyi` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/__main__.py` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpaces 1.26.4\nVersion:         1.26.4\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.WorkSpaces 1.26.68\nVersion:         1.26.68\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.4")
+    print("1.26.68")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/client.py` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     DescribeWorkspaceImagesPaginator,
     DescribeWorkspacesConnectionStatusPaginator,
     DescribeWorkspacesPaginator,
     ListAvailableManagementCidrRangesPaginator,
 )
 from .type_defs import (
     AssociateConnectionAliasResultTypeDef,
+    CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectionAliasPermissionTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
+    CreateStandbyWorkspacesResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     CreateWorkspaceImageResultTypeDef,
     CreateWorkspacesResultTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
@@ -76,14 +78,15 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
+    StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
@@ -238,14 +241,24 @@
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_ip_group)
         """
 
+    def create_standby_workspaces(
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
+    ) -> CreateStandbyWorkspacesResultTypeDef:
+        """
+        Creates a standby WorkSpace in a secondary Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_standby_workspaces)
+        """
+
     def create_tags(self, *, ResourceId: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Creates the specified tags for the specified WorkSpaces resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_tags)
         """
@@ -600,16 +613,16 @@
         IngestionProcess: WorkspaceImageIngestionProcessType,
         ImageName: str,
         ImageDescription: str,
         Tags: Sequence[TagTypeDef] = ...,
         Applications: Sequence[ApplicationType] = ...
     ) -> ImportWorkspaceImageResultTypeDef:
         """
-        Imports the specified Windows 10 Bring Your Own License (BYOL) or Windows Server
-        2016 BYOL image into Amazon WorkSpaces.
+        Imports the specified Windows 10 Bring Your Own License (BYOL) image into Amazon
+        WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#import_workspace_image)
         """
 
     def list_available_management_cidr_ranges(
         self, *, ManagementCidrRangeConstraint: str, MaxResults: int = ..., NextToken: str = ...
@@ -644,14 +657,31 @@
         Modifies the configuration of Bring Your Own License (BYOL) for the specified
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_account)
         """
 
+    def modify_certificate_based_auth_properties(
+        self,
+        *,
+        ResourceId: str,
+        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
+        PropertiesToDelete: Sequence[
+            Literal["CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"]
+        ] = ...
+    ) -> Dict[str, Any]:
+        """
+        Modifies the properties of the certificate-based authentication you want to use
+        with your WorkSpaces.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_certificate_based_auth_properties)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_certificate_based_auth_properties)
+        """
+
     def modify_client_properties(
         self, *, ResourceId: str, ClientProperties: ClientPropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the properties of the specified Amazon WorkSpaces clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_client_properties)
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/client.pyi` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     DescribeWorkspaceImagesPaginator,
     DescribeWorkspacesConnectionStatusPaginator,
     DescribeWorkspacesPaginator,
     ListAvailableManagementCidrRangesPaginator,
 )
 from .type_defs import (
     AssociateConnectionAliasResultTypeDef,
+    CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectionAliasPermissionTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
+    CreateStandbyWorkspacesResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     CreateWorkspaceImageResultTypeDef,
     CreateWorkspacesResultTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
@@ -76,14 +78,15 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
+    StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
@@ -224,14 +227,23 @@
     ) -> CreateIpGroupResultTypeDef:
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_ip_group)
         """
+    def create_standby_workspaces(
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
+    ) -> CreateStandbyWorkspacesResultTypeDef:
+        """
+        Creates a standby WorkSpace in a secondary Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_standby_workspaces)
+        """
     def create_tags(self, *, ResourceId: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Creates the specified tags for the specified WorkSpaces resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_tags)
         """
@@ -553,16 +565,16 @@
         IngestionProcess: WorkspaceImageIngestionProcessType,
         ImageName: str,
         ImageDescription: str,
         Tags: Sequence[TagTypeDef] = ...,
         Applications: Sequence[ApplicationType] = ...
     ) -> ImportWorkspaceImageResultTypeDef:
         """
-        Imports the specified Windows 10 Bring Your Own License (BYOL) or Windows Server
-        2016 BYOL image into Amazon WorkSpaces.
+        Imports the specified Windows 10 Bring Your Own License (BYOL) image into Amazon
+        WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.import_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#import_workspace_image)
         """
     def list_available_management_cidr_ranges(
         self, *, ManagementCidrRangeConstraint: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAvailableManagementCidrRangesResultTypeDef:
@@ -593,14 +605,30 @@
         """
         Modifies the configuration of Bring Your Own License (BYOL) for the specified
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_account)
         """
+    def modify_certificate_based_auth_properties(
+        self,
+        *,
+        ResourceId: str,
+        CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,
+        PropertiesToDelete: Sequence[
+            Literal["CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"]
+        ] = ...
+    ) -> Dict[str, Any]:
+        """
+        Modifies the properties of the certificate-based authentication you want to use
+        with your WorkSpaces.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_certificate_based_auth_properties)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_certificate_based_auth_properties)
+        """
     def modify_client_properties(
         self, *, ResourceId: str, ClientProperties: ClientPropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the properties of the specified Amazon WorkSpaces clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_client_properties)
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/literals.py` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,24 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccessPropertyValueType",
     "ApplicationType",
     "AssociationStatusType",
+    "BundleTypeType",
+    "CertificateBasedAuthStatusEnumType",
     "ClientDeviceTypeType",
     "ComputeType",
     "ConnectionAliasStateType",
     "ConnectionStateType",
     "DedicatedTenancyModificationStateEnumType",
     "DedicatedTenancySupportEnumType",
     "DedicatedTenancySupportResultEnumType",
+    "DeletableCertificateBasedAuthPropertyType",
     "DeletableSamlPropertyType",
     "DescribeAccountModificationsPaginatorName",
     "DescribeIpGroupsPaginatorName",
     "DescribeWorkspaceBundlesPaginatorName",
     "DescribeWorkspaceDirectoriesPaginatorName",
     "DescribeWorkspaceImagesPaginatorName",
     "DescribeWorkspacesConnectionStatusPaginatorName",
@@ -44,16 +47,18 @@
     "ModificationResourceEnumType",
     "ModificationStateEnumType",
     "OperatingSystemTypeType",
     "ProtocolType",
     "ReconnectEnumType",
     "RunningModeType",
     "SamlStatusEnumType",
+    "StandbyWorkspaceRelationshipTypeType",
     "TargetWorkspaceStateType",
     "TenancyType",
+    "WorkspaceBundleStateType",
     "WorkspaceDirectoryStateType",
     "WorkspaceDirectoryTypeType",
     "WorkspaceImageIngestionProcessType",
     "WorkspaceImageRequiredTenancyType",
     "WorkspaceImageStateType",
     "WorkspaceStateType",
     "WorkSpacesServiceName",
@@ -69,14 +74,16 @@
 AssociationStatusType = Literal[
     "ASSOCIATED_WITH_OWNER_ACCOUNT",
     "ASSOCIATED_WITH_SHARED_ACCOUNT",
     "NOT_ASSOCIATED",
     "PENDING_ASSOCIATION",
     "PENDING_DISASSOCIATION",
 ]
+BundleTypeType = Literal["REGULAR", "STANDBY"]
+CertificateBasedAuthStatusEnumType = Literal["DISABLED", "ENABLED"]
 ClientDeviceTypeType = Literal[
     "DeviceTypeAndroid",
     "DeviceTypeIos",
     "DeviceTypeLinux",
     "DeviceTypeOsx",
     "DeviceTypeWeb",
     "DeviceTypeWindows",
@@ -93,14 +100,17 @@
     "VALUE",
 ]
 ConnectionAliasStateType = Literal["CREATED", "CREATING", "DELETING"]
 ConnectionStateType = Literal["CONNECTED", "DISCONNECTED", "UNKNOWN"]
 DedicatedTenancyModificationStateEnumType = Literal["COMPLETED", "FAILED", "PENDING"]
 DedicatedTenancySupportEnumType = Literal["ENABLED"]
 DedicatedTenancySupportResultEnumType = Literal["DISABLED", "ENABLED"]
+DeletableCertificateBasedAuthPropertyType = Literal[
+    "CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"
+]
 DeletableSamlPropertyType = Literal[
     "SAML_PROPERTIES_RELAY_STATE_PARAMETER_NAME", "SAML_PROPERTIES_USER_ACCESS_URL"
 ]
 DescribeAccountModificationsPaginatorName = Literal["describe_account_modifications"]
 DescribeIpGroupsPaginatorName = Literal["describe_ip_groups"]
 DescribeWorkspaceBundlesPaginatorName = Literal["describe_workspace_bundles"]
 DescribeWorkspaceDirectoriesPaginatorName = Literal["describe_workspace_directories"]
@@ -113,16 +123,18 @@
 ModificationResourceEnumType = Literal["COMPUTE_TYPE", "ROOT_VOLUME", "USER_VOLUME"]
 ModificationStateEnumType = Literal["UPDATE_INITIATED", "UPDATE_IN_PROGRESS"]
 OperatingSystemTypeType = Literal["LINUX", "WINDOWS"]
 ProtocolType = Literal["PCOIP", "WSP"]
 ReconnectEnumType = Literal["DISABLED", "ENABLED"]
 RunningModeType = Literal["ALWAYS_ON", "AUTO_STOP", "MANUAL"]
 SamlStatusEnumType = Literal["DISABLED", "ENABLED", "ENABLED_WITH_DIRECTORY_LOGIN_FALLBACK"]
+StandbyWorkspaceRelationshipTypeType = Literal["PRIMARY", "STANDBY"]
 TargetWorkspaceStateType = Literal["ADMIN_MAINTENANCE", "AVAILABLE"]
 TenancyType = Literal["DEDICATED", "SHARED"]
+WorkspaceBundleStateType = Literal["AVAILABLE", "ERROR", "PENDING"]
 WorkspaceDirectoryStateType = Literal[
     "DEREGISTERED", "DEREGISTERING", "ERROR", "REGISTERED", "REGISTERING"
 ]
 WorkspaceDirectoryTypeType = Literal["AD_CONNECTOR", "SIMPLE_AD"]
 WorkspaceImageIngestionProcessType = Literal[
     "BYOL_GRAPHICS",
     "BYOL_GRAPHICSPRO",
@@ -174,14 +186,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -191,27 +204,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -240,14 +257,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -295,14 +313,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -313,30 +332,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -368,28 +390,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -398,14 +424,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -416,38 +443,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/literals.pyi` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,24 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccessPropertyValueType",
     "ApplicationType",
     "AssociationStatusType",
+    "BundleTypeType",
+    "CertificateBasedAuthStatusEnumType",
     "ClientDeviceTypeType",
     "ComputeType",
     "ConnectionAliasStateType",
     "ConnectionStateType",
     "DedicatedTenancyModificationStateEnumType",
     "DedicatedTenancySupportEnumType",
     "DedicatedTenancySupportResultEnumType",
+    "DeletableCertificateBasedAuthPropertyType",
     "DeletableSamlPropertyType",
     "DescribeAccountModificationsPaginatorName",
     "DescribeIpGroupsPaginatorName",
     "DescribeWorkspaceBundlesPaginatorName",
     "DescribeWorkspaceDirectoriesPaginatorName",
     "DescribeWorkspaceImagesPaginatorName",
     "DescribeWorkspacesConnectionStatusPaginatorName",
@@ -43,16 +46,18 @@
     "ModificationResourceEnumType",
     "ModificationStateEnumType",
     "OperatingSystemTypeType",
     "ProtocolType",
     "ReconnectEnumType",
     "RunningModeType",
     "SamlStatusEnumType",
+    "StandbyWorkspaceRelationshipTypeType",
     "TargetWorkspaceStateType",
     "TenancyType",
+    "WorkspaceBundleStateType",
     "WorkspaceDirectoryStateType",
     "WorkspaceDirectoryTypeType",
     "WorkspaceImageIngestionProcessType",
     "WorkspaceImageRequiredTenancyType",
     "WorkspaceImageStateType",
     "WorkspaceStateType",
     "WorkSpacesServiceName",
@@ -67,14 +72,16 @@
 AssociationStatusType = Literal[
     "ASSOCIATED_WITH_OWNER_ACCOUNT",
     "ASSOCIATED_WITH_SHARED_ACCOUNT",
     "NOT_ASSOCIATED",
     "PENDING_ASSOCIATION",
     "PENDING_DISASSOCIATION",
 ]
+BundleTypeType = Literal["REGULAR", "STANDBY"]
+CertificateBasedAuthStatusEnumType = Literal["DISABLED", "ENABLED"]
 ClientDeviceTypeType = Literal[
     "DeviceTypeAndroid",
     "DeviceTypeIos",
     "DeviceTypeLinux",
     "DeviceTypeOsx",
     "DeviceTypeWeb",
     "DeviceTypeWindows",
@@ -91,14 +98,17 @@
     "VALUE",
 ]
 ConnectionAliasStateType = Literal["CREATED", "CREATING", "DELETING"]
 ConnectionStateType = Literal["CONNECTED", "DISCONNECTED", "UNKNOWN"]
 DedicatedTenancyModificationStateEnumType = Literal["COMPLETED", "FAILED", "PENDING"]
 DedicatedTenancySupportEnumType = Literal["ENABLED"]
 DedicatedTenancySupportResultEnumType = Literal["DISABLED", "ENABLED"]
+DeletableCertificateBasedAuthPropertyType = Literal[
+    "CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"
+]
 DeletableSamlPropertyType = Literal[
     "SAML_PROPERTIES_RELAY_STATE_PARAMETER_NAME", "SAML_PROPERTIES_USER_ACCESS_URL"
 ]
 DescribeAccountModificationsPaginatorName = Literal["describe_account_modifications"]
 DescribeIpGroupsPaginatorName = Literal["describe_ip_groups"]
 DescribeWorkspaceBundlesPaginatorName = Literal["describe_workspace_bundles"]
 DescribeWorkspaceDirectoriesPaginatorName = Literal["describe_workspace_directories"]
@@ -111,16 +121,18 @@
 ModificationResourceEnumType = Literal["COMPUTE_TYPE", "ROOT_VOLUME", "USER_VOLUME"]
 ModificationStateEnumType = Literal["UPDATE_INITIATED", "UPDATE_IN_PROGRESS"]
 OperatingSystemTypeType = Literal["LINUX", "WINDOWS"]
 ProtocolType = Literal["PCOIP", "WSP"]
 ReconnectEnumType = Literal["DISABLED", "ENABLED"]
 RunningModeType = Literal["ALWAYS_ON", "AUTO_STOP", "MANUAL"]
 SamlStatusEnumType = Literal["DISABLED", "ENABLED", "ENABLED_WITH_DIRECTORY_LOGIN_FALLBACK"]
+StandbyWorkspaceRelationshipTypeType = Literal["PRIMARY", "STANDBY"]
 TargetWorkspaceStateType = Literal["ADMIN_MAINTENANCE", "AVAILABLE"]
 TenancyType = Literal["DEDICATED", "SHARED"]
+WorkspaceBundleStateType = Literal["AVAILABLE", "ERROR", "PENDING"]
 WorkspaceDirectoryStateType = Literal[
     "DEREGISTERED", "DEREGISTERING", "ERROR", "REGISTERED", "REGISTERING"
 ]
 WorkspaceDirectoryTypeType = Literal["AD_CONNECTOR", "SIMPLE_AD"]
 WorkspaceImageIngestionProcessType = Literal[
     "BYOL_GRAPHICS",
     "BYOL_GRAPHICSPRO",
@@ -172,14 +184,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -189,27 +202,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -238,14 +255,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -293,14 +311,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -311,30 +330,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -366,28 +388,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -396,14 +422,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -414,38 +441,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/paginator.py` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/paginator.pyi` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/type_defs.py` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AccessPropertyValueType,
     ApplicationType,
     AssociationStatusType,
+    BundleTypeType,
+    CertificateBasedAuthStatusEnumType,
     ClientDeviceTypeType,
     ComputeType,
     ConnectionAliasStateType,
     ConnectionStateType,
     DedicatedTenancyModificationStateEnumType,
     DedicatedTenancySupportResultEnumType,
     DeletableSamlPropertyType,
@@ -33,16 +35,18 @@
     ModificationResourceEnumType,
     ModificationStateEnumType,
     OperatingSystemTypeType,
     ProtocolType,
     ReconnectEnumType,
     RunningModeType,
     SamlStatusEnumType,
+    StandbyWorkspaceRelationshipTypeType,
     TargetWorkspaceStateType,
     TenancyType,
+    WorkspaceBundleStateType,
     WorkspaceDirectoryStateType,
     WorkspaceDirectoryTypeType,
     WorkspaceImageIngestionProcessType,
     WorkspaceImageRequiredTenancyType,
     WorkspaceImageStateType,
     WorkspaceStateType,
 )
@@ -59,21 +63,23 @@
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
+    "CertificateBasedAuthPropertiesTypeDef",
     "ClientPropertiesTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
+    "PendingCreateStandbyWorkspacesRequestTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
     "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
@@ -116,14 +122,15 @@
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
     "WorkspaceCreationPropertiesTypeDef",
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
+    "RelatedWorkspacePropertiesTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
@@ -139,14 +146,15 @@
     "DescribeAccountResultTypeDef",
     "ImportWorkspaceImageResultTypeDef",
     "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     "WorkspacesIpGroupTypeDef",
+    "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
@@ -154,14 +162,15 @@
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
     "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
+    "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
     "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
@@ -183,31 +192,34 @@
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
-    "WorkspaceTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
+    "WorkspaceTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
     "DescribeIpGroupsResultTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    "FailedCreateStandbyWorkspacesRequestTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
     "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
     "DescribeWorkspacesResultTypeDef",
     "DescribeWorkspaceImagesResultTypeDef",
+    "CreateStandbyWorkspacesResultTypeDef",
     "CreateWorkspacesResultTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
@@ -252,14 +264,23 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
+CertificateBasedAuthPropertiesTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+    total=False,
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
@@ -327,14 +348,25 @@
     {
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
 )
 
+PendingCreateStandbyWorkspacesRequestTypeDef = TypedDict(
+    "PendingCreateStandbyWorkspacesRequestTypeDef",
+    {
+        "UserName": str,
+        "DirectoryId": str,
+        "State": WorkspaceStateType,
+        "WorkspaceId": str,
+    },
+    total=False,
+)
+
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
     total=False,
 )
@@ -851,14 +883,25 @@
 RebuildRequestTypeDef = TypedDict(
     "RebuildRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
+RelatedWorkspacePropertiesTypeDef = TypedDict(
+    "RelatedWorkspacePropertiesTypeDef",
+    {
+        "WorkspaceId": str,
+        "Region": str,
+        "State": WorkspaceStateType,
+        "Type": StandbyWorkspaceRelationshipTypeType,
+    },
+    total=False,
+)
+
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -1059,14 +1102,39 @@
         "groupName": str,
         "groupDesc": str,
         "userRules": List[IpRuleItemTypeDef],
     },
     total=False,
 )
 
+_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
+    "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
+    "_OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
+    {
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
+        "PropertiesToDelete": Sequence[
+            Literal["CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"]
+        ],
+    },
+    total=False,
+)
+
+
+class ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef(
+    _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
+    _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
+):
+    pass
+
+
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
     },
     total=False,
@@ -1301,14 +1369,35 @@
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredStandbyWorkspaceTypeDef = TypedDict(
+    "_RequiredStandbyWorkspaceTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "DirectoryId": str,
+    },
+)
+_OptionalStandbyWorkspaceTypeDef = TypedDict(
+    "_OptionalStandbyWorkspaceTypeDef",
+    {
+        "VolumeEncryptionKey": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class StandbyWorkspaceTypeDef(_RequiredStandbyWorkspaceTypeDef, _OptionalStandbyWorkspaceTypeDef):
+    pass
+
+
 _RequiredCreateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleName": str,
         "BundleDescription": str,
         "ImageId": str,
         "ComputeType": ComputeTypeTypeDef,
@@ -1341,14 +1430,16 @@
         "Description": str,
         "ImageId": str,
         "RootStorage": RootStorageTypeDef,
         "UserStorage": UserStorageTypeDef,
         "ComputeType": ComputeTypeTypeDef,
         "LastUpdatedTime": datetime,
         "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
     },
     total=False,
 )
 
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
@@ -1630,14 +1721,15 @@
         "State": WorkspaceDirectoryStateType,
         "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
         "ipGroupIds": List[str],
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
         "Tenancy": TenancyType,
         "SelfservicePermissions": SelfservicePermissionsTypeDef,
         "SamlProperties": SamlPropertiesTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
@@ -1675,14 +1767,28 @@
 )
 
 
 class WorkspaceRequestTypeDef(_RequiredWorkspaceRequestTypeDef, _OptionalWorkspaceRequestTypeDef):
     pass
 
 
+RebootWorkspacesRequestRequestTypeDef = TypedDict(
+    "RebootWorkspacesRequestRequestTypeDef",
+    {
+        "RebootWorkspaceRequests": Sequence[RebootRequestTypeDef],
+    },
+)
+
+RebuildWorkspacesRequestRequestTypeDef = TypedDict(
+    "RebuildWorkspacesRequestRequestTypeDef",
+    {
+        "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
+    },
+)
+
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1693,32 +1799,19 @@
         "ErrorCode": str,
         "ComputerName": str,
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
+        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
     total=False,
 )
 
-RebootWorkspacesRequestRequestTypeDef = TypedDict(
-    "RebootWorkspacesRequestRequestTypeDef",
-    {
-        "RebootWorkspaceRequests": Sequence[RebootRequestTypeDef],
-    },
-)
-
-RebuildWorkspacesRequestRequestTypeDef = TypedDict(
-    "RebuildWorkspacesRequestRequestTypeDef",
-    {
-        "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
-    },
-)
-
 StartWorkspacesRequestRequestTypeDef = TypedDict(
     "StartWorkspacesRequestRequestTypeDef",
     {
         "StartWorkspaceRequests": Sequence[StartRequestTypeDef],
     },
 )
 
@@ -1776,14 +1869,32 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
+FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
+    "FailedCreateStandbyWorkspacesRequestTypeDef",
+    {
+        "StandbyWorkspaceRequest": StandbyWorkspaceTypeDef,
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1837,14 +1948,23 @@
     {
         "Images": List[WorkspaceImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesResultTypeDef = TypedDict(
+    "CreateStandbyWorkspacesResultTypeDef",
+    {
+        "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
+        "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces/type_defs.pyi` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AccessPropertyValueType,
     ApplicationType,
     AssociationStatusType,
+    BundleTypeType,
+    CertificateBasedAuthStatusEnumType,
     ClientDeviceTypeType,
     ComputeType,
     ConnectionAliasStateType,
     ConnectionStateType,
     DedicatedTenancyModificationStateEnumType,
     DedicatedTenancySupportResultEnumType,
     DeletableSamlPropertyType,
@@ -33,16 +35,18 @@
     ModificationResourceEnumType,
     ModificationStateEnumType,
     OperatingSystemTypeType,
     ProtocolType,
     ReconnectEnumType,
     RunningModeType,
     SamlStatusEnumType,
+    StandbyWorkspaceRelationshipTypeType,
     TargetWorkspaceStateType,
     TenancyType,
+    WorkspaceBundleStateType,
     WorkspaceDirectoryStateType,
     WorkspaceDirectoryTypeType,
     WorkspaceImageIngestionProcessType,
     WorkspaceImageRequiredTenancyType,
     WorkspaceImageStateType,
     WorkspaceStateType,
 )
@@ -58,21 +62,23 @@
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
+    "CertificateBasedAuthPropertiesTypeDef",
     "ClientPropertiesTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
+    "PendingCreateStandbyWorkspacesRequestTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
     "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
@@ -115,14 +121,15 @@
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
     "WorkspaceCreationPropertiesTypeDef",
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
+    "RelatedWorkspacePropertiesTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
@@ -138,14 +145,15 @@
     "DescribeAccountResultTypeDef",
     "ImportWorkspaceImageResultTypeDef",
     "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     "WorkspacesIpGroupTypeDef",
+    "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
@@ -153,14 +161,15 @@
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
     "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
+    "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
     "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
@@ -182,31 +191,34 @@
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
-    "WorkspaceTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
+    "WorkspaceTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
     "DescribeIpGroupsResultTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    "FailedCreateStandbyWorkspacesRequestTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
     "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
     "DescribeWorkspacesResultTypeDef",
     "DescribeWorkspaceImagesResultTypeDef",
+    "CreateStandbyWorkspacesResultTypeDef",
     "CreateWorkspacesResultTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
@@ -251,14 +263,23 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
+CertificateBasedAuthPropertiesTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+    total=False,
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
@@ -324,14 +345,25 @@
     {
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
 )
 
+PendingCreateStandbyWorkspacesRequestTypeDef = TypedDict(
+    "PendingCreateStandbyWorkspacesRequestTypeDef",
+    {
+        "UserName": str,
+        "DirectoryId": str,
+        "State": WorkspaceStateType,
+        "WorkspaceId": str,
+    },
+    total=False,
+)
+
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
     total=False,
 )
@@ -840,14 +872,25 @@
 RebuildRequestTypeDef = TypedDict(
     "RebuildRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
+RelatedWorkspacePropertiesTypeDef = TypedDict(
+    "RelatedWorkspacePropertiesTypeDef",
+    {
+        "WorkspaceId": str,
+        "Region": str,
+        "State": WorkspaceStateType,
+        "Type": StandbyWorkspaceRelationshipTypeType,
+    },
+    total=False,
+)
+
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -1046,14 +1089,37 @@
         "groupName": str,
         "groupDesc": str,
         "userRules": List[IpRuleItemTypeDef],
     },
     total=False,
 )
 
+_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
+    "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
+    "_OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
+    {
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
+        "PropertiesToDelete": Sequence[
+            Literal["CERTIFICATE_BASED_AUTH_PROPERTIES_CERTIFICATE_AUTHORITY_ARN"]
+        ],
+    },
+    total=False,
+)
+
+class ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef(
+    _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
+    _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
+):
+    pass
+
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
     },
     total=False,
@@ -1274,14 +1340,33 @@
 
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
+_RequiredStandbyWorkspaceTypeDef = TypedDict(
+    "_RequiredStandbyWorkspaceTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "DirectoryId": str,
+    },
+)
+_OptionalStandbyWorkspaceTypeDef = TypedDict(
+    "_OptionalStandbyWorkspaceTypeDef",
+    {
+        "VolumeEncryptionKey": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class StandbyWorkspaceTypeDef(_RequiredStandbyWorkspaceTypeDef, _OptionalStandbyWorkspaceTypeDef):
+    pass
+
 _RequiredCreateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleName": str,
         "BundleDescription": str,
         "ImageId": str,
         "ComputeType": ComputeTypeTypeDef,
@@ -1312,14 +1397,16 @@
         "Description": str,
         "ImageId": str,
         "RootStorage": RootStorageTypeDef,
         "UserStorage": UserStorageTypeDef,
         "ComputeType": ComputeTypeTypeDef,
         "LastUpdatedTime": datetime,
         "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
     },
     total=False,
 )
 
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
@@ -1595,14 +1682,15 @@
         "State": WorkspaceDirectoryStateType,
         "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
         "ipGroupIds": List[str],
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
         "Tenancy": TenancyType,
         "SelfservicePermissions": SelfservicePermissionsTypeDef,
         "SamlProperties": SamlPropertiesTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
     },
     total=False,
 )
 
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
@@ -1638,14 +1726,28 @@
     },
     total=False,
 )
 
 class WorkspaceRequestTypeDef(_RequiredWorkspaceRequestTypeDef, _OptionalWorkspaceRequestTypeDef):
     pass
 
+RebootWorkspacesRequestRequestTypeDef = TypedDict(
+    "RebootWorkspacesRequestRequestTypeDef",
+    {
+        "RebootWorkspaceRequests": Sequence[RebootRequestTypeDef],
+    },
+)
+
+RebuildWorkspacesRequestRequestTypeDef = TypedDict(
+    "RebuildWorkspacesRequestRequestTypeDef",
+    {
+        "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
+    },
+)
+
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1656,32 +1758,19 @@
         "ErrorCode": str,
         "ComputerName": str,
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
+        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
     total=False,
 )
 
-RebootWorkspacesRequestRequestTypeDef = TypedDict(
-    "RebootWorkspacesRequestRequestTypeDef",
-    {
-        "RebootWorkspaceRequests": Sequence[RebootRequestTypeDef],
-    },
-)
-
-RebuildWorkspacesRequestRequestTypeDef = TypedDict(
-    "RebuildWorkspacesRequestRequestTypeDef",
-    {
-        "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
-    },
-)
-
 StartWorkspacesRequestRequestTypeDef = TypedDict(
     "StartWorkspacesRequestRequestTypeDef",
     {
         "StartWorkspaceRequests": Sequence[StartRequestTypeDef],
     },
 )
 
@@ -1739,14 +1828,32 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
+FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
+    "FailedCreateStandbyWorkspacesRequestTypeDef",
+    {
+        "StandbyWorkspaceRequest": StandbyWorkspaceTypeDef,
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1800,14 +1907,23 @@
     {
         "Images": List[WorkspaceImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesResultTypeDef = TypedDict(
+    "CreateStandbyWorkspacesResultTypeDef",
+    {
+        "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
+        "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/PKG-INFO` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.26.4
-Summary: Type annotations for boto3.WorkSpaces 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.68
+Summary: Type annotations for boto3.WorkSpaces 1.26.68 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,21 +329,24 @@
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_workspaces.literals import (
     AccessPropertyValueType,
     ApplicationType,
     AssociationStatusType,
+    BundleTypeType,
+    CertificateBasedAuthStatusEnumType,
     ClientDeviceTypeType,
     ComputeType,
     ConnectionAliasStateType,
     ConnectionStateType,
     DedicatedTenancyModificationStateEnumType,
     DedicatedTenancySupportEnumType,
     DedicatedTenancySupportResultEnumType,
+    DeletableCertificateBasedAuthPropertyType,
     DeletableSamlPropertyType,
     DescribeAccountModificationsPaginatorName,
     DescribeIpGroupsPaginatorName,
     DescribeWorkspaceBundlesPaginatorName,
     DescribeWorkspaceDirectoriesPaginatorName,
     DescribeWorkspaceImagesPaginatorName,
     DescribeWorkspacesConnectionStatusPaginatorName,
@@ -353,16 +357,18 @@
     ModificationResourceEnumType,
     ModificationStateEnumType,
     OperatingSystemTypeType,
     ProtocolType,
     ReconnectEnumType,
     RunningModeType,
     SamlStatusEnumType,
+    StandbyWorkspaceRelationshipTypeType,
     TargetWorkspaceStateType,
     TenancyType,
+    WorkspaceBundleStateType,
     WorkspaceDirectoryStateType,
     WorkspaceDirectoryTypeType,
     WorkspaceImageIngestionProcessType,
     WorkspaceImageRequiredTenancyType,
     WorkspaceImageStateType,
     WorkspaceStateType,
     WorkSpacesServiceName,
@@ -387,21 +393,23 @@
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesTypeDef,
     ClientPropertiesTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
+    PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
@@ -444,14 +452,15 @@
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
+    RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
@@ -467,14 +476,15 @@
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
     WorkspacesIpGroupTypeDef,
+    ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
@@ -482,14 +492,15 @@
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
     DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
+    StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
     WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
@@ -511,31 +522,34 @@
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
     WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
-    WorkspaceTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
+    WorkspaceTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
     DescribeIpGroupsResultTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
+    CreateStandbyWorkspacesRequestRequestTypeDef,
+    FailedCreateStandbyWorkspacesRequestTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
     CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
     DescribeWorkspaceImagesResultTypeDef,
+    CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
 
 
 def get_structure() -> AccountModificationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workspaces-1.26.4/mypy_boto3_workspaces.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-1.26.68/mypy_boto3_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.26.4/setup.py` & `mypy-boto3-workspaces-1.26.68/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-workspaces",
-    version="1.26.4",
+    version="1.26.68",
     packages=["mypy_boto3_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpaces 1.26.4 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.WorkSpaces 1.26.68 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 workspaces type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_workspaces": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_workspaces": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

