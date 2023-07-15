# Comparing `tmp/iam_actions-1.2.20230714.tar.gz` & `tmp/iam_actions-1.2.20230715.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230714.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230715.tar", max compression
```

## Comparing `iam_actions-1.2.20230714.tar` & `iam_actions-1.2.20230715.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/README.md
--rw-r--r--   0        0        0      228 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/__init__.py
--rw-r--r--   0        0        0  4364411 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-14 02:53:36.118198 iam_actions-1.2.20230714/iam_actions/generate/services.py
--rw-r--r--   0        0        0   561038 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544152 2023-07-14 02:55:21.750086 iam_actions-1.2.20230714/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-14 02:55:22.510083 iam_actions-1.2.20230714/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230714/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230714/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-15 02:56:00.980660 iam_actions-1.2.20230715/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-15 02:56:00.980660 iam_actions-1.2.20230715/README.md
+-rw-r--r--   0        0        0      228 2023-07-15 02:56:00.980660 iam_actions-1.2.20230715/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4368735 2023-07-15 02:57:50.003279 iam_actions-1.2.20230715/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-15 02:56:00.980660 iam_actions-1.2.20230715/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-15 02:56:00.980660 iam_actions-1.2.20230715/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-15 02:56:00.980660 iam_actions-1.2.20230715/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-15 02:56:00.984660 iam_actions-1.2.20230715/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-15 02:56:00.984660 iam_actions-1.2.20230715/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-15 02:56:00.984660 iam_actions-1.2.20230715/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-15 02:56:00.984660 iam_actions-1.2.20230715/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-15 02:56:00.984660 iam_actions-1.2.20230715/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   561929 2023-07-15 02:57:50.003279 iam_actions-1.2.20230715/iam_actions/policies.json
+-rw-r--r--   0        0        0   197396 2023-07-15 02:57:50.003279 iam_actions-1.2.20230715/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   545040 2023-07-15 02:57:50.003279 iam_actions-1.2.20230715/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-15 02:57:50.795267 iam_actions-1.2.20230715/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230715/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230715/PKG-INFO
```

### Comparing `iam_actions-1.2.20230714/LICENSE` & `iam_actions-1.2.20230715/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/README.md` & `iam_actions-1.2.20230715/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/actions.json` & `iam_actions-1.2.20230715/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972081713209016%*

 * *Differences: {"'bedrock'": "OrderedDict([('StopModelCustomizationJob', OrderedDict([('access_level', "*

 * *              "'Undocumented'), ('action', 'StopModelCustomizationJob'), ('condition_keys', []), "*

 * *              "('description', 'Not Documented by AWS'), ('orphan', False), ('resources', [])])), "*

 * *              "('ListTagsForResource', OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'ListTagsForResource'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *              "AWS'), (' […]*

```diff
@@ -12599,14 +12599,152 @@
             "description": "Grants permission to update an AWS Batch scheduling policy in your account",
             "orphan": false,
             "resources": [
                 "scheduling-policy"
             ]
         }
     },
+    "bedrock": {
+        "CreateModelCustomizationJob": {
+            "access_level": "Undocumented",
+            "action": "CreateModelCustomizationJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteCustomModel": {
+            "access_level": "Undocumented",
+            "action": "DeleteCustomModel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeletePrompt": {
+            "access_level": "Undocumented",
+            "action": "DeletePrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetCustomModel": {
+            "access_level": "Undocumented",
+            "action": "GetCustomModel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetModelCustomizationJob": {
+            "access_level": "Undocumented",
+            "action": "GetModelCustomizationJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPrompt": {
+            "access_level": "Undocumented",
+            "action": "GetPrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "InvokeModel": {
+            "access_level": "Undocumented",
+            "action": "InvokeModel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "InvokeModelWithResponseStream": {
+            "access_level": "Undocumented",
+            "action": "InvokeModelWithResponseStream",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListCustomModels": {
+            "access_level": "Undocumented",
+            "action": "ListCustomModels",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListFoundationModels": {
+            "access_level": "Undocumented",
+            "action": "ListFoundationModels",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListModelCustomizationJobs": {
+            "access_level": "Undocumented",
+            "action": "ListModelCustomizationJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPrompts": {
+            "access_level": "Undocumented",
+            "action": "ListPrompts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopModelCustomizationJob": {
+            "access_level": "Undocumented",
+            "action": "StopModelCustomizationJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePrompt": {
+            "access_level": "Undocumented",
+            "action": "UpdatePrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "billing": {
         "GetBillingData": {
             "access_level": "Read",
             "action": "GetBillingData",
             "condition_keys": [],
             "description": "Grants permission to perform queries on billing information",
             "orphan": false,
@@ -128830,14 +128968,22 @@
             "access_level": "Read",
             "action": "GetSagemakerServicecatalogPortfolioStatus",
             "condition_keys": [],
             "description": "Grants permission to get a SageMaker Service Catalog Portfolio",
             "orphan": false,
             "resources": []
         },
+        "GetScalingPolicyConfigurationRecommendation": {
+            "access_level": "Undocumented",
+            "action": "GetScalingPolicyConfigurationRecommendation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetSearchSuggestions": {
             "access_level": "Read",
             "action": "GetSearchSuggestions",
             "condition_keys": [],
             "description": "Grants permission to get search suggestions when provided with a keyword",
             "orphan": false,
             "resources": []
@@ -138718,14 +138864,30 @@
             "access_level": "Read",
             "action": "GetAccountSettings",
             "condition_keys": [],
             "description": "Grants permission to get account settings",
             "orphan": false,
             "resources": []
         },
+        "GetAutocompletionMetadata": {
+            "access_level": "Read",
+            "action": "GetAutocompletionMetadata",
+            "condition_keys": [],
+            "description": "Grants permission to get database structure metadata for auto-completion",
+            "orphan": false,
+            "resources": []
+        },
+        "GetAutocompletionResource": {
+            "access_level": "Read",
+            "action": "GetAutocompletionResource",
+            "condition_keys": [],
+            "description": "Grants permission to get database structure information for auto-completion",
+            "orphan": false,
+            "resources": []
+        },
         "GetChart": {
             "access_level": "Read",
             "action": "GetChart",
             "condition_keys": [],
             "description": "Grants permission to get charts on your account",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230714/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230715/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230715/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/generate/generate.py` & `iam_actions-1.2.20230715/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230715/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230715/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/generate/services.py` & `iam_actions-1.2.20230715/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230714/iam_actions/policies.json` & `iam_actions-1.2.20230715/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997371779169031%*

 * *Differences: {"'serviceMap'": "{'Amazon SageMaker': {'Actions': {insert: [(182, "*

 * *                 "'GetScalingPolicyConfigurationRecommendation')]}}, 'AWS SQL Workbench': "*

 * *                 "{'Actions': {insert: [(28, 'GetAutocompletionMetadata'), (29, "*

 * *                 "'GetAutocompletionResource')]}}, 'Amazon Bedrock': OrderedDict([('StringPrefix', "*

 * *                 "'bedrock'), ('Actions', ['CreateModelCustomizationJob', 'DeleteCustomModel', "*

 * *                 "'DeletePrompt', 'GetCustomModel', 'GetModelCustomizat […]*

```diff
@@ -7874,14 +7874,16 @@
                 "DeleteTab",
                 "DriverExecute",
                 "DuplicateNotebook",
                 "ExportNotebook",
                 "GenerateSession",
                 "GetAccountInfo",
                 "GetAccountSettings",
+                "GetAutocompletionMetadata",
+                "GetAutocompletionResource",
                 "GetChart",
                 "GetConnection",
                 "GetNotebook",
                 "GetNotebookVersion",
                 "GetQueryExecutionHistory",
                 "GetSavedQuery",
                 "GetSchemaInference",
@@ -10241,14 +10243,44 @@
             "StringPrefix": "athena",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "Amazon Bedrock": {
+            "ARNFormat": "arn:aws:bedrock:${Region}:${Account}:${ResourceType}/${ResourceId}",
+            "ARNRegex": "^arn:aws:bedrock:.*:.*:.+",
+            "Actions": [
+                "CreateModelCustomizationJob",
+                "DeleteCustomModel",
+                "DeletePrompt",
+                "GetCustomModel",
+                "GetModelCustomizationJob",
+                "GetPrompt",
+                "InvokeModel",
+                "InvokeModelWithResponseStream",
+                "ListCustomModels",
+                "ListFoundationModels",
+                "ListModelCustomizationJobs",
+                "ListPrompts",
+                "ListTagsForResource",
+                "StopModelCustomizationJob",
+                "TagResource",
+                "UntagResource",
+                "UpdatePrompt"
+            ],
+            "HasResource": true,
+            "StringPrefix": "bedrock",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "Amazon Braket": {
             "ARNFormat": "arn:aws:braket:{$Region}:{$AccountI}>:.+",
             "ARNRegex": "^arn:aws:braket::.+",
             "Actions": [
                 "CancelJob",
                 "CancelQuantumTask",
                 "CreateJob",
@@ -18834,14 +18866,15 @@
                 "GetDeployments",
                 "GetDeviceFleetReport",
                 "GetDeviceRegistration",
                 "GetLineageGroupPolicy",
                 "GetModelPackageGroupPolicy",
                 "GetRecord",
                 "GetSagemakerServicecatalogPortfolioStatus",
+                "GetScalingPolicyConfigurationRecommendation",
                 "GetSearchSuggestions",
                 "ImportHubContent",
                 "InvokeEndpoint",
                 "InvokeEndpointAsync",
                 "ListActions",
                 "ListAlgorithms",
                 "ListAliases",
```

### Comparing `iam_actions-1.2.20230714/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230715/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972527472527473%*

 * *Differences: {"'bedrock'": 'OrderedDict()'}*

```diff
@@ -802,14 +802,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "scheduling-policy": {
             "arn_pattern": "arn:*:batch:*:*:scheduling-policy/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "bedrock": {},
     "billing": {},
     "billingconductor": {
         "billinggroup": {
             "arn_pattern": "arn:*:billingconductor::*:billinggroup/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "customlineitem": {
```

### Comparing `iam_actions-1.2.20230714/iam_actions/services.json` & `iam_actions-1.2.20230715/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99724903259176%*

 * *Differences: {"'bedrock'": "OrderedDict([('Actions', ['CreateModelCustomizationJob', 'DeleteCustomModel', "*

 * *              "'DeletePrompt', 'GetCustomModel', 'GetModelCustomizationJob', 'GetPrompt', "*

 * *              "'InvokeModel', 'InvokeModelWithResponseStream', 'ListCustomModels', "*

 * *              "'ListFoundationModels', 'ListModelCustomizationJobs', 'ListPrompts', "*

 * *              "'ListTagsForResource', 'StopModelCustomizationJob', 'TagResource', 'UntagResource', "*

 * *              "'UpdatePrompt']), ('ServiceNames', ['A […]*

```diff
@@ -2025,14 +2025,50 @@
             "batch:User"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Batch"
         ]
     },
+    "bedrock": {
+        "ARNFormats": [
+            "arn:aws:bedrock:${Region}:${Account}:${ResourceType}/${ResourceId}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:bedrock:.*:.*:.+"
+        ],
+        "Actions": [
+            "CreateModelCustomizationJob",
+            "DeleteCustomModel",
+            "DeletePrompt",
+            "GetCustomModel",
+            "GetModelCustomizationJob",
+            "GetPrompt",
+            "InvokeModel",
+            "InvokeModelWithResponseStream",
+            "ListCustomModels",
+            "ListFoundationModels",
+            "ListModelCustomizationJobs",
+            "ListPrompts",
+            "ListTagsForResource",
+            "StopModelCustomizationJob",
+            "TagResource",
+            "UntagResource",
+            "UpdatePrompt"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "Amazon Bedrock"
+        ]
+    },
     "billing": {
         "ARNFormats": [],
         "ARNRegexes": [],
         "Actions": [
             "GetBillingData",
             "GetBillingDetails",
             "GetBillingNotifications",
@@ -17767,14 +17803,15 @@
             "GetDeployments",
             "GetDeviceFleetReport",
             "GetDeviceRegistration",
             "GetLineageGroupPolicy",
             "GetModelPackageGroupPolicy",
             "GetRecord",
             "GetSagemakerServicecatalogPortfolioStatus",
+            "GetScalingPolicyConfigurationRecommendation",
             "GetSearchSuggestions",
             "ImportHubContent",
             "InvokeEndpoint",
             "InvokeEndpointAsync",
             "ListActions",
             "ListAlgorithms",
             "ListAliases",
@@ -19256,14 +19293,16 @@
             "DeleteTab",
             "DriverExecute",
             "DuplicateNotebook",
             "ExportNotebook",
             "GenerateSession",
             "GetAccountInfo",
             "GetAccountSettings",
+            "GetAutocompletionMetadata",
+            "GetAutocompletionResource",
             "GetChart",
             "GetConnection",
             "GetNotebook",
             "GetNotebookVersion",
             "GetQueryExecutionHistory",
             "GetSavedQuery",
             "GetSchemaInference",
```

### Comparing `iam_actions-1.2.20230714/pyproject.toml` & `iam_actions-1.2.20230715/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230714"
+version = "1.2.20230715"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230714/setup.py` & `iam_actions-1.2.20230715/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230714',
+    'version': '1.2.20230715',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230714/PKG-INFO` & `iam_actions-1.2.20230715/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230714
+Version: 1.2.20230715
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

