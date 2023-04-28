# Comparing `tmp/mypy-boto3-athena-1.26.4.tar.gz` & `tmp/mypy-boto3-athena-1.26.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-athena-1.26.4.tar", last modified: Mon Nov  7 20:50:35 2022, max compression
+gzip compressed data, was "mypy-boto3-athena-1.26.87.tar", last modified: Wed Mar  8 20:35:46 2023, max compression
```

## Comparing `mypy-boto3-athena-1.26.4.tar` & `mypy-boto3-athena-1.26.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.248330 mypy-boto3-athena-1.26.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17655 2022-11-07 20:50:35.244330 mypy-boto3-athena-1.26.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.244330 mypy-boto3-athena-1.26.4/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27814 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27763 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8815 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8255 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    37593 2022-11-07 20:48:59.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    37536 2022-11-07 20:48:59.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.244330 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17655 2022-11-07 20:50:35.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-07 20:50:35.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:35.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-07 20:50:35.000000 mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:35.248330 mypy-boto3-athena-1.26.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-11-07 20:48:58.000000 mypy-boto3-athena-1.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.194592 mypy-boto3-athena-1.26.87/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41676 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41602 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57696 2023-03-08 20:34:16.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57613 2023-03-08 20:34:15.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-08 20:35:46.000000 mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 20:35:46.198592 mypy-boto3-athena-1.26.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-08 20:34:14.000000 mypy-boto3-athena-1.26.87/setup.py
```

### Comparing `mypy-boto3-athena-1.26.4/LICENSE` & `mypy-boto3-athena-1.26.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.4/PKG-INFO` & `mypy-boto3-athena-1.26.87/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.26.4
-Summary: Type annotations for boto3.Athena 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.87
+Summary: Type annotations for boto3.Athena 1.26.87 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,147 +316,211 @@
 ### Literals
 
 `mypy_boto3_athena.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_athena.literals import (
+    CalculationExecutionStateType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
+    ExecutorStateType,
+    ExecutorTypeType,
     GetQueryResultsPaginatorName,
     ListDataCatalogsPaginatorName,
     ListDatabasesPaginatorName,
     ListNamedQueriesPaginatorName,
     ListQueryExecutionsPaginatorName,
     ListTableMetadataPaginatorName,
     ListTagsForResourcePaginatorName,
+    NotebookTypeType,
     QueryExecutionStateType,
     S3AclOptionType,
+    SessionStateType,
     StatementTypeType,
     WorkGroupStateType,
     AthenaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ColumnNullableType) -> bool:
+def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
+    ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
+    CalculationConfigurationTypeDef,
+    CalculationResultTypeDef,
+    CalculationStatisticsTypeDef,
+    CalculationStatusTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
+    CreateNotebookInputRequestTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
+    CreatePresignedNotebookUrlRequestRequestTypeDef,
+    CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
+    DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationTypeDef,
     EngineVersionTypeDef,
+    ExecutorsSummaryTypeDef,
+    ExportNotebookInputRequestTypeDef,
+    NotebookMetadataTypeDef,
+    FilterDefinitionTypeDef,
+    GetCalculationExecutionCodeRequestRequestTypeDef,
+    GetCalculationExecutionRequestRequestTypeDef,
+    GetCalculationExecutionStatusRequestRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
+    GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
     PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
+    GetSessionRequestRequestTypeDef,
+    SessionStatisticsTypeDef,
+    SessionStatusTypeDef,
+    GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
+    ImportNotebookInputRequestTypeDef,
+    ListApplicationDPUSizesInputRequestTypeDef,
+    ListCalculationExecutionsRequestRequestTypeDef,
     ListDataCatalogsInputRequestTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
+    ListExecutorsRequestRequestTypeDef,
     ListNamedQueriesInputRequestTypeDef,
+    ListNotebookSessionsRequestRequestTypeDef,
+    NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
+    ListSessionsRequestRequestTypeDef,
     ListTableMetadataInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
+    StopCalculationExecutionRequestRequestTypeDef,
     StopQueryExecutionInputRequestTypeDef,
+    TerminateSessionRequestRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
+    UpdateNotebookInputRequestTypeDef,
+    UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
     QueryExecutionStatusTypeDef,
     CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
     ListNamedQueriesOutputTypeDef,
     ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
+    StartCalculationExecutionRequestRequestTypeDef,
+    CalculationSummaryTypeDef,
+    GetCalculationExecutionResponseTypeDef,
+    GetCalculationExecutionStatusResponseTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
+    SessionConfigurationTypeDef,
+    StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
+    ListExecutorsResponseTypeDef,
+    ExportNotebookOutputTypeDef,
+    GetNotebookMetadataOutputTypeDef,
+    ListNotebookMetadataOutputTypeDef,
+    ListNotebookMetadataInputRequestTypeDef,
     GetQueryResultsInputGetQueryResultsPaginateTypeDef,
     ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDatabasesInputListDatabasesPaginateTypeDef,
     ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    GetSessionStatusResponseTypeDef,
+    SessionSummaryTypeDef,
+    ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
+    ListCalculationExecutionsResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
+    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
+    ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
     CreateWorkGroupInputRequestTypeDef,
     WorkGroupTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
```

