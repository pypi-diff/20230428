# Comparing `tmp/iam_actions-1.2.20230427.tar.gz` & `tmp/iam_actions-1.2.20230428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230427.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230428.tar", max compression
```

## Comparing `iam_actions-1.2.20230427.tar` & `iam_actions-1.2.20230428.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/README.md
--rw-r--r--   0        0        0      228 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/__init__.py
--rw-r--r--   0        0        0  4228268 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/services.py
--rw-r--r--   0        0        0   544282 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/policies.json
--rw-r--r--   0        0        0   190316 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   527862 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-27 02:28:38.853130 iam_actions-1.2.20230427/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230427/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230427/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/README.md
+-rw-r--r--   0        0        0      228 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4233746 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545011 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/policies.json
+-rw-r--r--   0        0        0   190316 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   528566 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-28 02:29:09.361723 iam_actions-1.2.20230428/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230428/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230428/PKG-INFO
```

### Comparing `iam_actions-1.2.20230427/LICENSE` & `iam_actions-1.2.20230428/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/README.md` & `iam_actions-1.2.20230428/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/actions.json` & `iam_actions-1.2.20230428/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995879213818564%*

 * *Differences: {"'connect'": "{'DeleteContactEvaluation': OrderedDict([('access_level', 'Undocumented'), "*

 * *              "('action', 'DeleteContactEvaluation'), ('condition_keys', []), ('description', 'Not "*

 * *              "Documented by AWS'), ('orphan', False), ('resources', [])]), 'ListEvaluationForms': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', 'ListEvaluationForms'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), (' […]*

```diff
@@ -29310,14 +29310,22 @@
                 "OrganizationConfigRule",
                 "OrganizationConformancePack",
                 "StoredQuery"
             ]
         }
     },
     "connect": {
+        "ActivateEvaluationForm": {
+            "access_level": "Undocumented",
+            "action": "ActivateEvaluationForm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "AssociateApprovedOrigin": {
             "access_level": "Write",
             "action": "AssociateApprovedOrigin",
             "condition_keys": [
                 "connect:InstanceId"
             ],
             "description": "Grants permission to associate approved origin for an existing Amazon Connect instance",
@@ -29528,14 +29536,22 @@
             ],
             "description": "Grants permission to create a contact flow module in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact-flow-module"
             ]
         },
+        "CreateEvaluationForm": {
+            "access_level": "Undocumented",
+            "action": "CreateEvaluationForm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateHoursOfOperation": {
             "access_level": "Write",
             "action": "CreateHoursOfOperation",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "connect:InstanceId"
@@ -29743,14 +29759,30 @@
             ],
             "description": "Grants permission to create a vocabulary in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "vocabulary"
             ]
         },
+        "DeactivateEvaluationForm": {
+            "access_level": "Undocumented",
+            "action": "DeactivateEvaluationForm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteContactEvaluation": {
+            "access_level": "Undocumented",
+            "action": "DeleteContactEvaluation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteContactFlow": {
             "access_level": "Write",
             "action": "DeleteContactFlow",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -29769,14 +29801,22 @@
             ],
             "description": "Grants permission to delete a contact flow module in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact-flow-module"
             ]
         },
+        "DeleteEvaluationForm": {
+            "access_level": "Undocumented",
+            "action": "DeleteEvaluationForm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteHoursOfOperation": {
             "access_level": "Write",
             "action": "DeleteHoursOfOperation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -29948,14 +29988,22 @@
             ],
             "description": "Grants permission to describe a contact in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact"
             ]
         },
+        "DescribeContactEvaluation": {
+            "access_level": "Undocumented",
+            "action": "DescribeContactEvaluation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeContactFlow": {
             "access_level": "Read",
             "action": "DescribeContactFlow",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -29974,14 +30022,22 @@
             ],
             "description": "Grants permission to describe a contact flow module in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact-flow-module"
             ]
         },
+        "DescribeEvaluationForm": {
+            "access_level": "Undocumented",
+            "action": "DescribeEvaluationForm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeForecastingPlanningSchedulingIntegration": {
             "access_level": "Read",
             "action": "DescribeForecastingPlanningSchedulingIntegration",
             "condition_keys": [
                 "connect:InstanceId"
             ],
             "description": "Grants permission to describe the status of forecasting, planning, and scheduling integration on an Amazon Connect instance",
@@ -30459,14 +30515,22 @@
             ],
             "description": "Grants permission to view the Lex bots of an existing Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
+        "ListContactEvaluations": {
+            "access_level": "Undocumented",
+            "action": "ListContactEvaluations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListContactFlowModules": {
             "access_level": "List",
             "action": "ListContactFlowModules",
             "condition_keys": [],
             "description": "Grants permission to list contact flow module resources in an Amazon Connect instance",
             "orphan": false,
             "resources": [
@@ -30503,14 +30567,30 @@
             ],
             "description": "Grants permission to list default vocabularies associated with a Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
+        "ListEvaluationFormVersions": {
+            "access_level": "Undocumented",
+            "action": "ListEvaluationFormVersions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListEvaluationForms": {
+            "access_level": "Undocumented",
+            "action": "ListEvaluationForms",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListHoursOfOperations": {
             "access_level": "List",
             "action": "ListHoursOfOperations",
             "condition_keys": [
                 "connect:InstanceId"
             ],
             "description": "Grants permission to list hours of operation resources in an Amazon Connect instance",
@@ -30966,14 +31046,22 @@
             "description": "Grants permission to initiate a chat using the Amazon Connect API",
             "orphan": false,
             "resources": [
                 "contact",
                 "contact-flow"
             ]
         },
+        "StartContactEvaluation": {
+            "access_level": "Undocumented",
+            "action": "StartContactEvaluation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartContactRecording": {
             "access_level": "Write",
             "action": "StartContactRecording",
             "condition_keys": [],
             "description": "Grants permission to start recording for the specified contact",
             "orphan": false,
             "resources": [
@@ -31068,14 +31156,22 @@
             ],
             "description": "Grants permission to disable forecasting, planning, and scheduling integration on an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
+        "SubmitContactEvaluation": {
+            "access_level": "Undocumented",
+            "action": "SubmitContactEvaluation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SuspendContactRecording": {
             "access_level": "Write",
             "action": "SuspendContactRecording",
             "condition_keys": [],
             "description": "Grants permission to suspend recording for the specified contact",
             "orphan": false,
             "resources": [
@@ -31190,14 +31286,22 @@
             ],
             "description": "Grants permission to create or update the contact attributes associated with the specified contact",
             "orphan": false,
             "resources": [
                 "contact"
             ]
         },
+        "UpdateContactEvaluation": {
+            "access_level": "Undocumented",
+            "action": "UpdateContactEvaluation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateContactFlowContent": {
             "access_level": "Write",
             "action": "UpdateContactFlowContent",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -31267,14 +31371,22 @@
             ],
             "description": "Grants permission to update the schedule of a contact that is already scheduled in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact"
             ]
         },
+        "UpdateEvaluationForm": {
+            "access_level": "Undocumented",
+            "action": "UpdateEvaluationForm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateHoursOfOperation": {
             "access_level": "Write",
             "action": "UpdateHoursOfOperation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -59627,18 +59739,18 @@
             "action": "GetAdminAccount",
             "condition_keys": [],
             "description": "Grants permission to return the AWS Organizations account that is associated with AWS Firewall Manager as the AWS Firewall Manager administrator",
             "orphan": false,
             "resources": []
         },
         "GetAdminScope": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAdminScope",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return information about the specified account's administrative scope",
             "orphan": false,
             "resources": []
         },
         "GetAppsList": {
             "access_level": "Read",
             "action": "GetAppsList",
             "condition_keys": [],
@@ -59721,26 +59833,26 @@
             "description": "Grants permission to retrieve violations for a resource based on the specified AWS Firewall Manager policy and AWS account",
             "orphan": false,
             "resources": [
                 "policy"
             ]
         },
         "ListAdminAccountsForOrganization": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAdminAccountsForOrganization",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return a AdminAccounts object that lists the Firewall Manager administrators within the organization that are onboarded to Firewall Manager by AssociateAdminAccount",
             "orphan": false,
             "resources": []
         },
         "ListAdminsManagingAccount": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAdminsManagingAccount",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the accounts that are managing the specified AWS Organizations member account",
             "orphan": false,
             "resources": []
         },
         "ListAppsLists": {
             "access_level": "List",
             "action": "ListAppsLists",
             "condition_keys": [],
@@ -59823,18 +59935,18 @@
             "action": "ListThirdPartyFirewallFirewallPolicies",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all of the third-party firewall policies that are associated with the third-party firewall administrator's account",
             "orphan": false,
             "resources": []
         },
         "PutAdminAccount": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutAdminAccount",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create or update an Firewall Manager administrator account",
             "orphan": false,
             "resources": []
         },
         "PutAppsList": {
             "access_level": "Write",
             "action": "PutAppsList",
             "condition_keys": [
@@ -69489,14 +69601,22 @@
             "access_level": "Write",
             "action": "SendSecurityTelemetry",
             "condition_keys": [],
             "description": "Grants permission to send security telemetry for a specific GuardDuty account in a Region",
             "orphan": false,
             "resources": []
         },
+        "StartMalwareScan": {
+            "access_level": "Undocumented",
+            "action": "StartMalwareScan",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartMonitoringMembers": {
             "access_level": "Write",
             "action": "StartMonitoringMembers",
             "condition_keys": [],
             "description": "Grants permission to a GuardDuty administrator account to monitor findings from GuardDuty member accounts",
             "orphan": false,
             "resources": []
@@ -81272,30 +81392,54 @@
             "access_level": "Write",
             "action": "CreateConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create an MSK configuration",
             "orphan": false,
             "resources": []
         },
+        "CreateVpcConnection": {
+            "access_level": "Undocumented",
+            "action": "CreateVpcConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteCluster": {
             "access_level": "Write",
             "action": "DeleteCluster",
             "condition_keys": [],
             "description": "Grants permission to delete an MSK cluster",
             "orphan": false,
             "resources": []
         },
+        "DeleteClusterPolicy": {
+            "access_level": "Undocumented",
+            "action": "DeleteClusterPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteConfiguration": {
             "access_level": "Write",
             "action": "DeleteConfiguration",
             "condition_keys": [],
             "description": "Grants permission to delete the specified MSK configuration",
             "orphan": false,
             "resources": []
         },
+        "DeleteVpcConnection": {
+            "access_level": "Undocumented",
+            "action": "DeleteVpcConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeCluster": {
             "access_level": "Read",
             "action": "DescribeCluster",
             "condition_keys": [],
             "description": "Grants permission to describe an MSK cluster",
             "orphan": false,
             "resources": []
@@ -81332,30 +81476,54 @@
             "condition_keys": [],
             "description": "Grants permission to describe an MSK configuration revision",
             "orphan": false,
             "resources": [
                 "configuration"
             ]
         },
+        "DescribeVpcConnection": {
+            "access_level": "Undocumented",
+            "action": "DescribeVpcConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetBootstrapBrokers": {
             "access_level": "Read",
             "action": "GetBootstrapBrokers",
             "condition_keys": [],
             "description": "Grants permission to get connection details for the brokers in an MSK cluster",
             "orphan": false,
             "resources": []
         },
+        "GetClusterPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetClusterPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetCompatibleKafkaVersions": {
             "access_level": "List",
             "action": "GetCompatibleKafkaVersions",
             "condition_keys": [],
             "description": "Grants permission to get a list of the Apache Kafka versions to which you can update an MSK cluster",
             "orphan": false,
             "resources": []
         },
+        "ListClientVpcConnections": {
+            "access_level": "Undocumented",
+            "action": "ListClientVpcConnections",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListClusterOperations": {
             "access_level": "List",
             "action": "ListClusterOperations",
             "condition_keys": [],
             "description": "Grants permission to return a list of all the operations that have been performed on the specified MSK cluster",
             "orphan": false,
             "resources": []
@@ -81422,22 +81590,46 @@
             "condition_keys": [],
             "description": "Grants permission to list tags of an MSK resource",
             "orphan": false,
             "resources": [
                 "cluster"
             ]
         },
+        "ListVpcConnections": {
+            "access_level": "Undocumented",
+            "action": "ListVpcConnections",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutClusterPolicy": {
+            "access_level": "Undocumented",
+            "action": "PutClusterPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RebootBroker": {
             "access_level": "Write",
             "action": "RebootBroker",
             "condition_keys": [],
             "description": "Grants permission to reboot broker",
             "orphan": false,
             "resources": []
         },
+        "RejectClientVpcConnection": {
+            "access_level": "Undocumented",
+            "action": "RejectClientVpcConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
```

### Comparing `iam_actions-1.2.20230427/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230428/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230428/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/generate/generate.py` & `iam_actions-1.2.20230428/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230428/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230428/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/generate/services.py` & `iam_actions-1.2.20230428/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/policies.json` & `iam_actions-1.2.20230428/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999994025316116%*

 * *Differences: {"'serviceMap'": "{'Amazon GuardDuty': {'Actions': {insert: [(54, 'StartMalwareScan')]}}, 'Amazon "*

 * *                 "Connect': {'Actions': {insert: [(0, 'ActivateEvaluationForm'), (18, "*

 * *                 "'CreateEvaluationForm'), (34, 'DeactivateEvaluationForm'), (35, "*

 * *                 "'DeleteContactEvaluation'), (38, 'DeleteEvaluationForm'), (53, "*

 * *                 "'DescribeContactEvaluation'), (56, 'DescribeEvaluationForm'), (96, "*

 * *                 "'ListContactEvaluations'), (101, 'ListEvaluationForm […]*

```diff
@@ -11191,14 +11191,15 @@
                 "aws:TagKeys"
             ]
         },
         "Amazon Connect": {
             "ARNFormat": "arn:aws:connect:${Region}:${Account}:instance/${InstanceId}",
             "ARNRegex": "^arn:aws:connect:.+:.+:instance/.+",
             "Actions": [
+                "ActivateEvaluationForm",
                 "AssociateApprovedOrigin",
                 "AssociateBot",
                 "AssociateCustomerProfilesDomain",
                 "AssociateDefaultVocabulary",
                 "AssociateInstanceStorageConfig",
                 "AssociateLambdaFunction",
                 "AssociateLexBot",
@@ -11208,14 +11209,15 @@
                 "AssociateSecurityKey",
                 "BatchAssociateAnalyticsDataSet",
                 "BatchDisassociateAnalyticsDataSet",
                 "ClaimPhoneNumber",
                 "CreateAgentStatus",
                 "CreateContactFlow",
                 "CreateContactFlowModule",
+                "CreateEvaluationForm",
                 "CreateHoursOfOperation",
                 "CreateInstance",
                 "CreateIntegrationAssociation",
                 "CreateParticipant",
                 "CreateQueue",
                 "CreateQuickConnect",
                 "CreateRoutingProfile",
@@ -11223,32 +11225,37 @@
                 "CreateSecurityProfile",
                 "CreateTaskTemplate",
                 "CreateTrafficDistributionGroup",
                 "CreateUseCase",
                 "CreateUser",
                 "CreateUserHierarchyGroup",
                 "CreateVocabulary",
+                "DeactivateEvaluationForm",
+                "DeleteContactEvaluation",
                 "DeleteContactFlow",
                 "DeleteContactFlowModule",
+                "DeleteEvaluationForm",
                 "DeleteHoursOfOperation",
                 "DeleteInstance",
                 "DeleteIntegrationAssociation",
                 "DeleteQuickConnect",
                 "DeleteRule",
                 "DeleteSecurityProfile",
                 "DeleteTaskTemplate",
                 "DeleteTrafficDistributionGroup",
                 "DeleteUseCase",
                 "DeleteUser",
                 "DeleteUserHierarchyGroup",
                 "DeleteVocabulary",
                 "DescribeAgentStatus",
                 "DescribeContact",
+                "DescribeContactEvaluation",
                 "DescribeContactFlow",
                 "DescribeContactFlowModule",
+                "DescribeEvaluationForm",
                 "DescribeForecastingPlanningSchedulingIntegration",
                 "DescribeHoursOfOperation",
                 "DescribeInstance",
                 "DescribeInstanceAttribute",
                 "DescribeInstanceStorageConfig",
                 "DescribePhoneNumber",
                 "DescribeQueue",
@@ -11280,18 +11287,21 @@
                 "GetMetricData",
                 "GetMetricDataV2",
                 "GetTaskTemplate",
                 "GetTrafficDistribution",
                 "ListAgentStatuses",
                 "ListApprovedOrigins",
                 "ListBots",
+                "ListContactEvaluations",
                 "ListContactFlowModules",
                 "ListContactFlows",
                 "ListContactReferences",
                 "ListDefaultVocabularies",
+                "ListEvaluationFormVersions",
+                "ListEvaluationForms",
                 "ListHoursOfOperations",
                 "ListInstanceAttributes",
                 "ListInstanceStorageConfigs",
                 "ListInstances",
                 "ListIntegrationAssociations",
                 "ListLambdaFunctions",
                 "ListLexBots",
@@ -11322,36 +11332,40 @@
                 "SearchAvailablePhoneNumbers",
                 "SearchQueues",
                 "SearchRoutingProfiles",
                 "SearchSecurityProfiles",
                 "SearchUsers",
                 "SearchVocabularies",
                 "StartChatContact",
+                "StartContactEvaluation",
                 "StartContactRecording",
                 "StartContactStreaming",
                 "StartForecastingPlanningSchedulingIntegration",
                 "StartOutboundVoiceContact",
                 "StartTaskContact",
                 "StopContact",
                 "StopContactRecording",
                 "StopContactStreaming",
                 "StopForecastingPlanningSchedulingIntegration",
+                "SubmitContactEvaluation",
                 "SuspendContactRecording",
                 "TagResource",
                 "TransferContact",
                 "UntagResource",
                 "UpdateAgentStatus",
                 "UpdateContact",
                 "UpdateContactAttributes",
+                "UpdateContactEvaluation",
                 "UpdateContactFlowContent",
                 "UpdateContactFlowMetadata",
                 "UpdateContactFlowModuleContent",
                 "UpdateContactFlowModuleMetadata",
                 "UpdateContactFlowName",
                 "UpdateContactSchedule",
+                "UpdateEvaluationForm",
                 "UpdateHoursOfOperation",
                 "UpdateInstanceAttribute",
                 "UpdateInstanceStorageConfig",
                 "UpdateParticipantRoleConfig",
                 "UpdatePhoneNumber",
                 "UpdateQueueHoursOfOperation",
                 "UpdateQueueMaxContacts",
@@ -14084,14 +14098,15 @@
                 "ListInvitations",
                 "ListMembers",
                 "ListOrganizationAdminAccounts",
                 "ListPublishingDestinations",
                 "ListTagsForResource",
                 "ListThreatIntelSets",
                 "SendSecurityTelemetry",
+                "StartMalwareScan",
                 "StartMonitoringMembers",
                 "StopMonitoringMembers",
                 "TagResource",
                 "UnarchiveFindings",
                 "UntagResource",
                 "UpdateDetector",
                 "UpdateFilter",
@@ -15488,33 +15503,42 @@
             "ARNRegex": "^arn:aws:kafka:.+",
             "Actions": [
                 "BatchAssociateScramSecret",
                 "BatchDisassociateScramSecret",
                 "CreateCluster",
                 "CreateClusterV2",
                 "CreateConfiguration",
+                "CreateVpcConnection",
                 "DeleteCluster",
+                "DeleteClusterPolicy",
                 "DeleteConfiguration",
+                "DeleteVpcConnection",
                 "DescribeCluster",
                 "DescribeClusterOperation",
                 "DescribeClusterV2",
                 "DescribeConfiguration",
                 "DescribeConfigurationRevision",
+                "DescribeVpcConnection",
                 "GetBootstrapBrokers",
+                "GetClusterPolicy",
                 "GetCompatibleKafkaVersions",
+                "ListClientVpcConnections",
                 "ListClusterOperations",
                 "ListClusters",
                 "ListClustersV2",
                 "ListConfigurationRevisions",
                 "ListConfigurations",
                 "ListKafkaVersions",
                 "ListNodes",
                 "ListScramSecrets",
                 "ListTagsForResource",
+                "ListVpcConnections",
+                "PutClusterPolicy",
                 "RebootBroker",
+                "RejectClientVpcConnection",
                 "TagResource",
                 "UntagResource",
                 "UpdateBrokerCount",
                 "UpdateBrokerStorage",
                 "UpdateBrokerType",
                 "UpdateClusterConfiguration",
                 "UpdateClusterKafkaVersion",
@@ -15525,15 +15549,16 @@
                 "UpdateStorage"
             ],
             "HasResource": true,
             "StringPrefix": "kafka",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "kafka:publicAccessEnabled"
             ]
         },
         "Amazon Managed Streaming for Kafka Connect": {
             "ARNFormat": "arn:aws:kafkaconnect:${Region}:${Account}:${ResourceType}/${ResourceName}/${UUID}",
             "ARNRegex": "^arn:aws:kafkaconnect:.+",
             "Actions": [
                 "CreateConnector",
```

### Comparing `iam_actions-1.2.20230427/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230428/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230427/iam_actions/services.json` & `iam_actions-1.2.20230428/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999374080735973%*

 * *Differences: {"'connect'": "{'Actions': {insert: [(0, 'ActivateEvaluationForm'), (18, 'CreateEvaluationForm'), "*

 * *              "(34, 'DeactivateEvaluationForm'), (35, 'DeleteContactEvaluation'), (38, "*

 * *              "'DeleteEvaluationForm'), (53, 'DescribeContactEvaluation'), (56, "*

 * *              "'DescribeEvaluationForm'), (96, 'ListContactEvaluations'), (101, "*

 * *              "'ListEvaluationFormVersions'), (102, 'ListEvaluationForms'), (141, "*

 * *              "'StartContactEvaluation'), (151, 'SubmitContactEvaluation'), […]*

```diff
@@ -4497,14 +4497,15 @@
         "ARNFormats": [
             "arn:aws:connect:${Region}:${Account}:instance/${InstanceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:connect:.+:.+:instance/.+"
         ],
         "Actions": [
+            "ActivateEvaluationForm",
             "AssociateApprovedOrigin",
             "AssociateBot",
             "AssociateCustomerProfilesDomain",
             "AssociateDefaultVocabulary",
             "AssociateInstanceStorageConfig",
             "AssociateLambdaFunction",
             "AssociateLexBot",
@@ -4514,14 +4515,15 @@
             "AssociateSecurityKey",
             "BatchAssociateAnalyticsDataSet",
             "BatchDisassociateAnalyticsDataSet",
             "ClaimPhoneNumber",
             "CreateAgentStatus",
             "CreateContactFlow",
             "CreateContactFlowModule",
+            "CreateEvaluationForm",
             "CreateHoursOfOperation",
             "CreateInstance",
             "CreateIntegrationAssociation",
             "CreateParticipant",
             "CreateQueue",
             "CreateQuickConnect",
             "CreateRoutingProfile",
@@ -4529,32 +4531,37 @@
             "CreateSecurityProfile",
             "CreateTaskTemplate",
             "CreateTrafficDistributionGroup",
             "CreateUseCase",
             "CreateUser",
             "CreateUserHierarchyGroup",
             "CreateVocabulary",
+            "DeactivateEvaluationForm",
+            "DeleteContactEvaluation",
             "DeleteContactFlow",
             "DeleteContactFlowModule",
+            "DeleteEvaluationForm",
             "DeleteHoursOfOperation",
             "DeleteInstance",
             "DeleteIntegrationAssociation",
             "DeleteQuickConnect",
             "DeleteRule",
             "DeleteSecurityProfile",
             "DeleteTaskTemplate",
             "DeleteTrafficDistributionGroup",
             "DeleteUseCase",
             "DeleteUser",
             "DeleteUserHierarchyGroup",
             "DeleteVocabulary",
             "DescribeAgentStatus",
             "DescribeContact",
+            "DescribeContactEvaluation",
             "DescribeContactFlow",
             "DescribeContactFlowModule",
+            "DescribeEvaluationForm",
             "DescribeForecastingPlanningSchedulingIntegration",
             "DescribeHoursOfOperation",
             "DescribeInstance",
             "DescribeInstanceAttribute",
             "DescribeInstanceStorageConfig",
             "DescribePhoneNumber",
             "DescribeQueue",
@@ -4586,18 +4593,21 @@
             "GetMetricData",
             "GetMetricDataV2",
             "GetTaskTemplate",
             "GetTrafficDistribution",
             "ListAgentStatuses",
             "ListApprovedOrigins",
             "ListBots",
+            "ListContactEvaluations",
             "ListContactFlowModules",
             "ListContactFlows",
             "ListContactReferences",
             "ListDefaultVocabularies",
+            "ListEvaluationFormVersions",
+            "ListEvaluationForms",
             "ListHoursOfOperations",
             "ListInstanceAttributes",
             "ListInstanceStorageConfigs",
             "ListInstances",
             "ListIntegrationAssociations",
             "ListLambdaFunctions",
             "ListLexBots",
@@ -4628,36 +4638,40 @@
             "SearchAvailablePhoneNumbers",
             "SearchQueues",
             "SearchRoutingProfiles",
             "SearchSecurityProfiles",
             "SearchUsers",
             "SearchVocabularies",
             "StartChatContact",
+            "StartContactEvaluation",
             "StartContactRecording",
             "StartContactStreaming",
             "StartForecastingPlanningSchedulingIntegration",
             "StartOutboundVoiceContact",
             "StartTaskContact",
             "StopContact",
             "StopContactRecording",
             "StopContactStreaming",
             "StopForecastingPlanningSchedulingIntegration",
+            "SubmitContactEvaluation",
             "SuspendContactRecording",
             "TagResource",
             "TransferContact",
             "UntagResource",
             "UpdateAgentStatus",
             "UpdateContact",
             "UpdateContactAttributes",
+            "UpdateContactEvaluation",
             "UpdateContactFlowContent",
             "UpdateContactFlowMetadata",
             "UpdateContactFlowModuleContent",
             "UpdateContactFlowModuleMetadata",
             "UpdateContactFlowName",
             "UpdateContactSchedule",
+            "UpdateEvaluationForm",
             "UpdateHoursOfOperation",
             "UpdateInstanceAttribute",
             "UpdateInstanceStorageConfig",
             "UpdateParticipantRoleConfig",
             "UpdatePhoneNumber",
             "UpdateQueueHoursOfOperation",
             "UpdateQueueMaxContacts",
@@ -9512,14 +9526,15 @@
             "ListInvitations",
             "ListMembers",
             "ListOrganizationAdminAccounts",
             "ListPublishingDestinations",
             "ListTagsForResource",
             "ListThreatIntelSets",
             "SendSecurityTelemetry",
+            "StartMalwareScan",
             "StartMonitoringMembers",
             "StopMonitoringMembers",
             "TagResource",
             "UnarchiveFindings",
             "UntagResource",
             "UpdateDetector",
             "UpdateFilter",
@@ -11299,33 +11314,42 @@
         ],
         "Actions": [
             "BatchAssociateScramSecret",
             "BatchDisassociateScramSecret",
             "CreateCluster",
             "CreateClusterV2",
             "CreateConfiguration",
+            "CreateVpcConnection",
             "DeleteCluster",
+            "DeleteClusterPolicy",
             "DeleteConfiguration",
+            "DeleteVpcConnection",
             "DescribeCluster",
             "DescribeClusterOperation",
             "DescribeClusterV2",
             "DescribeConfiguration",
             "DescribeConfigurationRevision",
+            "DescribeVpcConnection",
             "GetBootstrapBrokers",
+            "GetClusterPolicy",
             "GetCompatibleKafkaVersions",
+            "ListClientVpcConnections",
             "ListClusterOperations",
             "ListClusters",
             "ListClustersV2",
             "ListConfigurationRevisions",
             "ListConfigurations",
             "ListKafkaVersions",
             "ListNodes",
             "ListScramSecrets",
             "ListTagsForResource",
+            "ListVpcConnections",
+            "PutClusterPolicy",
             "RebootBroker",
+            "RejectClientVpcConnection",
             "TagResource",
             "UntagResource",
             "UpdateBrokerCount",
             "UpdateBrokerStorage",
             "UpdateBrokerType",
             "UpdateClusterConfiguration",
             "UpdateClusterKafkaVersion",
@@ -11334,15 +11358,16 @@
             "UpdateMonitoring",
             "UpdateSecurity",
             "UpdateStorage"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys"
+            "aws:TagKeys",
+            "kafka:publicAccessEnabled"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Managed Streaming for Apache Kafka"
         ]
     },
     "kafka-cluster": {
```

### Comparing `iam_actions-1.2.20230427/pyproject.toml` & `iam_actions-1.2.20230428/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230427"
+version = "1.2.20230428"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230427/setup.py` & `iam_actions-1.2.20230428/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230427',
+    'version': '1.2.20230428',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230427/PKG-INFO` & `iam_actions-1.2.20230428/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230427
+Version: 1.2.20230428
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