### Comparing `mypy-boto3-athena-1.26.4/README.md` & `mypy-boto3-athena-1.26.87/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,147 +284,211 @@
 ### Literals
 
 `mypy_boto3_athena.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_athena.literals import (
+    CalculationExecutionStateType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
+    ExecutorStateType,
+    ExecutorTypeType,
     GetQueryResultsPaginatorName,
     ListDataCatalogsPaginatorName,
     ListDatabasesPaginatorName,
     ListNamedQueriesPaginatorName,
     ListQueryExecutionsPaginatorName,
     ListTableMetadataPaginatorName,
     ListTagsForResourcePaginatorName,
+    NotebookTypeType,
     QueryExecutionStateType,
     S3AclOptionType,
+    SessionStateType,
     StatementTypeType,
     WorkGroupStateType,
     AthenaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ColumnNullableType) -> bool:
+def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
+    ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
+    CalculationConfigurationTypeDef,
+    CalculationResultTypeDef,
+    CalculationStatisticsTypeDef,
+    CalculationStatusTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
+    CreateNotebookInputRequestTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
+    CreatePresignedNotebookUrlRequestRequestTypeDef,
+    CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
+    DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationTypeDef,
     EngineVersionTypeDef,
+    ExecutorsSummaryTypeDef,
+    ExportNotebookInputRequestTypeDef,
+    NotebookMetadataTypeDef,
+    FilterDefinitionTypeDef,
+    GetCalculationExecutionCodeRequestRequestTypeDef,
+    GetCalculationExecutionRequestRequestTypeDef,
+    GetCalculationExecutionStatusRequestRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
+    GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
     PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
+    GetSessionRequestRequestTypeDef,
+    SessionStatisticsTypeDef,
+    SessionStatusTypeDef,
+    GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
+    ImportNotebookInputRequestTypeDef,
+    ListApplicationDPUSizesInputRequestTypeDef,
+    ListCalculationExecutionsRequestRequestTypeDef,
     ListDataCatalogsInputRequestTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
+    ListExecutorsRequestRequestTypeDef,
     ListNamedQueriesInputRequestTypeDef,
+    ListNotebookSessionsRequestRequestTypeDef,
+    NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
+    ListSessionsRequestRequestTypeDef,
     ListTableMetadataInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
+    StopCalculationExecutionRequestRequestTypeDef,
     StopQueryExecutionInputRequestTypeDef,
+    TerminateSessionRequestRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
+    UpdateNotebookInputRequestTypeDef,
+    UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
     QueryExecutionStatusTypeDef,
     CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
     ListNamedQueriesOutputTypeDef,
     ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
+    StartCalculationExecutionRequestRequestTypeDef,
+    CalculationSummaryTypeDef,
+    GetCalculationExecutionResponseTypeDef,
+    GetCalculationExecutionStatusResponseTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
+    SessionConfigurationTypeDef,
+    StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
+    ListExecutorsResponseTypeDef,
+    ExportNotebookOutputTypeDef,
+    GetNotebookMetadataOutputTypeDef,
+    ListNotebookMetadataOutputTypeDef,
+    ListNotebookMetadataInputRequestTypeDef,
     GetQueryResultsInputGetQueryResultsPaginateTypeDef,
     ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDatabasesInputListDatabasesPaginateTypeDef,
     ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    GetSessionStatusResponseTypeDef,
+    SessionSummaryTypeDef,
+    ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
+    ListCalculationExecutionsResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
+    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
+    ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
     CreateWorkGroupInputRequestTypeDef,
     WorkGroupTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.26.4\nVersion:         1.26.4\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Athena 1.26.87\nVersion:         1.26.87\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.4")
+    print("1.26.87")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,52 +14,81 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import DataCatalogTypeType, WorkGroupStateType
+from .literals import (
+    CalculationExecutionStateType,
+    DataCatalogTypeType,
+    ExecutorStateType,
+    SessionStateType,
+    WorkGroupStateType,
+)
 from .paginator import (
     GetQueryResultsPaginator,
     ListDatabasesPaginator,
     ListDataCatalogsPaginator,
     ListNamedQueriesPaginator,
     ListQueryExecutionsPaginator,
     ListTableMetadataPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
+    CalculationConfigurationTypeDef,
     CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    EngineConfigurationTypeDef,
+    ExportNotebookOutputTypeDef,
+    FilterDefinitionTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
+    GetCalculationExecutionResponseTypeDef,
+    GetCalculationExecutionStatusResponseTypeDef,
     GetDatabaseOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetNamedQueryOutputTypeDef,
+    GetNotebookMetadataOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetQueryResultsOutputTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
+    GetSessionResponseTypeDef,
+    GetSessionStatusResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     GetWorkGroupOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListCalculationExecutionsResponseTypeDef,
     ListDatabasesOutputTypeDef,
     ListDataCatalogsOutputTypeDef,
     ListEngineVersionsOutputTypeDef,
+    ListExecutorsResponseTypeDef,
     ListNamedQueriesOutputTypeDef,
+    ListNotebookMetadataOutputTypeDef,
+    ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     ListQueryExecutionsOutputTypeDef,
+    ListSessionsResponseTypeDef,
     ListTableMetadataOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWorkGroupsOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultConfigurationTypeDef,
     ResultReuseConfigurationTypeDef,
+    StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
     TagTypeDef,
+    TerminateSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -79,14 +108,15 @@
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     MetadataException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
+    SessionAlreadyExistsException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
 
 
 class AthenaClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/)
@@ -181,24 +211,44 @@
         """
         Creates a named query in the specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_named_query)
         """
 
+    def create_notebook(
+        self, *, WorkGroup: str, Name: str, ClientRequestToken: str = ...
+    ) -> CreateNotebookOutputTypeDef:
+        """
+        Creates an empty `ipynb` file in the specified Apache Spark enabled workgroup.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_notebook)
+        """
+
     def create_prepared_statement(
         self, *, StatementName: str, WorkGroup: str, QueryStatement: str, Description: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a prepared statement for use with SQL queries in Athena.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_prepared_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_prepared_statement)
         """
 
+    def create_presigned_notebook_url(
+        self, *, SessionId: str
+    ) -> CreatePresignedNotebookUrlResponseTypeDef:
+        """
+        Gets an authentication token and the URL at which the notebook can be accessed.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_presigned_notebook_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_presigned_notebook_url)
+        """
+
     def create_work_group(
         self,
         *,
         Name: str,
         Configuration: WorkGroupConfigurationTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
@@ -223,14 +273,22 @@
         Deletes the named query if you have access to the workgroup in which the query
         was saved.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_named_query)
         """
 
+    def delete_notebook(self, *, NotebookId: str) -> Dict[str, Any]:
+        """
+        Deletes the specified notebook.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_notebook)
+        """
+
     def delete_prepared_statement(self, *, StatementName: str, WorkGroup: str) -> Dict[str, Any]:
         """
         Deletes the prepared statement with the specified name from the specified
         workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_prepared_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_prepared_statement)
@@ -242,28 +300,67 @@
         """
         Deletes the workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_work_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_work_group)
         """
 
+    def export_notebook(self, *, NotebookId: str) -> ExportNotebookOutputTypeDef:
+        """
+        Exports the specified notebook and its metadata.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.export_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#export_notebook)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#generate_presigned_url)
         """
 
+    def get_calculation_execution(
+        self, *, CalculationExecutionId: str
+    ) -> GetCalculationExecutionResponseTypeDef:
+        """
+        Describes a previously submitted calculation execution.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution)
+        """
+
+    def get_calculation_execution_code(
+        self, *, CalculationExecutionId: str
+    ) -> GetCalculationExecutionCodeResponseTypeDef:
+        """
+        Retrieves a pre-signed URL to a copy of the code that was executed for the
+        calculation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_code)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_code)
+        """
+
+    def get_calculation_execution_status(
+        self, *, CalculationExecutionId: str
+    ) -> GetCalculationExecutionStatusResponseTypeDef:
+        """
+        Gets the status of a current calculation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_status)
+        """
+
     def get_data_catalog(self, *, Name: str) -> GetDataCatalogOutputTypeDef:
         """
         Returns the specified data catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_data_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_data_catalog)
         """
@@ -280,14 +377,22 @@
         """
         Returns information about a single query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_named_query)
         """
 
+    def get_notebook_metadata(self, *, NotebookId: str) -> GetNotebookMetadataOutputTypeDef:
+        """
+        Retrieves notebook metadata for the specified notebook ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_notebook_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_notebook_metadata)
+        """
+
     def get_prepared_statement(
         self, *, StatementName: str, WorkGroup: str
     ) -> GetPreparedStatementOutputTypeDef:
         """
         Retrieves the prepared statement with the specified name from the specified
         workgroup.
 
@@ -322,14 +427,31 @@
         Returns query execution runtime statistics related to a single execution of a
         query if you have access to the workgroup in which the query ran.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_query_runtime_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_query_runtime_statistics)
         """
 
+    def get_session(self, *, SessionId: str) -> GetSessionResponseTypeDef:
+        """
+        Gets the full details of a previously created session, including the session
+        status and configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_session)
+        """
+
+    def get_session_status(self, *, SessionId: str) -> GetSessionStatusResponseTypeDef:
+        """
+        Gets the current status of a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_session_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_session_status)
+        """
+
     def get_table_metadata(
         self, *, CatalogName: str, DatabaseName: str, TableName: str
     ) -> GetTableMetadataOutputTypeDef:
         """
         Returns table metadata for the specified catalog, database, and table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_table_metadata)
@@ -340,14 +462,57 @@
         """
         Returns information about the workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_work_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_work_group)
         """
 
+    def import_notebook(
+        self,
+        *,
+        WorkGroup: str,
+        Name: str,
+        Payload: str,
+        Type: Literal["IPYNB"],
+        ClientRequestToken: str = ...
+    ) -> ImportNotebookOutputTypeDef:
+        """
+        Imports a single `ipynb` file to a Spark enabled workgroup.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.import_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#import_notebook)
+        """
+
+    def list_application_dpu_sizes(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListApplicationDPUSizesOutputTypeDef:
+        """
+        Returns the supported DPU sizes for the supported application runtimes (for
+        example, `Jupyter 1.0` ).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_application_dpu_sizes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_application_dpu_sizes)
+        """
+
+    def list_calculation_executions(
+        self,
+        *,
+        SessionId: str,
+        StateFilter: CalculationExecutionStateType = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListCalculationExecutionsResponseTypeDef:
+        """
+        Lists the calculations that have been submitted to a session in descending
+        order.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_calculation_executions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_calculation_executions)
+        """
+
     def list_data_catalogs(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCatalogsOutputTypeDef:
         """
         Lists the data catalogs in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_data_catalogs)
@@ -371,25 +536,66 @@
         Returns a list of engine versions that are available to choose from, including
         the Auto option.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_engine_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_engine_versions)
         """
 
+    def list_executors(
+        self,
+        *,
+        SessionId: str,
+        ExecutorStateFilter: ExecutorStateType = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListExecutorsResponseTypeDef:
+        """
+        Lists, in descending order, the executors that have been submitted to a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_executors)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_executors)
+        """
+
     def list_named_queries(
         self, *, NextToken: str = ..., MaxResults: int = ..., WorkGroup: str = ...
     ) -> ListNamedQueriesOutputTypeDef:
         """
         Provides a list of available query IDs only for queries saved in the specified
         workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_named_queries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_named_queries)
         """
 
+    def list_notebook_metadata(
+        self,
+        *,
+        WorkGroup: str,
+        Filters: FilterDefinitionTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListNotebookMetadataOutputTypeDef:
+        """
+        Displays the notebook files for the specified workgroup in paginated format.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_metadata)
+        """
+
+    def list_notebook_sessions(
+        self, *, NotebookId: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListNotebookSessionsResponseTypeDef:
+        """
+        Lists, in descending order, the sessions that have been created in a notebook
+        that are in an active state like `CREATING` , `CREATED` , `IDLE` or `BUSY`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_sessions)
+        """
+
     def list_prepared_statements(
         self, *, WorkGroup: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPreparedStatementsOutputTypeDef:
         """
         Lists the prepared statements in the specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_prepared_statements)
@@ -403,14 +609,30 @@
         Provides a list of available query execution IDs for the queries in the
         specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_query_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_query_executions)
         """
 
+    def list_sessions(
+        self,
+        *,
+        WorkGroup: str,
+        StateFilter: SessionStateType = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListSessionsResponseTypeDef:
+        """
+        Lists the sessions in a workgroup that are in an active state like `CREATING` ,
+        `CREATED` , `IDLE` , or `BUSY`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_sessions)
+        """
+
     def list_table_metadata(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
         NextToken: str = ...,
@@ -439,14 +661,30 @@
         """
         Lists available workgroups for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
 
+    def start_calculation_execution(
+        self,
+        *,
+        SessionId: str,
+        Description: str = ...,
+        CalculationConfiguration: CalculationConfigurationTypeDef = ...,
+        CodeBlock: str = ...,
+        ClientRequestToken: str = ...
+    ) -> StartCalculationExecutionResponseTypeDef:
+        """
+        Submits calculations for execution within a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_calculation_execution)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_calculation_execution)
+        """
+
     def start_query_execution(
         self,
         *,
         QueryString: str,
         ClientRequestToken: str = ...,
         QueryExecutionContext: QueryExecutionContextTypeDef = ...,
         ResultConfiguration: ResultConfigurationTypeDef = ...,
@@ -457,14 +695,41 @@
         """
         Runs the SQL query statements contained in the `Query`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
 
+    def start_session(
+        self,
+        *,
+        WorkGroup: str,
+        EngineConfiguration: EngineConfigurationTypeDef,
+        Description: str = ...,
+        NotebookVersion: str = ...,
+        SessionIdleTimeoutInMinutes: int = ...,
+        ClientRequestToken: str = ...
+    ) -> StartSessionResponseTypeDef:
+        """
+        Creates a session for running calculations within a workgroup.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_session)
+        """
+
+    def stop_calculation_execution(
+        self, *, CalculationExecutionId: str
+    ) -> StopCalculationExecutionResponseTypeDef:
+        """
+        Requests the cancellation of a calculation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.stop_calculation_execution)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#stop_calculation_execution)
+        """
+
     def stop_query_execution(self, *, QueryExecutionId: str) -> Dict[str, Any]:
         """
         Stops a query execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.stop_query_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#stop_query_execution)
         """
@@ -473,14 +738,22 @@
         """
         Adds one or more tags to an Athena resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#tag_resource)
         """
 
+    def terminate_session(self, *, SessionId: str) -> TerminateSessionResponseTypeDef:
+        """
+        Terminates an active session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.terminate_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#terminate_session)
+        """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a data catalog or workgroup resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#untag_resource)
         """
@@ -506,14 +779,40 @@
         """
         Updates a  NamedQuery object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_named_query)
         """
 
+    def update_notebook(
+        self,
+        *,
+        NotebookId: str,
+        Payload: str,
+        Type: Literal["IPYNB"],
+        SessionId: str = ...,
+        ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the contents of a Spark notebook.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_notebook)
+        """
+
+    def update_notebook_metadata(
+        self, *, NotebookId: str, Name: str, ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the metadata for a notebook.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_notebook_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_notebook_metadata)
+        """
+
     def update_prepared_statement(
         self, *, StatementName: str, WorkGroup: str, QueryStatement: str, Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a prepared statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_prepared_statement)
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/client.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -14,52 +14,81 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import DataCatalogTypeType, WorkGroupStateType
+from .literals import (
+    CalculationExecutionStateType,
+    DataCatalogTypeType,
+    ExecutorStateType,
+    SessionStateType,
+    WorkGroupStateType,
+)
 from .paginator import (
     GetQueryResultsPaginator,
     ListDatabasesPaginator,
     ListDataCatalogsPaginator,
     ListNamedQueriesPaginator,
     ListQueryExecutionsPaginator,
     ListTableMetadataPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
+    CalculationConfigurationTypeDef,
     CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    EngineConfigurationTypeDef,
+    ExportNotebookOutputTypeDef,
+    FilterDefinitionTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
+    GetCalculationExecutionResponseTypeDef,
+    GetCalculationExecutionStatusResponseTypeDef,
     GetDatabaseOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetNamedQueryOutputTypeDef,
+    GetNotebookMetadataOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetQueryResultsOutputTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
+    GetSessionResponseTypeDef,
+    GetSessionStatusResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     GetWorkGroupOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListCalculationExecutionsResponseTypeDef,
     ListDatabasesOutputTypeDef,
     ListDataCatalogsOutputTypeDef,
     ListEngineVersionsOutputTypeDef,
+    ListExecutorsResponseTypeDef,
     ListNamedQueriesOutputTypeDef,
+    ListNotebookMetadataOutputTypeDef,
+    ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     ListQueryExecutionsOutputTypeDef,
+    ListSessionsResponseTypeDef,
     ListTableMetadataOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWorkGroupsOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultConfigurationTypeDef,
     ResultReuseConfigurationTypeDef,
+    StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
     TagTypeDef,
+    TerminateSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -76,14 +105,15 @@
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     MetadataException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
+    SessionAlreadyExistsException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
 
 class AthenaClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/)
     """
@@ -169,23 +199,41 @@
     ) -> CreateNamedQueryOutputTypeDef:
         """
         Creates a named query in the specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_named_query)
         """
+    def create_notebook(
+        self, *, WorkGroup: str, Name: str, ClientRequestToken: str = ...
+    ) -> CreateNotebookOutputTypeDef:
+        """
+        Creates an empty `ipynb` file in the specified Apache Spark enabled workgroup.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_notebook)
+        """
     def create_prepared_statement(
         self, *, StatementName: str, WorkGroup: str, QueryStatement: str, Description: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a prepared statement for use with SQL queries in Athena.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_prepared_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_prepared_statement)
         """
+    def create_presigned_notebook_url(
+        self, *, SessionId: str
+    ) -> CreatePresignedNotebookUrlResponseTypeDef:
+        """
+        Gets an authentication token and the URL at which the notebook can be accessed.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_presigned_notebook_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#create_presigned_notebook_url)
+        """
     def create_work_group(
         self,
         *,
         Name: str,
         Configuration: WorkGroupConfigurationTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
@@ -207,14 +255,21 @@
         """
         Deletes the named query if you have access to the workgroup in which the query
         was saved.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_named_query)
         """
+    def delete_notebook(self, *, NotebookId: str) -> Dict[str, Any]:
+        """
+        Deletes the specified notebook.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_notebook)
+        """
     def delete_prepared_statement(self, *, StatementName: str, WorkGroup: str) -> Dict[str, Any]:
         """
         Deletes the prepared statement with the specified name from the specified
         workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_prepared_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_prepared_statement)
@@ -224,27 +279,62 @@
     ) -> Dict[str, Any]:
         """
         Deletes the workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.delete_work_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#delete_work_group)
         """
+    def export_notebook(self, *, NotebookId: str) -> ExportNotebookOutputTypeDef:
+        """
+        Exports the specified notebook and its metadata.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.export_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#export_notebook)
+        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#generate_presigned_url)
         """
+    def get_calculation_execution(
+        self, *, CalculationExecutionId: str
+    ) -> GetCalculationExecutionResponseTypeDef:
+        """
+        Describes a previously submitted calculation execution.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution)
+        """
+    def get_calculation_execution_code(
+        self, *, CalculationExecutionId: str
+    ) -> GetCalculationExecutionCodeResponseTypeDef:
+        """
+        Retrieves a pre-signed URL to a copy of the code that was executed for the
+        calculation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_code)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_code)
+        """
+    def get_calculation_execution_status(
+        self, *, CalculationExecutionId: str
+    ) -> GetCalculationExecutionStatusResponseTypeDef:
+        """
+        Gets the status of a current calculation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_calculation_execution_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_calculation_execution_status)
+        """
     def get_data_catalog(self, *, Name: str) -> GetDataCatalogOutputTypeDef:
         """
         Returns the specified data catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_data_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_data_catalog)
         """
@@ -258,14 +348,21 @@
     def get_named_query(self, *, NamedQueryId: str) -> GetNamedQueryOutputTypeDef:
         """
         Returns information about a single query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_named_query)
         """
+    def get_notebook_metadata(self, *, NotebookId: str) -> GetNotebookMetadataOutputTypeDef:
+        """
+        Retrieves notebook metadata for the specified notebook ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_notebook_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_notebook_metadata)
+        """
     def get_prepared_statement(
         self, *, StatementName: str, WorkGroup: str
     ) -> GetPreparedStatementOutputTypeDef:
         """
         Retrieves the prepared statement with the specified name from the specified
         workgroup.
 
@@ -296,14 +393,29 @@
         """
         Returns query execution runtime statistics related to a single execution of a
         query if you have access to the workgroup in which the query ran.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_query_runtime_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_query_runtime_statistics)
         """
+    def get_session(self, *, SessionId: str) -> GetSessionResponseTypeDef:
+        """
+        Gets the full details of a previously created session, including the session
+        status and configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_session)
+        """
+    def get_session_status(self, *, SessionId: str) -> GetSessionStatusResponseTypeDef:
+        """
+        Gets the current status of a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_session_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_session_status)
+        """
     def get_table_metadata(
         self, *, CatalogName: str, DatabaseName: str, TableName: str
     ) -> GetTableMetadataOutputTypeDef:
         """
         Returns table metadata for the specified catalog, database, and table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_table_metadata)
@@ -312,14 +424,54 @@
     def get_work_group(self, *, WorkGroup: str) -> GetWorkGroupOutputTypeDef:
         """
         Returns information about the workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.get_work_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#get_work_group)
         """
+    def import_notebook(
+        self,
+        *,
+        WorkGroup: str,
+        Name: str,
+        Payload: str,
+        Type: Literal["IPYNB"],
+        ClientRequestToken: str = ...
+    ) -> ImportNotebookOutputTypeDef:
+        """
+        Imports a single `ipynb` file to a Spark enabled workgroup.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.import_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#import_notebook)
+        """
+    def list_application_dpu_sizes(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListApplicationDPUSizesOutputTypeDef:
+        """
+        Returns the supported DPU sizes for the supported application runtimes (for
+        example, `Jupyter 1.0` ).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_application_dpu_sizes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_application_dpu_sizes)
+        """
+    def list_calculation_executions(
+        self,
+        *,
+        SessionId: str,
+        StateFilter: CalculationExecutionStateType = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListCalculationExecutionsResponseTypeDef:
+        """
+        Lists the calculations that have been submitted to a session in descending
+        order.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_calculation_executions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_calculation_executions)
+        """
     def list_data_catalogs(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCatalogsOutputTypeDef:
         """
         Lists the data catalogs in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_data_catalogs)
@@ -340,24 +492,62 @@
         """
         Returns a list of engine versions that are available to choose from, including
         the Auto option.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_engine_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_engine_versions)
         """
+    def list_executors(
+        self,
+        *,
+        SessionId: str,
+        ExecutorStateFilter: ExecutorStateType = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListExecutorsResponseTypeDef:
+        """
+        Lists, in descending order, the executors that have been submitted to a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_executors)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_executors)
+        """
     def list_named_queries(
         self, *, NextToken: str = ..., MaxResults: int = ..., WorkGroup: str = ...
     ) -> ListNamedQueriesOutputTypeDef:
         """
         Provides a list of available query IDs only for queries saved in the specified
         workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_named_queries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_named_queries)
         """
+    def list_notebook_metadata(
+        self,
+        *,
+        WorkGroup: str,
+        Filters: FilterDefinitionTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListNotebookMetadataOutputTypeDef:
+        """
+        Displays the notebook files for the specified workgroup in paginated format.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_metadata)
+        """
+    def list_notebook_sessions(
+        self, *, NotebookId: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListNotebookSessionsResponseTypeDef:
+        """
+        Lists, in descending order, the sessions that have been created in a notebook
+        that are in an active state like `CREATING` , `CREATED` , `IDLE` or `BUSY`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_notebook_sessions)
+        """
     def list_prepared_statements(
         self, *, WorkGroup: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPreparedStatementsOutputTypeDef:
         """
         Lists the prepared statements in the specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_prepared_statements)
@@ -369,14 +559,29 @@
         """
         Provides a list of available query execution IDs for the queries in the
         specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_query_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_query_executions)
         """
+    def list_sessions(
+        self,
+        *,
+        WorkGroup: str,
+        StateFilter: SessionStateType = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListSessionsResponseTypeDef:
+        """
+        Lists the sessions in a workgroup that are in an active state like `CREATING` ,
+        `CREATED` , `IDLE` , or `BUSY`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_sessions)
+        """
     def list_table_metadata(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
         NextToken: str = ...,
@@ -402,14 +607,29 @@
     ) -> ListWorkGroupsOutputTypeDef:
         """
         Lists available workgroups for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
+    def start_calculation_execution(
+        self,
+        *,
+        SessionId: str,
+        Description: str = ...,
+        CalculationConfiguration: CalculationConfigurationTypeDef = ...,
+        CodeBlock: str = ...,
+        ClientRequestToken: str = ...
+    ) -> StartCalculationExecutionResponseTypeDef:
+        """
+        Submits calculations for execution within a session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_calculation_execution)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_calculation_execution)
+        """
     def start_query_execution(
         self,
         *,
         QueryString: str,
         ClientRequestToken: str = ...,
         QueryExecutionContext: QueryExecutionContextTypeDef = ...,
         ResultConfiguration: ResultConfigurationTypeDef = ...,
@@ -419,28 +639,60 @@
     ) -> StartQueryExecutionOutputTypeDef:
         """
         Runs the SQL query statements contained in the `Query`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
+    def start_session(
+        self,
+        *,
+        WorkGroup: str,
+        EngineConfiguration: EngineConfigurationTypeDef,
+        Description: str = ...,
+        NotebookVersion: str = ...,
+        SessionIdleTimeoutInMinutes: int = ...,
+        ClientRequestToken: str = ...
+    ) -> StartSessionResponseTypeDef:
+        """
+        Creates a session for running calculations within a workgroup.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_session)
+        """
+    def stop_calculation_execution(
+        self, *, CalculationExecutionId: str
+    ) -> StopCalculationExecutionResponseTypeDef:
+        """
+        Requests the cancellation of a calculation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.stop_calculation_execution)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#stop_calculation_execution)
+        """
     def stop_query_execution(self, *, QueryExecutionId: str) -> Dict[str, Any]:
         """
         Stops a query execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.stop_query_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#stop_query_execution)
         """
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more tags to an Athena resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#tag_resource)
         """
+    def terminate_session(self, *, SessionId: str) -> TerminateSessionResponseTypeDef:
+        """
+        Terminates an active session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.terminate_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#terminate_session)
+        """
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a data catalog or workgroup resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#untag_resource)
         """
@@ -463,14 +715,38 @@
     ) -> Dict[str, Any]:
         """
         Updates a  NamedQuery object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_named_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_named_query)
         """
+    def update_notebook(
+        self,
+        *,
+        NotebookId: str,
+        Payload: str,
+        Type: Literal["IPYNB"],
+        SessionId: str = ...,
+        ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the contents of a Spark notebook.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_notebook)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_notebook)
+        """
+    def update_notebook_metadata(
+        self, *, NotebookId: str, Name: str, ClientRequestToken: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the metadata for a notebook.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_notebook_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#update_notebook_metadata)
+        """
     def update_prepared_statement(
         self, *, StatementName: str, WorkGroup: str, QueryStatement: str, Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a prepared statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_prepared_statement)
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,62 +2,78 @@
 Type annotations for athena service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_athena.literals import ColumnNullableType
+    from mypy_boto3_athena.literals import CalculationExecutionStateType
 
-    data: ColumnNullableType = "NOT_NULL"
+    data: CalculationExecutionStateType = "CANCELED"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "CalculationExecutionStateType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
+    "ExecutorStateType",
+    "ExecutorTypeType",
     "GetQueryResultsPaginatorName",
     "ListDataCatalogsPaginatorName",
     "ListDatabasesPaginatorName",
     "ListNamedQueriesPaginatorName",
     "ListQueryExecutionsPaginatorName",
     "ListTableMetadataPaginatorName",
     "ListTagsForResourcePaginatorName",
+    "NotebookTypeType",
     "QueryExecutionStateType",
     "S3AclOptionType",
+    "SessionStateType",
     "StatementTypeType",
     "WorkGroupStateType",
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+CalculationExecutionStateType = Literal[
+    "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
+]
 ColumnNullableType = Literal["NOT_NULL", "NULLABLE", "UNKNOWN"]
 DataCatalogTypeType = Literal["GLUE", "HIVE", "LAMBDA"]
 EncryptionOptionType = Literal["CSE_KMS", "SSE_KMS", "SSE_S3"]
+ExecutorStateType = Literal[
+    "CREATED", "CREATING", "FAILED", "REGISTERED", "TERMINATED", "TERMINATING"
+]
+ExecutorTypeType = Literal["COORDINATOR", "GATEWAY", "WORKER"]
 GetQueryResultsPaginatorName = Literal["get_query_results"]
 ListDataCatalogsPaginatorName = Literal["list_data_catalogs"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListNamedQueriesPaginatorName = Literal["list_named_queries"]
 ListQueryExecutionsPaginatorName = Literal["list_query_executions"]
 ListTableMetadataPaginatorName = Literal["list_table_metadata"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
+NotebookTypeType = Literal["IPYNB"]
 QueryExecutionStateType = Literal["CANCELLED", "FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 S3AclOptionType = Literal["BUCKET_OWNER_FULL_CONTROL"]
+SessionStateType = Literal[
+    "BUSY", "CREATED", "CREATING", "DEGRADED", "FAILED", "IDLE", "TERMINATED", "TERMINATING"
+]
 StatementTypeType = Literal["DDL", "DML", "UTILITY"]
 WorkGroupStateType = Literal["DISABLED", "ENABLED"]
 AthenaServiceName = Literal["athena"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -77,14 +93,15 @@
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
@@ -94,27 +111,31 @@
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
@@ -143,14 +164,15 @@
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
@@ -195,17 +217,19 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
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
@@ -216,30 +240,33 @@
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
@@ -271,28 +298,32 @@
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
@@ -301,14 +332,15 @@
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
@@ -319,51 +351,58 @@
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
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/literals.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,60 +2,76 @@
 Type annotations for athena service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_athena.literals import ColumnNullableType
+    from mypy_boto3_athena.literals import CalculationExecutionStateType
 
-    data: ColumnNullableType = "NOT_NULL"
+    data: CalculationExecutionStateType = "CANCELED"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "CalculationExecutionStateType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
+    "ExecutorStateType",
+    "ExecutorTypeType",
     "GetQueryResultsPaginatorName",
     "ListDataCatalogsPaginatorName",
     "ListDatabasesPaginatorName",
     "ListNamedQueriesPaginatorName",
     "ListQueryExecutionsPaginatorName",
     "ListTableMetadataPaginatorName",
     "ListTagsForResourcePaginatorName",
+    "NotebookTypeType",
     "QueryExecutionStateType",
     "S3AclOptionType",
+    "SessionStateType",
     "StatementTypeType",
     "WorkGroupStateType",
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+CalculationExecutionStateType = Literal[
+    "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
+]
 ColumnNullableType = Literal["NOT_NULL", "NULLABLE", "UNKNOWN"]
 DataCatalogTypeType = Literal["GLUE", "HIVE", "LAMBDA"]
 EncryptionOptionType = Literal["CSE_KMS", "SSE_KMS", "SSE_S3"]
+ExecutorStateType = Literal[
+    "CREATED", "CREATING", "FAILED", "REGISTERED", "TERMINATED", "TERMINATING"
+]
+ExecutorTypeType = Literal["COORDINATOR", "GATEWAY", "WORKER"]
 GetQueryResultsPaginatorName = Literal["get_query_results"]
 ListDataCatalogsPaginatorName = Literal["list_data_catalogs"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListNamedQueriesPaginatorName = Literal["list_named_queries"]
 ListQueryExecutionsPaginatorName = Literal["list_query_executions"]
 ListTableMetadataPaginatorName = Literal["list_table_metadata"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
+NotebookTypeType = Literal["IPYNB"]
 QueryExecutionStateType = Literal["CANCELLED", "FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 S3AclOptionType = Literal["BUCKET_OWNER_FULL_CONTROL"]
+SessionStateType = Literal[
+    "BUSY", "CREATED", "CREATING", "DEGRADED", "FAILED", "IDLE", "TERMINATED", "TERMINATING"
+]
 StatementTypeType = Literal["DDL", "DML", "UTILITY"]
 WorkGroupStateType = Literal["DISABLED", "ENABLED"]
 AthenaServiceName = Literal["athena"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -75,14 +91,15 @@
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
@@ -92,27 +109,31 @@
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
@@ -141,14 +162,15 @@
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
@@ -193,17 +215,19 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
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
@@ -214,30 +238,33 @@
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
@@ -269,28 +296,32 @@
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
@@ -299,14 +330,15 @@
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
@@ -317,51 +349,58 @@
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
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,18 +12,22 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
+    CalculationExecutionStateType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
+    ExecutorStateType,
+    ExecutorTypeType,
     QueryExecutionStateType,
+    SessionStateType,
     StatementTypeType,
     WorkGroupStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -32,111 +36,170 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AclConfigurationTypeDef",
+    "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
+    "CalculationConfigurationTypeDef",
+    "CalculationResultTypeDef",
+    "CalculationStatisticsTypeDef",
+    "CalculationStatusTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
+    "CreateNotebookInputRequestTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
+    "CreatePresignedNotebookUrlRequestRequestTypeDef",
+    "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
+    "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
+    "ExecutorsSummaryTypeDef",
+    "ExportNotebookInputRequestTypeDef",
+    "NotebookMetadataTypeDef",
+    "FilterDefinitionTypeDef",
+    "GetCalculationExecutionCodeRequestRequestTypeDef",
+    "GetCalculationExecutionRequestRequestTypeDef",
+    "GetCalculationExecutionStatusRequestRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
+    "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
+    "GetSessionRequestRequestTypeDef",
+    "SessionStatisticsTypeDef",
+    "SessionStatusTypeDef",
+    "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
+    "ImportNotebookInputRequestTypeDef",
+    "ListApplicationDPUSizesInputRequestTypeDef",
+    "ListCalculationExecutionsRequestRequestTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
+    "ListExecutorsRequestRequestTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
+    "ListNotebookSessionsRequestRequestTypeDef",
+    "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
+    "ListSessionsRequestRequestTypeDef",
     "ListTableMetadataInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
+    "StopCalculationExecutionRequestRequestTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
+    "TerminateSessionRequestRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
+    "UpdateNotebookInputRequestTypeDef",
+    "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
     "QueryExecutionStatusTypeDef",
     "CreateNamedQueryOutputTypeDef",
+    "CreateNotebookOutputTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
+    "ImportNotebookOutputTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
     "ListNamedQueriesOutputTypeDef",
     "ListQueryExecutionsOutputTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
     "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
+    "StartCalculationExecutionRequestRequestTypeDef",
+    "CalculationSummaryTypeDef",
+    "GetCalculationExecutionResponseTypeDef",
+    "GetCalculationExecutionStatusResponseTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
+    "SessionConfigurationTypeDef",
+    "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
+    "ListExecutorsResponseTypeDef",
+    "ExportNotebookOutputTypeDef",
+    "GetNotebookMetadataOutputTypeDef",
+    "ListNotebookMetadataOutputTypeDef",
+    "ListNotebookMetadataInputRequestTypeDef",
     "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
     "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "GetSessionStatusResponseTypeDef",
+    "SessionSummaryTypeDef",
+    "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
+    "ListCalculationExecutionsResponseTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
+    "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
+    "ListSessionsResponseTypeDef",
     "GetQueryRuntimeStatisticsOutputTypeDef",
     "QueryExecutionTypeDef",
     "StartQueryExecutionInputRequestTypeDef",
     "GetQueryResultsOutputTypeDef",
     "CreateWorkGroupInputRequestTypeDef",
     "WorkGroupTypeDef",
     "UpdateWorkGroupInputRequestTypeDef",
@@ -148,14 +211,23 @@
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
     },
 )
 
+ApplicationDPUSizesTypeDef = TypedDict(
+    "ApplicationDPUSizesTypeDef",
+    {
+        "ApplicationRuntimeId": str,
+        "SupportedDPUSizes": List[int],
+    },
+    total=False,
+)
+
 AthenaErrorTypeDef = TypedDict(
     "AthenaErrorTypeDef",
     {
         "ErrorCategory": int,
         "ErrorType": int,
         "Retryable": bool,
         "ErrorMessage": str,
@@ -257,14 +329,53 @@
         "QueryExecutionId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+CalculationConfigurationTypeDef = TypedDict(
+    "CalculationConfigurationTypeDef",
+    {
+        "CodeBlock": str,
+    },
+    total=False,
+)
+
+CalculationResultTypeDef = TypedDict(
+    "CalculationResultTypeDef",
+    {
+        "StdOutS3Uri": str,
+        "StdErrorS3Uri": str,
+        "ResultS3Uri": str,
+        "ResultType": str,
+    },
+    total=False,
+)
+
+CalculationStatisticsTypeDef = TypedDict(
+    "CalculationStatisticsTypeDef",
+    {
+        "DpuExecutionInMillis": int,
+        "Progress": str,
+    },
+    total=False,
+)
+
+CalculationStatusTypeDef = TypedDict(
+    "CalculationStatusTypeDef",
+    {
+        "SubmissionDateTime": datetime,
+        "CompletionDateTime": datetime,
+        "State": CalculationExecutionStateType,
+        "StateChangeReason": str,
+    },
+    total=False,
+)
+
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Name": str,
         "Type": str,
     },
 )
@@ -338,14 +449,36 @@
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateNotebookInputRequestTypeDef = TypedDict(
+    "_RequiredCreateNotebookInputRequestTypeDef",
+    {
+        "WorkGroup": str,
+        "Name": str,
+    },
+)
+_OptionalCreateNotebookInputRequestTypeDef = TypedDict(
+    "_OptionalCreateNotebookInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class CreateNotebookInputRequestTypeDef(
+    _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
+):
+    pass
+
+
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -362,14 +495,28 @@
 class CreatePreparedStatementInputRequestTypeDef(
     _RequiredCreatePreparedStatementInputRequestTypeDef,
     _OptionalCreatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
 
+CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
+CustomerContentEncryptionConfigurationTypeDef = TypedDict(
+    "CustomerContentEncryptionConfigurationTypeDef",
+    {
+        "KmsKey": str,
+    },
+)
+
 DataCatalogSummaryTypeDef = TypedDict(
     "DataCatalogSummaryTypeDef",
     {
         "CatalogName": str,
         "Type": DataCatalogTypeType,
     },
     total=False,
@@ -434,14 +581,21 @@
 DeleteNamedQueryInputRequestTypeDef = TypedDict(
     "DeleteNamedQueryInputRequestTypeDef",
     {
         "NamedQueryId": str,
     },
 )
 
+DeleteNotebookInputRequestTypeDef = TypedDict(
+    "DeleteNotebookInputRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+
 DeletePreparedStatementInputRequestTypeDef = TypedDict(
     "DeletePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
     },
 )
@@ -484,23 +638,118 @@
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
 
+_RequiredEngineConfigurationTypeDef = TypedDict(
+    "_RequiredEngineConfigurationTypeDef",
+    {
+        "MaxConcurrentDpus": int,
+    },
+)
+_OptionalEngineConfigurationTypeDef = TypedDict(
+    "_OptionalEngineConfigurationTypeDef",
+    {
+        "CoordinatorDpuSize": int,
+        "DefaultExecutorDpuSize": int,
+        "AdditionalConfigs": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class EngineConfigurationTypeDef(
+    _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
+):
+    pass
+
+
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": str,
         "EffectiveEngineVersion": str,
     },
     total=False,
 )
 
+_RequiredExecutorsSummaryTypeDef = TypedDict(
+    "_RequiredExecutorsSummaryTypeDef",
+    {
+        "ExecutorId": str,
+    },
+)
+_OptionalExecutorsSummaryTypeDef = TypedDict(
+    "_OptionalExecutorsSummaryTypeDef",
+    {
+        "ExecutorType": ExecutorTypeType,
+        "StartDateTime": int,
+        "TerminationDateTime": int,
+        "ExecutorState": ExecutorStateType,
+        "ExecutorSize": int,
+    },
+    total=False,
+)
+
+
+class ExecutorsSummaryTypeDef(_RequiredExecutorsSummaryTypeDef, _OptionalExecutorsSummaryTypeDef):
+    pass
+
+
+ExportNotebookInputRequestTypeDef = TypedDict(
+    "ExportNotebookInputRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+
+NotebookMetadataTypeDef = TypedDict(
+    "NotebookMetadataTypeDef",
+    {
+        "NotebookId": str,
+        "Name": str,
+        "WorkGroup": str,
+        "CreationTime": datetime,
+        "Type": Literal["IPYNB"],
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+FilterDefinitionTypeDef = TypedDict(
+    "FilterDefinitionTypeDef",
+    {
+        "Name": str,
+    },
+    total=False,
+)
+
+GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
+    "GetCalculationExecutionCodeRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
+GetCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "GetCalculationExecutionRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
+GetCalculationExecutionStatusRequestRequestTypeDef = TypedDict(
+    "GetCalculationExecutionStatusRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
 GetDataCatalogInputRequestTypeDef = TypedDict(
     "GetDataCatalogInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -515,14 +764,21 @@
 GetNamedQueryInputRequestTypeDef = TypedDict(
     "GetNamedQueryInputRequestTypeDef",
     {
         "NamedQueryId": str,
     },
 )
 
+GetNotebookMetadataInputRequestTypeDef = TypedDict(
+    "GetNotebookMetadataInputRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+
 GetPreparedStatementInputRequestTypeDef = TypedDict(
     "GetPreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
     },
 )
@@ -569,14 +825,49 @@
 GetQueryRuntimeStatisticsInputRequestTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
+GetSessionRequestRequestTypeDef = TypedDict(
+    "GetSessionRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
+SessionStatisticsTypeDef = TypedDict(
+    "SessionStatisticsTypeDef",
+    {
+        "DpuExecutionInMillis": int,
+    },
+    total=False,
+)
+
+SessionStatusTypeDef = TypedDict(
+    "SessionStatusTypeDef",
+    {
+        "StartDateTime": datetime,
+        "LastModifiedDateTime": datetime,
+        "EndDateTime": datetime,
+        "IdleSinceDateTime": datetime,
+        "State": SessionStateType,
+        "StateChangeReason": str,
+    },
+    total=False,
+)
+
+GetSessionStatusRequestRequestTypeDef = TypedDict(
+    "GetSessionStatusRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
 GetTableMetadataInputRequestTypeDef = TypedDict(
     "GetTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
         "TableName": str,
     },
@@ -585,14 +876,71 @@
 GetWorkGroupInputRequestTypeDef = TypedDict(
     "GetWorkGroupInputRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 
+_RequiredImportNotebookInputRequestTypeDef = TypedDict(
+    "_RequiredImportNotebookInputRequestTypeDef",
+    {
+        "WorkGroup": str,
+        "Name": str,
+        "Payload": str,
+        "Type": Literal["IPYNB"],
+    },
+)
+_OptionalImportNotebookInputRequestTypeDef = TypedDict(
+    "_OptionalImportNotebookInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class ImportNotebookInputRequestTypeDef(
+    _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
+):
+    pass
+
+
+ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
+    "ListApplicationDPUSizesInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListCalculationExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCalculationExecutionsRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+_OptionalListCalculationExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCalculationExecutionsRequestRequestTypeDef",
+    {
+        "StateFilter": CalculationExecutionStateType,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListCalculationExecutionsRequestRequestTypeDef(
+    _RequiredListCalculationExecutionsRequestRequestTypeDef,
+    _OptionalListCalculationExecutionsRequestRequestTypeDef,
+):
+    pass
+
+
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -625,24 +973,79 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListExecutorsRequestRequestTypeDef = TypedDict(
+    "_RequiredListExecutorsRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+_OptionalListExecutorsRequestRequestTypeDef = TypedDict(
+    "_OptionalListExecutorsRequestRequestTypeDef",
+    {
+        "ExecutorStateFilter": ExecutorStateType,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListExecutorsRequestRequestTypeDef(
+    _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
+):
+    pass
+
+
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+_RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListNotebookSessionsRequestRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+_OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListNotebookSessionsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListNotebookSessionsRequestRequestTypeDef(
+    _RequiredListNotebookSessionsRequestRequestTypeDef,
+    _OptionalListNotebookSessionsRequestRequestTypeDef,
+):
+    pass
+
+
+NotebookSessionSummaryTypeDef = TypedDict(
+    "NotebookSessionSummaryTypeDef",
+    {
+        "SessionId": str,
+        "CreationTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredListPreparedStatementsInputRequestTypeDef = TypedDict(
     "_RequiredListPreparedStatementsInputRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListPreparedStatementsInputRequestTypeDef = TypedDict(
@@ -677,14 +1080,37 @@
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+_RequiredListSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionsRequestRequestTypeDef",
+    {
+        "WorkGroup": str,
+    },
+)
+_OptionalListSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionsRequestRequestTypeDef",
+    {
+        "StateFilter": SessionStateType,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListSessionsRequestRequestTypeDef(
+    _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -819,21 +1245,35 @@
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
 
+StopCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "StopCalculationExecutionRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
+TerminateSessionRequestRequestTypeDef = TypedDict(
+    "TerminateSessionRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -880,14 +1320,61 @@
 
 class UpdateNamedQueryInputRequestTypeDef(
     _RequiredUpdateNamedQueryInputRequestTypeDef, _OptionalUpdateNamedQueryInputRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateNotebookInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateNotebookInputRequestTypeDef",
+    {
+        "NotebookId": str,
+        "Payload": str,
+        "Type": Literal["IPYNB"],
+    },
+)
+_OptionalUpdateNotebookInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateNotebookInputRequestTypeDef",
+    {
+        "SessionId": str,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateNotebookInputRequestTypeDef(
+    _RequiredUpdateNotebookInputRequestTypeDef, _OptionalUpdateNotebookInputRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateNotebookMetadataInputRequestTypeDef",
+    {
+        "NotebookId": str,
+        "Name": str,
+    },
+)
+_OptionalUpdateNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateNotebookMetadataInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateNotebookMetadataInputRequestTypeDef(
+    _RequiredUpdateNotebookMetadataInputRequestTypeDef,
+    _OptionalUpdateNotebookMetadataInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -924,22 +1411,65 @@
     "CreateNamedQueryOutputTypeDef",
     {
         "NamedQueryId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListNamedQueriesOutputTypeDef = TypedDict(
     "ListNamedQueriesOutputTypeDef",
     {
         "NamedQueryIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -950,22 +1480,56 @@
     {
         "QueryExecutionIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartQueryExecutionOutputTypeDef = TypedDict(
     "StartQueryExecutionOutputTypeDef",
     {
         "QueryExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -984,14 +1548,72 @@
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCalculationExecutionRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+_OptionalStartCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCalculationExecutionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "CalculationConfiguration": CalculationConfigurationTypeDef,
+        "CodeBlock": str,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class StartCalculationExecutionRequestRequestTypeDef(
+    _RequiredStartCalculationExecutionRequestRequestTypeDef,
+    _OptionalStartCalculationExecutionRequestRequestTypeDef,
+):
+    pass
+
+
+CalculationSummaryTypeDef = TypedDict(
+    "CalculationSummaryTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "Description": str,
+        "Status": CalculationStatusTypeDef,
+    },
+    total=False,
+)
+
+GetCalculationExecutionResponseTypeDef = TypedDict(
+    "GetCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "SessionId": str,
+        "Description": str,
+        "WorkingDirectory": str,
+        "Status": CalculationStatusTypeDef,
+        "Statistics": CalculationStatisticsTypeDef,
+        "Result": CalculationResultTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionStatusResponseTypeDef = TypedDict(
+    "GetCalculationExecutionStatusResponseTypeDef",
+    {
+        "Status": CalculationStatusTypeDef,
+        "Statistics": CalculationStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1125,14 +1747,50 @@
         "RemoveExpectedBucketOwner": bool,
         "AclConfiguration": AclConfigurationTypeDef,
         "RemoveAclConfiguration": bool,
     },
     total=False,
 )
 
+SessionConfigurationTypeDef = TypedDict(
+    "SessionConfigurationTypeDef",
+    {
+        "ExecutionRole": str,
+        "WorkingDirectory": str,
+        "IdleTimeoutSeconds": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSessionRequestRequestTypeDef",
+    {
+        "WorkGroup": str,
+        "EngineConfiguration": EngineConfigurationTypeDef,
+    },
+)
+_OptionalStartSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSessionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "NotebookVersion": str,
+        "SessionIdleTimeoutInMinutes": int,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class StartSessionRequestRequestTypeDef(
+    _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
+):
+    pass
+
+
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1146,14 +1804,74 @@
         "Description": str,
         "CreationTime": datetime,
         "EngineVersion": EngineVersionTypeDef,
     },
     total=False,
 )
 
+ListExecutorsResponseTypeDef = TypedDict(
+    "ListExecutorsResponseTypeDef",
+    {
+        "SessionId": str,
+        "NextToken": str,
+        "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportNotebookOutputTypeDef = TypedDict(
+    "ExportNotebookOutputTypeDef",
+    {
+        "NotebookMetadata": NotebookMetadataTypeDef,
+        "Payload": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNotebookMetadataOutputTypeDef = TypedDict(
+    "GetNotebookMetadataOutputTypeDef",
+    {
+        "NotebookMetadata": NotebookMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNotebookMetadataOutputTypeDef = TypedDict(
+    "ListNotebookMetadataOutputTypeDef",
+    {
+        "NextToken": str,
+        "NotebookMetadataList": List[NotebookMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_RequiredListNotebookMetadataInputRequestTypeDef",
+    {
+        "WorkGroup": str,
+    },
+)
+_OptionalListNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_OptionalListNotebookMetadataInputRequestTypeDef",
+    {
+        "Filters": FilterDefinitionTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListNotebookMetadataInputRequestTypeDef(
+    _RequiredListNotebookMetadataInputRequestTypeDef,
+    _OptionalListNotebookMetadataInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
@@ -1262,14 +1980,44 @@
 class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
 
+GetSessionStatusResponseTypeDef = TypedDict(
+    "GetSessionStatusResponseTypeDef",
+    {
+        "SessionId": str,
+        "Status": SessionStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SessionSummaryTypeDef = TypedDict(
+    "SessionSummaryTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "EngineVersion": EngineVersionTypeDef,
+        "NotebookVersion": str,
+        "Status": SessionStatusTypeDef,
+    },
+    total=False,
+)
+
+ListNotebookSessionsResponseTypeDef = TypedDict(
+    "ListNotebookSessionsResponseTypeDef",
+    {
+        "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1304,14 +2052,23 @@
     "ResultReuseConfigurationTypeDef",
     {
         "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationTypeDef,
     },
     total=False,
 )
 
+ListCalculationExecutionsResponseTypeDef = TypedDict(
+    "ListCalculationExecutionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Calculations": List[CalculationSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1339,41 +2096,73 @@
     {
         "ResultConfiguration": ResultConfigurationTypeDef,
         "EnforceWorkGroupConfiguration": bool,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
+        "AdditionalConfiguration": str,
+        "ExecutionRole": str,
+        "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
 WorkGroupConfigurationUpdatesTypeDef = TypedDict(
     "WorkGroupConfigurationUpdatesTypeDef",
     {
         "EnforceWorkGroupConfiguration": bool,
         "ResultConfigurationUpdates": ResultConfigurationUpdatesTypeDef,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
         "RemoveBytesScannedCutoffPerQuery": bool,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
+        "RemoveCustomerContentEncryptionConfiguration": bool,
+        "AdditionalConfiguration": str,
+        "ExecutionRole": str,
+        "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "WorkGroup": str,
+        "EngineVersion": str,
+        "EngineConfiguration": EngineConfigurationTypeDef,
+        "NotebookVersion": str,
+        "SessionConfiguration": SessionConfigurationTypeDef,
+        "Status": SessionStatusTypeDef,
+        "Statistics": SessionStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListSessionsResponseTypeDef = TypedDict(
+    "ListSessionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Sessions": List[SessionSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1388,14 +2177,15 @@
         "ResultReuseConfiguration": ResultReuseConfigurationTypeDef,
         "QueryExecutionContext": QueryExecutionContextTypeDef,
         "Status": QueryExecutionStatusTypeDef,
         "Statistics": QueryExecutionStatisticsTypeDef,
         "WorkGroup": str,
         "EngineVersion": EngineVersionTypeDef,
         "ExecutionParameters": List[str],
+        "SubstatementType": str,
     },
     total=False,
 )
 
 _RequiredStartQueryExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartQueryExecutionInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena/type_defs.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -12,18 +12,22 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
+    CalculationExecutionStateType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
+    ExecutorStateType,
+    ExecutorTypeType,
     QueryExecutionStateType,
+    SessionStateType,
     StatementTypeType,
     WorkGroupStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -31,111 +35,170 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AclConfigurationTypeDef",
+    "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
+    "CalculationConfigurationTypeDef",
+    "CalculationResultTypeDef",
+    "CalculationStatisticsTypeDef",
+    "CalculationStatusTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
+    "CreateNotebookInputRequestTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
+    "CreatePresignedNotebookUrlRequestRequestTypeDef",
+    "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
+    "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
+    "ExecutorsSummaryTypeDef",
+    "ExportNotebookInputRequestTypeDef",
+    "NotebookMetadataTypeDef",
+    "FilterDefinitionTypeDef",
+    "GetCalculationExecutionCodeRequestRequestTypeDef",
+    "GetCalculationExecutionRequestRequestTypeDef",
+    "GetCalculationExecutionStatusRequestRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
+    "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
+    "GetSessionRequestRequestTypeDef",
+    "SessionStatisticsTypeDef",
+    "SessionStatusTypeDef",
+    "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
+    "ImportNotebookInputRequestTypeDef",
+    "ListApplicationDPUSizesInputRequestTypeDef",
+    "ListCalculationExecutionsRequestRequestTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
+    "ListExecutorsRequestRequestTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
+    "ListNotebookSessionsRequestRequestTypeDef",
+    "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
+    "ListSessionsRequestRequestTypeDef",
     "ListTableMetadataInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
+    "StopCalculationExecutionRequestRequestTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
+    "TerminateSessionRequestRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
+    "UpdateNotebookInputRequestTypeDef",
+    "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
     "QueryExecutionStatusTypeDef",
     "CreateNamedQueryOutputTypeDef",
+    "CreateNotebookOutputTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
+    "ImportNotebookOutputTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
     "ListNamedQueriesOutputTypeDef",
     "ListQueryExecutionsOutputTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
     "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
+    "StartCalculationExecutionRequestRequestTypeDef",
+    "CalculationSummaryTypeDef",
+    "GetCalculationExecutionResponseTypeDef",
+    "GetCalculationExecutionStatusResponseTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
+    "SessionConfigurationTypeDef",
+    "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
+    "ListExecutorsResponseTypeDef",
+    "ExportNotebookOutputTypeDef",
+    "GetNotebookMetadataOutputTypeDef",
+    "ListNotebookMetadataOutputTypeDef",
+    "ListNotebookMetadataInputRequestTypeDef",
     "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
     "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "GetSessionStatusResponseTypeDef",
+    "SessionSummaryTypeDef",
+    "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
+    "ListCalculationExecutionsResponseTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
+    "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
+    "ListSessionsResponseTypeDef",
     "GetQueryRuntimeStatisticsOutputTypeDef",
     "QueryExecutionTypeDef",
     "StartQueryExecutionInputRequestTypeDef",
     "GetQueryResultsOutputTypeDef",
     "CreateWorkGroupInputRequestTypeDef",
     "WorkGroupTypeDef",
     "UpdateWorkGroupInputRequestTypeDef",
@@ -147,14 +210,23 @@
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
     },
 )
 
+ApplicationDPUSizesTypeDef = TypedDict(
+    "ApplicationDPUSizesTypeDef",
+    {
+        "ApplicationRuntimeId": str,
+        "SupportedDPUSizes": List[int],
+    },
+    total=False,
+)
+
 AthenaErrorTypeDef = TypedDict(
     "AthenaErrorTypeDef",
     {
         "ErrorCategory": int,
         "ErrorType": int,
         "Retryable": bool,
         "ErrorMessage": str,
@@ -254,14 +326,53 @@
         "QueryExecutionId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+CalculationConfigurationTypeDef = TypedDict(
+    "CalculationConfigurationTypeDef",
+    {
+        "CodeBlock": str,
+    },
+    total=False,
+)
+
+CalculationResultTypeDef = TypedDict(
+    "CalculationResultTypeDef",
+    {
+        "StdOutS3Uri": str,
+        "StdErrorS3Uri": str,
+        "ResultS3Uri": str,
+        "ResultType": str,
+    },
+    total=False,
+)
+
+CalculationStatisticsTypeDef = TypedDict(
+    "CalculationStatisticsTypeDef",
+    {
+        "DpuExecutionInMillis": int,
+        "Progress": str,
+    },
+    total=False,
+)
+
+CalculationStatusTypeDef = TypedDict(
+    "CalculationStatusTypeDef",
+    {
+        "SubmissionDateTime": datetime,
+        "CompletionDateTime": datetime,
+        "State": CalculationExecutionStateType,
+        "StateChangeReason": str,
+    },
+    total=False,
+)
+
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Name": str,
         "Type": str,
     },
 )
@@ -329,14 +440,34 @@
 )
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
+_RequiredCreateNotebookInputRequestTypeDef = TypedDict(
+    "_RequiredCreateNotebookInputRequestTypeDef",
+    {
+        "WorkGroup": str,
+        "Name": str,
+    },
+)
+_OptionalCreateNotebookInputRequestTypeDef = TypedDict(
+    "_OptionalCreateNotebookInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class CreateNotebookInputRequestTypeDef(
+    _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
+):
+    pass
+
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -351,14 +482,28 @@
 
 class CreatePreparedStatementInputRequestTypeDef(
     _RequiredCreatePreparedStatementInputRequestTypeDef,
     _OptionalCreatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
+CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
+CustomerContentEncryptionConfigurationTypeDef = TypedDict(
+    "CustomerContentEncryptionConfigurationTypeDef",
+    {
+        "KmsKey": str,
+    },
+)
+
 DataCatalogSummaryTypeDef = TypedDict(
     "DataCatalogSummaryTypeDef",
     {
         "CatalogName": str,
         "Type": DataCatalogTypeType,
     },
     total=False,
@@ -419,14 +564,21 @@
 DeleteNamedQueryInputRequestTypeDef = TypedDict(
     "DeleteNamedQueryInputRequestTypeDef",
     {
         "NamedQueryId": str,
     },
 )
 
+DeleteNotebookInputRequestTypeDef = TypedDict(
+    "DeleteNotebookInputRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+
 DeletePreparedStatementInputRequestTypeDef = TypedDict(
     "DeletePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
     },
 )
@@ -465,23 +617,114 @@
 )
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+_RequiredEngineConfigurationTypeDef = TypedDict(
+    "_RequiredEngineConfigurationTypeDef",
+    {
+        "MaxConcurrentDpus": int,
+    },
+)
+_OptionalEngineConfigurationTypeDef = TypedDict(
+    "_OptionalEngineConfigurationTypeDef",
+    {
+        "CoordinatorDpuSize": int,
+        "DefaultExecutorDpuSize": int,
+        "AdditionalConfigs": Dict[str, str],
+    },
+    total=False,
+)
+
+class EngineConfigurationTypeDef(
+    _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
+):
+    pass
+
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": str,
         "EffectiveEngineVersion": str,
     },
     total=False,
 )
 
+_RequiredExecutorsSummaryTypeDef = TypedDict(
+    "_RequiredExecutorsSummaryTypeDef",
+    {
+        "ExecutorId": str,
+    },
+)
+_OptionalExecutorsSummaryTypeDef = TypedDict(
+    "_OptionalExecutorsSummaryTypeDef",
+    {
+        "ExecutorType": ExecutorTypeType,
+        "StartDateTime": int,
+        "TerminationDateTime": int,
+        "ExecutorState": ExecutorStateType,
+        "ExecutorSize": int,
+    },
+    total=False,
+)
+
+class ExecutorsSummaryTypeDef(_RequiredExecutorsSummaryTypeDef, _OptionalExecutorsSummaryTypeDef):
+    pass
+
+ExportNotebookInputRequestTypeDef = TypedDict(
+    "ExportNotebookInputRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+
+NotebookMetadataTypeDef = TypedDict(
+    "NotebookMetadataTypeDef",
+    {
+        "NotebookId": str,
+        "Name": str,
+        "WorkGroup": str,
+        "CreationTime": datetime,
+        "Type": Literal["IPYNB"],
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+FilterDefinitionTypeDef = TypedDict(
+    "FilterDefinitionTypeDef",
+    {
+        "Name": str,
+    },
+    total=False,
+)
+
+GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
+    "GetCalculationExecutionCodeRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
+GetCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "GetCalculationExecutionRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
+GetCalculationExecutionStatusRequestRequestTypeDef = TypedDict(
+    "GetCalculationExecutionStatusRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
 GetDataCatalogInputRequestTypeDef = TypedDict(
     "GetDataCatalogInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -496,14 +739,21 @@
 GetNamedQueryInputRequestTypeDef = TypedDict(
     "GetNamedQueryInputRequestTypeDef",
     {
         "NamedQueryId": str,
     },
 )
 
+GetNotebookMetadataInputRequestTypeDef = TypedDict(
+    "GetNotebookMetadataInputRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+
 GetPreparedStatementInputRequestTypeDef = TypedDict(
     "GetPreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
     },
 )
@@ -548,14 +798,49 @@
 GetQueryRuntimeStatisticsInputRequestTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
+GetSessionRequestRequestTypeDef = TypedDict(
+    "GetSessionRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
+SessionStatisticsTypeDef = TypedDict(
+    "SessionStatisticsTypeDef",
+    {
+        "DpuExecutionInMillis": int,
+    },
+    total=False,
+)
+
+SessionStatusTypeDef = TypedDict(
+    "SessionStatusTypeDef",
+    {
+        "StartDateTime": datetime,
+        "LastModifiedDateTime": datetime,
+        "EndDateTime": datetime,
+        "IdleSinceDateTime": datetime,
+        "State": SessionStateType,
+        "StateChangeReason": str,
+    },
+    total=False,
+)
+
+GetSessionStatusRequestRequestTypeDef = TypedDict(
+    "GetSessionStatusRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
 GetTableMetadataInputRequestTypeDef = TypedDict(
     "GetTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
         "TableName": str,
     },
@@ -564,14 +849,67 @@
 GetWorkGroupInputRequestTypeDef = TypedDict(
     "GetWorkGroupInputRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 
+_RequiredImportNotebookInputRequestTypeDef = TypedDict(
+    "_RequiredImportNotebookInputRequestTypeDef",
+    {
+        "WorkGroup": str,
+        "Name": str,
+        "Payload": str,
+        "Type": Literal["IPYNB"],
+    },
+)
+_OptionalImportNotebookInputRequestTypeDef = TypedDict(
+    "_OptionalImportNotebookInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class ImportNotebookInputRequestTypeDef(
+    _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
+):
+    pass
+
+ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
+    "ListApplicationDPUSizesInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListCalculationExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCalculationExecutionsRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+_OptionalListCalculationExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCalculationExecutionsRequestRequestTypeDef",
+    {
+        "StateFilter": CalculationExecutionStateType,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListCalculationExecutionsRequestRequestTypeDef(
+    _RequiredListCalculationExecutionsRequestRequestTypeDef,
+    _OptionalListCalculationExecutionsRequestRequestTypeDef,
+):
+    pass
+
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -602,24 +940,75 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListExecutorsRequestRequestTypeDef = TypedDict(
+    "_RequiredListExecutorsRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+_OptionalListExecutorsRequestRequestTypeDef = TypedDict(
+    "_OptionalListExecutorsRequestRequestTypeDef",
+    {
+        "ExecutorStateFilter": ExecutorStateType,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListExecutorsRequestRequestTypeDef(
+    _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
+):
+    pass
+
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+_RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListNotebookSessionsRequestRequestTypeDef",
+    {
+        "NotebookId": str,
+    },
+)
+_OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListNotebookSessionsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListNotebookSessionsRequestRequestTypeDef(
+    _RequiredListNotebookSessionsRequestRequestTypeDef,
+    _OptionalListNotebookSessionsRequestRequestTypeDef,
+):
+    pass
+
+NotebookSessionSummaryTypeDef = TypedDict(
+    "NotebookSessionSummaryTypeDef",
+    {
+        "SessionId": str,
+        "CreationTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredListPreparedStatementsInputRequestTypeDef = TypedDict(
     "_RequiredListPreparedStatementsInputRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListPreparedStatementsInputRequestTypeDef = TypedDict(
@@ -652,14 +1041,35 @@
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
+_RequiredListSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionsRequestRequestTypeDef",
+    {
+        "WorkGroup": str,
+    },
+)
+_OptionalListSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionsRequestRequestTypeDef",
+    {
+        "StateFilter": SessionStateType,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListSessionsRequestRequestTypeDef(
+    _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
+):
+    pass
+
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -788,21 +1198,35 @@
 )
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
+StopCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "StopCalculationExecutionRequestRequestTypeDef",
+    {
+        "CalculationExecutionId": str,
+    },
+)
+
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
+TerminateSessionRequestRequestTypeDef = TypedDict(
+    "TerminateSessionRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -845,14 +1269,57 @@
 )
 
 class UpdateNamedQueryInputRequestTypeDef(
     _RequiredUpdateNamedQueryInputRequestTypeDef, _OptionalUpdateNamedQueryInputRequestTypeDef
 ):
     pass
 
+_RequiredUpdateNotebookInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateNotebookInputRequestTypeDef",
+    {
+        "NotebookId": str,
+        "Payload": str,
+        "Type": Literal["IPYNB"],
+    },
+)
+_OptionalUpdateNotebookInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateNotebookInputRequestTypeDef",
+    {
+        "SessionId": str,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class UpdateNotebookInputRequestTypeDef(
+    _RequiredUpdateNotebookInputRequestTypeDef, _OptionalUpdateNotebookInputRequestTypeDef
+):
+    pass
+
+_RequiredUpdateNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateNotebookMetadataInputRequestTypeDef",
+    {
+        "NotebookId": str,
+        "Name": str,
+    },
+)
+_OptionalUpdateNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateNotebookMetadataInputRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class UpdateNotebookMetadataInputRequestTypeDef(
+    _RequiredUpdateNotebookMetadataInputRequestTypeDef,
+    _OptionalUpdateNotebookMetadataInputRequestTypeDef,
+):
+    pass
+
 _RequiredUpdatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -887,22 +1354,65 @@
     "CreateNamedQueryOutputTypeDef",
     {
         "NamedQueryId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListNamedQueriesOutputTypeDef = TypedDict(
     "ListNamedQueriesOutputTypeDef",
     {
         "NamedQueryIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -913,22 +1423,56 @@
     {
         "QueryExecutionIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartQueryExecutionOutputTypeDef = TypedDict(
     "StartQueryExecutionOutputTypeDef",
     {
         "QueryExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -947,14 +1491,70 @@
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCalculationExecutionRequestRequestTypeDef",
+    {
+        "SessionId": str,
+    },
+)
+_OptionalStartCalculationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCalculationExecutionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "CalculationConfiguration": CalculationConfigurationTypeDef,
+        "CodeBlock": str,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class StartCalculationExecutionRequestRequestTypeDef(
+    _RequiredStartCalculationExecutionRequestRequestTypeDef,
+    _OptionalStartCalculationExecutionRequestRequestTypeDef,
+):
+    pass
+
+CalculationSummaryTypeDef = TypedDict(
+    "CalculationSummaryTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "Description": str,
+        "Status": CalculationStatusTypeDef,
+    },
+    total=False,
+)
+
+GetCalculationExecutionResponseTypeDef = TypedDict(
+    "GetCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "SessionId": str,
+        "Description": str,
+        "WorkingDirectory": str,
+        "Status": CalculationStatusTypeDef,
+        "Statistics": CalculationStatisticsTypeDef,
+        "Result": CalculationResultTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionStatusResponseTypeDef = TypedDict(
+    "GetCalculationExecutionStatusResponseTypeDef",
+    {
+        "Status": CalculationStatusTypeDef,
+        "Statistics": CalculationStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1084,14 +1684,48 @@
         "RemoveExpectedBucketOwner": bool,
         "AclConfiguration": AclConfigurationTypeDef,
         "RemoveAclConfiguration": bool,
     },
     total=False,
 )
 
+SessionConfigurationTypeDef = TypedDict(
+    "SessionConfigurationTypeDef",
+    {
+        "ExecutionRole": str,
+        "WorkingDirectory": str,
+        "IdleTimeoutSeconds": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSessionRequestRequestTypeDef",
+    {
+        "WorkGroup": str,
+        "EngineConfiguration": EngineConfigurationTypeDef,
+    },
+)
+_OptionalStartSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSessionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "NotebookVersion": str,
+        "SessionIdleTimeoutInMinutes": int,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class StartSessionRequestRequestTypeDef(
+    _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
+):
+    pass
+
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1105,14 +1739,72 @@
         "Description": str,
         "CreationTime": datetime,
         "EngineVersion": EngineVersionTypeDef,
     },
     total=False,
 )
 
+ListExecutorsResponseTypeDef = TypedDict(
+    "ListExecutorsResponseTypeDef",
+    {
+        "SessionId": str,
+        "NextToken": str,
+        "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportNotebookOutputTypeDef = TypedDict(
+    "ExportNotebookOutputTypeDef",
+    {
+        "NotebookMetadata": NotebookMetadataTypeDef,
+        "Payload": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNotebookMetadataOutputTypeDef = TypedDict(
+    "GetNotebookMetadataOutputTypeDef",
+    {
+        "NotebookMetadata": NotebookMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNotebookMetadataOutputTypeDef = TypedDict(
+    "ListNotebookMetadataOutputTypeDef",
+    {
+        "NextToken": str,
+        "NotebookMetadataList": List[NotebookMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_RequiredListNotebookMetadataInputRequestTypeDef",
+    {
+        "WorkGroup": str,
+    },
+)
+_OptionalListNotebookMetadataInputRequestTypeDef = TypedDict(
+    "_OptionalListNotebookMetadataInputRequestTypeDef",
+    {
+        "Filters": FilterDefinitionTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListNotebookMetadataInputRequestTypeDef(
+    _RequiredListNotebookMetadataInputRequestTypeDef,
+    _OptionalListNotebookMetadataInputRequestTypeDef,
+):
+    pass
+
 _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
@@ -1213,14 +1905,44 @@
 
 class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+GetSessionStatusResponseTypeDef = TypedDict(
+    "GetSessionStatusResponseTypeDef",
+    {
+        "SessionId": str,
+        "Status": SessionStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SessionSummaryTypeDef = TypedDict(
+    "SessionSummaryTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "EngineVersion": EngineVersionTypeDef,
+        "NotebookVersion": str,
+        "Status": SessionStatusTypeDef,
+    },
+    total=False,
+)
+
+ListNotebookSessionsResponseTypeDef = TypedDict(
+    "ListNotebookSessionsResponseTypeDef",
+    {
+        "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1255,14 +1977,23 @@
     "ResultReuseConfigurationTypeDef",
     {
         "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationTypeDef,
     },
     total=False,
 )
 
+ListCalculationExecutionsResponseTypeDef = TypedDict(
+    "ListCalculationExecutionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Calculations": List[CalculationSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1290,41 +2021,73 @@
     {
         "ResultConfiguration": ResultConfigurationTypeDef,
         "EnforceWorkGroupConfiguration": bool,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
+        "AdditionalConfiguration": str,
+        "ExecutionRole": str,
+        "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
 WorkGroupConfigurationUpdatesTypeDef = TypedDict(
     "WorkGroupConfigurationUpdatesTypeDef",
     {
         "EnforceWorkGroupConfiguration": bool,
         "ResultConfigurationUpdates": ResultConfigurationUpdatesTypeDef,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
         "RemoveBytesScannedCutoffPerQuery": bool,
         "RequesterPaysEnabled": bool,
         "EngineVersion": EngineVersionTypeDef,
+        "RemoveCustomerContentEncryptionConfiguration": bool,
+        "AdditionalConfiguration": str,
+        "ExecutionRole": str,
+        "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "WorkGroup": str,
+        "EngineVersion": str,
+        "EngineConfiguration": EngineConfigurationTypeDef,
+        "NotebookVersion": str,
+        "SessionConfiguration": SessionConfigurationTypeDef,
+        "Status": SessionStatusTypeDef,
+        "Statistics": SessionStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListSessionsResponseTypeDef = TypedDict(
+    "ListSessionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Sessions": List[SessionSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1339,14 +2102,15 @@
         "ResultReuseConfiguration": ResultReuseConfigurationTypeDef,
         "QueryExecutionContext": QueryExecutionContextTypeDef,
         "Status": QueryExecutionStatusTypeDef,
         "Statistics": QueryExecutionStatisticsTypeDef,
         "WorkGroup": str,
         "EngineVersion": EngineVersionTypeDef,
         "ExecutionParameters": List[str],
+        "SubstatementType": str,
     },
     total=False,
 )
 
 _RequiredStartQueryExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartQueryExecutionInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.26.4
-Summary: Type annotations for boto3.Athena 1.26.4 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.87
+Summary: Type annotations for boto3.Athena 1.26.87 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,147 +316,211 @@
 ### Literals
 
 `mypy_boto3_athena.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_athena.literals import (
+    CalculationExecutionStateType,
     ColumnNullableType,
     DataCatalogTypeType,
     EncryptionOptionType,
+    ExecutorStateType,
+    ExecutorTypeType,
     GetQueryResultsPaginatorName,
     ListDataCatalogsPaginatorName,
     ListDatabasesPaginatorName,
     ListNamedQueriesPaginatorName,
     ListQueryExecutionsPaginatorName,
     ListTableMetadataPaginatorName,
     ListTagsForResourcePaginatorName,
+    NotebookTypeType,
     QueryExecutionStateType,
     S3AclOptionType,
+    SessionStateType,
     StatementTypeType,
     WorkGroupStateType,
     AthenaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ColumnNullableType) -> bool:
+def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
+    ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
+    CalculationConfigurationTypeDef,
+    CalculationResultTypeDef,
+    CalculationStatisticsTypeDef,
+    CalculationStatusTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
+    CreateNotebookInputRequestTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
+    CreatePresignedNotebookUrlRequestRequestTypeDef,
+    CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
+    DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationTypeDef,
     EngineVersionTypeDef,
+    ExecutorsSummaryTypeDef,
+    ExportNotebookInputRequestTypeDef,
+    NotebookMetadataTypeDef,
+    FilterDefinitionTypeDef,
+    GetCalculationExecutionCodeRequestRequestTypeDef,
+    GetCalculationExecutionRequestRequestTypeDef,
+    GetCalculationExecutionStatusRequestRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
+    GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
     PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
+    GetSessionRequestRequestTypeDef,
+    SessionStatisticsTypeDef,
+    SessionStatusTypeDef,
+    GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
+    ImportNotebookInputRequestTypeDef,
+    ListApplicationDPUSizesInputRequestTypeDef,
+    ListCalculationExecutionsRequestRequestTypeDef,
     ListDataCatalogsInputRequestTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
+    ListExecutorsRequestRequestTypeDef,
     ListNamedQueriesInputRequestTypeDef,
+    ListNotebookSessionsRequestRequestTypeDef,
+    NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
+    ListSessionsRequestRequestTypeDef,
     ListTableMetadataInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
+    StopCalculationExecutionRequestRequestTypeDef,
     StopQueryExecutionInputRequestTypeDef,
+    TerminateSessionRequestRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
+    UpdateNotebookInputRequestTypeDef,
+    UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
     QueryExecutionStatusTypeDef,
     CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
     ListNamedQueriesOutputTypeDef,
     ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
+    StartCalculationExecutionRequestRequestTypeDef,
+    CalculationSummaryTypeDef,
+    GetCalculationExecutionResponseTypeDef,
+    GetCalculationExecutionStatusResponseTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
+    SessionConfigurationTypeDef,
+    StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
+    ListExecutorsResponseTypeDef,
+    ExportNotebookOutputTypeDef,
+    GetNotebookMetadataOutputTypeDef,
+    ListNotebookMetadataOutputTypeDef,
+    ListNotebookMetadataInputRequestTypeDef,
     GetQueryResultsInputGetQueryResultsPaginateTypeDef,
     ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDatabasesInputListDatabasesPaginateTypeDef,
     ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    GetSessionStatusResponseTypeDef,
+    SessionSummaryTypeDef,
+    ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
+    ListCalculationExecutionsResponseTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
+    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
+    ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
     CreateWorkGroupInputRequestTypeDef,
     WorkGroupTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
```

### Comparing `mypy-boto3-athena-1.26.4/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.26.87/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.26.4/setup.py` & `mypy-boto3-athena-1.26.87/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.26.4",
+    version="1.26.87",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Athena 1.26.4 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Athena 1.26.87 service generated with mypy-boto3-builder 7.12.5"
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
     keywords="boto3 athena type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_athena": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_athena": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

