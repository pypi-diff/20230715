# Comparing `tmp/mypy-boto3-connect-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-connect-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
```

## Comparing `mypy-boto3-connect-1.28.3.post1.tar` & `mypy-boto3-connect-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.903361 mypy-boto3-connect-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-14 16:17:59.899361 mypy-boto3-connect-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    47528 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   152776 2023-07-14 16:15:23.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   152528 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    54807 2023-07-14 16:15:24.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:22.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   234700 2023-07-14 16:15:31.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   234387 2023-07-14 16:15:27.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.899361 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 16:17:59.000000 mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.903361 mypy-boto3-connect-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-14 16:15:21.000000 mypy-boto3-connect-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.314243 mypy-boto3-connect-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47783 2023-07-15 06:38:32.314243 mypy-boto3-connect-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46292 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.290242 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151314 2023-07-15 06:35:51.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151066 2023-07-15 06:35:50.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-15 06:35:52.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-15 06:35:52.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-15 06:35:51.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-15 06:35:51.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   230292 2023-07-15 06:35:59.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   229979 2023-07-15 06:35:55.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.310243 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47783 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.314243 mypy-boto3-connect-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-connect-1.28.3.post1/LICENSE` & `mypy-boto3-connect-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post1/PKG-INFO` & `mypy-boto3-connect-1.28.3.post2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-connect
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.7
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 connect type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-connect"></a>
 
 # mypy-boto3-connect
 
 [![PyPI - mypy-boto3-connect](https://img.shields.io/pypi/v/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
@@ -47,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -578,103 +546,103 @@
 ### Typed dictionaries
 
 `mypy_boto3_connect.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connect.type_defs import (
-    ActionSummaryOutputTypeDef,
+    ActionSummaryTypeDef,
     ActivateEvaluationFormRequestRequestTypeDef,
-    ActivateEvaluationFormResponseOutputTypeDef,
-    AgentContactReferenceOutputTypeDef,
-    AgentInfoOutputTypeDef,
-    AgentStatusOutputTypeDef,
-    AgentStatusReferenceOutputTypeDef,
-    AgentStatusSummaryOutputTypeDef,
+    ActivateEvaluationFormResponseTypeDef,
+    AgentContactReferenceTypeDef,
+    AgentInfoTypeDef,
+    AgentStatusReferenceTypeDef,
+    AgentStatusSummaryTypeDef,
+    AgentStatusTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     AssociateApprovedOriginRequestRequestTypeDef,
     AssociateBotRequestRequestTypeDef,
     AssociateDefaultVocabularyRequestRequestTypeDef,
     AssociateInstanceStorageConfigRequestRequestTypeDef,
-    AssociateInstanceStorageConfigResponseOutputTypeDef,
+    AssociateInstanceStorageConfigResponseTypeDef,
     AssociateLambdaFunctionRequestRequestTypeDef,
     AssociateLexBotRequestRequestTypeDef,
     AssociatePhoneNumberContactFlowRequestRequestTypeDef,
     AssociateQueueQuickConnectsRequestRequestTypeDef,
     AssociateRoutingProfileQueuesRequestRequestTypeDef,
     AssociateSecurityKeyRequestRequestTypeDef,
-    AssociateSecurityKeyResponseOutputTypeDef,
-    AttachmentReferenceOutputTypeDef,
-    AttributeOutputTypeDef,
-    AvailableNumberSummaryOutputTypeDef,
+    AssociateSecurityKeyResponseTypeDef,
+    AttachmentReferenceTypeDef,
+    AttributeTypeDef,
+    AvailableNumberSummaryTypeDef,
     ChatMessageTypeDef,
     ChatParticipantRoleConfigTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberRequestRequestTypeDef,
-    ClaimPhoneNumberResponseOutputTypeDef,
-    ClaimedPhoneNumberSummaryOutputTypeDef,
+    ClaimPhoneNumberResponseTypeDef,
+    ClaimedPhoneNumberSummaryTypeDef,
     ContactFilterTypeDef,
-    ContactFlowModuleOutputTypeDef,
-    ContactFlowModuleSummaryOutputTypeDef,
-    ContactFlowOutputTypeDef,
-    ContactFlowSummaryOutputTypeDef,
-    ContactOutputTypeDef,
+    ContactFlowModuleSummaryTypeDef,
+    ContactFlowModuleTypeDef,
+    ContactFlowSummaryTypeDef,
+    ContactFlowTypeDef,
+    ContactTypeDef,
     ControlPlaneTagFilterTypeDef,
     CreateAgentStatusRequestRequestTypeDef,
-    CreateAgentStatusResponseOutputTypeDef,
+    CreateAgentStatusResponseTypeDef,
     CreateContactFlowModuleRequestRequestTypeDef,
-    CreateContactFlowModuleResponseOutputTypeDef,
+    CreateContactFlowModuleResponseTypeDef,
     CreateContactFlowRequestRequestTypeDef,
-    CreateContactFlowResponseOutputTypeDef,
+    CreateContactFlowResponseTypeDef,
     CreateEvaluationFormRequestRequestTypeDef,
-    CreateEvaluationFormResponseOutputTypeDef,
+    CreateEvaluationFormResponseTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
-    CreateHoursOfOperationResponseOutputTypeDef,
+    CreateHoursOfOperationResponseTypeDef,
     CreateInstanceRequestRequestTypeDef,
-    CreateInstanceResponseOutputTypeDef,
+    CreateInstanceResponseTypeDef,
     CreateIntegrationAssociationRequestRequestTypeDef,
-    CreateIntegrationAssociationResponseOutputTypeDef,
+    CreateIntegrationAssociationResponseTypeDef,
     CreateParticipantRequestRequestTypeDef,
-    CreateParticipantResponseOutputTypeDef,
+    CreateParticipantResponseTypeDef,
     CreatePromptRequestRequestTypeDef,
-    CreatePromptResponseOutputTypeDef,
+    CreatePromptResponseTypeDef,
     CreateQueueRequestRequestTypeDef,
-    CreateQueueResponseOutputTypeDef,
+    CreateQueueResponseTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
-    CreateQuickConnectResponseOutputTypeDef,
+    CreateQuickConnectResponseTypeDef,
     CreateRoutingProfileRequestRequestTypeDef,
-    CreateRoutingProfileResponseOutputTypeDef,
+    CreateRoutingProfileResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseOutputTypeDef,
+    CreateRuleResponseTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
-    CreateSecurityProfileResponseOutputTypeDef,
+    CreateSecurityProfileResponseTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
-    CreateTaskTemplateResponseOutputTypeDef,
+    CreateTaskTemplateResponseTypeDef,
     CreateTrafficDistributionGroupRequestRequestTypeDef,
-    CreateTrafficDistributionGroupResponseOutputTypeDef,
+    CreateTrafficDistributionGroupResponseTypeDef,
     CreateUseCaseRequestRequestTypeDef,
-    CreateUseCaseResponseOutputTypeDef,
+    CreateUseCaseResponseTypeDef,
     CreateUserHierarchyGroupRequestRequestTypeDef,
-    CreateUserHierarchyGroupResponseOutputTypeDef,
+    CreateUserHierarchyGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseOutputTypeDef,
+    CreateUserResponseTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    CreateVocabularyResponseOutputTypeDef,
-    CredentialsOutputTypeDef,
+    CreateVocabularyResponseTypeDef,
+    CredentialsTypeDef,
     CrossChannelBehaviorOutputTypeDef,
     CrossChannelBehaviorTypeDef,
-    CurrentMetricDataOutputTypeDef,
+    CurrentMetricDataTypeDef,
     CurrentMetricOutputTypeDef,
-    CurrentMetricResultOutputTypeDef,
+    CurrentMetricResultTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DateReferenceOutputTypeDef,
+    DateReferenceTypeDef,
     DeactivateEvaluationFormRequestRequestTypeDef,
-    DeactivateEvaluationFormResponseOutputTypeDef,
-    DefaultVocabularyOutputTypeDef,
+    DeactivateEvaluationFormResponseTypeDef,
+    DefaultVocabularyTypeDef,
     DeleteContactEvaluationRequestRequestTypeDef,
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
@@ -686,90 +654,89 @@
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
-    DeleteVocabularyResponseOutputTypeDef,
+    DeleteVocabularyResponseTypeDef,
     DescribeAgentStatusRequestRequestTypeDef,
-    DescribeAgentStatusResponseOutputTypeDef,
+    DescribeAgentStatusResponseTypeDef,
     DescribeContactEvaluationRequestRequestTypeDef,
-    DescribeContactEvaluationResponseOutputTypeDef,
+    DescribeContactEvaluationResponseTypeDef,
     DescribeContactFlowModuleRequestRequestTypeDef,
-    DescribeContactFlowModuleResponseOutputTypeDef,
+    DescribeContactFlowModuleResponseTypeDef,
     DescribeContactFlowRequestRequestTypeDef,
-    DescribeContactFlowResponseOutputTypeDef,
+    DescribeContactFlowResponseTypeDef,
     DescribeContactRequestRequestTypeDef,
-    DescribeContactResponseOutputTypeDef,
+    DescribeContactResponseTypeDef,
     DescribeEvaluationFormRequestRequestTypeDef,
-    DescribeEvaluationFormResponseOutputTypeDef,
+    DescribeEvaluationFormResponseTypeDef,
     DescribeHoursOfOperationRequestRequestTypeDef,
-    DescribeHoursOfOperationResponseOutputTypeDef,
+    DescribeHoursOfOperationResponseTypeDef,
     DescribeInstanceAttributeRequestRequestTypeDef,
-    DescribeInstanceAttributeResponseOutputTypeDef,
+    DescribeInstanceAttributeResponseTypeDef,
     DescribeInstanceRequestRequestTypeDef,
-    DescribeInstanceResponseOutputTypeDef,
+    DescribeInstanceResponseTypeDef,
     DescribeInstanceStorageConfigRequestRequestTypeDef,
-    DescribeInstanceStorageConfigResponseOutputTypeDef,
+    DescribeInstanceStorageConfigResponseTypeDef,
     DescribePhoneNumberRequestRequestTypeDef,
-    DescribePhoneNumberResponseOutputTypeDef,
+    DescribePhoneNumberResponseTypeDef,
     DescribePromptRequestRequestTypeDef,
-    DescribePromptResponseOutputTypeDef,
+    DescribePromptResponseTypeDef,
     DescribeQueueRequestRequestTypeDef,
-    DescribeQueueResponseOutputTypeDef,
+    DescribeQueueResponseTypeDef,
     DescribeQuickConnectRequestRequestTypeDef,
-    DescribeQuickConnectResponseOutputTypeDef,
+    DescribeQuickConnectResponseTypeDef,
     DescribeRoutingProfileRequestRequestTypeDef,
-    DescribeRoutingProfileResponseOutputTypeDef,
+    DescribeRoutingProfileResponseTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseOutputTypeDef,
+    DescribeRuleResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
-    DescribeSecurityProfileResponseOutputTypeDef,
+    DescribeSecurityProfileResponseTypeDef,
     DescribeTrafficDistributionGroupRequestRequestTypeDef,
-    DescribeTrafficDistributionGroupResponseOutputTypeDef,
+    DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupRequestRequestTypeDef,
-    DescribeUserHierarchyGroupResponseOutputTypeDef,
+    DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureRequestRequestTypeDef,
-    DescribeUserHierarchyStructureResponseOutputTypeDef,
+    DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseOutputTypeDef,
+    DescribeUserResponseTypeDef,
     DescribeVocabularyRequestRequestTypeDef,
-    DescribeVocabularyResponseOutputTypeDef,
-    DimensionsOutputTypeDef,
+    DescribeVocabularyResponseTypeDef,
+    DimensionsTypeDef,
     DisassociateApprovedOriginRequestRequestTypeDef,
     DisassociateBotRequestRequestTypeDef,
     DisassociateInstanceStorageConfigRequestRequestTypeDef,
     DisassociateLambdaFunctionRequestRequestTypeDef,
     DisassociateLexBotRequestRequestTypeDef,
     DisassociatePhoneNumberContactFlowRequestRequestTypeDef,
     DisassociateQueueQuickConnectsRequestRequestTypeDef,
     DisassociateRoutingProfileQueuesRequestRequestTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
-    EmailReferenceOutputTypeDef,
+    EmailReferenceTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     EvaluationAnswerDataOutputTypeDef,
     EvaluationAnswerDataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationAnswerOutputOutputTypeDef,
-    EvaluationFormContentOutputTypeDef,
+    EvaluationAnswerOutputTypeDef,
+    EvaluationFormContentTypeDef,
     EvaluationFormItemOutputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormNumericQuestionAutomationOutputTypeDef,
     EvaluationFormNumericQuestionAutomationTypeDef,
     EvaluationFormNumericQuestionOptionOutputTypeDef,
     EvaluationFormNumericQuestionOptionTypeDef,
     EvaluationFormNumericQuestionPropertiesOutputTypeDef,
     EvaluationFormNumericQuestionPropertiesTypeDef,
-    EvaluationFormOutputTypeDef,
     EvaluationFormQuestionOutputTypeDef,
     EvaluationFormQuestionTypeDef,
     EvaluationFormQuestionTypePropertiesOutputTypeDef,
     EvaluationFormQuestionTypePropertiesTypeDef,
     EvaluationFormScoringStrategyOutputTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationFormSectionOutputTypeDef,
@@ -778,424 +745,425 @@
     EvaluationFormSingleSelectQuestionAutomationOptionTypeDef,
     EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationTypeDef,
     EvaluationFormSingleSelectQuestionOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionOptionTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesTypeDef,
-    EvaluationFormSummaryOutputTypeDef,
-    EvaluationFormVersionSummaryOutputTypeDef,
-    EvaluationMetadataOutputTypeDef,
+    EvaluationFormSummaryTypeDef,
+    EvaluationFormTypeDef,
+    EvaluationFormVersionSummaryTypeDef,
+    EvaluationMetadataTypeDef,
     EvaluationNoteOutputTypeDef,
     EvaluationNoteTypeDef,
-    EvaluationOutputTypeDef,
-    EvaluationScoreOutputTypeDef,
-    EvaluationSummaryOutputTypeDef,
+    EvaluationScoreTypeDef,
+    EvaluationSummaryTypeDef,
+    EvaluationTypeDef,
     EventBridgeActionDefinitionOutputTypeDef,
     EventBridgeActionDefinitionTypeDef,
     FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
-    GetContactAttributesResponseOutputTypeDef,
+    GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataRequestRequestTypeDef,
-    GetCurrentMetricDataResponseOutputTypeDef,
+    GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataRequestRequestTypeDef,
-    GetCurrentUserDataResponseOutputTypeDef,
+    GetCurrentUserDataResponseTypeDef,
     GetFederationTokenRequestRequestTypeDef,
-    GetFederationTokenResponseOutputTypeDef,
+    GetFederationTokenResponseTypeDef,
     GetMetricDataRequestGetMetricDataPaginateTypeDef,
     GetMetricDataRequestRequestTypeDef,
-    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataResponseTypeDef,
     GetMetricDataV2RequestRequestTypeDef,
-    GetMetricDataV2ResponseOutputTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     GetPromptFileRequestRequestTypeDef,
-    GetPromptFileResponseOutputTypeDef,
+    GetPromptFileResponseTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
-    GetTaskTemplateResponseOutputTypeDef,
+    GetTaskTemplateResponseTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
-    GetTrafficDistributionResponseOutputTypeDef,
+    GetTrafficDistributionResponseTypeDef,
     HierarchyGroupConditionTypeDef,
-    HierarchyGroupOutputTypeDef,
-    HierarchyGroupSummaryOutputTypeDef,
-    HierarchyGroupSummaryReferenceOutputTypeDef,
-    HierarchyLevelOutputTypeDef,
+    HierarchyGroupSummaryReferenceTypeDef,
+    HierarchyGroupSummaryTypeDef,
+    HierarchyGroupTypeDef,
+    HierarchyLevelTypeDef,
     HierarchyLevelUpdateTypeDef,
-    HierarchyPathOutputTypeDef,
-    HierarchyPathReferenceOutputTypeDef,
-    HierarchyStructureOutputTypeDef,
+    HierarchyPathReferenceTypeDef,
+    HierarchyPathTypeDef,
+    HierarchyStructureTypeDef,
     HierarchyStructureUpdateTypeDef,
-    HistoricalMetricDataOutputTypeDef,
+    HistoricalMetricDataTypeDef,
     HistoricalMetricOutputTypeDef,
-    HistoricalMetricResultOutputTypeDef,
+    HistoricalMetricResultTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigOutputTypeDef,
     HoursOfOperationConfigTypeDef,
-    HoursOfOperationOutputTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    HoursOfOperationSummaryOutputTypeDef,
+    HoursOfOperationSummaryTypeDef,
     HoursOfOperationTimeSliceOutputTypeDef,
     HoursOfOperationTimeSliceTypeDef,
-    InstanceOutputTypeDef,
-    InstanceStatusReasonOutputTypeDef,
+    HoursOfOperationTypeDef,
+    InstanceStatusReasonTypeDef,
     InstanceStorageConfigOutputTypeDef,
     InstanceStorageConfigTypeDef,
-    InstanceSummaryOutputTypeDef,
-    IntegrationAssociationSummaryOutputTypeDef,
+    InstanceSummaryTypeDef,
+    InstanceTypeDef,
+    IntegrationAssociationSummaryTypeDef,
     InvisibleFieldInfoOutputTypeDef,
     InvisibleFieldInfoTypeDef,
     KinesisFirehoseConfigOutputTypeDef,
     KinesisFirehoseConfigTypeDef,
     KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
     KinesisVideoStreamConfigOutputTypeDef,
     KinesisVideoStreamConfigTypeDef,
-    LexBotConfigOutputTypeDef,
+    LexBotConfigTypeDef,
     LexBotOutputTypeDef,
     LexBotTypeDef,
     LexV2BotOutputTypeDef,
     LexV2BotTypeDef,
     ListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     ListAgentStatusRequestRequestTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
     ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     ListApprovedOriginsRequestRequestTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
+    ListApprovedOriginsResponseTypeDef,
     ListBotsRequestListBotsPaginateTypeDef,
     ListBotsRequestRequestTypeDef,
-    ListBotsResponseOutputTypeDef,
+    ListBotsResponseTypeDef,
     ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     ListContactEvaluationsRequestRequestTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactEvaluationsResponseTypeDef,
     ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     ListContactFlowModulesRequestRequestTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowModulesResponseTypeDef,
     ListContactFlowsRequestListContactFlowsPaginateTypeDef,
     ListContactFlowsRequestRequestTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
+    ListContactFlowsResponseTypeDef,
     ListContactReferencesRequestListContactReferencesPaginateTypeDef,
     ListContactReferencesRequestRequestTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
+    ListContactReferencesResponseTypeDef,
     ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     ListDefaultVocabulariesRequestRequestTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
     ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     ListEvaluationFormVersionsRequestRequestTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
     ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     ListEvaluationFormsRequestRequestTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormsResponseTypeDef,
     ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     ListHoursOfOperationsRequestRequestTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
     ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     ListInstanceAttributesRequestRequestTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstanceAttributesResponseTypeDef,
     ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     ListInstanceStorageConfigsRequestRequestTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseOutputTypeDef,
+    ListInstancesResponseTypeDef,
     ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     ListIntegrationAssociationsRequestRequestTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
     ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     ListLambdaFunctionsRequestRequestTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
     ListLexBotsRequestListLexBotsPaginateTypeDef,
     ListLexBotsRequestRequestTypeDef,
-    ListLexBotsResponseOutputTypeDef,
+    ListLexBotsResponseTypeDef,
     ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersSummaryOutputTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersSummaryTypeDef,
     ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef,
     ListPhoneNumbersV2RequestRequestTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
     ListPromptsRequestListPromptsPaginateTypeDef,
     ListPromptsRequestRequestTypeDef,
-    ListPromptsResponseOutputTypeDef,
+    ListPromptsResponseTypeDef,
     ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     ListQueueQuickConnectsRequestRequestTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResponseOutputTypeDef,
+    ListQueuesResponseTypeDef,
     ListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     ListQuickConnectsRequestRequestTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
+    ListQuickConnectsResponseTypeDef,
     ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     ListRoutingProfileQueuesRequestRequestTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
     ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     ListRoutingProfilesRequestRequestTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
+    ListRoutingProfilesResponseTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListRulesResponseOutputTypeDef,
+    ListRulesResponseTypeDef,
     ListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     ListSecurityKeysRequestRequestTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityKeysResponseTypeDef,
     ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     ListSecurityProfilePermissionsRequestRequestTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
     ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
+    ListSecurityProfilesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     ListTaskTemplatesRequestRequestTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
+    ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef,
     ListTrafficDistributionGroupsRequestRequestTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesRequestListUseCasesPaginateTypeDef,
     ListUseCasesRequestRequestTypeDef,
-    ListUseCasesResponseOutputTypeDef,
+    ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListUsersResponseTypeDef,
     MediaConcurrencyOutputTypeDef,
     MediaConcurrencyTypeDef,
-    MetricDataV2OutputTypeDef,
+    MetricDataV2TypeDef,
     MetricFilterV2OutputTypeDef,
     MetricFilterV2TypeDef,
-    MetricResultV2OutputTypeDef,
+    MetricResultV2TypeDef,
     MetricV2OutputTypeDef,
     MetricV2TypeDef,
     MonitorContactRequestRequestTypeDef,
-    MonitorContactResponseOutputTypeDef,
+    MonitorContactResponseTypeDef,
     NotificationRecipientTypeOutputTypeDef,
     NotificationRecipientTypeTypeDef,
-    NumberReferenceOutputTypeDef,
+    NumberReferenceTypeDef,
     NumericQuestionPropertyValueAutomationOutputTypeDef,
     NumericQuestionPropertyValueAutomationTypeDef,
     OutboundCallerConfigOutputTypeDef,
     OutboundCallerConfigTypeDef,
     PaginatorConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerConfigurationTypeDef,
     ParticipantTimerValueTypeDef,
-    ParticipantTokenCredentialsOutputTypeDef,
+    ParticipantTokenCredentialsTypeDef,
     PersistentChatTypeDef,
     PhoneNumberQuickConnectConfigOutputTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
-    PhoneNumberStatusOutputTypeDef,
-    PhoneNumberSummaryOutputTypeDef,
-    PromptOutputTypeDef,
+    PhoneNumberStatusTypeDef,
+    PhoneNumberSummaryTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
-    PromptSummaryOutputTypeDef,
+    PromptSummaryTypeDef,
+    PromptTypeDef,
     PutUserStatusRequestRequestTypeDef,
-    QueueInfoOutputTypeDef,
-    QueueOutputTypeDef,
+    QueueInfoTypeDef,
     QueueQuickConnectConfigOutputTypeDef,
     QueueQuickConnectConfigTypeDef,
-    QueueReferenceOutputTypeDef,
+    QueueReferenceTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
-    QueueSummaryOutputTypeDef,
+    QueueSummaryTypeDef,
+    QueueTypeDef,
     QuickConnectConfigOutputTypeDef,
     QuickConnectConfigTypeDef,
-    QuickConnectOutputTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
-    QuickConnectSummaryOutputTypeDef,
+    QuickConnectSummaryTypeDef,
+    QuickConnectTypeDef,
     ReadOnlyFieldInfoOutputTypeDef,
     ReadOnlyFieldInfoTypeDef,
     ReferenceOutputTypeDef,
-    ReferenceSummaryOutputTypeDef,
+    ReferenceSummaryTypeDef,
     ReferenceTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     ReplicateInstanceRequestRequestTypeDef,
-    ReplicateInstanceResponseOutputTypeDef,
+    ReplicateInstanceResponseTypeDef,
     RequiredFieldInfoOutputTypeDef,
     RequiredFieldInfoTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     ResponseMetadataTypeDef,
     ResumeContactRecordingRequestRequestTypeDef,
-    RoutingProfileOutputTypeDef,
-    RoutingProfileQueueConfigSummaryOutputTypeDef,
+    RoutingProfileQueueConfigSummaryTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
-    RoutingProfileReferenceOutputTypeDef,
+    RoutingProfileReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RoutingProfileSummaryOutputTypeDef,
+    RoutingProfileSummaryTypeDef,
+    RoutingProfileTypeDef,
     RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    RuleOutputTypeDef,
-    RuleSummaryOutputTypeDef,
+    RuleSummaryTypeDef,
     RuleTriggerEventSourceOutputTypeDef,
     RuleTriggerEventSourceTypeDef,
+    RuleTypeDef,
     S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SearchHoursOfOperationsRequestRequestTypeDef,
     SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
     SearchPromptsRequestRequestTypeDef,
     SearchPromptsRequestSearchPromptsPaginateTypeDef,
-    SearchPromptsResponseOutputTypeDef,
+    SearchPromptsResponseTypeDef,
     SearchQueuesRequestRequestTypeDef,
     SearchQueuesRequestSearchQueuesPaginateTypeDef,
-    SearchQueuesResponseOutputTypeDef,
+    SearchQueuesResponseTypeDef,
     SearchQuickConnectsRequestRequestTypeDef,
     SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
+    SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsRequestRequestTypeDef,
     SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
+    SearchResourceTagsResponseTypeDef,
     SearchRoutingProfilesRequestRequestTypeDef,
     SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
     SearchSecurityProfilesRequestRequestTypeDef,
     SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchUsersRequestSearchUsersPaginateTypeDef,
-    SearchUsersResponseOutputTypeDef,
+    SearchUsersResponseTypeDef,
     SearchVocabulariesRequestRequestTypeDef,
     SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
-    SecurityKeyOutputTypeDef,
-    SecurityProfileOutputTypeDef,
+    SearchVocabulariesResponseTypeDef,
+    SecurityKeyTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
-    SecurityProfileSearchSummaryOutputTypeDef,
-    SecurityProfileSummaryOutputTypeDef,
+    SecurityProfileSearchSummaryTypeDef,
+    SecurityProfileSummaryTypeDef,
+    SecurityProfileTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     SendNotificationActionDefinitionOutputTypeDef,
     SendNotificationActionDefinitionTypeDef,
     SingleSelectQuestionRuleCategoryAutomationOutputTypeDef,
     SingleSelectQuestionRuleCategoryAutomationTypeDef,
     StartChatContactRequestRequestTypeDef,
-    StartChatContactResponseOutputTypeDef,
+    StartChatContactResponseTypeDef,
     StartContactEvaluationRequestRequestTypeDef,
-    StartContactEvaluationResponseOutputTypeDef,
+    StartContactEvaluationResponseTypeDef,
     StartContactRecordingRequestRequestTypeDef,
     StartContactStreamingRequestRequestTypeDef,
-    StartContactStreamingResponseOutputTypeDef,
+    StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactRequestRequestTypeDef,
-    StartOutboundVoiceContactResponseOutputTypeDef,
+    StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactRequestRequestTypeDef,
-    StartTaskContactResponseOutputTypeDef,
+    StartTaskContactResponseTypeDef,
     StopContactRecordingRequestRequestTypeDef,
     StopContactRequestRequestTypeDef,
     StopContactStreamingRequestRequestTypeDef,
     StringConditionTypeDef,
-    StringReferenceOutputTypeDef,
+    StringReferenceTypeDef,
     SubmitContactEvaluationRequestRequestTypeDef,
-    SubmitContactEvaluationResponseOutputTypeDef,
+    SubmitContactEvaluationResponseTypeDef,
     SuspendContactRecordingRequestRequestTypeDef,
     TagConditionTypeDef,
     TagResourceRequestRequestTypeDef,
     TagSearchConditionTypeDef,
-    TagSetOutputTypeDef,
+    TagSetTypeDef,
     TaskActionDefinitionOutputTypeDef,
     TaskActionDefinitionTypeDef,
     TaskTemplateConstraintsOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultFieldValueOutputTypeDef,
     TaskTemplateDefaultFieldValueTypeDef,
     TaskTemplateDefaultsOutputTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldIdentifierOutputTypeDef,
     TaskTemplateFieldIdentifierTypeDef,
     TaskTemplateFieldOutputTypeDef,
     TaskTemplateFieldTypeDef,
-    TaskTemplateMetadataOutputTypeDef,
+    TaskTemplateMetadataTypeDef,
     TelephonyConfigOutputTypeDef,
     TelephonyConfigTypeDef,
     ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ThresholdV2OutputTypeDef,
     ThresholdV2TypeDef,
-    TrafficDistributionGroupOutputTypeDef,
-    TrafficDistributionGroupSummaryOutputTypeDef,
+    TrafficDistributionGroupSummaryTypeDef,
+    TrafficDistributionGroupTypeDef,
     TransferContactRequestRequestTypeDef,
-    TransferContactResponseOutputTypeDef,
+    TransferContactResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     UpdateContactAttributesRequestRequestTypeDef,
     UpdateContactEvaluationRequestRequestTypeDef,
-    UpdateContactEvaluationResponseOutputTypeDef,
+    UpdateContactEvaluationResponseTypeDef,
     UpdateContactFlowContentRequestRequestTypeDef,
     UpdateContactFlowMetadataRequestRequestTypeDef,
     UpdateContactFlowModuleContentRequestRequestTypeDef,
     UpdateContactFlowModuleMetadataRequestRequestTypeDef,
     UpdateContactFlowNameRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     UpdateContactScheduleRequestRequestTypeDef,
     UpdateEvaluationFormRequestRequestTypeDef,
-    UpdateEvaluationFormResponseOutputTypeDef,
+    UpdateEvaluationFormResponseTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     UpdateInstanceAttributeRequestRequestTypeDef,
     UpdateInstanceStorageConfigRequestRequestTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResponseOutputTypeDef,
+    UpdatePhoneNumberResponseTypeDef,
     UpdatePromptRequestRequestTypeDef,
-    UpdatePromptResponseOutputTypeDef,
+    UpdatePromptResponseTypeDef,
     UpdateQueueHoursOfOperationRequestRequestTypeDef,
     UpdateQueueMaxContactsRequestRequestTypeDef,
     UpdateQueueNameRequestRequestTypeDef,
     UpdateQueueOutboundCallerConfigRequestRequestTypeDef,
     UpdateQueueStatusRequestRequestTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     UpdateQuickConnectNameRequestRequestTypeDef,
     UpdateRoutingProfileConcurrencyRequestRequestTypeDef,
     UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef,
     UpdateRoutingProfileNameRequestRequestTypeDef,
     UpdateRoutingProfileQueuesRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
-    UpdateTaskTemplateResponseOutputTypeDef,
+    UpdateTaskTemplateResponseTypeDef,
     UpdateTrafficDistributionRequestRequestTypeDef,
     UpdateUserHierarchyGroupNameRequestRequestTypeDef,
     UpdateUserHierarchyRequestRequestTypeDef,
     UpdateUserHierarchyStructureRequestRequestTypeDef,
     UpdateUserIdentityInfoRequestRequestTypeDef,
     UpdateUserPhoneConfigRequestRequestTypeDef,
     UpdateUserRoutingProfileRequestRequestTypeDef,
     UpdateUserSecurityProfilesRequestRequestTypeDef,
-    UrlReferenceOutputTypeDef,
-    UseCaseOutputTypeDef,
+    UrlReferenceTypeDef,
+    UseCaseTypeDef,
     UserDataFiltersTypeDef,
-    UserDataOutputTypeDef,
-    UserIdentityInfoLiteOutputTypeDef,
+    UserDataTypeDef,
+    UserIdentityInfoLiteTypeDef,
     UserIdentityInfoOutputTypeDef,
     UserIdentityInfoTypeDef,
-    UserOutputTypeDef,
     UserPhoneConfigOutputTypeDef,
     UserPhoneConfigTypeDef,
     UserQuickConnectConfigOutputTypeDef,
     UserQuickConnectConfigTypeDef,
-    UserReferenceOutputTypeDef,
+    UserReferenceTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
-    UserSearchSummaryOutputTypeDef,
-    UserSummaryOutputTypeDef,
-    VocabularyOutputTypeDef,
-    VocabularySummaryOutputTypeDef,
+    UserSearchSummaryTypeDef,
+    UserSummaryTypeDef,
+    UserTypeDef,
+    VocabularySummaryTypeDef,
+    VocabularyTypeDef,
     VoiceRecordingConfigurationTypeDef,
-    WisdomInfoOutputTypeDef,
+    WisdomInfoTypeDef,
 )
 
 
-def get_structure() -> ActionSummaryOutputTypeDef:
+def get_structure() -> ActionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connect-1.28.3.post1/README.md` & `mypy-boto3-connect-1.28.3.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-connect
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 connect type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-connect"></a>
 
 # mypy-boto3-connect
 
 [![PyPI - mypy-boto3-connect](https://img.shields.io/pypi/v/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -546,103 +578,103 @@
 ### Typed dictionaries
 
 `mypy_boto3_connect.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connect.type_defs import (
-    ActionSummaryOutputTypeDef,
+    ActionSummaryTypeDef,
     ActivateEvaluationFormRequestRequestTypeDef,
-    ActivateEvaluationFormResponseOutputTypeDef,
-    AgentContactReferenceOutputTypeDef,
-    AgentInfoOutputTypeDef,
-    AgentStatusOutputTypeDef,
-    AgentStatusReferenceOutputTypeDef,
-    AgentStatusSummaryOutputTypeDef,
+    ActivateEvaluationFormResponseTypeDef,
+    AgentContactReferenceTypeDef,
+    AgentInfoTypeDef,
+    AgentStatusReferenceTypeDef,
+    AgentStatusSummaryTypeDef,
+    AgentStatusTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     AssociateApprovedOriginRequestRequestTypeDef,
     AssociateBotRequestRequestTypeDef,
     AssociateDefaultVocabularyRequestRequestTypeDef,
     AssociateInstanceStorageConfigRequestRequestTypeDef,
-    AssociateInstanceStorageConfigResponseOutputTypeDef,
+    AssociateInstanceStorageConfigResponseTypeDef,
     AssociateLambdaFunctionRequestRequestTypeDef,
     AssociateLexBotRequestRequestTypeDef,
     AssociatePhoneNumberContactFlowRequestRequestTypeDef,
     AssociateQueueQuickConnectsRequestRequestTypeDef,
     AssociateRoutingProfileQueuesRequestRequestTypeDef,
     AssociateSecurityKeyRequestRequestTypeDef,
-    AssociateSecurityKeyResponseOutputTypeDef,
-    AttachmentReferenceOutputTypeDef,
-    AttributeOutputTypeDef,
-    AvailableNumberSummaryOutputTypeDef,
+    AssociateSecurityKeyResponseTypeDef,
+    AttachmentReferenceTypeDef,
+    AttributeTypeDef,
+    AvailableNumberSummaryTypeDef,
     ChatMessageTypeDef,
     ChatParticipantRoleConfigTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberRequestRequestTypeDef,
-    ClaimPhoneNumberResponseOutputTypeDef,
-    ClaimedPhoneNumberSummaryOutputTypeDef,
+    ClaimPhoneNumberResponseTypeDef,
+    ClaimedPhoneNumberSummaryTypeDef,
     ContactFilterTypeDef,
-    ContactFlowModuleOutputTypeDef,
-    ContactFlowModuleSummaryOutputTypeDef,
-    ContactFlowOutputTypeDef,
-    ContactFlowSummaryOutputTypeDef,
-    ContactOutputTypeDef,
+    ContactFlowModuleSummaryTypeDef,
+    ContactFlowModuleTypeDef,
+    ContactFlowSummaryTypeDef,
+    ContactFlowTypeDef,
+    ContactTypeDef,
     ControlPlaneTagFilterTypeDef,
     CreateAgentStatusRequestRequestTypeDef,
-    CreateAgentStatusResponseOutputTypeDef,
+    CreateAgentStatusResponseTypeDef,
     CreateContactFlowModuleRequestRequestTypeDef,
-    CreateContactFlowModuleResponseOutputTypeDef,
+    CreateContactFlowModuleResponseTypeDef,
     CreateContactFlowRequestRequestTypeDef,
-    CreateContactFlowResponseOutputTypeDef,
+    CreateContactFlowResponseTypeDef,
     CreateEvaluationFormRequestRequestTypeDef,
-    CreateEvaluationFormResponseOutputTypeDef,
+    CreateEvaluationFormResponseTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
-    CreateHoursOfOperationResponseOutputTypeDef,
+    CreateHoursOfOperationResponseTypeDef,
     CreateInstanceRequestRequestTypeDef,
-    CreateInstanceResponseOutputTypeDef,
+    CreateInstanceResponseTypeDef,
     CreateIntegrationAssociationRequestRequestTypeDef,
-    CreateIntegrationAssociationResponseOutputTypeDef,
+    CreateIntegrationAssociationResponseTypeDef,
     CreateParticipantRequestRequestTypeDef,
-    CreateParticipantResponseOutputTypeDef,
+    CreateParticipantResponseTypeDef,
     CreatePromptRequestRequestTypeDef,
-    CreatePromptResponseOutputTypeDef,
+    CreatePromptResponseTypeDef,
     CreateQueueRequestRequestTypeDef,
-    CreateQueueResponseOutputTypeDef,
+    CreateQueueResponseTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
-    CreateQuickConnectResponseOutputTypeDef,
+    CreateQuickConnectResponseTypeDef,
     CreateRoutingProfileRequestRequestTypeDef,
-    CreateRoutingProfileResponseOutputTypeDef,
+    CreateRoutingProfileResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseOutputTypeDef,
+    CreateRuleResponseTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
-    CreateSecurityProfileResponseOutputTypeDef,
+    CreateSecurityProfileResponseTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
-    CreateTaskTemplateResponseOutputTypeDef,
+    CreateTaskTemplateResponseTypeDef,
     CreateTrafficDistributionGroupRequestRequestTypeDef,
-    CreateTrafficDistributionGroupResponseOutputTypeDef,
+    CreateTrafficDistributionGroupResponseTypeDef,
     CreateUseCaseRequestRequestTypeDef,
-    CreateUseCaseResponseOutputTypeDef,
+    CreateUseCaseResponseTypeDef,
     CreateUserHierarchyGroupRequestRequestTypeDef,
-    CreateUserHierarchyGroupResponseOutputTypeDef,
+    CreateUserHierarchyGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseOutputTypeDef,
+    CreateUserResponseTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    CreateVocabularyResponseOutputTypeDef,
-    CredentialsOutputTypeDef,
+    CreateVocabularyResponseTypeDef,
+    CredentialsTypeDef,
     CrossChannelBehaviorOutputTypeDef,
     CrossChannelBehaviorTypeDef,
-    CurrentMetricDataOutputTypeDef,
+    CurrentMetricDataTypeDef,
     CurrentMetricOutputTypeDef,
-    CurrentMetricResultOutputTypeDef,
+    CurrentMetricResultTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DateReferenceOutputTypeDef,
+    DateReferenceTypeDef,
     DeactivateEvaluationFormRequestRequestTypeDef,
-    DeactivateEvaluationFormResponseOutputTypeDef,
-    DefaultVocabularyOutputTypeDef,
+    DeactivateEvaluationFormResponseTypeDef,
+    DefaultVocabularyTypeDef,
     DeleteContactEvaluationRequestRequestTypeDef,
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
@@ -654,90 +686,89 @@
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
-    DeleteVocabularyResponseOutputTypeDef,
+    DeleteVocabularyResponseTypeDef,
     DescribeAgentStatusRequestRequestTypeDef,
-    DescribeAgentStatusResponseOutputTypeDef,
+    DescribeAgentStatusResponseTypeDef,
     DescribeContactEvaluationRequestRequestTypeDef,
-    DescribeContactEvaluationResponseOutputTypeDef,
+    DescribeContactEvaluationResponseTypeDef,
     DescribeContactFlowModuleRequestRequestTypeDef,
-    DescribeContactFlowModuleResponseOutputTypeDef,
+    DescribeContactFlowModuleResponseTypeDef,
     DescribeContactFlowRequestRequestTypeDef,
-    DescribeContactFlowResponseOutputTypeDef,
+    DescribeContactFlowResponseTypeDef,
     DescribeContactRequestRequestTypeDef,
-    DescribeContactResponseOutputTypeDef,
+    DescribeContactResponseTypeDef,
     DescribeEvaluationFormRequestRequestTypeDef,
-    DescribeEvaluationFormResponseOutputTypeDef,
+    DescribeEvaluationFormResponseTypeDef,
     DescribeHoursOfOperationRequestRequestTypeDef,
-    DescribeHoursOfOperationResponseOutputTypeDef,
+    DescribeHoursOfOperationResponseTypeDef,
     DescribeInstanceAttributeRequestRequestTypeDef,
-    DescribeInstanceAttributeResponseOutputTypeDef,
+    DescribeInstanceAttributeResponseTypeDef,
     DescribeInstanceRequestRequestTypeDef,
-    DescribeInstanceResponseOutputTypeDef,
+    DescribeInstanceResponseTypeDef,
     DescribeInstanceStorageConfigRequestRequestTypeDef,
-    DescribeInstanceStorageConfigResponseOutputTypeDef,
+    DescribeInstanceStorageConfigResponseTypeDef,
     DescribePhoneNumberRequestRequestTypeDef,
-    DescribePhoneNumberResponseOutputTypeDef,
+    DescribePhoneNumberResponseTypeDef,
     DescribePromptRequestRequestTypeDef,
-    DescribePromptResponseOutputTypeDef,
+    DescribePromptResponseTypeDef,
     DescribeQueueRequestRequestTypeDef,
-    DescribeQueueResponseOutputTypeDef,
+    DescribeQueueResponseTypeDef,
     DescribeQuickConnectRequestRequestTypeDef,
-    DescribeQuickConnectResponseOutputTypeDef,
+    DescribeQuickConnectResponseTypeDef,
     DescribeRoutingProfileRequestRequestTypeDef,
-    DescribeRoutingProfileResponseOutputTypeDef,
+    DescribeRoutingProfileResponseTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseOutputTypeDef,
+    DescribeRuleResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
-    DescribeSecurityProfileResponseOutputTypeDef,
+    DescribeSecurityProfileResponseTypeDef,
     DescribeTrafficDistributionGroupRequestRequestTypeDef,
-    DescribeTrafficDistributionGroupResponseOutputTypeDef,
+    DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupRequestRequestTypeDef,
-    DescribeUserHierarchyGroupResponseOutputTypeDef,
+    DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureRequestRequestTypeDef,
-    DescribeUserHierarchyStructureResponseOutputTypeDef,
+    DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseOutputTypeDef,
+    DescribeUserResponseTypeDef,
     DescribeVocabularyRequestRequestTypeDef,
-    DescribeVocabularyResponseOutputTypeDef,
-    DimensionsOutputTypeDef,
+    DescribeVocabularyResponseTypeDef,
+    DimensionsTypeDef,
     DisassociateApprovedOriginRequestRequestTypeDef,
     DisassociateBotRequestRequestTypeDef,
     DisassociateInstanceStorageConfigRequestRequestTypeDef,
     DisassociateLambdaFunctionRequestRequestTypeDef,
     DisassociateLexBotRequestRequestTypeDef,
     DisassociatePhoneNumberContactFlowRequestRequestTypeDef,
     DisassociateQueueQuickConnectsRequestRequestTypeDef,
     DisassociateRoutingProfileQueuesRequestRequestTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
-    EmailReferenceOutputTypeDef,
+    EmailReferenceTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     EvaluationAnswerDataOutputTypeDef,
     EvaluationAnswerDataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationAnswerOutputOutputTypeDef,
-    EvaluationFormContentOutputTypeDef,
+    EvaluationAnswerOutputTypeDef,
+    EvaluationFormContentTypeDef,
     EvaluationFormItemOutputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormNumericQuestionAutomationOutputTypeDef,
     EvaluationFormNumericQuestionAutomationTypeDef,
     EvaluationFormNumericQuestionOptionOutputTypeDef,
     EvaluationFormNumericQuestionOptionTypeDef,
     EvaluationFormNumericQuestionPropertiesOutputTypeDef,
     EvaluationFormNumericQuestionPropertiesTypeDef,
-    EvaluationFormOutputTypeDef,
     EvaluationFormQuestionOutputTypeDef,
     EvaluationFormQuestionTypeDef,
     EvaluationFormQuestionTypePropertiesOutputTypeDef,
     EvaluationFormQuestionTypePropertiesTypeDef,
     EvaluationFormScoringStrategyOutputTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationFormSectionOutputTypeDef,
@@ -746,424 +777,425 @@
     EvaluationFormSingleSelectQuestionAutomationOptionTypeDef,
     EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationTypeDef,
     EvaluationFormSingleSelectQuestionOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionOptionTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesTypeDef,
-    EvaluationFormSummaryOutputTypeDef,
-    EvaluationFormVersionSummaryOutputTypeDef,
-    EvaluationMetadataOutputTypeDef,
+    EvaluationFormSummaryTypeDef,
+    EvaluationFormTypeDef,
+    EvaluationFormVersionSummaryTypeDef,
+    EvaluationMetadataTypeDef,
     EvaluationNoteOutputTypeDef,
     EvaluationNoteTypeDef,
-    EvaluationOutputTypeDef,
-    EvaluationScoreOutputTypeDef,
-    EvaluationSummaryOutputTypeDef,
+    EvaluationScoreTypeDef,
+    EvaluationSummaryTypeDef,
+    EvaluationTypeDef,
     EventBridgeActionDefinitionOutputTypeDef,
     EventBridgeActionDefinitionTypeDef,
     FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
-    GetContactAttributesResponseOutputTypeDef,
+    GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataRequestRequestTypeDef,
-    GetCurrentMetricDataResponseOutputTypeDef,
+    GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataRequestRequestTypeDef,
-    GetCurrentUserDataResponseOutputTypeDef,
+    GetCurrentUserDataResponseTypeDef,
     GetFederationTokenRequestRequestTypeDef,
-    GetFederationTokenResponseOutputTypeDef,
+    GetFederationTokenResponseTypeDef,
     GetMetricDataRequestGetMetricDataPaginateTypeDef,
     GetMetricDataRequestRequestTypeDef,
-    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataResponseTypeDef,
     GetMetricDataV2RequestRequestTypeDef,
-    GetMetricDataV2ResponseOutputTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     GetPromptFileRequestRequestTypeDef,
-    GetPromptFileResponseOutputTypeDef,
+    GetPromptFileResponseTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
-    GetTaskTemplateResponseOutputTypeDef,
+    GetTaskTemplateResponseTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
-    GetTrafficDistributionResponseOutputTypeDef,
+    GetTrafficDistributionResponseTypeDef,
     HierarchyGroupConditionTypeDef,
-    HierarchyGroupOutputTypeDef,
-    HierarchyGroupSummaryOutputTypeDef,
-    HierarchyGroupSummaryReferenceOutputTypeDef,
-    HierarchyLevelOutputTypeDef,
+    HierarchyGroupSummaryReferenceTypeDef,
+    HierarchyGroupSummaryTypeDef,
+    HierarchyGroupTypeDef,
+    HierarchyLevelTypeDef,
     HierarchyLevelUpdateTypeDef,
-    HierarchyPathOutputTypeDef,
-    HierarchyPathReferenceOutputTypeDef,
-    HierarchyStructureOutputTypeDef,
+    HierarchyPathReferenceTypeDef,
+    HierarchyPathTypeDef,
+    HierarchyStructureTypeDef,
     HierarchyStructureUpdateTypeDef,
-    HistoricalMetricDataOutputTypeDef,
+    HistoricalMetricDataTypeDef,
     HistoricalMetricOutputTypeDef,
-    HistoricalMetricResultOutputTypeDef,
+    HistoricalMetricResultTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigOutputTypeDef,
     HoursOfOperationConfigTypeDef,
-    HoursOfOperationOutputTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    HoursOfOperationSummaryOutputTypeDef,
+    HoursOfOperationSummaryTypeDef,
     HoursOfOperationTimeSliceOutputTypeDef,
     HoursOfOperationTimeSliceTypeDef,
-    InstanceOutputTypeDef,
-    InstanceStatusReasonOutputTypeDef,
+    HoursOfOperationTypeDef,
+    InstanceStatusReasonTypeDef,
     InstanceStorageConfigOutputTypeDef,
     InstanceStorageConfigTypeDef,
-    InstanceSummaryOutputTypeDef,
-    IntegrationAssociationSummaryOutputTypeDef,
+    InstanceSummaryTypeDef,
+    InstanceTypeDef,
+    IntegrationAssociationSummaryTypeDef,
     InvisibleFieldInfoOutputTypeDef,
     InvisibleFieldInfoTypeDef,
     KinesisFirehoseConfigOutputTypeDef,
     KinesisFirehoseConfigTypeDef,
     KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
     KinesisVideoStreamConfigOutputTypeDef,
     KinesisVideoStreamConfigTypeDef,
-    LexBotConfigOutputTypeDef,
+    LexBotConfigTypeDef,
     LexBotOutputTypeDef,
     LexBotTypeDef,
     LexV2BotOutputTypeDef,
     LexV2BotTypeDef,
     ListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     ListAgentStatusRequestRequestTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
     ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     ListApprovedOriginsRequestRequestTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
+    ListApprovedOriginsResponseTypeDef,
     ListBotsRequestListBotsPaginateTypeDef,
     ListBotsRequestRequestTypeDef,
-    ListBotsResponseOutputTypeDef,
+    ListBotsResponseTypeDef,
     ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     ListContactEvaluationsRequestRequestTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactEvaluationsResponseTypeDef,
     ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     ListContactFlowModulesRequestRequestTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowModulesResponseTypeDef,
     ListContactFlowsRequestListContactFlowsPaginateTypeDef,
     ListContactFlowsRequestRequestTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
+    ListContactFlowsResponseTypeDef,
     ListContactReferencesRequestListContactReferencesPaginateTypeDef,
     ListContactReferencesRequestRequestTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
+    ListContactReferencesResponseTypeDef,
     ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     ListDefaultVocabulariesRequestRequestTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
     ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     ListEvaluationFormVersionsRequestRequestTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
     ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     ListEvaluationFormsRequestRequestTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormsResponseTypeDef,
     ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     ListHoursOfOperationsRequestRequestTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
     ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     ListInstanceAttributesRequestRequestTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstanceAttributesResponseTypeDef,
     ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     ListInstanceStorageConfigsRequestRequestTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseOutputTypeDef,
+    ListInstancesResponseTypeDef,
     ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     ListIntegrationAssociationsRequestRequestTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
     ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     ListLambdaFunctionsRequestRequestTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
     ListLexBotsRequestListLexBotsPaginateTypeDef,
     ListLexBotsRequestRequestTypeDef,
-    ListLexBotsResponseOutputTypeDef,
+    ListLexBotsResponseTypeDef,
     ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersSummaryOutputTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersSummaryTypeDef,
     ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef,
     ListPhoneNumbersV2RequestRequestTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
     ListPromptsRequestListPromptsPaginateTypeDef,
     ListPromptsRequestRequestTypeDef,
-    ListPromptsResponseOutputTypeDef,
+    ListPromptsResponseTypeDef,
     ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     ListQueueQuickConnectsRequestRequestTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResponseOutputTypeDef,
+    ListQueuesResponseTypeDef,
     ListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     ListQuickConnectsRequestRequestTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
+    ListQuickConnectsResponseTypeDef,
     ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     ListRoutingProfileQueuesRequestRequestTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
     ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     ListRoutingProfilesRequestRequestTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
+    ListRoutingProfilesResponseTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListRulesResponseOutputTypeDef,
+    ListRulesResponseTypeDef,
     ListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     ListSecurityKeysRequestRequestTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityKeysResponseTypeDef,
     ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     ListSecurityProfilePermissionsRequestRequestTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
     ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
+    ListSecurityProfilesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     ListTaskTemplatesRequestRequestTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
+    ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef,
     ListTrafficDistributionGroupsRequestRequestTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesRequestListUseCasesPaginateTypeDef,
     ListUseCasesRequestRequestTypeDef,
-    ListUseCasesResponseOutputTypeDef,
+    ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListUsersResponseTypeDef,
     MediaConcurrencyOutputTypeDef,
     MediaConcurrencyTypeDef,
-    MetricDataV2OutputTypeDef,
+    MetricDataV2TypeDef,
     MetricFilterV2OutputTypeDef,
     MetricFilterV2TypeDef,
-    MetricResultV2OutputTypeDef,
+    MetricResultV2TypeDef,
     MetricV2OutputTypeDef,
     MetricV2TypeDef,
     MonitorContactRequestRequestTypeDef,
-    MonitorContactResponseOutputTypeDef,
+    MonitorContactResponseTypeDef,
     NotificationRecipientTypeOutputTypeDef,
     NotificationRecipientTypeTypeDef,
-    NumberReferenceOutputTypeDef,
+    NumberReferenceTypeDef,
     NumericQuestionPropertyValueAutomationOutputTypeDef,
     NumericQuestionPropertyValueAutomationTypeDef,
     OutboundCallerConfigOutputTypeDef,
     OutboundCallerConfigTypeDef,
     PaginatorConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerConfigurationTypeDef,
     ParticipantTimerValueTypeDef,
-    ParticipantTokenCredentialsOutputTypeDef,
+    ParticipantTokenCredentialsTypeDef,
     PersistentChatTypeDef,
     PhoneNumberQuickConnectConfigOutputTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
-    PhoneNumberStatusOutputTypeDef,
-    PhoneNumberSummaryOutputTypeDef,
-    PromptOutputTypeDef,
+    PhoneNumberStatusTypeDef,
+    PhoneNumberSummaryTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
-    PromptSummaryOutputTypeDef,
+    PromptSummaryTypeDef,
+    PromptTypeDef,
     PutUserStatusRequestRequestTypeDef,
-    QueueInfoOutputTypeDef,
-    QueueOutputTypeDef,
+    QueueInfoTypeDef,
     QueueQuickConnectConfigOutputTypeDef,
     QueueQuickConnectConfigTypeDef,
-    QueueReferenceOutputTypeDef,
+    QueueReferenceTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
-    QueueSummaryOutputTypeDef,
+    QueueSummaryTypeDef,
+    QueueTypeDef,
     QuickConnectConfigOutputTypeDef,
     QuickConnectConfigTypeDef,
-    QuickConnectOutputTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
-    QuickConnectSummaryOutputTypeDef,
+    QuickConnectSummaryTypeDef,
+    QuickConnectTypeDef,
     ReadOnlyFieldInfoOutputTypeDef,
     ReadOnlyFieldInfoTypeDef,
     ReferenceOutputTypeDef,
-    ReferenceSummaryOutputTypeDef,
+    ReferenceSummaryTypeDef,
     ReferenceTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     ReplicateInstanceRequestRequestTypeDef,
-    ReplicateInstanceResponseOutputTypeDef,
+    ReplicateInstanceResponseTypeDef,
     RequiredFieldInfoOutputTypeDef,
     RequiredFieldInfoTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     ResponseMetadataTypeDef,
     ResumeContactRecordingRequestRequestTypeDef,
-    RoutingProfileOutputTypeDef,
-    RoutingProfileQueueConfigSummaryOutputTypeDef,
+    RoutingProfileQueueConfigSummaryTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
-    RoutingProfileReferenceOutputTypeDef,
+    RoutingProfileReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RoutingProfileSummaryOutputTypeDef,
+    RoutingProfileSummaryTypeDef,
+    RoutingProfileTypeDef,
     RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    RuleOutputTypeDef,
-    RuleSummaryOutputTypeDef,
+    RuleSummaryTypeDef,
     RuleTriggerEventSourceOutputTypeDef,
     RuleTriggerEventSourceTypeDef,
+    RuleTypeDef,
     S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SearchHoursOfOperationsRequestRequestTypeDef,
     SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
     SearchPromptsRequestRequestTypeDef,
     SearchPromptsRequestSearchPromptsPaginateTypeDef,
-    SearchPromptsResponseOutputTypeDef,
+    SearchPromptsResponseTypeDef,
     SearchQueuesRequestRequestTypeDef,
     SearchQueuesRequestSearchQueuesPaginateTypeDef,
-    SearchQueuesResponseOutputTypeDef,
+    SearchQueuesResponseTypeDef,
     SearchQuickConnectsRequestRequestTypeDef,
     SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
+    SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsRequestRequestTypeDef,
     SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
+    SearchResourceTagsResponseTypeDef,
     SearchRoutingProfilesRequestRequestTypeDef,
     SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
     SearchSecurityProfilesRequestRequestTypeDef,
     SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchUsersRequestSearchUsersPaginateTypeDef,
-    SearchUsersResponseOutputTypeDef,
+    SearchUsersResponseTypeDef,
     SearchVocabulariesRequestRequestTypeDef,
     SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
-    SecurityKeyOutputTypeDef,
-    SecurityProfileOutputTypeDef,
+    SearchVocabulariesResponseTypeDef,
+    SecurityKeyTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
-    SecurityProfileSearchSummaryOutputTypeDef,
-    SecurityProfileSummaryOutputTypeDef,
+    SecurityProfileSearchSummaryTypeDef,
+    SecurityProfileSummaryTypeDef,
+    SecurityProfileTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     SendNotificationActionDefinitionOutputTypeDef,
     SendNotificationActionDefinitionTypeDef,
     SingleSelectQuestionRuleCategoryAutomationOutputTypeDef,
     SingleSelectQuestionRuleCategoryAutomationTypeDef,
     StartChatContactRequestRequestTypeDef,
-    StartChatContactResponseOutputTypeDef,
+    StartChatContactResponseTypeDef,
     StartContactEvaluationRequestRequestTypeDef,
-    StartContactEvaluationResponseOutputTypeDef,
+    StartContactEvaluationResponseTypeDef,
     StartContactRecordingRequestRequestTypeDef,
     StartContactStreamingRequestRequestTypeDef,
-    StartContactStreamingResponseOutputTypeDef,
+    StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactRequestRequestTypeDef,
-    StartOutboundVoiceContactResponseOutputTypeDef,
+    StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactRequestRequestTypeDef,
-    StartTaskContactResponseOutputTypeDef,
+    StartTaskContactResponseTypeDef,
     StopContactRecordingRequestRequestTypeDef,
     StopContactRequestRequestTypeDef,
     StopContactStreamingRequestRequestTypeDef,
     StringConditionTypeDef,
-    StringReferenceOutputTypeDef,
+    StringReferenceTypeDef,
     SubmitContactEvaluationRequestRequestTypeDef,
-    SubmitContactEvaluationResponseOutputTypeDef,
+    SubmitContactEvaluationResponseTypeDef,
     SuspendContactRecordingRequestRequestTypeDef,
     TagConditionTypeDef,
     TagResourceRequestRequestTypeDef,
     TagSearchConditionTypeDef,
-    TagSetOutputTypeDef,
+    TagSetTypeDef,
     TaskActionDefinitionOutputTypeDef,
     TaskActionDefinitionTypeDef,
     TaskTemplateConstraintsOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultFieldValueOutputTypeDef,
     TaskTemplateDefaultFieldValueTypeDef,
     TaskTemplateDefaultsOutputTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldIdentifierOutputTypeDef,
     TaskTemplateFieldIdentifierTypeDef,
     TaskTemplateFieldOutputTypeDef,
     TaskTemplateFieldTypeDef,
-    TaskTemplateMetadataOutputTypeDef,
+    TaskTemplateMetadataTypeDef,
     TelephonyConfigOutputTypeDef,
     TelephonyConfigTypeDef,
     ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ThresholdV2OutputTypeDef,
     ThresholdV2TypeDef,
-    TrafficDistributionGroupOutputTypeDef,
-    TrafficDistributionGroupSummaryOutputTypeDef,
+    TrafficDistributionGroupSummaryTypeDef,
+    TrafficDistributionGroupTypeDef,
     TransferContactRequestRequestTypeDef,
-    TransferContactResponseOutputTypeDef,
+    TransferContactResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     UpdateContactAttributesRequestRequestTypeDef,
     UpdateContactEvaluationRequestRequestTypeDef,
-    UpdateContactEvaluationResponseOutputTypeDef,
+    UpdateContactEvaluationResponseTypeDef,
     UpdateContactFlowContentRequestRequestTypeDef,
     UpdateContactFlowMetadataRequestRequestTypeDef,
     UpdateContactFlowModuleContentRequestRequestTypeDef,
     UpdateContactFlowModuleMetadataRequestRequestTypeDef,
     UpdateContactFlowNameRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     UpdateContactScheduleRequestRequestTypeDef,
     UpdateEvaluationFormRequestRequestTypeDef,
-    UpdateEvaluationFormResponseOutputTypeDef,
+    UpdateEvaluationFormResponseTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     UpdateInstanceAttributeRequestRequestTypeDef,
     UpdateInstanceStorageConfigRequestRequestTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResponseOutputTypeDef,
+    UpdatePhoneNumberResponseTypeDef,
     UpdatePromptRequestRequestTypeDef,
-    UpdatePromptResponseOutputTypeDef,
+    UpdatePromptResponseTypeDef,
     UpdateQueueHoursOfOperationRequestRequestTypeDef,
     UpdateQueueMaxContactsRequestRequestTypeDef,
     UpdateQueueNameRequestRequestTypeDef,
     UpdateQueueOutboundCallerConfigRequestRequestTypeDef,
     UpdateQueueStatusRequestRequestTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     UpdateQuickConnectNameRequestRequestTypeDef,
     UpdateRoutingProfileConcurrencyRequestRequestTypeDef,
     UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef,
     UpdateRoutingProfileNameRequestRequestTypeDef,
     UpdateRoutingProfileQueuesRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
-    UpdateTaskTemplateResponseOutputTypeDef,
+    UpdateTaskTemplateResponseTypeDef,
     UpdateTrafficDistributionRequestRequestTypeDef,
     UpdateUserHierarchyGroupNameRequestRequestTypeDef,
     UpdateUserHierarchyRequestRequestTypeDef,
     UpdateUserHierarchyStructureRequestRequestTypeDef,
     UpdateUserIdentityInfoRequestRequestTypeDef,
     UpdateUserPhoneConfigRequestRequestTypeDef,
     UpdateUserRoutingProfileRequestRequestTypeDef,
     UpdateUserSecurityProfilesRequestRequestTypeDef,
-    UrlReferenceOutputTypeDef,
-    UseCaseOutputTypeDef,
+    UrlReferenceTypeDef,
+    UseCaseTypeDef,
     UserDataFiltersTypeDef,
-    UserDataOutputTypeDef,
-    UserIdentityInfoLiteOutputTypeDef,
+    UserDataTypeDef,
+    UserIdentityInfoLiteTypeDef,
     UserIdentityInfoOutputTypeDef,
     UserIdentityInfoTypeDef,
-    UserOutputTypeDef,
     UserPhoneConfigOutputTypeDef,
     UserPhoneConfigTypeDef,
     UserQuickConnectConfigOutputTypeDef,
     UserQuickConnectConfigTypeDef,
-    UserReferenceOutputTypeDef,
+    UserReferenceTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
-    UserSearchSummaryOutputTypeDef,
-    UserSummaryOutputTypeDef,
-    VocabularyOutputTypeDef,
-    VocabularySummaryOutputTypeDef,
+    UserSearchSummaryTypeDef,
+    UserSummaryTypeDef,
+    UserTypeDef,
+    VocabularySummaryTypeDef,
+    VocabularyTypeDef,
     VoiceRecordingConfigurationTypeDef,
-    WisdomInfoOutputTypeDef,
+    WisdomInfoTypeDef,
 )
 
 
-def get_structure() -> ActionSummaryOutputTypeDef:
+def get_structure() -> ActionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
-        " 7.14.7\nDocs:           "
+        "Type annotations for boto3.Connect 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
+        " 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.3.post1")
+    print("1.28.3.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,178 +91,178 @@
     SearchResourceTagsPaginator,
     SearchRoutingProfilesPaginator,
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 from .type_defs import (
-    ActivateEvaluationFormResponseOutputTypeDef,
+    ActivateEvaluationFormResponseTypeDef,
     AnswerMachineDetectionConfigTypeDef,
-    AssociateInstanceStorageConfigResponseOutputTypeDef,
-    AssociateSecurityKeyResponseOutputTypeDef,
+    AssociateInstanceStorageConfigResponseTypeDef,
+    AssociateSecurityKeyResponseTypeDef,
     ChatMessageTypeDef,
     ChatStreamingConfigurationTypeDef,
-    ClaimPhoneNumberResponseOutputTypeDef,
-    CreateAgentStatusResponseOutputTypeDef,
-    CreateContactFlowModuleResponseOutputTypeDef,
-    CreateContactFlowResponseOutputTypeDef,
-    CreateEvaluationFormResponseOutputTypeDef,
-    CreateHoursOfOperationResponseOutputTypeDef,
-    CreateInstanceResponseOutputTypeDef,
-    CreateIntegrationAssociationResponseOutputTypeDef,
-    CreateParticipantResponseOutputTypeDef,
-    CreatePromptResponseOutputTypeDef,
-    CreateQueueResponseOutputTypeDef,
-    CreateQuickConnectResponseOutputTypeDef,
-    CreateRoutingProfileResponseOutputTypeDef,
-    CreateRuleResponseOutputTypeDef,
-    CreateSecurityProfileResponseOutputTypeDef,
-    CreateTaskTemplateResponseOutputTypeDef,
-    CreateTrafficDistributionGroupResponseOutputTypeDef,
-    CreateUseCaseResponseOutputTypeDef,
-    CreateUserHierarchyGroupResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    CreateVocabularyResponseOutputTypeDef,
+    ClaimPhoneNumberResponseTypeDef,
+    CreateAgentStatusResponseTypeDef,
+    CreateContactFlowModuleResponseTypeDef,
+    CreateContactFlowResponseTypeDef,
+    CreateEvaluationFormResponseTypeDef,
+    CreateHoursOfOperationResponseTypeDef,
+    CreateInstanceResponseTypeDef,
+    CreateIntegrationAssociationResponseTypeDef,
+    CreateParticipantResponseTypeDef,
+    CreatePromptResponseTypeDef,
+    CreateQueueResponseTypeDef,
+    CreateQuickConnectResponseTypeDef,
+    CreateRoutingProfileResponseTypeDef,
+    CreateRuleResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateTaskTemplateResponseTypeDef,
+    CreateTrafficDistributionGroupResponseTypeDef,
+    CreateUseCaseResponseTypeDef,
+    CreateUserHierarchyGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DeactivateEvaluationFormResponseOutputTypeDef,
-    DeleteVocabularyResponseOutputTypeDef,
-    DescribeAgentStatusResponseOutputTypeDef,
-    DescribeContactEvaluationResponseOutputTypeDef,
-    DescribeContactFlowModuleResponseOutputTypeDef,
-    DescribeContactFlowResponseOutputTypeDef,
-    DescribeContactResponseOutputTypeDef,
-    DescribeEvaluationFormResponseOutputTypeDef,
-    DescribeHoursOfOperationResponseOutputTypeDef,
-    DescribeInstanceAttributeResponseOutputTypeDef,
-    DescribeInstanceResponseOutputTypeDef,
-    DescribeInstanceStorageConfigResponseOutputTypeDef,
-    DescribePhoneNumberResponseOutputTypeDef,
-    DescribePromptResponseOutputTypeDef,
-    DescribeQueueResponseOutputTypeDef,
-    DescribeQuickConnectResponseOutputTypeDef,
-    DescribeRoutingProfileResponseOutputTypeDef,
-    DescribeRuleResponseOutputTypeDef,
-    DescribeSecurityProfileResponseOutputTypeDef,
-    DescribeTrafficDistributionGroupResponseOutputTypeDef,
-    DescribeUserHierarchyGroupResponseOutputTypeDef,
-    DescribeUserHierarchyStructureResponseOutputTypeDef,
-    DescribeUserResponseOutputTypeDef,
-    DescribeVocabularyResponseOutputTypeDef,
+    DeactivateEvaluationFormResponseTypeDef,
+    DeleteVocabularyResponseTypeDef,
+    DescribeAgentStatusResponseTypeDef,
+    DescribeContactEvaluationResponseTypeDef,
+    DescribeContactFlowModuleResponseTypeDef,
+    DescribeContactFlowResponseTypeDef,
+    DescribeContactResponseTypeDef,
+    DescribeEvaluationFormResponseTypeDef,
+    DescribeHoursOfOperationResponseTypeDef,
+    DescribeInstanceAttributeResponseTypeDef,
+    DescribeInstanceResponseTypeDef,
+    DescribeInstanceStorageConfigResponseTypeDef,
+    DescribePhoneNumberResponseTypeDef,
+    DescribePromptResponseTypeDef,
+    DescribeQueueResponseTypeDef,
+    DescribeQuickConnectResponseTypeDef,
+    DescribeRoutingProfileResponseTypeDef,
+    DescribeRuleResponseTypeDef,
+    DescribeSecurityProfileResponseTypeDef,
+    DescribeTrafficDistributionGroupResponseTypeDef,
+    DescribeUserHierarchyGroupResponseTypeDef,
+    DescribeUserHierarchyStructureResponseTypeDef,
+    DescribeUserResponseTypeDef,
+    DescribeVocabularyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
-    GetContactAttributesResponseOutputTypeDef,
-    GetCurrentMetricDataResponseOutputTypeDef,
-    GetCurrentUserDataResponseOutputTypeDef,
-    GetFederationTokenResponseOutputTypeDef,
-    GetMetricDataResponseOutputTypeDef,
-    GetMetricDataV2ResponseOutputTypeDef,
-    GetPromptFileResponseOutputTypeDef,
-    GetTaskTemplateResponseOutputTypeDef,
-    GetTrafficDistributionResponseOutputTypeDef,
+    GetContactAttributesResponseTypeDef,
+    GetCurrentMetricDataResponseTypeDef,
+    GetCurrentUserDataResponseTypeDef,
+    GetFederationTokenResponseTypeDef,
+    GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
+    GetPromptFileResponseTypeDef,
+    GetTaskTemplateResponseTypeDef,
+    GetTrafficDistributionResponseTypeDef,
     HierarchyStructureUpdateTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
     InstanceStorageConfigTypeDef,
     LexBotTypeDef,
     LexV2BotTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
-    ListBotsResponseOutputTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
-    ListInstancesResponseOutputTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
-    ListLexBotsResponseOutputTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
-    ListPromptsResponseOutputTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
-    ListQueuesResponseOutputTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
-    ListRulesResponseOutputTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
-    ListUseCasesResponseOutputTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
+    ListApprovedOriginsResponseTypeDef,
+    ListBotsResponseTypeDef,
+    ListContactEvaluationsResponseTypeDef,
+    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowsResponseTypeDef,
+    ListContactReferencesResponseTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
+    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
+    ListInstanceAttributesResponseTypeDef,
+    ListInstancesResponseTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
+    ListLexBotsResponseTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
+    ListPromptsResponseTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
+    ListQueuesResponseTypeDef,
+    ListQuickConnectsResponseTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfilesResponseTypeDef,
+    ListRulesResponseTypeDef,
+    ListSecurityKeysResponseTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskTemplatesResponseTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
+    ListUseCasesResponseTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
+    ListUsersResponseTypeDef,
     MediaConcurrencyTypeDef,
     MetricV2TypeDef,
-    MonitorContactResponseOutputTypeDef,
+    MonitorContactResponseTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ReferenceTypeDef,
-    ReplicateInstanceResponseOutputTypeDef,
+    ReplicateInstanceResponseTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
     RuleActionTypeDef,
     RuleTriggerEventSourceTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
-    SearchPromptsResponseOutputTypeDef,
-    SearchQueuesResponseOutputTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
-    SearchUsersResponseOutputTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
+    SearchPromptsResponseTypeDef,
+    SearchQueuesResponseTypeDef,
+    SearchQuickConnectsResponseTypeDef,
+    SearchResourceTagsResponseTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
+    SearchUsersResponseTypeDef,
+    SearchVocabulariesResponseTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
-    StartChatContactResponseOutputTypeDef,
-    StartContactEvaluationResponseOutputTypeDef,
-    StartContactStreamingResponseOutputTypeDef,
-    StartOutboundVoiceContactResponseOutputTypeDef,
-    StartTaskContactResponseOutputTypeDef,
-    SubmitContactEvaluationResponseOutputTypeDef,
+    StartChatContactResponseTypeDef,
+    StartContactEvaluationResponseTypeDef,
+    StartContactStreamingResponseTypeDef,
+    StartOutboundVoiceContactResponseTypeDef,
+    StartTaskContactResponseTypeDef,
+    SubmitContactEvaluationResponseTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldTypeDef,
     TelephonyConfigTypeDef,
-    TransferContactResponseOutputTypeDef,
-    UpdateContactEvaluationResponseOutputTypeDef,
-    UpdateEvaluationFormResponseOutputTypeDef,
+    TransferContactResponseTypeDef,
+    UpdateContactEvaluationResponseTypeDef,
+    UpdateEvaluationFormResponseTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
-    UpdatePhoneNumberResponseOutputTypeDef,
-    UpdatePromptResponseOutputTypeDef,
-    UpdateTaskTemplateResponseOutputTypeDef,
+    UpdatePhoneNumberResponseTypeDef,
+    UpdatePromptResponseTypeDef,
+    UpdateTaskTemplateResponseTypeDef,
     UserDataFiltersTypeDef,
     UserIdentityInfoTypeDef,
     UserPhoneConfigTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
     VoiceRecordingConfigurationTypeDef,
 )
@@ -325,15 +325,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#exceptions)
         """
 
     def activate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> ActivateEvaluationFormResponseOutputTypeDef:
+    ) -> ActivateEvaluationFormResponseTypeDef:
         """
         Activates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.activate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#activate_evaluation_form)
         """
 
@@ -369,15 +369,15 @@
 
     def associate_instance_storage_config(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         StorageConfig: "InstanceStorageConfigTypeDef"
-    ) -> AssociateInstanceStorageConfigResponseOutputTypeDef:
+    ) -> AssociateInstanceStorageConfigResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_instance_storage_config)
         """
 
@@ -433,15 +433,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_routing_profile_queues)
         """
 
     def associate_security_key(
         self, *, InstanceId: str, Key: str
-    ) -> AssociateSecurityKeyResponseOutputTypeDef:
+    ) -> AssociateSecurityKeyResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_security_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_security_key)
         """
 
@@ -457,15 +457,15 @@
         self,
         *,
         TargetArn: str,
         PhoneNumber: str,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> ClaimPhoneNumberResponseOutputTypeDef:
+    ) -> ClaimPhoneNumberResponseTypeDef:
         """
         Claims an available phone number to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#claim_phone_number)
         """
@@ -483,15 +483,15 @@
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
         DisplayOrder: int = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateAgentStatusResponseOutputTypeDef:
+    ) -> CreateAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_agent_status)
         """
 
@@ -500,15 +500,15 @@
         *,
         InstanceId: str,
         Name: str,
         Type: ContactFlowTypeType,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateContactFlowResponseOutputTypeDef:
+    ) -> CreateContactFlowResponseTypeDef:
         """
         Creates a flow for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow)
         """
 
@@ -517,15 +517,15 @@
         *,
         InstanceId: str,
         Name: str,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> CreateContactFlowModuleResponseOutputTypeDef:
+    ) -> CreateContactFlowModuleResponseTypeDef:
         """
         Creates a flow module for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow_module)
         """
 
@@ -534,15 +534,15 @@
         *,
         InstanceId: str,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> CreateEvaluationFormResponseOutputTypeDef:
+    ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_evaluation_form)
         """
 
@@ -551,15 +551,15 @@
         *,
         InstanceId: str,
         Name: str,
         TimeZone: str,
         Config: Sequence["HoursOfOperationConfigTypeDef"],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateHoursOfOperationResponseOutputTypeDef:
+    ) -> CreateHoursOfOperationResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_hours_of_operation)
         """
 
@@ -568,15 +568,15 @@
         *,
         IdentityManagementType: DirectoryTypeType,
         InboundCallsEnabled: bool,
         OutboundCallsEnabled: bool,
         ClientToken: str = ...,
         InstanceAlias: str = ...,
         DirectoryId: str = ...
-    ) -> CreateInstanceResponseOutputTypeDef:
+    ) -> CreateInstanceResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_instance)
         """
 
@@ -586,15 +586,15 @@
         InstanceId: str,
         IntegrationType: IntegrationTypeType,
         IntegrationArn: str,
         SourceApplicationUrl: str = ...,
         SourceApplicationName: str = ...,
         SourceType: SourceTypeType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateIntegrationAssociationResponseOutputTypeDef:
+    ) -> CreateIntegrationAssociationResponseTypeDef:
         """
         Creates an Amazon Web Services resource association with an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_integration_association)
         """
@@ -602,15 +602,15 @@
     def create_participant(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ParticipantDetails: "ParticipantDetailsToAddTypeDef",
         ClientToken: str = ...
-    ) -> CreateParticipantResponseOutputTypeDef:
+    ) -> CreateParticipantResponseTypeDef:
         """
         Adds a new participant into an on-going chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_participant)
         """
 
@@ -618,15 +618,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         S3Uri: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreatePromptResponseOutputTypeDef:
+    ) -> CreatePromptResponseTypeDef:
         """
         Creates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_prompt)
         """
 
@@ -637,15 +637,15 @@
         Name: str,
         HoursOfOperationId: str,
         Description: str = ...,
         OutboundCallerConfig: "OutboundCallerConfigTypeDef" = ...,
         MaxContacts: int = ...,
         QuickConnectIds: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQueueResponseOutputTypeDef:
+    ) -> CreateQueueResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_queue)
         """
 
@@ -653,15 +653,15 @@
         self,
         *,
         InstanceId: str,
         Name: str,
         QuickConnectConfig: "QuickConnectConfigTypeDef",
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQuickConnectResponseOutputTypeDef:
+    ) -> CreateQuickConnectResponseTypeDef:
         """
         Creates a quick connect for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_quick_connect)
         """
 
@@ -671,15 +671,15 @@
         InstanceId: str,
         Name: str,
         Description: str,
         DefaultOutboundQueueId: str,
         MediaConcurrencies: Sequence["MediaConcurrencyTypeDef"],
         QueueConfigs: Sequence["RoutingProfileQueueConfigTypeDef"] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateRoutingProfileResponseOutputTypeDef:
+    ) -> CreateRoutingProfileResponseTypeDef:
         """
         Creates a new routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_routing_profile)
         """
 
@@ -689,15 +689,15 @@
         InstanceId: str,
         Name: str,
         TriggerEventSource: "RuleTriggerEventSourceTypeDef",
         Function: str,
         Actions: Sequence["RuleActionTypeDef"],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...
-    ) -> CreateRuleResponseOutputTypeDef:
+    ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_rule)
         """
 
@@ -707,15 +707,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...
-    ) -> CreateSecurityProfileResponseOutputTypeDef:
+    ) -> CreateSecurityProfileResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_security_profile)
         """
 
@@ -727,15 +727,15 @@
         Fields: Sequence["TaskTemplateFieldTypeDef"],
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...
-    ) -> CreateTaskTemplateResponseOutputTypeDef:
+    ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_task_template)
         """
 
@@ -743,15 +743,15 @@
         self,
         *,
         Name: str,
         InstanceId: str,
         Description: str = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateTrafficDistributionGroupResponseOutputTypeDef:
+    ) -> CreateTrafficDistributionGroupResponseTypeDef:
         """
         Creates a traffic distribution group given an Amazon Connect instance that has
         been replicated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_traffic_distribution_group)
         """
@@ -759,15 +759,15 @@
     def create_use_case(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         UseCaseType: UseCaseTypeType,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUseCaseResponseOutputTypeDef:
+    ) -> CreateUseCaseResponseTypeDef:
         """
         Creates a use case for an integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_use_case)
         """
 
@@ -780,25 +780,25 @@
         RoutingProfileId: str,
         InstanceId: str,
         Password: str = ...,
         IdentityInfo: "UserIdentityInfoTypeDef" = ...,
         DirectoryUserId: str = ...,
         HierarchyGroupId: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUserResponseOutputTypeDef:
+    ) -> CreateUserResponseTypeDef:
         """
         Creates a user account for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user)
         """
 
     def create_user_hierarchy_group(
         self, *, Name: str, InstanceId: str, ParentGroupId: str = ..., Tags: Mapping[str, str] = ...
-    ) -> CreateUserHierarchyGroupResponseOutputTypeDef:
+    ) -> CreateUserHierarchyGroupResponseTypeDef:
         """
         Creates a new user hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user_hierarchy_group)
         """
 
@@ -807,25 +807,25 @@
         *,
         InstanceId: str,
         VocabularyName: str,
         LanguageCode: VocabularyLanguageCodeType,
         Content: str,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVocabularyResponseOutputTypeDef:
+    ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a custom vocabulary associated with your Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_vocabulary)
         """
 
     def deactivate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> DeactivateEvaluationFormResponseOutputTypeDef:
+    ) -> DeactivateEvaluationFormResponseTypeDef:
         """
         Deactivates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#deactivate_evaluation_form)
         """
 
@@ -994,230 +994,224 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_user_hierarchy_group)
         """
 
     def delete_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DeleteVocabularyResponseOutputTypeDef:
+    ) -> DeleteVocabularyResponseTypeDef:
         """
         Deletes the vocabulary that has the given identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_vocabulary)
         """
 
     def describe_agent_status(
         self, *, InstanceId: str, AgentStatusId: str
-    ) -> DescribeAgentStatusResponseOutputTypeDef:
+    ) -> DescribeAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_agent_status)
         """
 
     def describe_contact(
         self, *, InstanceId: str, ContactId: str
-    ) -> DescribeContactResponseOutputTypeDef:
+    ) -> DescribeContactResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact)
         """
 
     def describe_contact_evaluation(
         self, *, InstanceId: str, EvaluationId: str
-    ) -> DescribeContactEvaluationResponseOutputTypeDef:
+    ) -> DescribeContactEvaluationResponseTypeDef:
         """
         Describes a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_evaluation)
         """
 
     def describe_contact_flow(
         self, *, InstanceId: str, ContactFlowId: str
-    ) -> DescribeContactFlowResponseOutputTypeDef:
+    ) -> DescribeContactFlowResponseTypeDef:
         """
         Describes the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow)
         """
 
     def describe_contact_flow_module(
         self, *, InstanceId: str, ContactFlowModuleId: str
-    ) -> DescribeContactFlowModuleResponseOutputTypeDef:
+    ) -> DescribeContactFlowModuleResponseTypeDef:
         """
         Describes the specified flow module.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow_module)
         """
 
     def describe_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int = ...
-    ) -> DescribeEvaluationFormResponseOutputTypeDef:
+    ) -> DescribeEvaluationFormResponseTypeDef:
         """
         Describes an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_evaluation_form)
         """
 
     def describe_hours_of_operation(
         self, *, InstanceId: str, HoursOfOperationId: str
-    ) -> DescribeHoursOfOperationResponseOutputTypeDef:
+    ) -> DescribeHoursOfOperationResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_hours_of_operation)
         """
 
-    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseOutputTypeDef:
+    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance)
         """
 
     def describe_instance_attribute(
         self, *, InstanceId: str, AttributeType: InstanceAttributeTypeType
-    ) -> DescribeInstanceAttributeResponseOutputTypeDef:
+    ) -> DescribeInstanceAttributeResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_attribute)
         """
 
     def describe_instance_storage_config(
         self, *, InstanceId: str, AssociationId: str, ResourceType: InstanceStorageResourceTypeType
-    ) -> DescribeInstanceStorageConfigResponseOutputTypeDef:
+    ) -> DescribeInstanceStorageConfigResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_storage_config)
         """
 
-    def describe_phone_number(
-        self, *, PhoneNumberId: str
-    ) -> DescribePhoneNumberResponseOutputTypeDef:
+    def describe_phone_number(self, *, PhoneNumberId: str) -> DescribePhoneNumberResponseTypeDef:
         """
         Gets details and status of a phone number that’s claimed to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_phone_number)
         """
 
-    def describe_prompt(
-        self, *, InstanceId: str, PromptId: str
-    ) -> DescribePromptResponseOutputTypeDef:
+    def describe_prompt(self, *, InstanceId: str, PromptId: str) -> DescribePromptResponseTypeDef:
         """
         Describes the prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_prompt)
         """
 
-    def describe_queue(
-        self, *, InstanceId: str, QueueId: str
-    ) -> DescribeQueueResponseOutputTypeDef:
+    def describe_queue(self, *, InstanceId: str, QueueId: str) -> DescribeQueueResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_queue)
         """
 
     def describe_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
-    ) -> DescribeQuickConnectResponseOutputTypeDef:
+    ) -> DescribeQuickConnectResponseTypeDef:
         """
         Describes the quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_quick_connect)
         """
 
     def describe_routing_profile(
         self, *, InstanceId: str, RoutingProfileId: str
-    ) -> DescribeRoutingProfileResponseOutputTypeDef:
+    ) -> DescribeRoutingProfileResponseTypeDef:
         """
         Describes the specified routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_routing_profile)
         """
 
-    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseOutputTypeDef:
+    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseTypeDef:
         """
         Describes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_rule)
         """
 
     def describe_security_profile(
         self, *, SecurityProfileId: str, InstanceId: str
-    ) -> DescribeSecurityProfileResponseOutputTypeDef:
+    ) -> DescribeSecurityProfileResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_security_profile)
         """
 
     def describe_traffic_distribution_group(
         self, *, TrafficDistributionGroupId: str
-    ) -> DescribeTrafficDistributionGroupResponseOutputTypeDef:
+    ) -> DescribeTrafficDistributionGroupResponseTypeDef:
         """
         Gets details and status of a traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_traffic_distribution_group)
         """
 
-    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseOutputTypeDef:
+    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseTypeDef:
         """
         Describes the specified user account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user)
         """
 
     def describe_user_hierarchy_group(
         self, *, HierarchyGroupId: str, InstanceId: str
-    ) -> DescribeUserHierarchyGroupResponseOutputTypeDef:
+    ) -> DescribeUserHierarchyGroupResponseTypeDef:
         """
         Describes the specified hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_group)
         """
 
     def describe_user_hierarchy_structure(
         self, *, InstanceId: str
-    ) -> DescribeUserHierarchyStructureResponseOutputTypeDef:
+    ) -> DescribeUserHierarchyStructureResponseTypeDef:
         """
         Describes the hierarchy structure of the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_structure)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_structure)
         """
 
     def describe_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DescribeVocabularyResponseOutputTypeDef:
+    ) -> DescribeVocabularyResponseTypeDef:
         """
         Describes the specified vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_vocabulary)
         """
 
@@ -1339,15 +1333,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#generate_presigned_url)
         """
 
     def get_contact_attributes(
         self, *, InstanceId: str, InitialContactId: str
-    ) -> GetContactAttributesResponseOutputTypeDef:
+    ) -> GetContactAttributesResponseTypeDef:
         """
         Retrieves the contact attributes for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_contact_attributes)
         """
 
@@ -1357,38 +1351,38 @@
         InstanceId: str,
         Filters: "FiltersTypeDef",
         CurrentMetrics: Sequence["CurrentMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortCriteria: Sequence["CurrentMetricSortCriteriaTypeDef"] = ...
-    ) -> GetCurrentMetricDataResponseOutputTypeDef:
+    ) -> GetCurrentMetricDataResponseTypeDef:
         """
         Gets the real-time metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_metric_data)
         """
 
     def get_current_user_data(
         self,
         *,
         InstanceId: str,
         Filters: "UserDataFiltersTypeDef",
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetCurrentUserDataResponseOutputTypeDef:
+    ) -> GetCurrentUserDataResponseTypeDef:
         """
         Gets the real-time active user data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_user_data)
         """
 
-    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseOutputTypeDef:
+    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseTypeDef:
         """
         Retrieves a token for federation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_federation_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_federation_token)
         """
 
@@ -1399,15 +1393,15 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataResponseOutputTypeDef:
+    ) -> GetMetricDataResponseTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data)
         """
 
@@ -1418,44 +1412,42 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: Sequence["FilterV2TypeDef"],
         Metrics: Sequence["MetricV2TypeDef"],
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataV2ResponseOutputTypeDef:
+    ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data_v2)
         """
 
-    def get_prompt_file(
-        self, *, InstanceId: str, PromptId: str
-    ) -> GetPromptFileResponseOutputTypeDef:
+    def get_prompt_file(self, *, InstanceId: str, PromptId: str) -> GetPromptFileResponseTypeDef:
         """
         Gets the prompt file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_prompt_file)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_prompt_file)
         """
 
     def get_task_template(
         self, *, InstanceId: str, TaskTemplateId: str, SnapshotVersion: str = ...
-    ) -> GetTaskTemplateResponseOutputTypeDef:
+    ) -> GetTaskTemplateResponseTypeDef:
         """
         Gets details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_task_template)
         """
 
-    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseOutputTypeDef:
+    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseTypeDef:
         """
         Retrieves the current traffic distribution for a given traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_traffic_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_traffic_distribution)
         """
@@ -1463,65 +1455,65 @@
     def list_agent_statuses(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...
-    ) -> ListAgentStatusResponseOutputTypeDef:
+    ) -> ListAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_agent_statuses)
         """
 
     def list_approved_origins(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListApprovedOriginsResponseOutputTypeDef:
+    ) -> ListApprovedOriginsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_approved_origins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_approved_origins)
         """
 
     def list_bots(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListBotsResponseOutputTypeDef:
+    ) -> ListBotsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_bots)
         """
 
     def list_contact_evaluations(
         self, *, InstanceId: str, ContactId: str, NextToken: str = ...
-    ) -> ListContactEvaluationsResponseOutputTypeDef:
+    ) -> ListContactEvaluationsResponseTypeDef:
         """
         Lists contact evaluations in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_evaluations)
         """
 
     def list_contact_flow_modules(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ContactFlowModuleState: ContactFlowModuleStateType = ...
-    ) -> ListContactFlowModulesResponseOutputTypeDef:
+    ) -> ListContactFlowModulesResponseTypeDef:
         """
         Provides information about the flow modules for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flow_modules)
         """
@@ -1529,147 +1521,147 @@
     def list_contact_flows(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListContactFlowsResponseOutputTypeDef:
+    ) -> ListContactFlowsResponseTypeDef:
         """
         Provides information about the flows for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flows)
         """
 
     def list_contact_references(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         NextToken: str = ...
-    ) -> ListContactReferencesResponseOutputTypeDef:
+    ) -> ListContactReferencesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_references)
         """
 
     def list_default_vocabularies(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListDefaultVocabulariesResponseOutputTypeDef:
+    ) -> ListDefaultVocabulariesResponseTypeDef:
         """
         Lists the default vocabularies for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_default_vocabularies)
         """
 
     def list_evaluation_form_versions(
         self, *, InstanceId: str, EvaluationFormId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormVersionsResponseOutputTypeDef:
+    ) -> ListEvaluationFormVersionsResponseTypeDef:
         """
         Lists versions of an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_form_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_form_versions)
         """
 
     def list_evaluation_forms(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormsResponseOutputTypeDef:
+    ) -> ListEvaluationFormsResponseTypeDef:
         """
         Lists evaluation forms in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_forms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_forms)
         """
 
     def list_hours_of_operations(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListHoursOfOperationsResponseOutputTypeDef:
+    ) -> ListHoursOfOperationsResponseTypeDef:
         """
         Provides information about the hours of operation for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_hours_of_operations)
         """
 
     def list_instance_attributes(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstanceAttributesResponseOutputTypeDef:
+    ) -> ListInstanceAttributesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_attributes)
         """
 
     def list_instance_storage_configs(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListInstanceStorageConfigsResponseOutputTypeDef:
+    ) -> ListInstanceStorageConfigsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_storage_configs)
         """
 
     def list_instances(
         self, *, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstancesResponseOutputTypeDef:
+    ) -> ListInstancesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instances)
         """
 
     def list_integration_associations(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListIntegrationAssociationsResponseOutputTypeDef:
+    ) -> ListIntegrationAssociationsResponseTypeDef:
         """
         Provides summary information about the Amazon Web Services resource associations
         for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_integration_associations)
         """
 
     def list_lambda_functions(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLambdaFunctionsResponseOutputTypeDef:
+    ) -> ListLambdaFunctionsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lambda_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lambda_functions)
         """
 
     def list_lex_bots(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLexBotsResponseOutputTypeDef:
+    ) -> ListLexBotsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lex_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lex_bots)
         """
 
@@ -1677,15 +1669,15 @@
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListPhoneNumbersResponseOutputTypeDef:
+    ) -> ListPhoneNumbersResponseTypeDef:
         """
         Provides information about the phone numbers for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers)
         """
@@ -1695,88 +1687,88 @@
         *,
         TargetArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...
-    ) -> ListPhoneNumbersV2ResponseOutputTypeDef:
+    ) -> ListPhoneNumbersV2ResponseTypeDef:
         """
         Lists phone numbers claimed to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers_v2)
         """
 
     def list_prompts(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListPromptsResponseOutputTypeDef:
+    ) -> ListPromptsResponseTypeDef:
         """
         Provides information about the prompts for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_prompts)
         """
 
     def list_queue_quick_connects(
         self, *, InstanceId: str, QueueId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListQueueQuickConnectsResponseOutputTypeDef:
+    ) -> ListQueueQuickConnectsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queue_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queue_quick_connects)
         """
 
     def list_queues(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListQueuesResponseOutputTypeDef:
+    ) -> ListQueuesResponseTypeDef:
         """
         Provides information about the queues for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queues)
         """
 
     def list_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...
-    ) -> ListQuickConnectsResponseOutputTypeDef:
+    ) -> ListQuickConnectsResponseTypeDef:
         """
         Provides information about the quick connects for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_quick_connects)
         """
 
     def list_routing_profile_queues(
         self, *, InstanceId: str, RoutingProfileId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfileQueuesResponseOutputTypeDef:
+    ) -> ListRoutingProfileQueuesResponseTypeDef:
         """
         Lists the queues associated with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profile_queues)
         """
 
     def list_routing_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfilesResponseOutputTypeDef:
+    ) -> ListRoutingProfilesResponseTypeDef:
         """
         Provides summary information about the routing profiles for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profiles)
         """
@@ -1785,61 +1777,59 @@
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListRulesResponseOutputTypeDef:
+    ) -> ListRulesResponseTypeDef:
         """
         List all rules for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_rules)
         """
 
     def list_security_keys(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityKeysResponseOutputTypeDef:
+    ) -> ListSecurityKeysResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_keys)
         """
 
     def list_security_profile_permissions(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListSecurityProfilePermissionsResponseOutputTypeDef:
+    ) -> ListSecurityProfilePermissionsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profile_permissions)
         """
 
     def list_security_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityProfilesResponseOutputTypeDef:
+    ) -> ListSecurityProfilesResponseTypeDef:
         """
         Provides summary information about the security profiles for the specified
         Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profiles)
         """
 
-    def list_tags_for_resource(
-        self, *, resourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_tags_for_resource)
         """
 
@@ -1847,61 +1837,61 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...
-    ) -> ListTaskTemplatesResponseOutputTypeDef:
+    ) -> ListTaskTemplatesResponseTypeDef:
         """
         Lists task templates for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_task_templates)
         """
 
     def list_traffic_distribution_groups(
         self, *, MaxResults: int = ..., NextToken: str = ..., InstanceId: str = ...
-    ) -> ListTrafficDistributionGroupsResponseOutputTypeDef:
+    ) -> ListTrafficDistributionGroupsResponseTypeDef:
         """
         Lists traffic distribution groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_traffic_distribution_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_traffic_distribution_groups)
         """
 
     def list_use_cases(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListUseCasesResponseOutputTypeDef:
+    ) -> ListUseCasesResponseTypeDef:
         """
         Lists the use cases for the integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_use_cases)
         """
 
     def list_user_hierarchy_groups(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUserHierarchyGroupsResponseOutputTypeDef:
+    ) -> ListUserHierarchyGroupsResponseTypeDef:
         """
         Provides summary information about the hierarchy groups for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_user_hierarchy_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_user_hierarchy_groups)
         """
 
     def list_users(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUsersResponseOutputTypeDef:
+    ) -> ListUsersResponseTypeDef:
         """
         Provides summary information about the users for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_users)
         """
@@ -1910,15 +1900,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         UserId: str,
         AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,
         ClientToken: str = ...
-    ) -> MonitorContactResponseOutputTypeDef:
+    ) -> MonitorContactResponseTypeDef:
         """
         Initiates silent monitoring of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#monitor_contact)
         """
 
@@ -1941,15 +1931,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.release_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#release_phone_number)
         """
 
     def replicate_instance(
         self, *, InstanceId: str, ReplicaRegion: str, ReplicaAlias: str, ClientToken: str = ...
-    ) -> ReplicateInstanceResponseOutputTypeDef:
+    ) -> ReplicateInstanceResponseTypeDef:
         """
         Replicates an Amazon Connect instance in the specified Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.replicate_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#replicate_instance)
         """
@@ -1970,15 +1960,15 @@
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> SearchAvailablePhoneNumbersResponseOutputTypeDef:
+    ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches for available phone numbers that you can claim to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_available_phone_numbers)
         """
@@ -1987,15 +1977,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...
-    ) -> SearchHoursOfOperationsResponseOutputTypeDef:
+    ) -> SearchHoursOfOperationsResponseTypeDef:
         """
         Searches the hours of operation in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_hours_of_operations)
         """
@@ -2004,15 +1994,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...
-    ) -> SearchPromptsResponseOutputTypeDef:
+    ) -> SearchPromptsResponseTypeDef:
         """
         Searches prompts in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_prompts)
         """
 
@@ -2020,15 +2010,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
-    ) -> SearchQueuesResponseOutputTypeDef:
+    ) -> SearchQueuesResponseTypeDef:
         """
         Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_queues)
         """
 
@@ -2036,15 +2026,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...
-    ) -> SearchQuickConnectsResponseOutputTypeDef:
+    ) -> SearchQuickConnectsResponseTypeDef:
         """
         Searches quick connects in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_quick_connects)
         """
 
@@ -2052,15 +2042,15 @@
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...
-    ) -> SearchResourceTagsResponseOutputTypeDef:
+    ) -> SearchResourceTagsResponseTypeDef:
         """
         Searches tags used in an Amazon Connect instance using optional search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_resource_tags)
         """
 
@@ -2068,15 +2058,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
-    ) -> SearchRoutingProfilesResponseOutputTypeDef:
+    ) -> SearchRoutingProfilesResponseTypeDef:
         """
         Searches routing profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_routing_profiles)
         """
@@ -2085,15 +2075,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...
-    ) -> SearchSecurityProfilesResponseOutputTypeDef:
+    ) -> SearchSecurityProfilesResponseTypeDef:
         """
         Searches security profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_security_profiles)
         """
@@ -2102,15 +2092,15 @@
         self,
         *,
         InstanceId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...
-    ) -> SearchUsersResponseOutputTypeDef:
+    ) -> SearchUsersResponseTypeDef:
         """
         Searches users in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_users)
         """
 
@@ -2119,15 +2109,15 @@
         *,
         InstanceId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...
-    ) -> SearchVocabulariesResponseOutputTypeDef:
+    ) -> SearchVocabulariesResponseTypeDef:
         """
         Searches for vocabularies within a specific Amazon Connect instance using
         `State`, `NameStartsWith`, and `LanguageCode`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_vocabularies)
         """
@@ -2141,25 +2131,25 @@
         Attributes: Mapping[str, str] = ...,
         InitialMessage: "ChatMessageTypeDef" = ...,
         ClientToken: str = ...,
         ChatDurationInMinutes: int = ...,
         SupportedMessagingContentTypes: Sequence[str] = ...,
         PersistentChat: "PersistentChatTypeDef" = ...,
         RelatedContactId: str = ...
-    ) -> StartChatContactResponseOutputTypeDef:
+    ) -> StartChatContactResponseTypeDef:
         """
         Initiates a flow to start a new chat for the customer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_chat_contact)
         """
 
     def start_contact_evaluation(
         self, *, InstanceId: str, ContactId: str, EvaluationFormId: str, ClientToken: str = ...
-    ) -> StartContactEvaluationResponseOutputTypeDef:
+    ) -> StartContactEvaluationResponseTypeDef:
         """
         Starts an empty evaluation in the specified Amazon Connect instance, using the
         given evaluation form for the particular contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_evaluation)
         """
@@ -2183,15 +2173,15 @@
     def start_contact_streaming(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ChatStreamingConfiguration: "ChatStreamingConfigurationTypeDef",
         ClientToken: str
-    ) -> StartContactStreamingResponseOutputTypeDef:
+    ) -> StartContactStreamingResponseTypeDef:
         """
         Initiates real-time message streaming for a new chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_streaming)
         """
 
@@ -2204,15 +2194,15 @@
         ClientToken: str = ...,
         SourcePhoneNumber: str = ...,
         QueueId: str = ...,
         Attributes: Mapping[str, str] = ...,
         AnswerMachineDetectionConfig: "AnswerMachineDetectionConfigTypeDef" = ...,
         CampaignId: str = ...,
         TrafficType: TrafficTypeType = ...
-    ) -> StartOutboundVoiceContactResponseOutputTypeDef:
+    ) -> StartOutboundVoiceContactResponseTypeDef:
         """
         Places an outbound call to a contact, and then initiates the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_outbound_voice_contact)
         """
 
@@ -2227,15 +2217,15 @@
         References: Mapping[str, "ReferenceTypeDef"] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         ScheduledTime: Union[datetime, str] = ...,
         TaskTemplateId: str = ...,
         QuickConnectId: str = ...,
         RelatedContactId: str = ...
-    ) -> StartTaskContactResponseOutputTypeDef:
+    ) -> StartTaskContactResponseTypeDef:
         """
         Initiates a flow to start a new task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_task_contact)
         """
 
@@ -2270,15 +2260,15 @@
     def submit_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> SubmitContactEvaluationResponseOutputTypeDef:
+    ) -> SubmitContactEvaluationResponseTypeDef:
         """
         Submits a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#submit_contact_evaluation)
         """
 
@@ -2308,15 +2298,15 @@
         *,
         InstanceId: str,
         ContactId: str,
         ContactFlowId: str,
         QueueId: str = ...,
         UserId: str = ...,
         ClientToken: str = ...
-    ) -> TransferContactResponseOutputTypeDef:
+    ) -> TransferContactResponseTypeDef:
         """
         Transfers contacts from one agent or queue to another agent or queue at any
         point after a contact is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#transfer_contact)
         """
@@ -2379,15 +2369,15 @@
     def update_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> UpdateContactEvaluationResponseOutputTypeDef:
+    ) -> UpdateContactEvaluationResponseTypeDef:
         """
         Updates details about a contact evaluation in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_contact_evaluation)
         """
@@ -2472,15 +2462,15 @@
         EvaluationFormVersion: int,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> UpdateEvaluationFormResponseOutputTypeDef:
+    ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_evaluation_form)
         """
@@ -2540,15 +2530,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_participant_role_config)
         """
 
     def update_phone_number(
         self, *, PhoneNumberId: str, TargetArn: str, ClientToken: str = ...
-    ) -> UpdatePhoneNumberResponseOutputTypeDef:
+    ) -> UpdatePhoneNumberResponseTypeDef:
         """
         Updates your claimed phone number from its current Amazon Connect instance or
         traffic distribution group to another Amazon Connect instance or traffic
         distribution group in the same Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number)
@@ -2558,15 +2548,15 @@
         self,
         *,
         InstanceId: str,
         PromptId: str,
         Name: str = ...,
         Description: str = ...,
         S3Uri: str = ...
-    ) -> UpdatePromptResponseOutputTypeDef:
+    ) -> UpdatePromptResponseTypeDef:
         """
         Updates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_prompt)
         """
 
@@ -2735,15 +2725,15 @@
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         Fields: Sequence["TaskTemplateFieldTypeDef"] = ...
-    ) -> UpdateTaskTemplateResponseOutputTypeDef:
+    ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_task_template)
         """
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -91,178 +91,178 @@
     SearchResourceTagsPaginator,
     SearchRoutingProfilesPaginator,
     SearchSecurityProfilesPaginator,
     SearchUsersPaginator,
     SearchVocabulariesPaginator,
 )
 from .type_defs import (
-    ActivateEvaluationFormResponseOutputTypeDef,
+    ActivateEvaluationFormResponseTypeDef,
     AnswerMachineDetectionConfigTypeDef,
-    AssociateInstanceStorageConfigResponseOutputTypeDef,
-    AssociateSecurityKeyResponseOutputTypeDef,
+    AssociateInstanceStorageConfigResponseTypeDef,
+    AssociateSecurityKeyResponseTypeDef,
     ChatMessageTypeDef,
     ChatStreamingConfigurationTypeDef,
-    ClaimPhoneNumberResponseOutputTypeDef,
-    CreateAgentStatusResponseOutputTypeDef,
-    CreateContactFlowModuleResponseOutputTypeDef,
-    CreateContactFlowResponseOutputTypeDef,
-    CreateEvaluationFormResponseOutputTypeDef,
-    CreateHoursOfOperationResponseOutputTypeDef,
-    CreateInstanceResponseOutputTypeDef,
-    CreateIntegrationAssociationResponseOutputTypeDef,
-    CreateParticipantResponseOutputTypeDef,
-    CreatePromptResponseOutputTypeDef,
-    CreateQueueResponseOutputTypeDef,
-    CreateQuickConnectResponseOutputTypeDef,
-    CreateRoutingProfileResponseOutputTypeDef,
-    CreateRuleResponseOutputTypeDef,
-    CreateSecurityProfileResponseOutputTypeDef,
-    CreateTaskTemplateResponseOutputTypeDef,
-    CreateTrafficDistributionGroupResponseOutputTypeDef,
-    CreateUseCaseResponseOutputTypeDef,
-    CreateUserHierarchyGroupResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    CreateVocabularyResponseOutputTypeDef,
+    ClaimPhoneNumberResponseTypeDef,
+    CreateAgentStatusResponseTypeDef,
+    CreateContactFlowModuleResponseTypeDef,
+    CreateContactFlowResponseTypeDef,
+    CreateEvaluationFormResponseTypeDef,
+    CreateHoursOfOperationResponseTypeDef,
+    CreateInstanceResponseTypeDef,
+    CreateIntegrationAssociationResponseTypeDef,
+    CreateParticipantResponseTypeDef,
+    CreatePromptResponseTypeDef,
+    CreateQueueResponseTypeDef,
+    CreateQuickConnectResponseTypeDef,
+    CreateRoutingProfileResponseTypeDef,
+    CreateRuleResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateTaskTemplateResponseTypeDef,
+    CreateTrafficDistributionGroupResponseTypeDef,
+    CreateUseCaseResponseTypeDef,
+    CreateUserHierarchyGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DeactivateEvaluationFormResponseOutputTypeDef,
-    DeleteVocabularyResponseOutputTypeDef,
-    DescribeAgentStatusResponseOutputTypeDef,
-    DescribeContactEvaluationResponseOutputTypeDef,
-    DescribeContactFlowModuleResponseOutputTypeDef,
-    DescribeContactFlowResponseOutputTypeDef,
-    DescribeContactResponseOutputTypeDef,
-    DescribeEvaluationFormResponseOutputTypeDef,
-    DescribeHoursOfOperationResponseOutputTypeDef,
-    DescribeInstanceAttributeResponseOutputTypeDef,
-    DescribeInstanceResponseOutputTypeDef,
-    DescribeInstanceStorageConfigResponseOutputTypeDef,
-    DescribePhoneNumberResponseOutputTypeDef,
-    DescribePromptResponseOutputTypeDef,
-    DescribeQueueResponseOutputTypeDef,
-    DescribeQuickConnectResponseOutputTypeDef,
-    DescribeRoutingProfileResponseOutputTypeDef,
-    DescribeRuleResponseOutputTypeDef,
-    DescribeSecurityProfileResponseOutputTypeDef,
-    DescribeTrafficDistributionGroupResponseOutputTypeDef,
-    DescribeUserHierarchyGroupResponseOutputTypeDef,
-    DescribeUserHierarchyStructureResponseOutputTypeDef,
-    DescribeUserResponseOutputTypeDef,
-    DescribeVocabularyResponseOutputTypeDef,
+    DeactivateEvaluationFormResponseTypeDef,
+    DeleteVocabularyResponseTypeDef,
+    DescribeAgentStatusResponseTypeDef,
+    DescribeContactEvaluationResponseTypeDef,
+    DescribeContactFlowModuleResponseTypeDef,
+    DescribeContactFlowResponseTypeDef,
+    DescribeContactResponseTypeDef,
+    DescribeEvaluationFormResponseTypeDef,
+    DescribeHoursOfOperationResponseTypeDef,
+    DescribeInstanceAttributeResponseTypeDef,
+    DescribeInstanceResponseTypeDef,
+    DescribeInstanceStorageConfigResponseTypeDef,
+    DescribePhoneNumberResponseTypeDef,
+    DescribePromptResponseTypeDef,
+    DescribeQueueResponseTypeDef,
+    DescribeQuickConnectResponseTypeDef,
+    DescribeRoutingProfileResponseTypeDef,
+    DescribeRuleResponseTypeDef,
+    DescribeSecurityProfileResponseTypeDef,
+    DescribeTrafficDistributionGroupResponseTypeDef,
+    DescribeUserHierarchyGroupResponseTypeDef,
+    DescribeUserHierarchyStructureResponseTypeDef,
+    DescribeUserResponseTypeDef,
+    DescribeVocabularyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
-    GetContactAttributesResponseOutputTypeDef,
-    GetCurrentMetricDataResponseOutputTypeDef,
-    GetCurrentUserDataResponseOutputTypeDef,
-    GetFederationTokenResponseOutputTypeDef,
-    GetMetricDataResponseOutputTypeDef,
-    GetMetricDataV2ResponseOutputTypeDef,
-    GetPromptFileResponseOutputTypeDef,
-    GetTaskTemplateResponseOutputTypeDef,
-    GetTrafficDistributionResponseOutputTypeDef,
+    GetContactAttributesResponseTypeDef,
+    GetCurrentMetricDataResponseTypeDef,
+    GetCurrentUserDataResponseTypeDef,
+    GetFederationTokenResponseTypeDef,
+    GetMetricDataResponseTypeDef,
+    GetMetricDataV2ResponseTypeDef,
+    GetPromptFileResponseTypeDef,
+    GetTaskTemplateResponseTypeDef,
+    GetTrafficDistributionResponseTypeDef,
     HierarchyStructureUpdateTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
     InstanceStorageConfigTypeDef,
     LexBotTypeDef,
     LexV2BotTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
-    ListBotsResponseOutputTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
-    ListInstancesResponseOutputTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
-    ListLexBotsResponseOutputTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
-    ListPromptsResponseOutputTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
-    ListQueuesResponseOutputTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
-    ListRulesResponseOutputTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
-    ListUseCasesResponseOutputTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
+    ListApprovedOriginsResponseTypeDef,
+    ListBotsResponseTypeDef,
+    ListContactEvaluationsResponseTypeDef,
+    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowsResponseTypeDef,
+    ListContactReferencesResponseTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
+    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
+    ListInstanceAttributesResponseTypeDef,
+    ListInstancesResponseTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
+    ListLexBotsResponseTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
+    ListPromptsResponseTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
+    ListQueuesResponseTypeDef,
+    ListQuickConnectsResponseTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfilesResponseTypeDef,
+    ListRulesResponseTypeDef,
+    ListSecurityKeysResponseTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskTemplatesResponseTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
+    ListUseCasesResponseTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
+    ListUsersResponseTypeDef,
     MediaConcurrencyTypeDef,
     MetricV2TypeDef,
-    MonitorContactResponseOutputTypeDef,
+    MonitorContactResponseTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectConfigTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ReferenceTypeDef,
-    ReplicateInstanceResponseOutputTypeDef,
+    ReplicateInstanceResponseTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
     RuleActionTypeDef,
     RuleTriggerEventSourceTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
-    SearchPromptsResponseOutputTypeDef,
-    SearchQueuesResponseOutputTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
-    SearchUsersResponseOutputTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
+    SearchPromptsResponseTypeDef,
+    SearchQueuesResponseTypeDef,
+    SearchQuickConnectsResponseTypeDef,
+    SearchResourceTagsResponseTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
+    SearchUsersResponseTypeDef,
+    SearchVocabulariesResponseTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
-    StartChatContactResponseOutputTypeDef,
-    StartContactEvaluationResponseOutputTypeDef,
-    StartContactStreamingResponseOutputTypeDef,
-    StartOutboundVoiceContactResponseOutputTypeDef,
-    StartTaskContactResponseOutputTypeDef,
-    SubmitContactEvaluationResponseOutputTypeDef,
+    StartChatContactResponseTypeDef,
+    StartContactEvaluationResponseTypeDef,
+    StartContactStreamingResponseTypeDef,
+    StartOutboundVoiceContactResponseTypeDef,
+    StartTaskContactResponseTypeDef,
+    SubmitContactEvaluationResponseTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldTypeDef,
     TelephonyConfigTypeDef,
-    TransferContactResponseOutputTypeDef,
-    UpdateContactEvaluationResponseOutputTypeDef,
-    UpdateEvaluationFormResponseOutputTypeDef,
+    TransferContactResponseTypeDef,
+    UpdateContactEvaluationResponseTypeDef,
+    UpdateEvaluationFormResponseTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
-    UpdatePhoneNumberResponseOutputTypeDef,
-    UpdatePromptResponseOutputTypeDef,
-    UpdateTaskTemplateResponseOutputTypeDef,
+    UpdatePhoneNumberResponseTypeDef,
+    UpdatePromptResponseTypeDef,
+    UpdateTaskTemplateResponseTypeDef,
     UserDataFiltersTypeDef,
     UserIdentityInfoTypeDef,
     UserPhoneConfigTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
     VoiceRecordingConfigurationTypeDef,
 )
@@ -320,15 +320,15 @@
         ConnectClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#exceptions)
         """
     def activate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> ActivateEvaluationFormResponseOutputTypeDef:
+    ) -> ActivateEvaluationFormResponseTypeDef:
         """
         Activates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.activate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#activate_evaluation_form)
         """
     def associate_approved_origin(
@@ -360,15 +360,15 @@
         """
     def associate_instance_storage_config(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         StorageConfig: "InstanceStorageConfigTypeDef"
-    ) -> AssociateInstanceStorageConfigResponseOutputTypeDef:
+    ) -> AssociateInstanceStorageConfigResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_instance_storage_config)
         """
     def associate_lambda_function(
@@ -418,15 +418,15 @@
         Associates a set of queues with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_routing_profile_queues)
         """
     def associate_security_key(
         self, *, InstanceId: str, Key: str
-    ) -> AssociateSecurityKeyResponseOutputTypeDef:
+    ) -> AssociateSecurityKeyResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_security_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#associate_security_key)
         """
     def can_paginate(self, operation_name: str) -> bool:
@@ -440,15 +440,15 @@
         self,
         *,
         TargetArn: str,
         PhoneNumber: str,
         PhoneNumberDescription: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> ClaimPhoneNumberResponseOutputTypeDef:
+    ) -> ClaimPhoneNumberResponseTypeDef:
         """
         Claims an available phone number to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#claim_phone_number)
         """
@@ -464,15 +464,15 @@
         *,
         InstanceId: str,
         Name: str,
         State: AgentStatusStateType,
         Description: str = ...,
         DisplayOrder: int = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateAgentStatusResponseOutputTypeDef:
+    ) -> CreateAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_agent_status)
         """
     def create_contact_flow(
@@ -480,15 +480,15 @@
         *,
         InstanceId: str,
         Name: str,
         Type: ContactFlowTypeType,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateContactFlowResponseOutputTypeDef:
+    ) -> CreateContactFlowResponseTypeDef:
         """
         Creates a flow for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow)
         """
     def create_contact_flow_module(
@@ -496,15 +496,15 @@
         *,
         InstanceId: str,
         Name: str,
         Content: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...
-    ) -> CreateContactFlowModuleResponseOutputTypeDef:
+    ) -> CreateContactFlowModuleResponseTypeDef:
         """
         Creates a flow module for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_contact_flow_module)
         """
     def create_evaluation_form(
@@ -512,15 +512,15 @@
         *,
         InstanceId: str,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> CreateEvaluationFormResponseOutputTypeDef:
+    ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_evaluation_form)
         """
     def create_hours_of_operation(
@@ -528,15 +528,15 @@
         *,
         InstanceId: str,
         Name: str,
         TimeZone: str,
         Config: Sequence["HoursOfOperationConfigTypeDef"],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateHoursOfOperationResponseOutputTypeDef:
+    ) -> CreateHoursOfOperationResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_hours_of_operation)
         """
     def create_instance(
@@ -544,15 +544,15 @@
         *,
         IdentityManagementType: DirectoryTypeType,
         InboundCallsEnabled: bool,
         OutboundCallsEnabled: bool,
         ClientToken: str = ...,
         InstanceAlias: str = ...,
         DirectoryId: str = ...
-    ) -> CreateInstanceResponseOutputTypeDef:
+    ) -> CreateInstanceResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_instance)
         """
     def create_integration_association(
@@ -561,45 +561,45 @@
         InstanceId: str,
         IntegrationType: IntegrationTypeType,
         IntegrationArn: str,
         SourceApplicationUrl: str = ...,
         SourceApplicationName: str = ...,
         SourceType: SourceTypeType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateIntegrationAssociationResponseOutputTypeDef:
+    ) -> CreateIntegrationAssociationResponseTypeDef:
         """
         Creates an Amazon Web Services resource association with an Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_integration_association)
         """
     def create_participant(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ParticipantDetails: "ParticipantDetailsToAddTypeDef",
         ClientToken: str = ...
-    ) -> CreateParticipantResponseOutputTypeDef:
+    ) -> CreateParticipantResponseTypeDef:
         """
         Adds a new participant into an on-going chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_participant)
         """
     def create_prompt(
         self,
         *,
         InstanceId: str,
         Name: str,
         S3Uri: str,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreatePromptResponseOutputTypeDef:
+    ) -> CreatePromptResponseTypeDef:
         """
         Creates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_prompt)
         """
     def create_queue(
@@ -609,30 +609,30 @@
         Name: str,
         HoursOfOperationId: str,
         Description: str = ...,
         OutboundCallerConfig: "OutboundCallerConfigTypeDef" = ...,
         MaxContacts: int = ...,
         QuickConnectIds: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQueueResponseOutputTypeDef:
+    ) -> CreateQueueResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_queue)
         """
     def create_quick_connect(
         self,
         *,
         InstanceId: str,
         Name: str,
         QuickConnectConfig: "QuickConnectConfigTypeDef",
         Description: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateQuickConnectResponseOutputTypeDef:
+    ) -> CreateQuickConnectResponseTypeDef:
         """
         Creates a quick connect for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_quick_connect)
         """
     def create_routing_profile(
@@ -641,15 +641,15 @@
         InstanceId: str,
         Name: str,
         Description: str,
         DefaultOutboundQueueId: str,
         MediaConcurrencies: Sequence["MediaConcurrencyTypeDef"],
         QueueConfigs: Sequence["RoutingProfileQueueConfigTypeDef"] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateRoutingProfileResponseOutputTypeDef:
+    ) -> CreateRoutingProfileResponseTypeDef:
         """
         Creates a new routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_routing_profile)
         """
     def create_rule(
@@ -658,15 +658,15 @@
         InstanceId: str,
         Name: str,
         TriggerEventSource: "RuleTriggerEventSourceTypeDef",
         Function: str,
         Actions: Sequence["RuleActionTypeDef"],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...
-    ) -> CreateRuleResponseOutputTypeDef:
+    ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_rule)
         """
     def create_security_profile(
@@ -675,15 +675,15 @@
         SecurityProfileName: str,
         InstanceId: str,
         Description: str = ...,
         Permissions: Sequence[str] = ...,
         Tags: Mapping[str, str] = ...,
         AllowedAccessControlTags: Mapping[str, str] = ...,
         TagRestrictedResources: Sequence[str] = ...
-    ) -> CreateSecurityProfileResponseOutputTypeDef:
+    ) -> CreateSecurityProfileResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_security_profile)
         """
     def create_task_template(
@@ -694,45 +694,45 @@
         Fields: Sequence["TaskTemplateFieldTypeDef"],
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...
-    ) -> CreateTaskTemplateResponseOutputTypeDef:
+    ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_task_template)
         """
     def create_traffic_distribution_group(
         self,
         *,
         Name: str,
         InstanceId: str,
         Description: str = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateTrafficDistributionGroupResponseOutputTypeDef:
+    ) -> CreateTrafficDistributionGroupResponseTypeDef:
         """
         Creates a traffic distribution group given an Amazon Connect instance that has
         been replicated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_traffic_distribution_group)
         """
     def create_use_case(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         UseCaseType: UseCaseTypeType,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUseCaseResponseOutputTypeDef:
+    ) -> CreateUseCaseResponseTypeDef:
         """
         Creates a use case for an integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_use_case)
         """
     def create_user(
@@ -744,24 +744,24 @@
         RoutingProfileId: str,
         InstanceId: str,
         Password: str = ...,
         IdentityInfo: "UserIdentityInfoTypeDef" = ...,
         DirectoryUserId: str = ...,
         HierarchyGroupId: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateUserResponseOutputTypeDef:
+    ) -> CreateUserResponseTypeDef:
         """
         Creates a user account for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user)
         """
     def create_user_hierarchy_group(
         self, *, Name: str, InstanceId: str, ParentGroupId: str = ..., Tags: Mapping[str, str] = ...
-    ) -> CreateUserHierarchyGroupResponseOutputTypeDef:
+    ) -> CreateUserHierarchyGroupResponseTypeDef:
         """
         Creates a new user hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_user_hierarchy_group)
         """
     def create_vocabulary(
@@ -769,24 +769,24 @@
         *,
         InstanceId: str,
         VocabularyName: str,
         LanguageCode: VocabularyLanguageCodeType,
         Content: str,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVocabularyResponseOutputTypeDef:
+    ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a custom vocabulary associated with your Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#create_vocabulary)
         """
     def deactivate_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int
-    ) -> DeactivateEvaluationFormResponseOutputTypeDef:
+    ) -> DeactivateEvaluationFormResponseTypeDef:
         """
         Deactivates an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#deactivate_evaluation_form)
         """
     def delete_contact_evaluation(
@@ -936,208 +936,202 @@
         Deletes an existing user hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_user_hierarchy_group)
         """
     def delete_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DeleteVocabularyResponseOutputTypeDef:
+    ) -> DeleteVocabularyResponseTypeDef:
         """
         Deletes the vocabulary that has the given identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_vocabulary)
         """
     def describe_agent_status(
         self, *, InstanceId: str, AgentStatusId: str
-    ) -> DescribeAgentStatusResponseOutputTypeDef:
+    ) -> DescribeAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_agent_status)
         """
     def describe_contact(
         self, *, InstanceId: str, ContactId: str
-    ) -> DescribeContactResponseOutputTypeDef:
+    ) -> DescribeContactResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact)
         """
     def describe_contact_evaluation(
         self, *, InstanceId: str, EvaluationId: str
-    ) -> DescribeContactEvaluationResponseOutputTypeDef:
+    ) -> DescribeContactEvaluationResponseTypeDef:
         """
         Describes a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_evaluation)
         """
     def describe_contact_flow(
         self, *, InstanceId: str, ContactFlowId: str
-    ) -> DescribeContactFlowResponseOutputTypeDef:
+    ) -> DescribeContactFlowResponseTypeDef:
         """
         Describes the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow)
         """
     def describe_contact_flow_module(
         self, *, InstanceId: str, ContactFlowModuleId: str
-    ) -> DescribeContactFlowModuleResponseOutputTypeDef:
+    ) -> DescribeContactFlowModuleResponseTypeDef:
         """
         Describes the specified flow module.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow_module)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_contact_flow_module)
         """
     def describe_evaluation_form(
         self, *, InstanceId: str, EvaluationFormId: str, EvaluationFormVersion: int = ...
-    ) -> DescribeEvaluationFormResponseOutputTypeDef:
+    ) -> DescribeEvaluationFormResponseTypeDef:
         """
         Describes an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_evaluation_form)
         """
     def describe_hours_of_operation(
         self, *, InstanceId: str, HoursOfOperationId: str
-    ) -> DescribeHoursOfOperationResponseOutputTypeDef:
+    ) -> DescribeHoursOfOperationResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_hours_of_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_hours_of_operation)
         """
-    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseOutputTypeDef:
+    def describe_instance(self, *, InstanceId: str) -> DescribeInstanceResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance)
         """
     def describe_instance_attribute(
         self, *, InstanceId: str, AttributeType: InstanceAttributeTypeType
-    ) -> DescribeInstanceAttributeResponseOutputTypeDef:
+    ) -> DescribeInstanceAttributeResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_attribute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_attribute)
         """
     def describe_instance_storage_config(
         self, *, InstanceId: str, AssociationId: str, ResourceType: InstanceStorageResourceTypeType
-    ) -> DescribeInstanceStorageConfigResponseOutputTypeDef:
+    ) -> DescribeInstanceStorageConfigResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_instance_storage_config)
         """
-    def describe_phone_number(
-        self, *, PhoneNumberId: str
-    ) -> DescribePhoneNumberResponseOutputTypeDef:
+    def describe_phone_number(self, *, PhoneNumberId: str) -> DescribePhoneNumberResponseTypeDef:
         """
         Gets details and status of a phone number that’s claimed to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_phone_number)
         """
-    def describe_prompt(
-        self, *, InstanceId: str, PromptId: str
-    ) -> DescribePromptResponseOutputTypeDef:
+    def describe_prompt(self, *, InstanceId: str, PromptId: str) -> DescribePromptResponseTypeDef:
         """
         Describes the prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_prompt)
         """
-    def describe_queue(
-        self, *, InstanceId: str, QueueId: str
-    ) -> DescribeQueueResponseOutputTypeDef:
+    def describe_queue(self, *, InstanceId: str, QueueId: str) -> DescribeQueueResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_queue)
         """
     def describe_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
-    ) -> DescribeQuickConnectResponseOutputTypeDef:
+    ) -> DescribeQuickConnectResponseTypeDef:
         """
         Describes the quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_quick_connect)
         """
     def describe_routing_profile(
         self, *, InstanceId: str, RoutingProfileId: str
-    ) -> DescribeRoutingProfileResponseOutputTypeDef:
+    ) -> DescribeRoutingProfileResponseTypeDef:
         """
         Describes the specified routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_routing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_routing_profile)
         """
-    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseOutputTypeDef:
+    def describe_rule(self, *, InstanceId: str, RuleId: str) -> DescribeRuleResponseTypeDef:
         """
         Describes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_rule)
         """
     def describe_security_profile(
         self, *, SecurityProfileId: str, InstanceId: str
-    ) -> DescribeSecurityProfileResponseOutputTypeDef:
+    ) -> DescribeSecurityProfileResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_security_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_security_profile)
         """
     def describe_traffic_distribution_group(
         self, *, TrafficDistributionGroupId: str
-    ) -> DescribeTrafficDistributionGroupResponseOutputTypeDef:
+    ) -> DescribeTrafficDistributionGroupResponseTypeDef:
         """
         Gets details and status of a traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_traffic_distribution_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_traffic_distribution_group)
         """
-    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseOutputTypeDef:
+    def describe_user(self, *, UserId: str, InstanceId: str) -> DescribeUserResponseTypeDef:
         """
         Describes the specified user account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user)
         """
     def describe_user_hierarchy_group(
         self, *, HierarchyGroupId: str, InstanceId: str
-    ) -> DescribeUserHierarchyGroupResponseOutputTypeDef:
+    ) -> DescribeUserHierarchyGroupResponseTypeDef:
         """
         Describes the specified hierarchy group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_group)
         """
     def describe_user_hierarchy_structure(
         self, *, InstanceId: str
-    ) -> DescribeUserHierarchyStructureResponseOutputTypeDef:
+    ) -> DescribeUserHierarchyStructureResponseTypeDef:
         """
         Describes the hierarchy structure of the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_structure)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_user_hierarchy_structure)
         """
     def describe_vocabulary(
         self, *, InstanceId: str, VocabularyId: str
-    ) -> DescribeVocabularyResponseOutputTypeDef:
+    ) -> DescribeVocabularyResponseTypeDef:
         """
         Describes the specified vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#describe_vocabulary)
         """
     def disassociate_approved_origin(
@@ -1247,15 +1241,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#generate_presigned_url)
         """
     def get_contact_attributes(
         self, *, InstanceId: str, InitialContactId: str
-    ) -> GetContactAttributesResponseOutputTypeDef:
+    ) -> GetContactAttributesResponseTypeDef:
         """
         Retrieves the contact attributes for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_contact_attributes)
         """
     def get_current_metric_data(
@@ -1264,36 +1258,36 @@
         InstanceId: str,
         Filters: "FiltersTypeDef",
         CurrentMetrics: Sequence["CurrentMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortCriteria: Sequence["CurrentMetricSortCriteriaTypeDef"] = ...
-    ) -> GetCurrentMetricDataResponseOutputTypeDef:
+    ) -> GetCurrentMetricDataResponseTypeDef:
         """
         Gets the real-time metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_metric_data)
         """
     def get_current_user_data(
         self,
         *,
         InstanceId: str,
         Filters: "UserDataFiltersTypeDef",
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetCurrentUserDataResponseOutputTypeDef:
+    ) -> GetCurrentUserDataResponseTypeDef:
         """
         Gets the real-time active user data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_current_user_data)
         """
-    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseOutputTypeDef:
+    def get_federation_token(self, *, InstanceId: str) -> GetFederationTokenResponseTypeDef:
         """
         Retrieves a token for federation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_federation_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_federation_token)
         """
     def get_metric_data(
@@ -1303,15 +1297,15 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataResponseOutputTypeDef:
+    ) -> GetMetricDataResponseTypeDef:
         """
         Gets historical metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data)
         """
     def get_metric_data_v2(
@@ -1321,253 +1315,251 @@
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: Sequence["FilterV2TypeDef"],
         Metrics: Sequence["MetricV2TypeDef"],
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> GetMetricDataV2ResponseOutputTypeDef:
+    ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_metric_data_v2)
         """
-    def get_prompt_file(
-        self, *, InstanceId: str, PromptId: str
-    ) -> GetPromptFileResponseOutputTypeDef:
+    def get_prompt_file(self, *, InstanceId: str, PromptId: str) -> GetPromptFileResponseTypeDef:
         """
         Gets the prompt file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_prompt_file)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_prompt_file)
         """
     def get_task_template(
         self, *, InstanceId: str, TaskTemplateId: str, SnapshotVersion: str = ...
-    ) -> GetTaskTemplateResponseOutputTypeDef:
+    ) -> GetTaskTemplateResponseTypeDef:
         """
         Gets details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_task_template)
         """
-    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseOutputTypeDef:
+    def get_traffic_distribution(self, *, Id: str) -> GetTrafficDistributionResponseTypeDef:
         """
         Retrieves the current traffic distribution for a given traffic distribution
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_traffic_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#get_traffic_distribution)
         """
     def list_agent_statuses(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...
-    ) -> ListAgentStatusResponseOutputTypeDef:
+    ) -> ListAgentStatusResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_agent_statuses)
         """
     def list_approved_origins(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListApprovedOriginsResponseOutputTypeDef:
+    ) -> ListApprovedOriginsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_approved_origins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_approved_origins)
         """
     def list_bots(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListBotsResponseOutputTypeDef:
+    ) -> ListBotsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_bots)
         """
     def list_contact_evaluations(
         self, *, InstanceId: str, ContactId: str, NextToken: str = ...
-    ) -> ListContactEvaluationsResponseOutputTypeDef:
+    ) -> ListContactEvaluationsResponseTypeDef:
         """
         Lists contact evaluations in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_evaluations)
         """
     def list_contact_flow_modules(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ContactFlowModuleState: ContactFlowModuleStateType = ...
-    ) -> ListContactFlowModulesResponseOutputTypeDef:
+    ) -> ListContactFlowModulesResponseTypeDef:
         """
         Provides information about the flow modules for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flow_modules)
         """
     def list_contact_flows(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListContactFlowsResponseOutputTypeDef:
+    ) -> ListContactFlowsResponseTypeDef:
         """
         Provides information about the flows for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_flows)
         """
     def list_contact_references(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         NextToken: str = ...
-    ) -> ListContactReferencesResponseOutputTypeDef:
+    ) -> ListContactReferencesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_contact_references)
         """
     def list_default_vocabularies(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListDefaultVocabulariesResponseOutputTypeDef:
+    ) -> ListDefaultVocabulariesResponseTypeDef:
         """
         Lists the default vocabularies for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_default_vocabularies)
         """
     def list_evaluation_form_versions(
         self, *, InstanceId: str, EvaluationFormId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormVersionsResponseOutputTypeDef:
+    ) -> ListEvaluationFormVersionsResponseTypeDef:
         """
         Lists versions of an evaluation form in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_form_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_form_versions)
         """
     def list_evaluation_forms(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListEvaluationFormsResponseOutputTypeDef:
+    ) -> ListEvaluationFormsResponseTypeDef:
         """
         Lists evaluation forms in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_forms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_evaluation_forms)
         """
     def list_hours_of_operations(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListHoursOfOperationsResponseOutputTypeDef:
+    ) -> ListHoursOfOperationsResponseTypeDef:
         """
         Provides information about the hours of operation for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_hours_of_operations)
         """
     def list_instance_attributes(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstanceAttributesResponseOutputTypeDef:
+    ) -> ListInstanceAttributesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_attributes)
         """
     def list_instance_storage_configs(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListInstanceStorageConfigsResponseOutputTypeDef:
+    ) -> ListInstanceStorageConfigsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instance_storage_configs)
         """
     def list_instances(
         self, *, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListInstancesResponseOutputTypeDef:
+    ) -> ListInstancesResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_instances)
         """
     def list_integration_associations(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListIntegrationAssociationsResponseOutputTypeDef:
+    ) -> ListIntegrationAssociationsResponseTypeDef:
         """
         Provides summary information about the Amazon Web Services resource associations
         for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_integration_associations)
         """
     def list_lambda_functions(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLambdaFunctionsResponseOutputTypeDef:
+    ) -> ListLambdaFunctionsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lambda_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lambda_functions)
         """
     def list_lex_bots(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListLexBotsResponseOutputTypeDef:
+    ) -> ListLexBotsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lex_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_lex_bots)
         """
     def list_phone_numbers(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListPhoneNumbersResponseOutputTypeDef:
+    ) -> ListPhoneNumbersResponseTypeDef:
         """
         Provides information about the phone numbers for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers)
         """
@@ -1576,82 +1568,82 @@
         *,
         TargetArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...
-    ) -> ListPhoneNumbersV2ResponseOutputTypeDef:
+    ) -> ListPhoneNumbersV2ResponseTypeDef:
         """
         Lists phone numbers claimed to your Amazon Connect instance or traffic
         distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_phone_numbers_v2)
         """
     def list_prompts(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListPromptsResponseOutputTypeDef:
+    ) -> ListPromptsResponseTypeDef:
         """
         Provides information about the prompts for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_prompts)
         """
     def list_queue_quick_connects(
         self, *, InstanceId: str, QueueId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListQueueQuickConnectsResponseOutputTypeDef:
+    ) -> ListQueueQuickConnectsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queue_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queue_quick_connects)
         """
     def list_queues(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListQueuesResponseOutputTypeDef:
+    ) -> ListQueuesResponseTypeDef:
         """
         Provides information about the queues for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_queues)
         """
     def list_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...
-    ) -> ListQuickConnectsResponseOutputTypeDef:
+    ) -> ListQuickConnectsResponseTypeDef:
         """
         Provides information about the quick connects for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_quick_connects)
         """
     def list_routing_profile_queues(
         self, *, InstanceId: str, RoutingProfileId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfileQueuesResponseOutputTypeDef:
+    ) -> ListRoutingProfileQueuesResponseTypeDef:
         """
         Lists the queues associated with a routing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profile_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profile_queues)
         """
     def list_routing_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListRoutingProfilesResponseOutputTypeDef:
+    ) -> ListRoutingProfilesResponseTypeDef:
         """
         Provides summary information about the routing profiles for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_routing_profiles)
         """
@@ -1659,114 +1651,112 @@
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> ListRulesResponseOutputTypeDef:
+    ) -> ListRulesResponseTypeDef:
         """
         List all rules for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_rules)
         """
     def list_security_keys(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityKeysResponseOutputTypeDef:
+    ) -> ListSecurityKeysResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_keys)
         """
     def list_security_profile_permissions(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListSecurityProfilePermissionsResponseOutputTypeDef:
+    ) -> ListSecurityProfilePermissionsResponseTypeDef:
         """
         This API is in preview release for Amazon Connect and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profile_permissions)
         """
     def list_security_profiles(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityProfilesResponseOutputTypeDef:
+    ) -> ListSecurityProfilesResponseTypeDef:
         """
         Provides summary information about the security profiles for the specified
         Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_security_profiles)
         """
-    def list_tags_for_resource(
-        self, *, resourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_tags_for_resource)
         """
     def list_task_templates(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...
-    ) -> ListTaskTemplatesResponseOutputTypeDef:
+    ) -> ListTaskTemplatesResponseTypeDef:
         """
         Lists task templates for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_task_templates)
         """
     def list_traffic_distribution_groups(
         self, *, MaxResults: int = ..., NextToken: str = ..., InstanceId: str = ...
-    ) -> ListTrafficDistributionGroupsResponseOutputTypeDef:
+    ) -> ListTrafficDistributionGroupsResponseTypeDef:
         """
         Lists traffic distribution groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_traffic_distribution_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_traffic_distribution_groups)
         """
     def list_use_cases(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         NextToken: str = ...,
         MaxResults: int = ...
-    ) -> ListUseCasesResponseOutputTypeDef:
+    ) -> ListUseCasesResponseTypeDef:
         """
         Lists the use cases for the integration association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_use_cases)
         """
     def list_user_hierarchy_groups(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUserHierarchyGroupsResponseOutputTypeDef:
+    ) -> ListUserHierarchyGroupsResponseTypeDef:
         """
         Provides summary information about the hierarchy groups for the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_user_hierarchy_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_user_hierarchy_groups)
         """
     def list_users(
         self, *, InstanceId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListUsersResponseOutputTypeDef:
+    ) -> ListUsersResponseTypeDef:
         """
         Provides summary information about the users for the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#list_users)
         """
@@ -1774,15 +1764,15 @@
         self,
         *,
         InstanceId: str,
         ContactId: str,
         UserId: str,
         AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,
         ClientToken: str = ...
-    ) -> MonitorContactResponseOutputTypeDef:
+    ) -> MonitorContactResponseTypeDef:
         """
         Initiates silent monitoring of a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#monitor_contact)
         """
     def put_user_status(
@@ -1802,15 +1792,15 @@
         traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.release_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#release_phone_number)
         """
     def replicate_instance(
         self, *, InstanceId: str, ReplicaRegion: str, ReplicaAlias: str, ClientToken: str = ...
-    ) -> ReplicateInstanceResponseOutputTypeDef:
+    ) -> ReplicateInstanceResponseTypeDef:
         """
         Replicates an Amazon Connect instance in the specified Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.replicate_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#replicate_instance)
         """
@@ -1829,15 +1819,15 @@
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> SearchAvailablePhoneNumbersResponseOutputTypeDef:
+    ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches for available phone numbers that you can claim to your Amazon Connect
         instance or traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_available_phone_numbers)
         """
@@ -1845,15 +1835,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...
-    ) -> SearchHoursOfOperationsResponseOutputTypeDef:
+    ) -> SearchHoursOfOperationsResponseTypeDef:
         """
         Searches the hours of operation in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_hours_of_operations)
         """
@@ -1861,75 +1851,75 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...
-    ) -> SearchPromptsResponseOutputTypeDef:
+    ) -> SearchPromptsResponseTypeDef:
         """
         Searches prompts in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_prompts)
         """
     def search_queues(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
-    ) -> SearchQueuesResponseOutputTypeDef:
+    ) -> SearchQueuesResponseTypeDef:
         """
         Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_queues)
         """
     def search_quick_connects(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...
-    ) -> SearchQuickConnectsResponseOutputTypeDef:
+    ) -> SearchQuickConnectsResponseTypeDef:
         """
         Searches quick connects in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_quick_connects)
         """
     def search_resource_tags(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...
-    ) -> SearchResourceTagsResponseOutputTypeDef:
+    ) -> SearchResourceTagsResponseTypeDef:
         """
         Searches tags used in an Amazon Connect instance using optional search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_resource_tags)
         """
     def search_routing_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
-    ) -> SearchRoutingProfilesResponseOutputTypeDef:
+    ) -> SearchRoutingProfilesResponseTypeDef:
         """
         Searches routing profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_routing_profiles)
         """
@@ -1937,15 +1927,15 @@
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...
-    ) -> SearchSecurityProfilesResponseOutputTypeDef:
+    ) -> SearchSecurityProfilesResponseTypeDef:
         """
         Searches security profiles in an Amazon Connect instance, with optional
         filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_security_profiles)
         """
@@ -1953,15 +1943,15 @@
         self,
         *,
         InstanceId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...
-    ) -> SearchUsersResponseOutputTypeDef:
+    ) -> SearchUsersResponseTypeDef:
         """
         Searches users in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_users)
         """
     def search_vocabularies(
@@ -1969,15 +1959,15 @@
         *,
         InstanceId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...
-    ) -> SearchVocabulariesResponseOutputTypeDef:
+    ) -> SearchVocabulariesResponseTypeDef:
         """
         Searches for vocabularies within a specific Amazon Connect instance using
         `State`, `NameStartsWith`, and `LanguageCode`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#search_vocabularies)
         """
@@ -1990,24 +1980,24 @@
         Attributes: Mapping[str, str] = ...,
         InitialMessage: "ChatMessageTypeDef" = ...,
         ClientToken: str = ...,
         ChatDurationInMinutes: int = ...,
         SupportedMessagingContentTypes: Sequence[str] = ...,
         PersistentChat: "PersistentChatTypeDef" = ...,
         RelatedContactId: str = ...
-    ) -> StartChatContactResponseOutputTypeDef:
+    ) -> StartChatContactResponseTypeDef:
         """
         Initiates a flow to start a new chat for the customer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_chat_contact)
         """
     def start_contact_evaluation(
         self, *, InstanceId: str, ContactId: str, EvaluationFormId: str, ClientToken: str = ...
-    ) -> StartContactEvaluationResponseOutputTypeDef:
+    ) -> StartContactEvaluationResponseTypeDef:
         """
         Starts an empty evaluation in the specified Amazon Connect instance, using the
         given evaluation form for the particular contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_evaluation)
         """
@@ -2029,15 +2019,15 @@
     def start_contact_streaming(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ChatStreamingConfiguration: "ChatStreamingConfigurationTypeDef",
         ClientToken: str
-    ) -> StartContactStreamingResponseOutputTypeDef:
+    ) -> StartContactStreamingResponseTypeDef:
         """
         Initiates real-time message streaming for a new chat contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_contact_streaming)
         """
     def start_outbound_voice_contact(
@@ -2049,15 +2039,15 @@
         ClientToken: str = ...,
         SourcePhoneNumber: str = ...,
         QueueId: str = ...,
         Attributes: Mapping[str, str] = ...,
         AnswerMachineDetectionConfig: "AnswerMachineDetectionConfigTypeDef" = ...,
         CampaignId: str = ...,
         TrafficType: TrafficTypeType = ...
-    ) -> StartOutboundVoiceContactResponseOutputTypeDef:
+    ) -> StartOutboundVoiceContactResponseTypeDef:
         """
         Places an outbound call to a contact, and then initiates the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_outbound_voice_contact)
         """
     def start_task_contact(
@@ -2071,15 +2061,15 @@
         References: Mapping[str, "ReferenceTypeDef"] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         ScheduledTime: Union[datetime, str] = ...,
         TaskTemplateId: str = ...,
         QuickConnectId: str = ...,
         RelatedContactId: str = ...
-    ) -> StartTaskContactResponseOutputTypeDef:
+    ) -> StartTaskContactResponseTypeDef:
         """
         Initiates a flow to start a new task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#start_task_contact)
         """
     def stop_contact(self, *, ContactId: str, InstanceId: str) -> Dict[str, Any]:
@@ -2110,15 +2100,15 @@
     def submit_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> SubmitContactEvaluationResponseOutputTypeDef:
+    ) -> SubmitContactEvaluationResponseTypeDef:
         """
         Submits a contact evaluation in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#submit_contact_evaluation)
         """
     def suspend_contact_recording(
@@ -2145,15 +2135,15 @@
         *,
         InstanceId: str,
         ContactId: str,
         ContactFlowId: str,
         QueueId: str = ...,
         UserId: str = ...,
         ClientToken: str = ...
-    ) -> TransferContactResponseOutputTypeDef:
+    ) -> TransferContactResponseTypeDef:
         """
         Transfers contacts from one agent or queue to another agent or queue at any
         point after a contact is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#transfer_contact)
         """
@@ -2211,15 +2201,15 @@
     def update_contact_evaluation(
         self,
         *,
         InstanceId: str,
         EvaluationId: str,
         Answers: Mapping[str, "EvaluationAnswerInputTypeDef"] = ...,
         Notes: Mapping[str, "EvaluationNoteTypeDef"] = ...
-    ) -> UpdateContactEvaluationResponseOutputTypeDef:
+    ) -> UpdateContactEvaluationResponseTypeDef:
         """
         Updates details about a contact evaluation in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_contact_evaluation)
         """
@@ -2297,15 +2287,15 @@
         EvaluationFormVersion: int,
         Title: str,
         Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: "EvaluationFormScoringStrategyTypeDef" = ...,
         ClientToken: str = ...
-    ) -> UpdateEvaluationFormResponseOutputTypeDef:
+    ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified Amazon
         Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_evaluation_form)
         """
@@ -2360,15 +2350,15 @@
         when agents are automatically disconnected from a chat due to idleness.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_participant_role_config)
         """
     def update_phone_number(
         self, *, PhoneNumberId: str, TargetArn: str, ClientToken: str = ...
-    ) -> UpdatePhoneNumberResponseOutputTypeDef:
+    ) -> UpdatePhoneNumberResponseTypeDef:
         """
         Updates your claimed phone number from its current Amazon Connect instance or
         traffic distribution group to another Amazon Connect instance or traffic
         distribution group in the same Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_phone_number)
@@ -2377,15 +2367,15 @@
         self,
         *,
         InstanceId: str,
         PromptId: str,
         Name: str = ...,
         Description: str = ...,
         S3Uri: str = ...
-    ) -> UpdatePromptResponseOutputTypeDef:
+    ) -> UpdatePromptResponseTypeDef:
         """
         Updates a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_prompt)
         """
     def update_queue_hours_of_operation(
@@ -2540,15 +2530,15 @@
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
         Constraints: "TaskTemplateConstraintsTypeDef" = ...,
         Defaults: "TaskTemplateDefaultsTypeDef" = ...,
         Status: TaskTemplateStatusType = ...,
         Fields: Sequence["TaskTemplateFieldTypeDef"] = ...
-    ) -> UpdateTaskTemplateResponseOutputTypeDef:
+    ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#update_task_template)
         """
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,72 +129,72 @@
     RulePublishStatusType,
     TaskTemplateStatusType,
     VocabularyLanguageCodeType,
     VocabularyStateType,
 )
 from .type_defs import (
     FiltersTypeDef,
-    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataResponseTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
-    ListBotsResponseOutputTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
-    ListInstancesResponseOutputTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
-    ListLexBotsResponseOutputTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
-    ListPromptsResponseOutputTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
-    ListQueuesResponseOutputTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
-    ListRulesResponseOutputTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
-    ListUseCasesResponseOutputTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
+    ListApprovedOriginsResponseTypeDef,
+    ListBotsResponseTypeDef,
+    ListContactEvaluationsResponseTypeDef,
+    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowsResponseTypeDef,
+    ListContactReferencesResponseTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
+    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
+    ListInstanceAttributesResponseTypeDef,
+    ListInstancesResponseTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
+    ListLexBotsResponseTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
+    ListPromptsResponseTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
+    ListQueuesResponseTypeDef,
+    ListQuickConnectsResponseTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfilesResponseTypeDef,
+    ListRulesResponseTypeDef,
+    ListSecurityKeysResponseTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilesResponseTypeDef,
+    ListTaskTemplatesResponseTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
+    ListUseCasesResponseTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
+    ListUsersResponseTypeDef,
     PaginatorConfigTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
-    SearchPromptsResponseOutputTypeDef,
-    SearchQueuesResponseOutputTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
-    SearchUsersResponseOutputTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
+    SearchPromptsResponseTypeDef,
+    SearchQueuesResponseTypeDef,
+    SearchQuickConnectsResponseTypeDef,
+    SearchResourceTagsResponseTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
+    SearchUsersResponseTypeDef,
+    SearchVocabulariesResponseTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
 )
 
 __all__ = (
@@ -268,15 +268,15 @@
         InstanceId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetMetricDataResponseOutputTypeDef]:
+    ) -> _PageIterator[GetMetricDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#getmetricdatapaginator)
         """
 
 
 class ListAgentStatusesPaginator(Paginator):
@@ -287,30 +287,30 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentStatusResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAgentStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listagentstatusespaginator)
         """
 
 
 class ListApprovedOriginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListApprovedOriginsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListApprovedOriginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
         """
 
 
 class ListBotsPaginator(Paginator):
@@ -321,30 +321,30 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBotsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listbotspaginator)
         """
 
 
 class ListContactEvaluationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactEvaluationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
         """
 
 
 class ListContactFlowModulesPaginator(Paginator):
@@ -355,15 +355,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleState: ContactFlowModuleStateType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowModulesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactFlowModulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowmodulespaginator)
         """
 
 
 class ListContactFlowsPaginator(Paginator):
@@ -374,15 +374,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowspaginator)
         """
 
 
 class ListContactReferencesPaginator(Paginator):
@@ -394,15 +394,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactReferencesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactreferencespaginator)
         """
 
 
 class ListDefaultVocabulariesPaginator(Paginator):
@@ -413,15 +413,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDefaultVocabulariesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDefaultVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listdefaultvocabulariespaginator)
         """
 
 
 class ListEvaluationFormVersionsPaginator(Paginator):
@@ -432,60 +432,60 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormVersionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformversionspaginator)
         """
 
 
 class ListEvaluationFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
         """
 
 
 class ListHoursOfOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListHoursOfOperationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListHoursOfOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
         """
 
 
 class ListInstanceAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceAttributesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
         """
 
 
 class ListInstanceStorageConfigsPaginator(Paginator):
@@ -496,30 +496,30 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceStorageConfigsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceStorageConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancestorageconfigspaginator)
         """
 
 
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstancesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
         """
 
 
 class ListIntegrationAssociationsPaginator(Paginator):
@@ -530,45 +530,45 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListIntegrationAssociationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListIntegrationAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listintegrationassociationspaginator)
         """
 
 
 class ListLambdaFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLambdaFunctionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLambdaFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
         """
 
 
 class ListLexBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLexBotsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLexBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
         """
 
 
 class ListPhoneNumbersPaginator(Paginator):
@@ -580,15 +580,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumberspaginator)
         """
 
 
 class ListPhoneNumbersV2Paginator(Paginator):
@@ -601,45 +601,45 @@
         self,
         *,
         TargetArn: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersV2ResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumbersv2paginator)
         """
 
 
 class ListPromptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPromptsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPromptsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
         """
 
 
 class ListQueueQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, QueueId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueueQuickConnectsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListQueueQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
         """
 
 
 class ListQueuesPaginator(Paginator):
@@ -650,15 +650,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueuesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuespaginator)
         """
 
 
 class ListQuickConnectsPaginator(Paginator):
@@ -669,15 +669,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQuickConnectsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listquickconnectspaginator)
         """
 
 
 class ListRoutingProfileQueuesPaginator(Paginator):
@@ -688,30 +688,30 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfileQueuesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRoutingProfileQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilequeuespaginator)
         """
 
 
 class ListRoutingProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRoutingProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
         """
 
 
 class ListRulesPaginator(Paginator):
@@ -723,30 +723,30 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRulesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listrulespaginator)
         """
 
 
 class ListSecurityKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityKeysResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecurityKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
         """
 
 
 class ListSecurityProfilePermissionsPaginator(Paginator):
@@ -757,30 +757,30 @@
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilePermissionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilepermissionspaginator)
         """
 
 
 class ListSecurityProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
         """
 
 
 class ListTaskTemplatesPaginator(Paginator):
@@ -792,30 +792,30 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskTemplatesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTaskTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtasktemplatespaginator)
         """
 
 
 class ListTrafficDistributionGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTrafficDistributionGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTrafficDistributionGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
         """
 
 
 class ListUseCasesPaginator(Paginator):
@@ -826,45 +826,45 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUseCasesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUseCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listusecasespaginator)
         """
 
 
 class ListUserHierarchyGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserHierarchyGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserHierarchyGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
         """
 
 
 class SearchAvailablePhoneNumbersPaginator(Paginator):
@@ -877,15 +877,15 @@
         self,
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchavailablephonenumberspaginator)
         """
 
 
 class SearchHoursOfOperationsPaginator(Paginator):
@@ -897,15 +897,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchHoursOfOperationsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchHoursOfOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchhoursofoperationspaginator)
         """
 
 
 class SearchPromptsPaginator(Paginator):
@@ -917,15 +917,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchPromptsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchPromptsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpromptspaginator)
         """
 
 
 class SearchQueuesPaginator(Paginator):
@@ -937,15 +937,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQueuesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchqueuespaginator)
         """
 
 
 class SearchQuickConnectsPaginator(Paginator):
@@ -957,15 +957,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQuickConnectsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchquickconnectspaginator)
         """
 
 
 class SearchResourceTagsPaginator(Paginator):
@@ -977,15 +977,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchResourceTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchresourcetagspaginator)
         """
 
 
 class SearchRoutingProfilesPaginator(Paginator):
@@ -997,15 +997,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchRoutingProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchRoutingProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchroutingprofilespaginator)
         """
 
 
 class SearchSecurityProfilesPaginator(Paginator):
@@ -1017,15 +1017,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchSecurityProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchsecurityprofilespaginator)
         """
 
 
 class SearchUsersPaginator(Paginator):
@@ -1037,15 +1037,15 @@
     def paginate(
         self,
         *,
         InstanceId: str = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchuserspaginator)
         """
 
 
 class SearchVocabulariesPaginator(Paginator):
@@ -1058,12 +1058,12 @@
         self,
         *,
         InstanceId: str,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchVocabulariesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchvocabulariespaginator)
         """
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -129,72 +129,72 @@
     RulePublishStatusType,
     TaskTemplateStatusType,
     VocabularyLanguageCodeType,
     VocabularyStateType,
 )
 from .type_defs import (
     FiltersTypeDef,
-    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataResponseTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
-    ListBotsResponseOutputTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
-    ListInstancesResponseOutputTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
-    ListLexBotsResponseOutputTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
-    ListPromptsResponseOutputTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
-    ListQueuesResponseOutputTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
-    ListRulesResponseOutputTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
-    ListUseCasesResponseOutputTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
+    ListApprovedOriginsResponseTypeDef,
+    ListBotsResponseTypeDef,
+    ListContactEvaluationsResponseTypeDef,
+    ListContactFlowModulesResponseTypeDef,
+    ListContactFlowsResponseTypeDef,
+    ListContactReferencesResponseTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
+    ListEvaluationFormsResponseTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
+    ListInstanceAttributesResponseTypeDef,
+    ListInstancesResponseTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
+    ListLexBotsResponseTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
+    ListPromptsResponseTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
+    ListQueuesResponseTypeDef,
+    ListQuickConnectsResponseTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
+    ListRoutingProfilesResponseTypeDef,
+    ListRulesResponseTypeDef,
+    ListSecurityKeysResponseTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
+    ListSecurityProfilesResponseTypeDef,
+    ListTaskTemplatesResponseTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
+    ListUseCasesResponseTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
+    ListUsersResponseTypeDef,
     PaginatorConfigTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
-    SearchPromptsResponseOutputTypeDef,
-    SearchQueuesResponseOutputTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
-    SearchUsersResponseOutputTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
+    SearchPromptsResponseTypeDef,
+    SearchQueuesResponseTypeDef,
+    SearchQuickConnectsResponseTypeDef,
+    SearchResourceTagsResponseTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
+    SearchUsersResponseTypeDef,
+    SearchVocabulariesResponseTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
 )
 
 __all__ = (
@@ -265,15 +265,15 @@
         InstanceId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         Filters: "FiltersTypeDef",
         HistoricalMetrics: Sequence["HistoricalMetricTypeDef"],
         Groupings: Sequence[GroupingType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetMetricDataResponseOutputTypeDef]:
+    ) -> _PageIterator[GetMetricDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#getmetricdatapaginator)
         """
 
 class ListAgentStatusesPaginator(Paginator):
     """
@@ -283,29 +283,29 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentStatusResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAgentStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listagentstatusespaginator)
         """
 
 class ListApprovedOriginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListApprovedOriginsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListApprovedOriginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listapprovedoriginspaginator)
         """
 
 class ListBotsPaginator(Paginator):
     """
@@ -315,29 +315,29 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LexVersion: LexVersionType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBotsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listbotspaginator)
         """
 
 class ListContactEvaluationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactEvaluationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactevaluationspaginator)
         """
 
 class ListContactFlowModulesPaginator(Paginator):
     """
@@ -347,15 +347,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowModuleState: ContactFlowModuleStateType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowModulesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactFlowModulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowmodulespaginator)
         """
 
 class ListContactFlowsPaginator(Paginator):
     """
@@ -365,15 +365,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactFlowsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactflowspaginator)
         """
 
 class ListContactReferencesPaginator(Paginator):
     """
@@ -384,15 +384,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         ContactId: str,
         ReferenceTypes: Sequence[ReferenceTypeType],
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListContactReferencesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListContactReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listcontactreferencespaginator)
         """
 
 class ListDefaultVocabulariesPaginator(Paginator):
     """
@@ -402,15 +402,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDefaultVocabulariesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDefaultVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listdefaultvocabulariespaginator)
         """
 
 class ListEvaluationFormVersionsPaginator(Paginator):
     """
@@ -420,57 +420,57 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormVersionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationFormVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformversionspaginator)
         """
 
 class ListEvaluationFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEvaluationFormsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEvaluationFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListEvaluationForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listevaluationformspaginator)
         """
 
 class ListHoursOfOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListHoursOfOperationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListHoursOfOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listhoursofoperationspaginator)
         """
 
 class ListInstanceAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceAttributesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstanceattributespaginator)
         """
 
 class ListInstanceStorageConfigsPaginator(Paginator):
     """
@@ -480,29 +480,29 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceType: InstanceStorageResourceTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceStorageConfigsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceStorageConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancestorageconfigspaginator)
         """
 
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstancesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listinstancespaginator)
         """
 
 class ListIntegrationAssociationsPaginator(Paginator):
     """
@@ -512,43 +512,43 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationType: IntegrationTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListIntegrationAssociationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListIntegrationAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listintegrationassociationspaginator)
         """
 
 class ListLambdaFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLambdaFunctionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLambdaFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlambdafunctionspaginator)
         """
 
 class ListLexBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLexBotsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLexBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listlexbotspaginator)
         """
 
 class ListPhoneNumbersPaginator(Paginator):
     """
@@ -559,15 +559,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumberspaginator)
         """
 
 class ListPhoneNumbersV2Paginator(Paginator):
     """
@@ -579,43 +579,43 @@
         self,
         *,
         TargetArn: str = ...,
         PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,
         PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPhoneNumbersV2ResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPhoneNumbersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listphonenumbersv2paginator)
         """
 
 class ListPromptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPromptsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPromptsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listpromptspaginator)
         """
 
 class ListQueueQuickConnectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, QueueId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueueQuickConnectsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListQueueQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuequickconnectspaginator)
         """
 
 class ListQueuesPaginator(Paginator):
     """
@@ -625,15 +625,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QueueTypes: Sequence[QueueTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQueuesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listqueuespaginator)
         """
 
 class ListQuickConnectsPaginator(Paginator):
     """
@@ -643,15 +643,15 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListQuickConnectsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listquickconnectspaginator)
         """
 
 class ListRoutingProfileQueuesPaginator(Paginator):
     """
@@ -661,29 +661,29 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         RoutingProfileId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfileQueuesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRoutingProfileQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilequeuespaginator)
         """
 
 class ListRoutingProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoutingProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRoutingProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listroutingprofilespaginator)
         """
 
 class ListRulesPaginator(Paginator):
     """
@@ -694,29 +694,29 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         PublishStatus: RulePublishStatusType = ...,
         EventSourceName: EventSourceNameType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRulesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listrulespaginator)
         """
 
 class ListSecurityKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityKeysResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecurityKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecuritykeyspaginator)
         """
 
 class ListSecurityProfilePermissionsPaginator(Paginator):
     """
@@ -726,29 +726,29 @@
 
     def paginate(
         self,
         *,
         SecurityProfileId: str,
         InstanceId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilePermissionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilepermissionspaginator)
         """
 
 class ListSecurityProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecurityProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listsecurityprofilespaginator)
         """
 
 class ListTaskTemplatesPaginator(Paginator):
     """
@@ -759,29 +759,29 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         Status: TaskTemplateStatusType = ...,
         Name: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskTemplatesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTaskTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTaskTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtasktemplatespaginator)
         """
 
 class ListTrafficDistributionGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTrafficDistributionGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTrafficDistributionGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListTrafficDistributionGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listtrafficdistributiongroupspaginator)
         """
 
 class ListUseCasesPaginator(Paginator):
     """
@@ -791,43 +791,43 @@
 
     def paginate(
         self,
         *,
         InstanceId: str,
         IntegrationAssociationId: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUseCasesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUseCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listusecasespaginator)
         """
 
 class ListUserHierarchyGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserHierarchyGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserHierarchyGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserhierarchygroupspaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#listuserspaginator)
         """
 
 class SearchAvailablePhoneNumbersPaginator(Paginator):
     """
@@ -839,15 +839,15 @@
         self,
         *,
         TargetArn: str,
         PhoneNumberCountryCode: PhoneNumberCountryCodeType,
         PhoneNumberType: PhoneNumberTypeType,
         PhoneNumberPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchAvailablePhoneNumbersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchAvailablePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchavailablephonenumberspaginator)
         """
 
 class SearchHoursOfOperationsPaginator(Paginator):
     """
@@ -858,15 +858,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "HoursOfOperationSearchFilterTypeDef" = ...,
         SearchCriteria: "HoursOfOperationSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchHoursOfOperationsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchHoursOfOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchHoursOfOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchhoursofoperationspaginator)
         """
 
 class SearchPromptsPaginator(Paginator):
     """
@@ -877,15 +877,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "PromptSearchFilterTypeDef" = ...,
         SearchCriteria: "PromptSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchPromptsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchPromptsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchPrompts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchpromptspaginator)
         """
 
 class SearchQueuesPaginator(Paginator):
     """
@@ -896,15 +896,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QueueSearchFilterTypeDef" = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQueuesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchqueuespaginator)
         """
 
 class SearchQuickConnectsPaginator(Paginator):
     """
@@ -915,15 +915,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "QuickConnectSearchFilterTypeDef" = ...,
         SearchCriteria: "QuickConnectSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchQuickConnectsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchQuickConnectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchQuickConnects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchquickconnectspaginator)
         """
 
 class SearchResourceTagsPaginator(Paginator):
     """
@@ -934,15 +934,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         ResourceTypes: Sequence[str] = ...,
         SearchCriteria: "ResourceTagsSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchResourceTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchresourcetagspaginator)
         """
 
 class SearchRoutingProfilesPaginator(Paginator):
     """
@@ -953,15 +953,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchFilter: "RoutingProfileSearchFilterTypeDef" = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchRoutingProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchRoutingProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchRoutingProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchroutingprofilespaginator)
         """
 
 class SearchSecurityProfilesPaginator(Paginator):
     """
@@ -972,15 +972,15 @@
     def paginate(
         self,
         *,
         InstanceId: str,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: "SecurityProfilesSearchFilterTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchSecurityProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchsecurityprofilespaginator)
         """
 
 class SearchUsersPaginator(Paginator):
     """
@@ -991,15 +991,15 @@
     def paginate(
         self,
         *,
         InstanceId: str = ...,
         SearchFilter: "UserSearchFilterTypeDef" = ...,
         SearchCriteria: "UserSearchCriteriaTypeDef" = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchuserspaginator)
         """
 
 class SearchVocabulariesPaginator(Paginator):
     """
@@ -1011,12 +1011,12 @@
         self,
         *,
         InstanceId: str,
         State: VocabularyStateType = ...,
         NameStartsWith: str = ...,
         LanguageCode: VocabularyLanguageCodeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SearchVocabulariesResponseOutputTypeDef]:
+    ) -> _PageIterator[SearchVocabulariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/paginators/#searchvocabulariespaginator)
         """
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connect service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connect.type_defs import ActionSummaryOutputTypeDef
+    from mypy_boto3_connect.type_defs import ActionSummaryTypeDef
 
-    data: ActionSummaryOutputTypeDef = {...}
+    data: ActionSummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -85,103 +85,103 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActionSummaryOutputTypeDef",
+    "ActionSummaryTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
-    "ActivateEvaluationFormResponseOutputTypeDef",
-    "AgentContactReferenceOutputTypeDef",
-    "AgentInfoOutputTypeDef",
-    "AgentStatusOutputTypeDef",
-    "AgentStatusReferenceOutputTypeDef",
-    "AgentStatusSummaryOutputTypeDef",
+    "ActivateEvaluationFormResponseTypeDef",
+    "AgentContactReferenceTypeDef",
+    "AgentInfoTypeDef",
+    "AgentStatusReferenceTypeDef",
+    "AgentStatusSummaryTypeDef",
+    "AgentStatusTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "AssociateApprovedOriginRequestRequestTypeDef",
     "AssociateBotRequestRequestTypeDef",
     "AssociateDefaultVocabularyRequestRequestTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
-    "AssociateInstanceStorageConfigResponseOutputTypeDef",
+    "AssociateInstanceStorageConfigResponseTypeDef",
     "AssociateLambdaFunctionRequestRequestTypeDef",
     "AssociateLexBotRequestRequestTypeDef",
     "AssociatePhoneNumberContactFlowRequestRequestTypeDef",
     "AssociateQueueQuickConnectsRequestRequestTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "AssociateSecurityKeyRequestRequestTypeDef",
-    "AssociateSecurityKeyResponseOutputTypeDef",
-    "AttachmentReferenceOutputTypeDef",
-    "AttributeOutputTypeDef",
-    "AvailableNumberSummaryOutputTypeDef",
+    "AssociateSecurityKeyResponseTypeDef",
+    "AttachmentReferenceTypeDef",
+    "AttributeTypeDef",
+    "AvailableNumberSummaryTypeDef",
     "ChatMessageTypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "ChatStreamingConfigurationTypeDef",
     "ClaimPhoneNumberRequestRequestTypeDef",
-    "ClaimPhoneNumberResponseOutputTypeDef",
-    "ClaimedPhoneNumberSummaryOutputTypeDef",
+    "ClaimPhoneNumberResponseTypeDef",
+    "ClaimedPhoneNumberSummaryTypeDef",
     "ContactFilterTypeDef",
-    "ContactFlowModuleOutputTypeDef",
-    "ContactFlowModuleSummaryOutputTypeDef",
-    "ContactFlowOutputTypeDef",
-    "ContactFlowSummaryOutputTypeDef",
-    "ContactOutputTypeDef",
+    "ContactFlowModuleSummaryTypeDef",
+    "ContactFlowModuleTypeDef",
+    "ContactFlowSummaryTypeDef",
+    "ContactFlowTypeDef",
+    "ContactTypeDef",
     "ControlPlaneTagFilterTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
-    "CreateAgentStatusResponseOutputTypeDef",
+    "CreateAgentStatusResponseTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
-    "CreateContactFlowModuleResponseOutputTypeDef",
+    "CreateContactFlowModuleResponseTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
-    "CreateContactFlowResponseOutputTypeDef",
+    "CreateContactFlowResponseTypeDef",
     "CreateEvaluationFormRequestRequestTypeDef",
-    "CreateEvaluationFormResponseOutputTypeDef",
+    "CreateEvaluationFormResponseTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
-    "CreateHoursOfOperationResponseOutputTypeDef",
+    "CreateHoursOfOperationResponseTypeDef",
     "CreateInstanceRequestRequestTypeDef",
-    "CreateInstanceResponseOutputTypeDef",
+    "CreateInstanceResponseTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
-    "CreateIntegrationAssociationResponseOutputTypeDef",
+    "CreateIntegrationAssociationResponseTypeDef",
     "CreateParticipantRequestRequestTypeDef",
-    "CreateParticipantResponseOutputTypeDef",
+    "CreateParticipantResponseTypeDef",
     "CreatePromptRequestRequestTypeDef",
-    "CreatePromptResponseOutputTypeDef",
+    "CreatePromptResponseTypeDef",
     "CreateQueueRequestRequestTypeDef",
-    "CreateQueueResponseOutputTypeDef",
+    "CreateQueueResponseTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
-    "CreateQuickConnectResponseOutputTypeDef",
+    "CreateQuickConnectResponseTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
-    "CreateRoutingProfileResponseOutputTypeDef",
+    "CreateRoutingProfileResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
-    "CreateRuleResponseOutputTypeDef",
+    "CreateRuleResponseTypeDef",
     "CreateSecurityProfileRequestRequestTypeDef",
-    "CreateSecurityProfileResponseOutputTypeDef",
+    "CreateSecurityProfileResponseTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
-    "CreateTaskTemplateResponseOutputTypeDef",
+    "CreateTaskTemplateResponseTypeDef",
     "CreateTrafficDistributionGroupRequestRequestTypeDef",
-    "CreateTrafficDistributionGroupResponseOutputTypeDef",
+    "CreateTrafficDistributionGroupResponseTypeDef",
     "CreateUseCaseRequestRequestTypeDef",
-    "CreateUseCaseResponseOutputTypeDef",
+    "CreateUseCaseResponseTypeDef",
     "CreateUserHierarchyGroupRequestRequestTypeDef",
-    "CreateUserHierarchyGroupResponseOutputTypeDef",
+    "CreateUserHierarchyGroupResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseOutputTypeDef",
+    "CreateUserResponseTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "CreateVocabularyResponseOutputTypeDef",
-    "CredentialsOutputTypeDef",
+    "CreateVocabularyResponseTypeDef",
+    "CredentialsTypeDef",
     "CrossChannelBehaviorOutputTypeDef",
     "CrossChannelBehaviorTypeDef",
-    "CurrentMetricDataOutputTypeDef",
+    "CurrentMetricDataTypeDef",
     "CurrentMetricOutputTypeDef",
-    "CurrentMetricResultOutputTypeDef",
+    "CurrentMetricResultTypeDef",
     "CurrentMetricSortCriteriaTypeDef",
     "CurrentMetricTypeDef",
-    "DateReferenceOutputTypeDef",
+    "DateReferenceTypeDef",
     "DeactivateEvaluationFormRequestRequestTypeDef",
-    "DeactivateEvaluationFormResponseOutputTypeDef",
-    "DefaultVocabularyOutputTypeDef",
+    "DeactivateEvaluationFormResponseTypeDef",
+    "DefaultVocabularyTypeDef",
     "DeleteContactEvaluationRequestRequestTypeDef",
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
@@ -193,90 +193,89 @@
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
-    "DeleteVocabularyResponseOutputTypeDef",
+    "DeleteVocabularyResponseTypeDef",
     "DescribeAgentStatusRequestRequestTypeDef",
-    "DescribeAgentStatusResponseOutputTypeDef",
+    "DescribeAgentStatusResponseTypeDef",
     "DescribeContactEvaluationRequestRequestTypeDef",
-    "DescribeContactEvaluationResponseOutputTypeDef",
+    "DescribeContactEvaluationResponseTypeDef",
     "DescribeContactFlowModuleRequestRequestTypeDef",
-    "DescribeContactFlowModuleResponseOutputTypeDef",
+    "DescribeContactFlowModuleResponseTypeDef",
     "DescribeContactFlowRequestRequestTypeDef",
-    "DescribeContactFlowResponseOutputTypeDef",
+    "DescribeContactFlowResponseTypeDef",
     "DescribeContactRequestRequestTypeDef",
-    "DescribeContactResponseOutputTypeDef",
+    "DescribeContactResponseTypeDef",
     "DescribeEvaluationFormRequestRequestTypeDef",
-    "DescribeEvaluationFormResponseOutputTypeDef",
+    "DescribeEvaluationFormResponseTypeDef",
     "DescribeHoursOfOperationRequestRequestTypeDef",
-    "DescribeHoursOfOperationResponseOutputTypeDef",
+    "DescribeHoursOfOperationResponseTypeDef",
     "DescribeInstanceAttributeRequestRequestTypeDef",
-    "DescribeInstanceAttributeResponseOutputTypeDef",
+    "DescribeInstanceAttributeResponseTypeDef",
     "DescribeInstanceRequestRequestTypeDef",
-    "DescribeInstanceResponseOutputTypeDef",
+    "DescribeInstanceResponseTypeDef",
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
-    "DescribeInstanceStorageConfigResponseOutputTypeDef",
+    "DescribeInstanceStorageConfigResponseTypeDef",
     "DescribePhoneNumberRequestRequestTypeDef",
-    "DescribePhoneNumberResponseOutputTypeDef",
+    "DescribePhoneNumberResponseTypeDef",
     "DescribePromptRequestRequestTypeDef",
-    "DescribePromptResponseOutputTypeDef",
+    "DescribePromptResponseTypeDef",
     "DescribeQueueRequestRequestTypeDef",
-    "DescribeQueueResponseOutputTypeDef",
+    "DescribeQueueResponseTypeDef",
     "DescribeQuickConnectRequestRequestTypeDef",
-    "DescribeQuickConnectResponseOutputTypeDef",
+    "DescribeQuickConnectResponseTypeDef",
     "DescribeRoutingProfileRequestRequestTypeDef",
-    "DescribeRoutingProfileResponseOutputTypeDef",
+    "DescribeRoutingProfileResponseTypeDef",
     "DescribeRuleRequestRequestTypeDef",
-    "DescribeRuleResponseOutputTypeDef",
+    "DescribeRuleResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
-    "DescribeSecurityProfileResponseOutputTypeDef",
+    "DescribeSecurityProfileResponseTypeDef",
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
-    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
+    "DescribeTrafficDistributionGroupResponseTypeDef",
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
-    "DescribeUserHierarchyGroupResponseOutputTypeDef",
+    "DescribeUserHierarchyGroupResponseTypeDef",
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
-    "DescribeUserHierarchyStructureResponseOutputTypeDef",
+    "DescribeUserHierarchyStructureResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "DescribeUserResponseOutputTypeDef",
+    "DescribeUserResponseTypeDef",
     "DescribeVocabularyRequestRequestTypeDef",
-    "DescribeVocabularyResponseOutputTypeDef",
-    "DimensionsOutputTypeDef",
+    "DescribeVocabularyResponseTypeDef",
+    "DimensionsTypeDef",
     "DisassociateApprovedOriginRequestRequestTypeDef",
     "DisassociateBotRequestRequestTypeDef",
     "DisassociateInstanceStorageConfigRequestRequestTypeDef",
     "DisassociateLambdaFunctionRequestRequestTypeDef",
     "DisassociateLexBotRequestRequestTypeDef",
     "DisassociatePhoneNumberContactFlowRequestRequestTypeDef",
     "DisassociateQueueQuickConnectsRequestRequestTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DismissUserContactRequestRequestTypeDef",
     "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "EmailReferenceOutputTypeDef",
+    "EmailReferenceTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "EvaluationAnswerDataOutputTypeDef",
     "EvaluationAnswerDataTypeDef",
     "EvaluationAnswerInputTypeDef",
-    "EvaluationAnswerOutputOutputTypeDef",
-    "EvaluationFormContentOutputTypeDef",
+    "EvaluationAnswerOutputTypeDef",
+    "EvaluationFormContentTypeDef",
     "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
     "EvaluationFormNumericQuestionAutomationOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
     "EvaluationFormNumericQuestionOptionOutputTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
     "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
-    "EvaluationFormOutputTypeDef",
     "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
     "EvaluationFormQuestionTypePropertiesOutputTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
     "EvaluationFormScoringStrategyOutputTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
     "EvaluationFormSectionOutputTypeDef",
@@ -285,502 +284,503 @@
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionOptionOutputTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
-    "EvaluationFormSummaryOutputTypeDef",
-    "EvaluationFormVersionSummaryOutputTypeDef",
-    "EvaluationMetadataOutputTypeDef",
+    "EvaluationFormSummaryTypeDef",
+    "EvaluationFormTypeDef",
+    "EvaluationFormVersionSummaryTypeDef",
+    "EvaluationMetadataTypeDef",
     "EvaluationNoteOutputTypeDef",
     "EvaluationNoteTypeDef",
-    "EvaluationOutputTypeDef",
-    "EvaluationScoreOutputTypeDef",
-    "EvaluationSummaryOutputTypeDef",
+    "EvaluationScoreTypeDef",
+    "EvaluationSummaryTypeDef",
+    "EvaluationTypeDef",
     "EventBridgeActionDefinitionOutputTypeDef",
     "EventBridgeActionDefinitionTypeDef",
     "FilterV2TypeDef",
     "FiltersTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
-    "GetContactAttributesResponseOutputTypeDef",
+    "GetContactAttributesResponseTypeDef",
     "GetCurrentMetricDataRequestRequestTypeDef",
-    "GetCurrentMetricDataResponseOutputTypeDef",
+    "GetCurrentMetricDataResponseTypeDef",
     "GetCurrentUserDataRequestRequestTypeDef",
-    "GetCurrentUserDataResponseOutputTypeDef",
+    "GetCurrentUserDataResponseTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
-    "GetFederationTokenResponseOutputTypeDef",
+    "GetFederationTokenResponseTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
-    "GetMetricDataResponseOutputTypeDef",
+    "GetMetricDataResponseTypeDef",
     "GetMetricDataV2RequestRequestTypeDef",
-    "GetMetricDataV2ResponseOutputTypeDef",
+    "GetMetricDataV2ResponseTypeDef",
     "GetPromptFileRequestRequestTypeDef",
-    "GetPromptFileResponseOutputTypeDef",
+    "GetPromptFileResponseTypeDef",
     "GetTaskTemplateRequestRequestTypeDef",
-    "GetTaskTemplateResponseOutputTypeDef",
+    "GetTaskTemplateResponseTypeDef",
     "GetTrafficDistributionRequestRequestTypeDef",
-    "GetTrafficDistributionResponseOutputTypeDef",
+    "GetTrafficDistributionResponseTypeDef",
     "HierarchyGroupConditionTypeDef",
-    "HierarchyGroupOutputTypeDef",
-    "HierarchyGroupSummaryOutputTypeDef",
-    "HierarchyGroupSummaryReferenceOutputTypeDef",
-    "HierarchyLevelOutputTypeDef",
+    "HierarchyGroupSummaryReferenceTypeDef",
+    "HierarchyGroupSummaryTypeDef",
+    "HierarchyGroupTypeDef",
+    "HierarchyLevelTypeDef",
     "HierarchyLevelUpdateTypeDef",
-    "HierarchyPathOutputTypeDef",
-    "HierarchyPathReferenceOutputTypeDef",
-    "HierarchyStructureOutputTypeDef",
+    "HierarchyPathReferenceTypeDef",
+    "HierarchyPathTypeDef",
+    "HierarchyStructureTypeDef",
     "HierarchyStructureUpdateTypeDef",
-    "HistoricalMetricDataOutputTypeDef",
+    "HistoricalMetricDataTypeDef",
     "HistoricalMetricOutputTypeDef",
-    "HistoricalMetricResultOutputTypeDef",
+    "HistoricalMetricResultTypeDef",
     "HistoricalMetricTypeDef",
     "HoursOfOperationConfigOutputTypeDef",
     "HoursOfOperationConfigTypeDef",
-    "HoursOfOperationOutputTypeDef",
     "HoursOfOperationSearchCriteriaTypeDef",
     "HoursOfOperationSearchFilterTypeDef",
-    "HoursOfOperationSummaryOutputTypeDef",
+    "HoursOfOperationSummaryTypeDef",
     "HoursOfOperationTimeSliceOutputTypeDef",
     "HoursOfOperationTimeSliceTypeDef",
-    "InstanceOutputTypeDef",
-    "InstanceStatusReasonOutputTypeDef",
+    "HoursOfOperationTypeDef",
+    "InstanceStatusReasonTypeDef",
     "InstanceStorageConfigOutputTypeDef",
     "InstanceStorageConfigTypeDef",
-    "InstanceSummaryOutputTypeDef",
-    "IntegrationAssociationSummaryOutputTypeDef",
+    "InstanceSummaryTypeDef",
+    "InstanceTypeDef",
+    "IntegrationAssociationSummaryTypeDef",
     "InvisibleFieldInfoOutputTypeDef",
     "InvisibleFieldInfoTypeDef",
     "KinesisFirehoseConfigOutputTypeDef",
     "KinesisFirehoseConfigTypeDef",
     "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
     "KinesisVideoStreamConfigOutputTypeDef",
     "KinesisVideoStreamConfigTypeDef",
-    "LexBotConfigOutputTypeDef",
+    "LexBotConfigTypeDef",
     "LexBotOutputTypeDef",
     "LexBotTypeDef",
     "LexV2BotOutputTypeDef",
     "LexV2BotTypeDef",
     "ListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     "ListAgentStatusRequestRequestTypeDef",
-    "ListAgentStatusResponseOutputTypeDef",
+    "ListAgentStatusResponseTypeDef",
     "ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     "ListApprovedOriginsRequestRequestTypeDef",
-    "ListApprovedOriginsResponseOutputTypeDef",
+    "ListApprovedOriginsResponseTypeDef",
     "ListBotsRequestListBotsPaginateTypeDef",
     "ListBotsRequestRequestTypeDef",
-    "ListBotsResponseOutputTypeDef",
+    "ListBotsResponseTypeDef",
     "ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     "ListContactEvaluationsRequestRequestTypeDef",
-    "ListContactEvaluationsResponseOutputTypeDef",
+    "ListContactEvaluationsResponseTypeDef",
     "ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
     "ListContactFlowModulesRequestRequestTypeDef",
-    "ListContactFlowModulesResponseOutputTypeDef",
+    "ListContactFlowModulesResponseTypeDef",
     "ListContactFlowsRequestListContactFlowsPaginateTypeDef",
     "ListContactFlowsRequestRequestTypeDef",
-    "ListContactFlowsResponseOutputTypeDef",
+    "ListContactFlowsResponseTypeDef",
     "ListContactReferencesRequestListContactReferencesPaginateTypeDef",
     "ListContactReferencesRequestRequestTypeDef",
-    "ListContactReferencesResponseOutputTypeDef",
+    "ListContactReferencesResponseTypeDef",
     "ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
     "ListDefaultVocabulariesRequestRequestTypeDef",
-    "ListDefaultVocabulariesResponseOutputTypeDef",
+    "ListDefaultVocabulariesResponseTypeDef",
     "ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     "ListEvaluationFormVersionsRequestRequestTypeDef",
-    "ListEvaluationFormVersionsResponseOutputTypeDef",
+    "ListEvaluationFormVersionsResponseTypeDef",
     "ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     "ListEvaluationFormsRequestRequestTypeDef",
-    "ListEvaluationFormsResponseOutputTypeDef",
+    "ListEvaluationFormsResponseTypeDef",
     "ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     "ListHoursOfOperationsRequestRequestTypeDef",
-    "ListHoursOfOperationsResponseOutputTypeDef",
+    "ListHoursOfOperationsResponseTypeDef",
     "ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     "ListInstanceAttributesRequestRequestTypeDef",
-    "ListInstanceAttributesResponseOutputTypeDef",
+    "ListInstanceAttributesResponseTypeDef",
     "ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     "ListInstanceStorageConfigsRequestRequestTypeDef",
-    "ListInstanceStorageConfigsResponseOutputTypeDef",
+    "ListInstanceStorageConfigsResponseTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
-    "ListInstancesResponseOutputTypeDef",
+    "ListInstancesResponseTypeDef",
     "ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
     "ListIntegrationAssociationsRequestRequestTypeDef",
-    "ListIntegrationAssociationsResponseOutputTypeDef",
+    "ListIntegrationAssociationsResponseTypeDef",
     "ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     "ListLambdaFunctionsRequestRequestTypeDef",
-    "ListLambdaFunctionsResponseOutputTypeDef",
+    "ListLambdaFunctionsResponseTypeDef",
     "ListLexBotsRequestListLexBotsPaginateTypeDef",
     "ListLexBotsRequestRequestTypeDef",
-    "ListLexBotsResponseOutputTypeDef",
+    "ListLexBotsResponseTypeDef",
     "ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
-    "ListPhoneNumbersResponseOutputTypeDef",
-    "ListPhoneNumbersSummaryOutputTypeDef",
+    "ListPhoneNumbersResponseTypeDef",
+    "ListPhoneNumbersSummaryTypeDef",
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     "ListPhoneNumbersV2RequestRequestTypeDef",
-    "ListPhoneNumbersV2ResponseOutputTypeDef",
+    "ListPhoneNumbersV2ResponseTypeDef",
     "ListPromptsRequestListPromptsPaginateTypeDef",
     "ListPromptsRequestRequestTypeDef",
-    "ListPromptsResponseOutputTypeDef",
+    "ListPromptsResponseTypeDef",
     "ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     "ListQueueQuickConnectsRequestRequestTypeDef",
-    "ListQueueQuickConnectsResponseOutputTypeDef",
+    "ListQueueQuickConnectsResponseTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResponseOutputTypeDef",
+    "ListQueuesResponseTypeDef",
     "ListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
     "ListQuickConnectsRequestRequestTypeDef",
-    "ListQuickConnectsResponseOutputTypeDef",
+    "ListQuickConnectsResponseTypeDef",
     "ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     "ListRoutingProfileQueuesRequestRequestTypeDef",
-    "ListRoutingProfileQueuesResponseOutputTypeDef",
+    "ListRoutingProfileQueuesResponseTypeDef",
     "ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     "ListRoutingProfilesRequestRequestTypeDef",
-    "ListRoutingProfilesResponseOutputTypeDef",
+    "ListRoutingProfilesResponseTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListRulesResponseOutputTypeDef",
+    "ListRulesResponseTypeDef",
     "ListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     "ListSecurityKeysRequestRequestTypeDef",
-    "ListSecurityKeysResponseOutputTypeDef",
+    "ListSecurityKeysResponseTypeDef",
     "ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     "ListSecurityProfilePermissionsRequestRequestTypeDef",
-    "ListSecurityProfilePermissionsResponseOutputTypeDef",
+    "ListSecurityProfilePermissionsResponseTypeDef",
     "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
-    "ListSecurityProfilesResponseOutputTypeDef",
+    "ListSecurityProfilesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef",
     "ListTaskTemplatesRequestRequestTypeDef",
-    "ListTaskTemplatesResponseOutputTypeDef",
+    "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
-    "ListTrafficDistributionGroupsResponseOutputTypeDef",
+    "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesRequestListUseCasesPaginateTypeDef",
     "ListUseCasesRequestRequestTypeDef",
-    "ListUseCasesResponseOutputTypeDef",
+    "ListUseCasesResponseTypeDef",
     "ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
-    "ListUserHierarchyGroupsResponseOutputTypeDef",
+    "ListUserHierarchyGroupsResponseTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListUsersResponseOutputTypeDef",
+    "ListUsersResponseTypeDef",
     "MediaConcurrencyOutputTypeDef",
     "MediaConcurrencyTypeDef",
-    "MetricDataV2OutputTypeDef",
+    "MetricDataV2TypeDef",
     "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
-    "MetricResultV2OutputTypeDef",
+    "MetricResultV2TypeDef",
     "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
-    "MonitorContactResponseOutputTypeDef",
+    "MonitorContactResponseTypeDef",
     "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
-    "NumberReferenceOutputTypeDef",
+    "NumberReferenceTypeDef",
     "NumericQuestionPropertyValueAutomationOutputTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
     "OutboundCallerConfigOutputTypeDef",
     "OutboundCallerConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "ParticipantTimerValueTypeDef",
-    "ParticipantTokenCredentialsOutputTypeDef",
+    "ParticipantTokenCredentialsTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigOutputTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
-    "PhoneNumberStatusOutputTypeDef",
-    "PhoneNumberSummaryOutputTypeDef",
-    "PromptOutputTypeDef",
+    "PhoneNumberStatusTypeDef",
+    "PhoneNumberSummaryTypeDef",
     "PromptSearchCriteriaTypeDef",
     "PromptSearchFilterTypeDef",
-    "PromptSummaryOutputTypeDef",
+    "PromptSummaryTypeDef",
+    "PromptTypeDef",
     "PutUserStatusRequestRequestTypeDef",
-    "QueueInfoOutputTypeDef",
-    "QueueOutputTypeDef",
+    "QueueInfoTypeDef",
     "QueueQuickConnectConfigOutputTypeDef",
     "QueueQuickConnectConfigTypeDef",
-    "QueueReferenceOutputTypeDef",
+    "QueueReferenceTypeDef",
     "QueueSearchCriteriaTypeDef",
     "QueueSearchFilterTypeDef",
-    "QueueSummaryOutputTypeDef",
+    "QueueSummaryTypeDef",
+    "QueueTypeDef",
     "QuickConnectConfigOutputTypeDef",
     "QuickConnectConfigTypeDef",
-    "QuickConnectOutputTypeDef",
     "QuickConnectSearchCriteriaTypeDef",
     "QuickConnectSearchFilterTypeDef",
-    "QuickConnectSummaryOutputTypeDef",
+    "QuickConnectSummaryTypeDef",
+    "QuickConnectTypeDef",
     "ReadOnlyFieldInfoOutputTypeDef",
     "ReadOnlyFieldInfoTypeDef",
     "ReferenceOutputTypeDef",
-    "ReferenceSummaryOutputTypeDef",
+    "ReferenceSummaryTypeDef",
     "ReferenceTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReplicateInstanceRequestRequestTypeDef",
-    "ReplicateInstanceResponseOutputTypeDef",
+    "ReplicateInstanceResponseTypeDef",
     "RequiredFieldInfoOutputTypeDef",
     "RequiredFieldInfoTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeContactRecordingRequestRequestTypeDef",
-    "RoutingProfileOutputTypeDef",
-    "RoutingProfileQueueConfigSummaryOutputTypeDef",
+    "RoutingProfileQueueConfigSummaryTypeDef",
     "RoutingProfileQueueConfigTypeDef",
     "RoutingProfileQueueReferenceTypeDef",
-    "RoutingProfileReferenceOutputTypeDef",
+    "RoutingProfileReferenceTypeDef",
     "RoutingProfileSearchCriteriaTypeDef",
     "RoutingProfileSearchFilterTypeDef",
-    "RoutingProfileSummaryOutputTypeDef",
+    "RoutingProfileSummaryTypeDef",
+    "RoutingProfileTypeDef",
     "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
-    "RuleOutputTypeDef",
-    "RuleSummaryOutputTypeDef",
+    "RuleSummaryTypeDef",
     "RuleTriggerEventSourceOutputTypeDef",
     "RuleTriggerEventSourceTypeDef",
+    "RuleTypeDef",
     "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
-    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SearchHoursOfOperationsRequestRequestTypeDef",
     "SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
-    "SearchHoursOfOperationsResponseOutputTypeDef",
+    "SearchHoursOfOperationsResponseTypeDef",
     "SearchPromptsRequestRequestTypeDef",
     "SearchPromptsRequestSearchPromptsPaginateTypeDef",
-    "SearchPromptsResponseOutputTypeDef",
+    "SearchPromptsResponseTypeDef",
     "SearchQueuesRequestRequestTypeDef",
     "SearchQueuesRequestSearchQueuesPaginateTypeDef",
-    "SearchQueuesResponseOutputTypeDef",
+    "SearchQueuesResponseTypeDef",
     "SearchQuickConnectsRequestRequestTypeDef",
     "SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
-    "SearchQuickConnectsResponseOutputTypeDef",
+    "SearchQuickConnectsResponseTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
-    "SearchResourceTagsResponseOutputTypeDef",
+    "SearchResourceTagsResponseTypeDef",
     "SearchRoutingProfilesRequestRequestTypeDef",
     "SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
-    "SearchRoutingProfilesResponseOutputTypeDef",
+    "SearchRoutingProfilesResponseTypeDef",
     "SearchSecurityProfilesRequestRequestTypeDef",
     "SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
-    "SearchSecurityProfilesResponseOutputTypeDef",
+    "SearchSecurityProfilesResponseTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchUsersRequestSearchUsersPaginateTypeDef",
-    "SearchUsersResponseOutputTypeDef",
+    "SearchUsersResponseTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
-    "SearchVocabulariesResponseOutputTypeDef",
-    "SecurityKeyOutputTypeDef",
-    "SecurityProfileOutputTypeDef",
+    "SearchVocabulariesResponseTypeDef",
+    "SecurityKeyTypeDef",
     "SecurityProfileSearchCriteriaTypeDef",
-    "SecurityProfileSearchSummaryOutputTypeDef",
-    "SecurityProfileSummaryOutputTypeDef",
+    "SecurityProfileSearchSummaryTypeDef",
+    "SecurityProfileSummaryTypeDef",
+    "SecurityProfileTypeDef",
     "SecurityProfilesSearchFilterTypeDef",
     "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "StartChatContactRequestRequestTypeDef",
-    "StartChatContactResponseOutputTypeDef",
+    "StartChatContactResponseTypeDef",
     "StartContactEvaluationRequestRequestTypeDef",
-    "StartContactEvaluationResponseOutputTypeDef",
+    "StartContactEvaluationResponseTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
     "StartContactStreamingRequestRequestTypeDef",
-    "StartContactStreamingResponseOutputTypeDef",
+    "StartContactStreamingResponseTypeDef",
     "StartOutboundVoiceContactRequestRequestTypeDef",
-    "StartOutboundVoiceContactResponseOutputTypeDef",
+    "StartOutboundVoiceContactResponseTypeDef",
     "StartTaskContactRequestRequestTypeDef",
-    "StartTaskContactResponseOutputTypeDef",
+    "StartTaskContactResponseTypeDef",
     "StopContactRecordingRequestRequestTypeDef",
     "StopContactRequestRequestTypeDef",
     "StopContactStreamingRequestRequestTypeDef",
     "StringConditionTypeDef",
-    "StringReferenceOutputTypeDef",
+    "StringReferenceTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
-    "SubmitContactEvaluationResponseOutputTypeDef",
+    "SubmitContactEvaluationResponseTypeDef",
     "SuspendContactRecordingRequestRequestTypeDef",
     "TagConditionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagSearchConditionTypeDef",
-    "TagSetOutputTypeDef",
+    "TagSetTypeDef",
     "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
     "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
     "TaskTemplateDefaultFieldValueOutputTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
     "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
     "TaskTemplateFieldIdentifierOutputTypeDef",
     "TaskTemplateFieldIdentifierTypeDef",
     "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
-    "TaskTemplateMetadataOutputTypeDef",
+    "TaskTemplateMetadataTypeDef",
     "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
     "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
     "ThresholdV2OutputTypeDef",
     "ThresholdV2TypeDef",
-    "TrafficDistributionGroupOutputTypeDef",
-    "TrafficDistributionGroupSummaryOutputTypeDef",
+    "TrafficDistributionGroupSummaryTypeDef",
+    "TrafficDistributionGroupTypeDef",
     "TransferContactRequestRequestTypeDef",
-    "TransferContactResponseOutputTypeDef",
+    "TransferContactResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "UpdateContactAttributesRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
-    "UpdateContactEvaluationResponseOutputTypeDef",
+    "UpdateContactEvaluationResponseTypeDef",
     "UpdateContactFlowContentRequestRequestTypeDef",
     "UpdateContactFlowMetadataRequestRequestTypeDef",
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     "UpdateContactFlowModuleMetadataRequestRequestTypeDef",
     "UpdateContactFlowNameRequestRequestTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "UpdateContactScheduleRequestRequestTypeDef",
     "UpdateEvaluationFormRequestRequestTypeDef",
-    "UpdateEvaluationFormResponseOutputTypeDef",
+    "UpdateEvaluationFormResponseTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "UpdateInstanceAttributeRequestRequestTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
-    "UpdatePhoneNumberResponseOutputTypeDef",
+    "UpdatePhoneNumberResponseTypeDef",
     "UpdatePromptRequestRequestTypeDef",
-    "UpdatePromptResponseOutputTypeDef",
+    "UpdatePromptResponseTypeDef",
     "UpdateQueueHoursOfOperationRequestRequestTypeDef",
     "UpdateQueueMaxContactsRequestRequestTypeDef",
     "UpdateQueueNameRequestRequestTypeDef",
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     "UpdateQueueStatusRequestRequestTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "UpdateQuickConnectNameRequestRequestTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef",
     "UpdateRoutingProfileNameRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
-    "UpdateTaskTemplateResponseOutputTypeDef",
+    "UpdateTaskTemplateResponseTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     "UpdateUserHierarchyRequestRequestTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "UpdateUserIdentityInfoRequestRequestTypeDef",
     "UpdateUserPhoneConfigRequestRequestTypeDef",
     "UpdateUserRoutingProfileRequestRequestTypeDef",
     "UpdateUserSecurityProfilesRequestRequestTypeDef",
-    "UrlReferenceOutputTypeDef",
-    "UseCaseOutputTypeDef",
+    "UrlReferenceTypeDef",
+    "UseCaseTypeDef",
     "UserDataFiltersTypeDef",
-    "UserDataOutputTypeDef",
-    "UserIdentityInfoLiteOutputTypeDef",
+    "UserDataTypeDef",
+    "UserIdentityInfoLiteTypeDef",
     "UserIdentityInfoOutputTypeDef",
     "UserIdentityInfoTypeDef",
-    "UserOutputTypeDef",
     "UserPhoneConfigOutputTypeDef",
     "UserPhoneConfigTypeDef",
     "UserQuickConnectConfigOutputTypeDef",
     "UserQuickConnectConfigTypeDef",
-    "UserReferenceOutputTypeDef",
+    "UserReferenceTypeDef",
     "UserSearchCriteriaTypeDef",
     "UserSearchFilterTypeDef",
-    "UserSearchSummaryOutputTypeDef",
-    "UserSummaryOutputTypeDef",
-    "VocabularyOutputTypeDef",
-    "VocabularySummaryOutputTypeDef",
+    "UserSearchSummaryTypeDef",
+    "UserSummaryTypeDef",
+    "UserTypeDef",
+    "VocabularySummaryTypeDef",
+    "VocabularyTypeDef",
     "VoiceRecordingConfigurationTypeDef",
-    "WisdomInfoOutputTypeDef",
+    "WisdomInfoTypeDef",
 )
 
-ActionSummaryOutputTypeDef = TypedDict(
-    "ActionSummaryOutputTypeDef",
+ActionSummaryTypeDef = TypedDict(
+    "ActionSummaryTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 
 ActivateEvaluationFormRequestRequestTypeDef = TypedDict(
     "ActivateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-ActivateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "ActivateEvaluationFormResponseOutputTypeDef",
+ActivateEvaluationFormResponseTypeDef = TypedDict(
+    "ActivateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentContactReferenceOutputTypeDef = TypedDict(
-    "AgentContactReferenceOutputTypeDef",
+AgentContactReferenceTypeDef = TypedDict(
+    "AgentContactReferenceTypeDef",
     {
         "ContactId": str,
         "Channel": ChannelType,
         "InitiationMethod": ContactInitiationMethodType,
         "AgentContactState": ContactStateType,
         "StateStartTimestamp": datetime,
         "ConnectedToAgentTimestamp": datetime,
-        "Queue": "QueueReferenceOutputTypeDef",
+        "Queue": "QueueReferenceTypeDef",
     },
 )
 
-AgentInfoOutputTypeDef = TypedDict(
-    "AgentInfoOutputTypeDef",
+AgentInfoTypeDef = TypedDict(
+    "AgentInfoTypeDef",
     {
         "Id": str,
         "ConnectedToAgentTimestamp": datetime,
     },
 )
 
-AgentStatusOutputTypeDef = TypedDict(
-    "AgentStatusOutputTypeDef",
-    {
-        "AgentStatusARN": str,
-        "AgentStatusId": str,
-        "Name": str,
-        "Description": str,
-        "Type": AgentStatusTypeType,
-        "DisplayOrder": int,
-        "State": AgentStatusStateType,
-        "Tags": Dict[str, str],
-    },
-)
-
-AgentStatusReferenceOutputTypeDef = TypedDict(
-    "AgentStatusReferenceOutputTypeDef",
+AgentStatusReferenceTypeDef = TypedDict(
+    "AgentStatusReferenceTypeDef",
     {
         "StatusStartTimestamp": datetime,
         "StatusArn": str,
         "StatusName": str,
     },
 )
 
-AgentStatusSummaryOutputTypeDef = TypedDict(
-    "AgentStatusSummaryOutputTypeDef",
+AgentStatusSummaryTypeDef = TypedDict(
+    "AgentStatusSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": AgentStatusTypeType,
     },
 )
 
+AgentStatusTypeDef = TypedDict(
+    "AgentStatusTypeDef",
+    {
+        "AgentStatusARN": str,
+        "AgentStatusId": str,
+        "Name": str,
+        "Description": str,
+        "Type": AgentStatusTypeType,
+        "DisplayOrder": int,
+        "State": AgentStatusStateType,
+        "Tags": Dict[str, str],
+    },
+)
+
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": bool,
         "AwaitAnswerMachinePrompt": bool,
     },
     total=False,
@@ -844,16 +844,16 @@
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": "InstanceStorageConfigTypeDef",
     },
 )
 
-AssociateInstanceStorageConfigResponseOutputTypeDef = TypedDict(
-    "AssociateInstanceStorageConfigResponseOutputTypeDef",
+AssociateInstanceStorageConfigResponseTypeDef = TypedDict(
+    "AssociateInstanceStorageConfigResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateLambdaFunctionRequestRequestTypeDef = TypedDict(
@@ -903,41 +903,41 @@
     "AssociateSecurityKeyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Key": str,
     },
 )
 
-AssociateSecurityKeyResponseOutputTypeDef = TypedDict(
-    "AssociateSecurityKeyResponseOutputTypeDef",
+AssociateSecurityKeyResponseTypeDef = TypedDict(
+    "AssociateSecurityKeyResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachmentReferenceOutputTypeDef = TypedDict(
-    "AttachmentReferenceOutputTypeDef",
+AttachmentReferenceTypeDef = TypedDict(
+    "AttachmentReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
         "Status": ReferenceStatusType,
     },
 )
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
+AttributeTypeDef = TypedDict(
+    "AttributeTypeDef",
     {
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
 )
 
-AvailableNumberSummaryOutputTypeDef = TypedDict(
-    "AvailableNumberSummaryOutputTypeDef",
+AvailableNumberSummaryTypeDef = TypedDict(
+    "AvailableNumberSummaryTypeDef",
     {
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
 )
 
@@ -983,114 +983,114 @@
 
 class ClaimPhoneNumberRequestRequestTypeDef(
     _RequiredClaimPhoneNumberRequestRequestTypeDef, _OptionalClaimPhoneNumberRequestRequestTypeDef
 ):
     pass
 
 
-ClaimPhoneNumberResponseOutputTypeDef = TypedDict(
-    "ClaimPhoneNumberResponseOutputTypeDef",
+ClaimPhoneNumberResponseTypeDef = TypedDict(
+    "ClaimPhoneNumberResponseTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClaimedPhoneNumberSummaryOutputTypeDef = TypedDict(
-    "ClaimedPhoneNumberSummaryOutputTypeDef",
+ClaimedPhoneNumberSummaryTypeDef = TypedDict(
+    "ClaimedPhoneNumberSummaryTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberDescription": str,
         "TargetArn": str,
         "Tags": Dict[str, str],
-        "PhoneNumberStatus": "PhoneNumberStatusOutputTypeDef",
+        "PhoneNumberStatus": "PhoneNumberStatusTypeDef",
     },
 )
 
 ContactFilterTypeDef = TypedDict(
     "ContactFilterTypeDef",
     {
         "ContactStates": Sequence[ContactStateType],
     },
     total=False,
 )
 
-ContactFlowModuleOutputTypeDef = TypedDict(
-    "ContactFlowModuleOutputTypeDef",
+ContactFlowModuleSummaryTypeDef = TypedDict(
+    "ContactFlowModuleSummaryTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "State": ContactFlowModuleStateType,
+    },
+)
+
+ContactFlowModuleTypeDef = TypedDict(
+    "ContactFlowModuleTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Content": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
         "Status": ContactFlowModuleStatusType,
         "Tags": Dict[str, str],
     },
 )
 
-ContactFlowModuleSummaryOutputTypeDef = TypedDict(
-    "ContactFlowModuleSummaryOutputTypeDef",
+ContactFlowSummaryTypeDef = TypedDict(
+    "ContactFlowSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "State": ContactFlowModuleStateType,
+        "ContactFlowType": ContactFlowTypeType,
+        "ContactFlowState": ContactFlowStateType,
     },
 )
 
-ContactFlowOutputTypeDef = TypedDict(
-    "ContactFlowOutputTypeDef",
+ContactFlowTypeDef = TypedDict(
+    "ContactFlowTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "State": ContactFlowStateType,
         "Description": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
 )
 
-ContactFlowSummaryOutputTypeDef = TypedDict(
-    "ContactFlowSummaryOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "ContactFlowType": ContactFlowTypeType,
-        "ContactFlowState": ContactFlowStateType,
-    },
-)
-
-ContactOutputTypeDef = TypedDict(
-    "ContactOutputTypeDef",
+ContactTypeDef = TypedDict(
+    "ContactTypeDef",
     {
         "Arn": str,
         "Id": str,
         "InitialContactId": str,
         "PreviousContactId": str,
         "InitiationMethod": ContactInitiationMethodType,
         "Name": str,
         "Description": str,
         "Channel": ChannelType,
-        "QueueInfo": "QueueInfoOutputTypeDef",
-        "AgentInfo": "AgentInfoOutputTypeDef",
+        "QueueInfo": "QueueInfoTypeDef",
+        "AgentInfo": "AgentInfoTypeDef",
         "InitiationTimestamp": datetime,
         "DisconnectTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ScheduledTimestamp": datetime,
         "RelatedContactId": str,
-        "WisdomInfo": "WisdomInfoOutputTypeDef",
+        "WisdomInfo": "WisdomInfoTypeDef",
     },
 )
 
 ControlPlaneTagFilterTypeDef = TypedDict(
     "ControlPlaneTagFilterTypeDef",
     {
         "OrConditions": Sequence[Sequence["TagConditionTypeDef"]],
@@ -1121,16 +1121,16 @@
 
 class CreateAgentStatusRequestRequestTypeDef(
     _RequiredCreateAgentStatusRequestRequestTypeDef, _OptionalCreateAgentStatusRequestRequestTypeDef
 ):
     pass
 
 
-CreateAgentStatusResponseOutputTypeDef = TypedDict(
-    "CreateAgentStatusResponseOutputTypeDef",
+CreateAgentStatusResponseTypeDef = TypedDict(
+    "CreateAgentStatusResponseTypeDef",
     {
         "AgentStatusARN": str,
         "AgentStatusId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1156,16 +1156,16 @@
 class CreateContactFlowModuleRequestRequestTypeDef(
     _RequiredCreateContactFlowModuleRequestRequestTypeDef,
     _OptionalCreateContactFlowModuleRequestRequestTypeDef,
 ):
     pass
 
 
-CreateContactFlowModuleResponseOutputTypeDef = TypedDict(
-    "CreateContactFlowModuleResponseOutputTypeDef",
+CreateContactFlowModuleResponseTypeDef = TypedDict(
+    "CreateContactFlowModuleResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1190,16 +1190,16 @@
 
 class CreateContactFlowRequestRequestTypeDef(
     _RequiredCreateContactFlowRequestRequestTypeDef, _OptionalCreateContactFlowRequestRequestTypeDef
 ):
     pass
 
 
-CreateContactFlowResponseOutputTypeDef = TypedDict(
-    "CreateContactFlowResponseOutputTypeDef",
+CreateContactFlowResponseTypeDef = TypedDict(
+    "CreateContactFlowResponseTypeDef",
     {
         "ContactFlowId": str,
         "ContactFlowArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1225,16 +1225,16 @@
 class CreateEvaluationFormRequestRequestTypeDef(
     _RequiredCreateEvaluationFormRequestRequestTypeDef,
     _OptionalCreateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
 
-CreateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "CreateEvaluationFormResponseOutputTypeDef",
+CreateEvaluationFormResponseTypeDef = TypedDict(
+    "CreateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1260,16 +1260,16 @@
 class CreateHoursOfOperationRequestRequestTypeDef(
     _RequiredCreateHoursOfOperationRequestRequestTypeDef,
     _OptionalCreateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateHoursOfOperationResponseOutputTypeDef = TypedDict(
-    "CreateHoursOfOperationResponseOutputTypeDef",
+CreateHoursOfOperationResponseTypeDef = TypedDict(
+    "CreateHoursOfOperationResponseTypeDef",
     {
         "HoursOfOperationId": str,
         "HoursOfOperationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1294,16 +1294,16 @@
 
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
 
-CreateInstanceResponseOutputTypeDef = TypedDict(
-    "CreateInstanceResponseOutputTypeDef",
+CreateInstanceResponseTypeDef = TypedDict(
+    "CreateInstanceResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1330,16 +1330,16 @@
 class CreateIntegrationAssociationRequestRequestTypeDef(
     _RequiredCreateIntegrationAssociationRequestRequestTypeDef,
     _OptionalCreateIntegrationAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateIntegrationAssociationResponseOutputTypeDef = TypedDict(
-    "CreateIntegrationAssociationResponseOutputTypeDef",
+CreateIntegrationAssociationResponseTypeDef = TypedDict(
+    "CreateIntegrationAssociationResponseTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1362,18 +1362,18 @@
 
 class CreateParticipantRequestRequestTypeDef(
     _RequiredCreateParticipantRequestRequestTypeDef, _OptionalCreateParticipantRequestRequestTypeDef
 ):
     pass
 
 
-CreateParticipantResponseOutputTypeDef = TypedDict(
-    "CreateParticipantResponseOutputTypeDef",
+CreateParticipantResponseTypeDef = TypedDict(
+    "CreateParticipantResponseTypeDef",
     {
-        "ParticipantCredentials": "ParticipantTokenCredentialsOutputTypeDef",
+        "ParticipantCredentials": "ParticipantTokenCredentialsTypeDef",
         "ParticipantId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePromptRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePromptRequestRequestTypeDef",
@@ -1395,16 +1395,16 @@
 
 class CreatePromptRequestRequestTypeDef(
     _RequiredCreatePromptRequestRequestTypeDef, _OptionalCreatePromptRequestRequestTypeDef
 ):
     pass
 
 
-CreatePromptResponseOutputTypeDef = TypedDict(
-    "CreatePromptResponseOutputTypeDef",
+CreatePromptResponseTypeDef = TypedDict(
+    "CreatePromptResponseTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1431,16 +1431,16 @@
 
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
 
-CreateQueueResponseOutputTypeDef = TypedDict(
-    "CreateQueueResponseOutputTypeDef",
+CreateQueueResponseTypeDef = TypedDict(
+    "CreateQueueResponseTypeDef",
     {
         "QueueArn": str,
         "QueueId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1465,16 +1465,16 @@
 class CreateQuickConnectRequestRequestTypeDef(
     _RequiredCreateQuickConnectRequestRequestTypeDef,
     _OptionalCreateQuickConnectRequestRequestTypeDef,
 ):
     pass
 
 
-CreateQuickConnectResponseOutputTypeDef = TypedDict(
-    "CreateQuickConnectResponseOutputTypeDef",
+CreateQuickConnectResponseTypeDef = TypedDict(
+    "CreateQuickConnectResponseTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1501,16 +1501,16 @@
 class CreateRoutingProfileRequestRequestTypeDef(
     _RequiredCreateRoutingProfileRequestRequestTypeDef,
     _OptionalCreateRoutingProfileRequestRequestTypeDef,
 ):
     pass
 
 
-CreateRoutingProfileResponseOutputTypeDef = TypedDict(
-    "CreateRoutingProfileResponseOutputTypeDef",
+CreateRoutingProfileResponseTypeDef = TypedDict(
+    "CreateRoutingProfileResponseTypeDef",
     {
         "RoutingProfileArn": str,
         "RoutingProfileId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1536,16 +1536,16 @@
 
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
 
-CreateRuleResponseOutputTypeDef = TypedDict(
-    "CreateRuleResponseOutputTypeDef",
+CreateRuleResponseTypeDef = TypedDict(
+    "CreateRuleResponseTypeDef",
     {
         "RuleArn": str,
         "RuleId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1572,16 +1572,16 @@
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSecurityProfileResponseOutputTypeDef = TypedDict(
-    "CreateSecurityProfileResponseOutputTypeDef",
+CreateSecurityProfileResponseTypeDef = TypedDict(
+    "CreateSecurityProfileResponseTypeDef",
     {
         "SecurityProfileId": str,
         "SecurityProfileArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1610,16 +1610,16 @@
 class CreateTaskTemplateRequestRequestTypeDef(
     _RequiredCreateTaskTemplateRequestRequestTypeDef,
     _OptionalCreateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-CreateTaskTemplateResponseOutputTypeDef = TypedDict(
-    "CreateTaskTemplateResponseOutputTypeDef",
+CreateTaskTemplateResponseTypeDef = TypedDict(
+    "CreateTaskTemplateResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1644,16 +1644,16 @@
 class CreateTrafficDistributionGroupRequestRequestTypeDef(
     _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef,
     _OptionalCreateTrafficDistributionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-CreateTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
-    "CreateTrafficDistributionGroupResponseOutputTypeDef",
+CreateTrafficDistributionGroupResponseTypeDef = TypedDict(
+    "CreateTrafficDistributionGroupResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1676,16 +1676,16 @@
 
 class CreateUseCaseRequestRequestTypeDef(
     _RequiredCreateUseCaseRequestRequestTypeDef, _OptionalCreateUseCaseRequestRequestTypeDef
 ):
     pass
 
 
-CreateUseCaseResponseOutputTypeDef = TypedDict(
-    "CreateUseCaseResponseOutputTypeDef",
+CreateUseCaseResponseTypeDef = TypedDict(
+    "CreateUseCaseResponseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1709,16 +1709,16 @@
 class CreateUserHierarchyGroupRequestRequestTypeDef(
     _RequiredCreateUserHierarchyGroupRequestRequestTypeDef,
     _OptionalCreateUserHierarchyGroupRequestRequestTypeDef,
 ):
     pass
 
 
-CreateUserHierarchyGroupResponseOutputTypeDef = TypedDict(
-    "CreateUserHierarchyGroupResponseOutputTypeDef",
+CreateUserHierarchyGroupResponseTypeDef = TypedDict(
+    "CreateUserHierarchyGroupResponseTypeDef",
     {
         "HierarchyGroupId": str,
         "HierarchyGroupArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1747,16 +1747,16 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
-CreateUserResponseOutputTypeDef = TypedDict(
-    "CreateUserResponseOutputTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
         "UserId": str,
         "UserArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1781,26 +1781,26 @@
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-CreateVocabularyResponseOutputTypeDef = TypedDict(
-    "CreateVocabularyResponseOutputTypeDef",
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CredentialsOutputTypeDef = TypedDict(
-    "CredentialsOutputTypeDef",
+CredentialsTypeDef = TypedDict(
+    "CredentialsTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
     },
 )
@@ -1815,35 +1815,35 @@
 CrossChannelBehaviorTypeDef = TypedDict(
     "CrossChannelBehaviorTypeDef",
     {
         "BehaviorType": BehaviorTypeType,
     },
 )
 
-CurrentMetricDataOutputTypeDef = TypedDict(
-    "CurrentMetricDataOutputTypeDef",
+CurrentMetricDataTypeDef = TypedDict(
+    "CurrentMetricDataTypeDef",
     {
         "Metric": "CurrentMetricOutputTypeDef",
         "Value": float,
     },
 )
 
 CurrentMetricOutputTypeDef = TypedDict(
     "CurrentMetricOutputTypeDef",
     {
         "Name": CurrentMetricNameType,
         "Unit": UnitType,
     },
 )
 
-CurrentMetricResultOutputTypeDef = TypedDict(
-    "CurrentMetricResultOutputTypeDef",
+CurrentMetricResultTypeDef = TypedDict(
+    "CurrentMetricResultTypeDef",
     {
-        "Dimensions": "DimensionsOutputTypeDef",
-        "Collections": List["CurrentMetricDataOutputTypeDef"],
+        "Dimensions": "DimensionsTypeDef",
+        "Collections": List["CurrentMetricDataTypeDef"],
     },
 )
 
 CurrentMetricSortCriteriaTypeDef = TypedDict(
     "CurrentMetricSortCriteriaTypeDef",
     {
         "SortByMetric": CurrentMetricNameType,
@@ -1857,16 +1857,16 @@
     {
         "Name": CurrentMetricNameType,
         "Unit": UnitType,
     },
     total=False,
 )
 
-DateReferenceOutputTypeDef = TypedDict(
-    "DateReferenceOutputTypeDef",
+DateReferenceTypeDef = TypedDict(
+    "DateReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 DeactivateEvaluationFormRequestRequestTypeDef = TypedDict(
@@ -1874,26 +1874,26 @@
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-DeactivateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "DeactivateEvaluationFormResponseOutputTypeDef",
+DeactivateEvaluationFormResponseTypeDef = TypedDict(
+    "DeactivateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DefaultVocabularyOutputTypeDef = TypedDict(
-    "DefaultVocabularyOutputTypeDef",
+DefaultVocabularyTypeDef = TypedDict(
+    "DefaultVocabularyTypeDef",
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "VocabularyId": str,
         "VocabularyName": str,
     },
 )
@@ -2060,16 +2060,16 @@
     "DeleteVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DeleteVocabularyResponseOutputTypeDef = TypedDict(
-    "DeleteVocabularyResponseOutputTypeDef",
+DeleteVocabularyResponseTypeDef = TypedDict(
+    "DeleteVocabularyResponseTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2078,83 +2078,83 @@
     "DescribeAgentStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-DescribeAgentStatusResponseOutputTypeDef = TypedDict(
-    "DescribeAgentStatusResponseOutputTypeDef",
+DescribeAgentStatusResponseTypeDef = TypedDict(
+    "DescribeAgentStatusResponseTypeDef",
     {
-        "AgentStatus": "AgentStatusOutputTypeDef",
+        "AgentStatus": "AgentStatusTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactEvaluationRequestRequestTypeDef = TypedDict(
     "DescribeContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
 
-DescribeContactEvaluationResponseOutputTypeDef = TypedDict(
-    "DescribeContactEvaluationResponseOutputTypeDef",
+DescribeContactEvaluationResponseTypeDef = TypedDict(
+    "DescribeContactEvaluationResponseTypeDef",
     {
-        "Evaluation": "EvaluationOutputTypeDef",
-        "EvaluationForm": "EvaluationFormContentOutputTypeDef",
+        "Evaluation": "EvaluationTypeDef",
+        "EvaluationForm": "EvaluationFormContentTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowModuleRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowModuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
     },
 )
 
-DescribeContactFlowModuleResponseOutputTypeDef = TypedDict(
-    "DescribeContactFlowModuleResponseOutputTypeDef",
+DescribeContactFlowModuleResponseTypeDef = TypedDict(
+    "DescribeContactFlowModuleResponseTypeDef",
     {
-        "ContactFlowModule": "ContactFlowModuleOutputTypeDef",
+        "ContactFlowModule": "ContactFlowModuleTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
 
-DescribeContactFlowResponseOutputTypeDef = TypedDict(
-    "DescribeContactFlowResponseOutputTypeDef",
+DescribeContactFlowResponseTypeDef = TypedDict(
+    "DescribeContactFlowResponseTypeDef",
     {
-        "ContactFlow": "ContactFlowOutputTypeDef",
+        "ContactFlow": "ContactFlowTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactRequestRequestTypeDef = TypedDict(
     "DescribeContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
 
-DescribeContactResponseOutputTypeDef = TypedDict(
-    "DescribeContactResponseOutputTypeDef",
+DescribeContactResponseTypeDef = TypedDict(
+    "DescribeContactResponseTypeDef",
     {
-        "Contact": "ContactOutputTypeDef",
+        "Contact": "ContactTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEvaluationFormRequestRequestTypeDef",
     {
@@ -2174,281 +2174,281 @@
 class DescribeEvaluationFormRequestRequestTypeDef(
     _RequiredDescribeEvaluationFormRequestRequestTypeDef,
     _OptionalDescribeEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeEvaluationFormResponseOutputTypeDef = TypedDict(
-    "DescribeEvaluationFormResponseOutputTypeDef",
+DescribeEvaluationFormResponseTypeDef = TypedDict(
+    "DescribeEvaluationFormResponseTypeDef",
     {
-        "EvaluationForm": "EvaluationFormOutputTypeDef",
+        "EvaluationForm": "EvaluationFormTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DescribeHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
 
-DescribeHoursOfOperationResponseOutputTypeDef = TypedDict(
-    "DescribeHoursOfOperationResponseOutputTypeDef",
+DescribeHoursOfOperationResponseTypeDef = TypedDict(
+    "DescribeHoursOfOperationResponseTypeDef",
     {
-        "HoursOfOperation": "HoursOfOperationOutputTypeDef",
+        "HoursOfOperation": "HoursOfOperationTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceAttributeRequestRequestTypeDef = TypedDict(
     "DescribeInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
     },
 )
 
-DescribeInstanceAttributeResponseOutputTypeDef = TypedDict(
-    "DescribeInstanceAttributeResponseOutputTypeDef",
+DescribeInstanceAttributeResponseTypeDef = TypedDict(
+    "DescribeInstanceAttributeResponseTypeDef",
     {
-        "Attribute": "AttributeOutputTypeDef",
+        "Attribute": "AttributeTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceRequestRequestTypeDef = TypedDict(
     "DescribeInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeInstanceResponseOutputTypeDef = TypedDict(
-    "DescribeInstanceResponseOutputTypeDef",
+DescribeInstanceResponseTypeDef = TypedDict(
+    "DescribeInstanceResponseTypeDef",
     {
-        "Instance": "InstanceOutputTypeDef",
+        "Instance": "InstanceTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
 
-DescribeInstanceStorageConfigResponseOutputTypeDef = TypedDict(
-    "DescribeInstanceStorageConfigResponseOutputTypeDef",
+DescribeInstanceStorageConfigResponseTypeDef = TypedDict(
+    "DescribeInstanceStorageConfigResponseTypeDef",
     {
         "StorageConfig": "InstanceStorageConfigOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePhoneNumberRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-DescribePhoneNumberResponseOutputTypeDef = TypedDict(
-    "DescribePhoneNumberResponseOutputTypeDef",
+DescribePhoneNumberResponseTypeDef = TypedDict(
+    "DescribePhoneNumberResponseTypeDef",
     {
-        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryOutputTypeDef",
+        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePromptRequestRequestTypeDef = TypedDict(
     "DescribePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-DescribePromptResponseOutputTypeDef = TypedDict(
-    "DescribePromptResponseOutputTypeDef",
+DescribePromptResponseTypeDef = TypedDict(
+    "DescribePromptResponseTypeDef",
     {
-        "Prompt": "PromptOutputTypeDef",
+        "Prompt": "PromptTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueueRequestRequestTypeDef = TypedDict(
     "DescribeQueueRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
 
-DescribeQueueResponseOutputTypeDef = TypedDict(
-    "DescribeQueueResponseOutputTypeDef",
+DescribeQueueResponseTypeDef = TypedDict(
+    "DescribeQueueResponseTypeDef",
     {
-        "Queue": "QueueOutputTypeDef",
+        "Queue": "QueueTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQuickConnectRequestRequestTypeDef = TypedDict(
     "DescribeQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
-DescribeQuickConnectResponseOutputTypeDef = TypedDict(
-    "DescribeQuickConnectResponseOutputTypeDef",
+DescribeQuickConnectResponseTypeDef = TypedDict(
+    "DescribeQuickConnectResponseTypeDef",
     {
-        "QuickConnect": "QuickConnectOutputTypeDef",
+        "QuickConnect": "QuickConnectTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRoutingProfileRequestRequestTypeDef = TypedDict(
     "DescribeRoutingProfileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
 
-DescribeRoutingProfileResponseOutputTypeDef = TypedDict(
-    "DescribeRoutingProfileResponseOutputTypeDef",
+DescribeRoutingProfileResponseTypeDef = TypedDict(
+    "DescribeRoutingProfileResponseTypeDef",
     {
-        "RoutingProfile": "RoutingProfileOutputTypeDef",
+        "RoutingProfile": "RoutingProfileTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRuleRequestRequestTypeDef = TypedDict(
     "DescribeRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
 
-DescribeRuleResponseOutputTypeDef = TypedDict(
-    "DescribeRuleResponseOutputTypeDef",
+DescribeRuleResponseTypeDef = TypedDict(
+    "DescribeRuleResponseTypeDef",
     {
-        "Rule": "RuleOutputTypeDef",
+        "Rule": "RuleTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
 
-DescribeSecurityProfileResponseOutputTypeDef = TypedDict(
-    "DescribeSecurityProfileResponseOutputTypeDef",
+DescribeSecurityProfileResponseTypeDef = TypedDict(
+    "DescribeSecurityProfileResponseTypeDef",
     {
-        "SecurityProfile": "SecurityProfileOutputTypeDef",
+        "SecurityProfile": "SecurityProfileTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrafficDistributionGroupRequestRequestTypeDef = TypedDict(
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
     {
         "TrafficDistributionGroupId": str,
     },
 )
 
-DescribeTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
-    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
+DescribeTrafficDistributionGroupResponseTypeDef = TypedDict(
+    "DescribeTrafficDistributionGroupResponseTypeDef",
     {
-        "TrafficDistributionGroup": "TrafficDistributionGroupOutputTypeDef",
+        "TrafficDistributionGroup": "TrafficDistributionGroupTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyGroupRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyGroupResponseOutputTypeDef = TypedDict(
-    "DescribeUserHierarchyGroupResponseOutputTypeDef",
+DescribeUserHierarchyGroupResponseTypeDef = TypedDict(
+    "DescribeUserHierarchyGroupResponseTypeDef",
     {
-        "HierarchyGroup": "HierarchyGroupOutputTypeDef",
+        "HierarchyGroup": "HierarchyGroupTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyStructureRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyStructureResponseOutputTypeDef = TypedDict(
-    "DescribeUserHierarchyStructureResponseOutputTypeDef",
+DescribeUserHierarchyStructureResponseTypeDef = TypedDict(
+    "DescribeUserHierarchyStructureResponseTypeDef",
     {
-        "HierarchyStructure": "HierarchyStructureOutputTypeDef",
+        "HierarchyStructure": "HierarchyStructureTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserResponseOutputTypeDef = TypedDict(
-    "DescribeUserResponseOutputTypeDef",
+DescribeUserResponseTypeDef = TypedDict(
+    "DescribeUserResponseTypeDef",
     {
-        "User": "UserOutputTypeDef",
+        "User": "UserTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVocabularyRequestRequestTypeDef = TypedDict(
     "DescribeVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DescribeVocabularyResponseOutputTypeDef = TypedDict(
-    "DescribeVocabularyResponseOutputTypeDef",
+DescribeVocabularyResponseTypeDef = TypedDict(
+    "DescribeVocabularyResponseTypeDef",
     {
-        "Vocabulary": "VocabularyOutputTypeDef",
+        "Vocabulary": "VocabularyTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DimensionsOutputTypeDef = TypedDict(
-    "DimensionsOutputTypeDef",
+DimensionsTypeDef = TypedDict(
+    "DimensionsTypeDef",
     {
-        "Queue": "QueueReferenceOutputTypeDef",
+        "Queue": "QueueReferenceTypeDef",
         "Channel": ChannelType,
-        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceTypeDef",
     },
 )
 
 DisassociateApprovedOriginRequestRequestTypeDef = TypedDict(
     "DisassociateApprovedOriginRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -2559,16 +2559,16 @@
     "DistributionTypeDef",
     {
         "Region": str,
         "Percentage": int,
     },
 )
 
-EmailReferenceOutputTypeDef = TypedDict(
-    "EmailReferenceOutputTypeDef",
+EmailReferenceTypeDef = TypedDict(
+    "EmailReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
@@ -2617,24 +2617,24 @@
     "EvaluationAnswerInputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
     },
     total=False,
 )
 
-EvaluationAnswerOutputOutputTypeDef = TypedDict(
-    "EvaluationAnswerOutputOutputTypeDef",
+EvaluationAnswerOutputTypeDef = TypedDict(
+    "EvaluationAnswerOutputTypeDef",
     {
         "Value": "EvaluationAnswerDataOutputTypeDef",
         "SystemSuggestedValue": "EvaluationAnswerDataOutputTypeDef",
     },
 )
 
-EvaluationFormContentOutputTypeDef = TypedDict(
-    "EvaluationFormContentOutputTypeDef",
+EvaluationFormContentTypeDef = TypedDict(
+    "EvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "Description": str,
         "Items": List["EvaluationFormItemOutputTypeDef"],
@@ -2738,34 +2738,14 @@
 class EvaluationFormNumericQuestionPropertiesTypeDef(
     _RequiredEvaluationFormNumericQuestionPropertiesTypeDef,
     _OptionalEvaluationFormNumericQuestionPropertiesTypeDef,
 ):
     pass
 
 
-EvaluationFormOutputTypeDef = TypedDict(
-    "EvaluationFormOutputTypeDef",
-    {
-        "EvaluationFormId": str,
-        "EvaluationFormVersion": int,
-        "Locked": bool,
-        "EvaluationFormArn": str,
-        "Title": str,
-        "Description": str,
-        "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemOutputTypeDef"],
-        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
-        "CreatedTime": datetime,
-        "CreatedBy": str,
-        "LastModifiedTime": datetime,
-        "LastModifiedBy": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 EvaluationFormQuestionOutputTypeDef = TypedDict(
     "EvaluationFormQuestionOutputTypeDef",
     {
         "Title": str,
         "Instructions": str,
         "RefId": str,
         "NotApplicableEnabled": bool,
@@ -2976,16 +2956,16 @@
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
 
-EvaluationFormSummaryOutputTypeDef = TypedDict(
-    "EvaluationFormSummaryOutputTypeDef",
+EvaluationFormSummaryTypeDef = TypedDict(
+    "EvaluationFormSummaryTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
@@ -2993,36 +2973,56 @@
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
         "LatestVersion": int,
         "ActiveVersion": int,
     },
 )
 
-EvaluationFormVersionSummaryOutputTypeDef = TypedDict(
-    "EvaluationFormVersionSummaryOutputTypeDef",
+EvaluationFormTypeDef = TypedDict(
+    "EvaluationFormTypeDef",
+    {
+        "EvaluationFormId": str,
+        "EvaluationFormVersion": int,
+        "Locked": bool,
+        "EvaluationFormArn": str,
+        "Title": str,
+        "Description": str,
+        "Status": EvaluationFormVersionStatusType,
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
+        "CreatedTime": datetime,
+        "CreatedBy": str,
+        "LastModifiedTime": datetime,
+        "LastModifiedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+EvaluationFormVersionSummaryTypeDef = TypedDict(
+    "EvaluationFormVersionSummaryTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "Status": EvaluationFormVersionStatusType,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 
-EvaluationMetadataOutputTypeDef = TypedDict(
-    "EvaluationMetadataOutputTypeDef",
+EvaluationMetadataTypeDef = TypedDict(
+    "EvaluationMetadataTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
         "ContactAgentId": str,
-        "Score": "EvaluationScoreOutputTypeDef",
+        "Score": "EvaluationScoreTypeDef",
     },
 )
 
 EvaluationNoteOutputTypeDef = TypedDict(
     "EvaluationNoteOutputTypeDef",
     {
         "Value": str,
@@ -3033,54 +3033,54 @@
     "EvaluationNoteTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-EvaluationOutputTypeDef = TypedDict(
-    "EvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "EvaluationArn": str,
-        "Metadata": "EvaluationMetadataOutputTypeDef",
-        "Answers": Dict[str, "EvaluationAnswerOutputOutputTypeDef"],
-        "Notes": Dict[str, "EvaluationNoteOutputTypeDef"],
-        "Status": EvaluationStatusType,
-        "Scores": Dict[str, "EvaluationScoreOutputTypeDef"],
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
-        "Tags": Dict[str, str],
-    },
-)
-
-EvaluationScoreOutputTypeDef = TypedDict(
-    "EvaluationScoreOutputTypeDef",
+EvaluationScoreTypeDef = TypedDict(
+    "EvaluationScoreTypeDef",
     {
         "Percentage": float,
         "NotApplicable": bool,
         "AutomaticFail": bool,
     },
 )
 
-EvaluationSummaryOutputTypeDef = TypedDict(
-    "EvaluationSummaryOutputTypeDef",
+EvaluationSummaryTypeDef = TypedDict(
+    "EvaluationSummaryTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
-        "Score": "EvaluationScoreOutputTypeDef",
+        "Score": "EvaluationScoreTypeDef",
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
 )
 
+EvaluationTypeDef = TypedDict(
+    "EvaluationTypeDef",
+    {
+        "EvaluationId": str,
+        "EvaluationArn": str,
+        "Metadata": "EvaluationMetadataTypeDef",
+        "Answers": Dict[str, "EvaluationAnswerOutputTypeDef"],
+        "Notes": Dict[str, "EvaluationNoteOutputTypeDef"],
+        "Status": EvaluationStatusType,
+        "Scores": Dict[str, "EvaluationScoreTypeDef"],
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+        "Tags": Dict[str, str],
+    },
+)
+
 EventBridgeActionDefinitionOutputTypeDef = TypedDict(
     "EventBridgeActionDefinitionOutputTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -3114,16 +3114,16 @@
     "GetContactAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InitialContactId": str,
     },
 )
 
-GetContactAttributesResponseOutputTypeDef = TypedDict(
-    "GetContactAttributesResponseOutputTypeDef",
+GetContactAttributesResponseTypeDef = TypedDict(
+    "GetContactAttributesResponseTypeDef",
     {
         "Attributes": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentMetricDataRequestRequestTypeDef = TypedDict(
@@ -3149,19 +3149,19 @@
 class GetCurrentMetricDataRequestRequestTypeDef(
     _RequiredGetCurrentMetricDataRequestRequestTypeDef,
     _OptionalGetCurrentMetricDataRequestRequestTypeDef,
 ):
     pass
 
 
-GetCurrentMetricDataResponseOutputTypeDef = TypedDict(
-    "GetCurrentMetricDataResponseOutputTypeDef",
+GetCurrentMetricDataResponseTypeDef = TypedDict(
+    "GetCurrentMetricDataResponseTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["CurrentMetricResultOutputTypeDef"],
+        "MetricResults": List["CurrentMetricResultTypeDef"],
         "DataSnapshotTime": datetime,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentUserDataRequestRequestTypeDef = TypedDict(
@@ -3184,35 +3184,35 @@
 class GetCurrentUserDataRequestRequestTypeDef(
     _RequiredGetCurrentUserDataRequestRequestTypeDef,
     _OptionalGetCurrentUserDataRequestRequestTypeDef,
 ):
     pass
 
 
-GetCurrentUserDataResponseOutputTypeDef = TypedDict(
-    "GetCurrentUserDataResponseOutputTypeDef",
+GetCurrentUserDataResponseTypeDef = TypedDict(
+    "GetCurrentUserDataResponseTypeDef",
     {
         "NextToken": str,
-        "UserDataList": List["UserDataOutputTypeDef"],
+        "UserDataList": List["UserDataTypeDef"],
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFederationTokenRequestRequestTypeDef = TypedDict(
     "GetFederationTokenRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-GetFederationTokenResponseOutputTypeDef = TypedDict(
-    "GetFederationTokenResponseOutputTypeDef",
+GetFederationTokenResponseTypeDef = TypedDict(
+    "GetFederationTokenResponseTypeDef",
     {
-        "Credentials": "CredentialsOutputTypeDef",
+        "Credentials": "CredentialsTypeDef",
         "SignInUrl": str,
         "UserArn": str,
         "UserId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3266,19 +3266,19 @@
 
 class GetMetricDataRequestRequestTypeDef(
     _RequiredGetMetricDataRequestRequestTypeDef, _OptionalGetMetricDataRequestRequestTypeDef
 ):
     pass
 
 
-GetMetricDataResponseOutputTypeDef = TypedDict(
-    "GetMetricDataResponseOutputTypeDef",
+GetMetricDataResponseTypeDef = TypedDict(
+    "GetMetricDataResponseTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["HistoricalMetricResultOutputTypeDef"],
+        "MetricResults": List["HistoricalMetricResultTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataV2RequestRequestTypeDef",
     {
@@ -3302,33 +3302,33 @@
 
 class GetMetricDataV2RequestRequestTypeDef(
     _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
 ):
     pass
 
 
-GetMetricDataV2ResponseOutputTypeDef = TypedDict(
-    "GetMetricDataV2ResponseOutputTypeDef",
+GetMetricDataV2ResponseTypeDef = TypedDict(
+    "GetMetricDataV2ResponseTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["MetricResultV2OutputTypeDef"],
+        "MetricResults": List["MetricResultV2TypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPromptFileRequestRequestTypeDef = TypedDict(
     "GetPromptFileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-GetPromptFileResponseOutputTypeDef = TypedDict(
-    "GetPromptFileResponseOutputTypeDef",
+GetPromptFileResponseTypeDef = TypedDict(
+    "GetPromptFileResponseTypeDef",
     {
         "PromptPresignedUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTaskTemplateRequestRequestTypeDef = TypedDict(
@@ -3349,16 +3349,16 @@
 
 class GetTaskTemplateRequestRequestTypeDef(
     _RequiredGetTaskTemplateRequestRequestTypeDef, _OptionalGetTaskTemplateRequestRequestTypeDef
 ):
     pass
 
 
-GetTaskTemplateResponseOutputTypeDef = TypedDict(
-    "GetTaskTemplateResponseOutputTypeDef",
+GetTaskTemplateResponseTypeDef = TypedDict(
+    "GetTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
@@ -3376,16 +3376,16 @@
 GetTrafficDistributionRequestRequestTypeDef = TypedDict(
     "GetTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficDistributionResponseOutputTypeDef = TypedDict(
-    "GetTrafficDistributionResponseOutputTypeDef",
+GetTrafficDistributionResponseTypeDef = TypedDict(
+    "GetTrafficDistributionResponseTypeDef",
     {
         "TelephonyConfig": "TelephonyConfigOutputTypeDef",
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3395,89 +3395,89 @@
     {
         "Value": str,
         "HierarchyGroupMatchType": HierarchyGroupMatchTypeType,
     },
     total=False,
 )
 
-HierarchyGroupOutputTypeDef = TypedDict(
-    "HierarchyGroupOutputTypeDef",
+HierarchyGroupSummaryReferenceTypeDef = TypedDict(
+    "HierarchyGroupSummaryReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
-        "Name": str,
-        "LevelId": str,
-        "HierarchyPath": "HierarchyPathOutputTypeDef",
-        "Tags": Dict[str, str],
     },
 )
 
-HierarchyGroupSummaryOutputTypeDef = TypedDict(
-    "HierarchyGroupSummaryOutputTypeDef",
+HierarchyGroupSummaryTypeDef = TypedDict(
+    "HierarchyGroupSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-HierarchyGroupSummaryReferenceOutputTypeDef = TypedDict(
-    "HierarchyGroupSummaryReferenceOutputTypeDef",
+HierarchyGroupTypeDef = TypedDict(
+    "HierarchyGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
+        "Name": str,
+        "LevelId": str,
+        "HierarchyPath": "HierarchyPathTypeDef",
+        "Tags": Dict[str, str],
     },
 )
 
-HierarchyLevelOutputTypeDef = TypedDict(
-    "HierarchyLevelOutputTypeDef",
+HierarchyLevelTypeDef = TypedDict(
+    "HierarchyLevelTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
 HierarchyLevelUpdateTypeDef = TypedDict(
     "HierarchyLevelUpdateTypeDef",
     {
         "Name": str,
     },
 )
 
-HierarchyPathOutputTypeDef = TypedDict(
-    "HierarchyPathOutputTypeDef",
+HierarchyPathReferenceTypeDef = TypedDict(
+    "HierarchyPathReferenceTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelThree": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelFour": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelFive": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelOne": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelThree": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelFour": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelFive": "HierarchyGroupSummaryReferenceTypeDef",
     },
 )
 
-HierarchyPathReferenceOutputTypeDef = TypedDict(
-    "HierarchyPathReferenceOutputTypeDef",
+HierarchyPathTypeDef = TypedDict(
+    "HierarchyPathTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelThree": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelFour": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelFive": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelOne": "HierarchyGroupSummaryTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryTypeDef",
+        "LevelThree": "HierarchyGroupSummaryTypeDef",
+        "LevelFour": "HierarchyGroupSummaryTypeDef",
+        "LevelFive": "HierarchyGroupSummaryTypeDef",
     },
 )
 
-HierarchyStructureOutputTypeDef = TypedDict(
-    "HierarchyStructureOutputTypeDef",
+HierarchyStructureTypeDef = TypedDict(
+    "HierarchyStructureTypeDef",
     {
-        "LevelOne": "HierarchyLevelOutputTypeDef",
-        "LevelTwo": "HierarchyLevelOutputTypeDef",
-        "LevelThree": "HierarchyLevelOutputTypeDef",
-        "LevelFour": "HierarchyLevelOutputTypeDef",
-        "LevelFive": "HierarchyLevelOutputTypeDef",
+        "LevelOne": "HierarchyLevelTypeDef",
+        "LevelTwo": "HierarchyLevelTypeDef",
+        "LevelThree": "HierarchyLevelTypeDef",
+        "LevelFour": "HierarchyLevelTypeDef",
+        "LevelFive": "HierarchyLevelTypeDef",
     },
 )
 
 HierarchyStructureUpdateTypeDef = TypedDict(
     "HierarchyStructureUpdateTypeDef",
     {
         "LevelOne": "HierarchyLevelUpdateTypeDef",
@@ -3485,16 +3485,16 @@
         "LevelThree": "HierarchyLevelUpdateTypeDef",
         "LevelFour": "HierarchyLevelUpdateTypeDef",
         "LevelFive": "HierarchyLevelUpdateTypeDef",
     },
     total=False,
 )
 
-HistoricalMetricDataOutputTypeDef = TypedDict(
-    "HistoricalMetricDataOutputTypeDef",
+HistoricalMetricDataTypeDef = TypedDict(
+    "HistoricalMetricDataTypeDef",
     {
         "Metric": "HistoricalMetricOutputTypeDef",
         "Value": float,
     },
 )
 
 HistoricalMetricOutputTypeDef = TypedDict(
@@ -3503,19 +3503,19 @@
         "Name": HistoricalMetricNameType,
         "Threshold": "ThresholdOutputTypeDef",
         "Statistic": StatisticType,
         "Unit": UnitType,
     },
 )
 
-HistoricalMetricResultOutputTypeDef = TypedDict(
-    "HistoricalMetricResultOutputTypeDef",
+HistoricalMetricResultTypeDef = TypedDict(
+    "HistoricalMetricResultTypeDef",
     {
-        "Dimensions": "DimensionsOutputTypeDef",
-        "Collections": List["HistoricalMetricDataOutputTypeDef"],
+        "Dimensions": "DimensionsTypeDef",
+        "Collections": List["HistoricalMetricDataTypeDef"],
     },
 )
 
 HistoricalMetricTypeDef = TypedDict(
     "HistoricalMetricTypeDef",
     {
         "Name": HistoricalMetricNameType,
@@ -3540,27 +3540,14 @@
     {
         "Day": HoursOfOperationDaysType,
         "StartTime": "HoursOfOperationTimeSliceTypeDef",
         "EndTime": "HoursOfOperationTimeSliceTypeDef",
     },
 )
 
-HoursOfOperationOutputTypeDef = TypedDict(
-    "HoursOfOperationOutputTypeDef",
-    {
-        "HoursOfOperationId": str,
-        "HoursOfOperationArn": str,
-        "Name": str,
-        "Description": str,
-        "TimeZone": str,
-        "Config": List["HoursOfOperationConfigOutputTypeDef"],
-        "Tags": Dict[str, str],
-    },
-)
-
 HoursOfOperationSearchCriteriaTypeDef = TypedDict(
     "HoursOfOperationSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -3571,16 +3558,16 @@
     "HoursOfOperationSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-HoursOfOperationSummaryOutputTypeDef = TypedDict(
-    "HoursOfOperationSummaryOutputTypeDef",
+HoursOfOperationSummaryTypeDef = TypedDict(
+    "HoursOfOperationSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
@@ -3596,33 +3583,29 @@
     "HoursOfOperationTimeSliceTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
 
-InstanceOutputTypeDef = TypedDict(
-    "InstanceOutputTypeDef",
+HoursOfOperationTypeDef = TypedDict(
+    "HoursOfOperationTypeDef",
     {
-        "Id": str,
-        "Arn": str,
-        "IdentityManagementType": DirectoryTypeType,
-        "InstanceAlias": str,
-        "CreatedTime": datetime,
-        "ServiceRole": str,
-        "InstanceStatus": InstanceStatusType,
-        "StatusReason": "InstanceStatusReasonOutputTypeDef",
-        "InboundCallsEnabled": bool,
-        "OutboundCallsEnabled": bool,
-        "InstanceAccessUrl": str,
+        "HoursOfOperationId": str,
+        "HoursOfOperationArn": str,
+        "Name": str,
+        "Description": str,
+        "TimeZone": str,
+        "Config": List["HoursOfOperationConfigOutputTypeDef"],
+        "Tags": Dict[str, str],
     },
 )
 
-InstanceStatusReasonOutputTypeDef = TypedDict(
-    "InstanceStatusReasonOutputTypeDef",
+InstanceStatusReasonTypeDef = TypedDict(
+    "InstanceStatusReasonTypeDef",
     {
         "Message": str,
     },
 )
 
 InstanceStorageConfigOutputTypeDef = TypedDict(
     "InstanceStorageConfigOutputTypeDef",
@@ -3657,32 +3640,49 @@
 
 class InstanceStorageConfigTypeDef(
     _RequiredInstanceStorageConfigTypeDef, _OptionalInstanceStorageConfigTypeDef
 ):
     pass
 
 
-InstanceSummaryOutputTypeDef = TypedDict(
-    "InstanceSummaryOutputTypeDef",
+InstanceSummaryTypeDef = TypedDict(
+    "InstanceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "IdentityManagementType": DirectoryTypeType,
         "InstanceAlias": str,
         "CreatedTime": datetime,
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
 )
 
-IntegrationAssociationSummaryOutputTypeDef = TypedDict(
-    "IntegrationAssociationSummaryOutputTypeDef",
+InstanceTypeDef = TypedDict(
+    "InstanceTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "IdentityManagementType": DirectoryTypeType,
+        "InstanceAlias": str,
+        "CreatedTime": datetime,
+        "ServiceRole": str,
+        "InstanceStatus": InstanceStatusType,
+        "StatusReason": "InstanceStatusReasonTypeDef",
+        "InboundCallsEnabled": bool,
+        "OutboundCallsEnabled": bool,
+        "InstanceAccessUrl": str,
+    },
+)
+
+IntegrationAssociationSummaryTypeDef = TypedDict(
+    "IntegrationAssociationSummaryTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
         "SourceApplicationUrl": str,
@@ -3748,16 +3748,16 @@
     {
         "Prefix": str,
         "RetentionPeriodHours": int,
         "EncryptionConfig": "EncryptionConfigTypeDef",
     },
 )
 
-LexBotConfigOutputTypeDef = TypedDict(
-    "LexBotConfigOutputTypeDef",
+LexBotConfigTypeDef = TypedDict(
+    "LexBotConfigTypeDef",
     {
         "LexBot": "LexBotOutputTypeDef",
         "LexV2Bot": "LexV2BotOutputTypeDef",
     },
 )
 
 LexBotOutputTypeDef = TypedDict(
@@ -3833,19 +3833,19 @@
 
 class ListAgentStatusRequestRequestTypeDef(
     _RequiredListAgentStatusRequestRequestTypeDef, _OptionalListAgentStatusRequestRequestTypeDef
 ):
     pass
 
 
-ListAgentStatusResponseOutputTypeDef = TypedDict(
-    "ListAgentStatusResponseOutputTypeDef",
+ListAgentStatusResponseTypeDef = TypedDict(
+    "ListAgentStatusResponseTypeDef",
     {
         "NextToken": str,
-        "AgentStatusSummaryList": List["AgentStatusSummaryOutputTypeDef"],
+        "AgentStatusSummaryList": List["AgentStatusSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
@@ -3887,16 +3887,16 @@
 class ListApprovedOriginsRequestRequestTypeDef(
     _RequiredListApprovedOriginsRequestRequestTypeDef,
     _OptionalListApprovedOriginsRequestRequestTypeDef,
 ):
     pass
 
 
-ListApprovedOriginsResponseOutputTypeDef = TypedDict(
-    "ListApprovedOriginsResponseOutputTypeDef",
+ListApprovedOriginsResponseTypeDef = TypedDict(
+    "ListApprovedOriginsResponseTypeDef",
     {
         "Origins": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3941,18 +3941,18 @@
 
 class ListBotsRequestRequestTypeDef(
     _RequiredListBotsRequestRequestTypeDef, _OptionalListBotsRequestRequestTypeDef
 ):
     pass
 
 
-ListBotsResponseOutputTypeDef = TypedDict(
-    "ListBotsResponseOutputTypeDef",
+ListBotsResponseTypeDef = TypedDict(
+    "ListBotsResponseTypeDef",
     {
-        "LexBots": List["LexBotConfigOutputTypeDef"],
+        "LexBots": List["LexBotConfigTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
@@ -3996,18 +3996,18 @@
 class ListContactEvaluationsRequestRequestTypeDef(
     _RequiredListContactEvaluationsRequestRequestTypeDef,
     _OptionalListContactEvaluationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListContactEvaluationsResponseOutputTypeDef = TypedDict(
-    "ListContactEvaluationsResponseOutputTypeDef",
+ListContactEvaluationsResponseTypeDef = TypedDict(
+    "ListContactEvaluationsResponseTypeDef",
     {
-        "EvaluationSummaryList": List["EvaluationSummaryOutputTypeDef"],
+        "EvaluationSummaryList": List["EvaluationSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
@@ -4052,18 +4052,18 @@
 class ListContactFlowModulesRequestRequestTypeDef(
     _RequiredListContactFlowModulesRequestRequestTypeDef,
     _OptionalListContactFlowModulesRequestRequestTypeDef,
 ):
     pass
 
 
-ListContactFlowModulesResponseOutputTypeDef = TypedDict(
-    "ListContactFlowModulesResponseOutputTypeDef",
+ListContactFlowModulesResponseTypeDef = TypedDict(
+    "ListContactFlowModulesResponseTypeDef",
     {
-        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryOutputTypeDef"],
+        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef",
@@ -4107,18 +4107,18 @@
 
 class ListContactFlowsRequestRequestTypeDef(
     _RequiredListContactFlowsRequestRequestTypeDef, _OptionalListContactFlowsRequestRequestTypeDef
 ):
     pass
 
 
-ListContactFlowsResponseOutputTypeDef = TypedDict(
-    "ListContactFlowsResponseOutputTypeDef",
+ListContactFlowsResponseTypeDef = TypedDict(
+    "ListContactFlowsResponseTypeDef",
     {
-        "ContactFlowSummaryList": List["ContactFlowSummaryOutputTypeDef"],
+        "ContactFlowSummaryList": List["ContactFlowSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef",
@@ -4164,18 +4164,18 @@
 class ListContactReferencesRequestRequestTypeDef(
     _RequiredListContactReferencesRequestRequestTypeDef,
     _OptionalListContactReferencesRequestRequestTypeDef,
 ):
     pass
 
 
-ListContactReferencesResponseOutputTypeDef = TypedDict(
-    "ListContactReferencesResponseOutputTypeDef",
+ListContactReferencesResponseTypeDef = TypedDict(
+    "ListContactReferencesResponseTypeDef",
     {
-        "ReferenceSummaryList": List["ReferenceSummaryOutputTypeDef"],
+        "ReferenceSummaryList": List["ReferenceSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
@@ -4220,18 +4220,18 @@
 class ListDefaultVocabulariesRequestRequestTypeDef(
     _RequiredListDefaultVocabulariesRequestRequestTypeDef,
     _OptionalListDefaultVocabulariesRequestRequestTypeDef,
 ):
     pass
 
 
-ListDefaultVocabulariesResponseOutputTypeDef = TypedDict(
-    "ListDefaultVocabulariesResponseOutputTypeDef",
+ListDefaultVocabulariesResponseTypeDef = TypedDict(
+    "ListDefaultVocabulariesResponseTypeDef",
     {
-        "DefaultVocabularyList": List["DefaultVocabularyOutputTypeDef"],
+        "DefaultVocabularyList": List["DefaultVocabularyTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
@@ -4276,18 +4276,18 @@
 class ListEvaluationFormVersionsRequestRequestTypeDef(
     _RequiredListEvaluationFormVersionsRequestRequestTypeDef,
     _OptionalListEvaluationFormVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListEvaluationFormVersionsResponseOutputTypeDef = TypedDict(
-    "ListEvaluationFormVersionsResponseOutputTypeDef",
+ListEvaluationFormVersionsResponseTypeDef = TypedDict(
+    "ListEvaluationFormVersionsResponseTypeDef",
     {
-        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryOutputTypeDef"],
+        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
@@ -4330,18 +4330,18 @@
 class ListEvaluationFormsRequestRequestTypeDef(
     _RequiredListEvaluationFormsRequestRequestTypeDef,
     _OptionalListEvaluationFormsRequestRequestTypeDef,
 ):
     pass
 
 
-ListEvaluationFormsResponseOutputTypeDef = TypedDict(
-    "ListEvaluationFormsResponseOutputTypeDef",
+ListEvaluationFormsResponseTypeDef = TypedDict(
+    "ListEvaluationFormsResponseTypeDef",
     {
-        "EvaluationFormSummaryList": List["EvaluationFormSummaryOutputTypeDef"],
+        "EvaluationFormSummaryList": List["EvaluationFormSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
@@ -4384,18 +4384,18 @@
 class ListHoursOfOperationsRequestRequestTypeDef(
     _RequiredListHoursOfOperationsRequestRequestTypeDef,
     _OptionalListHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListHoursOfOperationsResponseOutputTypeDef = TypedDict(
-    "ListHoursOfOperationsResponseOutputTypeDef",
+ListHoursOfOperationsResponseTypeDef = TypedDict(
+    "ListHoursOfOperationsResponseTypeDef",
     {
-        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryOutputTypeDef"],
+        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
@@ -4438,18 +4438,18 @@
 class ListInstanceAttributesRequestRequestTypeDef(
     _RequiredListInstanceAttributesRequestRequestTypeDef,
     _OptionalListInstanceAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-ListInstanceAttributesResponseOutputTypeDef = TypedDict(
-    "ListInstanceAttributesResponseOutputTypeDef",
+ListInstanceAttributesResponseTypeDef = TypedDict(
+    "ListInstanceAttributesResponseTypeDef",
     {
-        "Attributes": List["AttributeOutputTypeDef"],
+        "Attributes": List["AttributeTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
@@ -4494,16 +4494,16 @@
 class ListInstanceStorageConfigsRequestRequestTypeDef(
     _RequiredListInstanceStorageConfigsRequestRequestTypeDef,
     _OptionalListInstanceStorageConfigsRequestRequestTypeDef,
 ):
     pass
 
 
-ListInstanceStorageConfigsResponseOutputTypeDef = TypedDict(
-    "ListInstanceStorageConfigsResponseOutputTypeDef",
+ListInstanceStorageConfigsResponseTypeDef = TypedDict(
+    "ListInstanceStorageConfigsResponseTypeDef",
     {
         "StorageConfigs": List["InstanceStorageConfigOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4520,18 +4520,18 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListInstancesResponseOutputTypeDef = TypedDict(
-    "ListInstancesResponseOutputTypeDef",
+ListInstancesResponseTypeDef = TypedDict(
+    "ListInstancesResponseTypeDef",
     {
-        "InstanceSummaryList": List["InstanceSummaryOutputTypeDef"],
+        "InstanceSummaryList": List["InstanceSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
@@ -4576,18 +4576,18 @@
 class ListIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListIntegrationAssociationsResponseOutputTypeDef = TypedDict(
-    "ListIntegrationAssociationsResponseOutputTypeDef",
+ListIntegrationAssociationsResponseTypeDef = TypedDict(
+    "ListIntegrationAssociationsResponseTypeDef",
     {
-        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryOutputTypeDef"],
+        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
@@ -4630,16 +4630,16 @@
 class ListLambdaFunctionsRequestRequestTypeDef(
     _RequiredListLambdaFunctionsRequestRequestTypeDef,
     _OptionalListLambdaFunctionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListLambdaFunctionsResponseOutputTypeDef = TypedDict(
-    "ListLambdaFunctionsResponseOutputTypeDef",
+ListLambdaFunctionsResponseTypeDef = TypedDict(
+    "ListLambdaFunctionsResponseTypeDef",
     {
         "LambdaFunctions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4683,16 +4683,16 @@
 
 class ListLexBotsRequestRequestTypeDef(
     _RequiredListLexBotsRequestRequestTypeDef, _OptionalListLexBotsRequestRequestTypeDef
 ):
     pass
 
 
-ListLexBotsResponseOutputTypeDef = TypedDict(
-    "ListLexBotsResponseOutputTypeDef",
+ListLexBotsResponseTypeDef = TypedDict(
+    "ListLexBotsResponseTypeDef",
     {
         "LexBots": List["LexBotOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4740,25 +4740,25 @@
 
 class ListPhoneNumbersRequestRequestTypeDef(
     _RequiredListPhoneNumbersRequestRequestTypeDef, _OptionalListPhoneNumbersRequestRequestTypeDef
 ):
     pass
 
 
-ListPhoneNumbersResponseOutputTypeDef = TypedDict(
-    "ListPhoneNumbersResponseOutputTypeDef",
+ListPhoneNumbersResponseTypeDef = TypedDict(
+    "ListPhoneNumbersResponseTypeDef",
     {
-        "PhoneNumberSummaryList": List["PhoneNumberSummaryOutputTypeDef"],
+        "PhoneNumberSummaryList": List["PhoneNumberSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPhoneNumbersSummaryOutputTypeDef = TypedDict(
-    "ListPhoneNumbersSummaryOutputTypeDef",
+ListPhoneNumbersSummaryTypeDef = TypedDict(
+    "ListPhoneNumbersSummaryTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": str,
@@ -4786,19 +4786,19 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberPrefix": str,
     },
     total=False,
 )
 
-ListPhoneNumbersV2ResponseOutputTypeDef = TypedDict(
-    "ListPhoneNumbersV2ResponseOutputTypeDef",
+ListPhoneNumbersV2ResponseTypeDef = TypedDict(
+    "ListPhoneNumbersV2ResponseTypeDef",
     {
         "NextToken": str,
-        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryOutputTypeDef"],
+        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPromptsRequestListPromptsPaginateTypeDef = TypedDict(
     "_RequiredListPromptsRequestListPromptsPaginateTypeDef",
     {
@@ -4839,18 +4839,18 @@
 
 class ListPromptsRequestRequestTypeDef(
     _RequiredListPromptsRequestRequestTypeDef, _OptionalListPromptsRequestRequestTypeDef
 ):
     pass
 
 
-ListPromptsResponseOutputTypeDef = TypedDict(
-    "ListPromptsResponseOutputTypeDef",
+ListPromptsResponseTypeDef = TypedDict(
+    "ListPromptsResponseTypeDef",
     {
-        "PromptSummaryList": List["PromptSummaryOutputTypeDef"],
+        "PromptSummaryList": List["PromptSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
@@ -4895,19 +4895,19 @@
 class ListQueueQuickConnectsRequestRequestTypeDef(
     _RequiredListQueueQuickConnectsRequestRequestTypeDef,
     _OptionalListQueueQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
 
-ListQueueQuickConnectsResponseOutputTypeDef = TypedDict(
-    "ListQueueQuickConnectsResponseOutputTypeDef",
+ListQueueQuickConnectsResponseTypeDef = TypedDict(
+    "ListQueueQuickConnectsResponseTypeDef",
     {
         "NextToken": str,
-        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
     "_RequiredListQueuesRequestListQueuesPaginateTypeDef",
     {
@@ -4950,18 +4950,18 @@
 
 class ListQueuesRequestRequestTypeDef(
     _RequiredListQueuesRequestRequestTypeDef, _OptionalListQueuesRequestRequestTypeDef
 ):
     pass
 
 
-ListQueuesResponseOutputTypeDef = TypedDict(
-    "ListQueuesResponseOutputTypeDef",
+ListQueuesResponseTypeDef = TypedDict(
+    "ListQueuesResponseTypeDef",
     {
-        "QueueSummaryList": List["QueueSummaryOutputTypeDef"],
+        "QueueSummaryList": List["QueueSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
@@ -5005,18 +5005,18 @@
 
 class ListQuickConnectsRequestRequestTypeDef(
     _RequiredListQuickConnectsRequestRequestTypeDef, _OptionalListQuickConnectsRequestRequestTypeDef
 ):
     pass
 
 
-ListQuickConnectsResponseOutputTypeDef = TypedDict(
-    "ListQuickConnectsResponseOutputTypeDef",
+ListQuickConnectsResponseTypeDef = TypedDict(
+    "ListQuickConnectsResponseTypeDef",
     {
-        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
@@ -5061,21 +5061,19 @@
 class ListRoutingProfileQueuesRequestRequestTypeDef(
     _RequiredListRoutingProfileQueuesRequestRequestTypeDef,
     _OptionalListRoutingProfileQueuesRequestRequestTypeDef,
 ):
     pass
 
 
-ListRoutingProfileQueuesResponseOutputTypeDef = TypedDict(
-    "ListRoutingProfileQueuesResponseOutputTypeDef",
+ListRoutingProfileQueuesResponseTypeDef = TypedDict(
+    "ListRoutingProfileQueuesResponseTypeDef",
     {
         "NextToken": str,
-        "RoutingProfileQueueConfigSummaryList": List[
-            "RoutingProfileQueueConfigSummaryOutputTypeDef"
-        ],
+        "RoutingProfileQueueConfigSummaryList": List["RoutingProfileQueueConfigSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
@@ -5117,18 +5115,18 @@
 class ListRoutingProfilesRequestRequestTypeDef(
     _RequiredListRoutingProfilesRequestRequestTypeDef,
     _OptionalListRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
 
-ListRoutingProfilesResponseOutputTypeDef = TypedDict(
-    "ListRoutingProfilesResponseOutputTypeDef",
+ListRoutingProfilesResponseTypeDef = TypedDict(
+    "ListRoutingProfilesResponseTypeDef",
     {
-        "RoutingProfileSummaryList": List["RoutingProfileSummaryOutputTypeDef"],
+        "RoutingProfileSummaryList": List["RoutingProfileSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
@@ -5174,18 +5172,18 @@
 
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
 
-ListRulesResponseOutputTypeDef = TypedDict(
-    "ListRulesResponseOutputTypeDef",
+ListRulesResponseTypeDef = TypedDict(
+    "ListRulesResponseTypeDef",
     {
-        "RuleSummaryList": List["RuleSummaryOutputTypeDef"],
+        "RuleSummaryList": List["RuleSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
@@ -5227,18 +5225,18 @@
 
 class ListSecurityKeysRequestRequestTypeDef(
     _RequiredListSecurityKeysRequestRequestTypeDef, _OptionalListSecurityKeysRequestRequestTypeDef
 ):
     pass
 
 
-ListSecurityKeysResponseOutputTypeDef = TypedDict(
-    "ListSecurityKeysResponseOutputTypeDef",
+ListSecurityKeysResponseTypeDef = TypedDict(
+    "ListSecurityKeysResponseTypeDef",
     {
-        "SecurityKeys": List["SecurityKeyOutputTypeDef"],
+        "SecurityKeys": List["SecurityKeyTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
@@ -5283,16 +5281,16 @@
 class ListSecurityProfilePermissionsRequestRequestTypeDef(
     _RequiredListSecurityProfilePermissionsRequestRequestTypeDef,
     _OptionalListSecurityProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListSecurityProfilePermissionsResponseOutputTypeDef = TypedDict(
-    "ListSecurityProfilePermissionsResponseOutputTypeDef",
+ListSecurityProfilePermissionsResponseTypeDef = TypedDict(
+    "ListSecurityProfilePermissionsResponseTypeDef",
     {
         "Permissions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -5337,32 +5335,32 @@
 class ListSecurityProfilesRequestRequestTypeDef(
     _RequiredListSecurityProfilesRequestRequestTypeDef,
     _OptionalListSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
 
-ListSecurityProfilesResponseOutputTypeDef = TypedDict(
-    "ListSecurityProfilesResponseOutputTypeDef",
+ListSecurityProfilesResponseTypeDef = TypedDict(
+    "ListSecurityProfilesResponseTypeDef",
     {
-        "SecurityProfileSummaryList": List["SecurityProfileSummaryOutputTypeDef"],
+        "SecurityProfileSummaryList": List["SecurityProfileSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
@@ -5409,18 +5407,18 @@
 
 class ListTaskTemplatesRequestRequestTypeDef(
     _RequiredListTaskTemplatesRequestRequestTypeDef, _OptionalListTaskTemplatesRequestRequestTypeDef
 ):
     pass
 
 
-ListTaskTemplatesResponseOutputTypeDef = TypedDict(
-    "ListTaskTemplatesResponseOutputTypeDef",
+ListTaskTemplatesResponseTypeDef = TypedDict(
+    "ListTaskTemplatesResponseTypeDef",
     {
-        "TaskTemplates": List["TaskTemplateMetadataOutputTypeDef"],
+        "TaskTemplates": List["TaskTemplateMetadataTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef = TypedDict(
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
@@ -5437,19 +5435,19 @@
         "MaxResults": int,
         "NextToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
-ListTrafficDistributionGroupsResponseOutputTypeDef = TypedDict(
-    "ListTrafficDistributionGroupsResponseOutputTypeDef",
+ListTrafficDistributionGroupsResponseTypeDef = TypedDict(
+    "ListTrafficDistributionGroupsResponseTypeDef",
     {
         "NextToken": str,
-        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryOutputTypeDef"],
+        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUseCasesRequestListUseCasesPaginateTypeDef = TypedDict(
     "_RequiredListUseCasesRequestListUseCasesPaginateTypeDef",
     {
@@ -5492,18 +5490,18 @@
 
 class ListUseCasesRequestRequestTypeDef(
     _RequiredListUseCasesRequestRequestTypeDef, _OptionalListUseCasesRequestRequestTypeDef
 ):
     pass
 
 
-ListUseCasesResponseOutputTypeDef = TypedDict(
-    "ListUseCasesResponseOutputTypeDef",
+ListUseCasesResponseTypeDef = TypedDict(
+    "ListUseCasesResponseTypeDef",
     {
-        "UseCaseSummaryList": List["UseCaseOutputTypeDef"],
+        "UseCaseSummaryList": List["UseCaseTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
@@ -5546,18 +5544,18 @@
 class ListUserHierarchyGroupsRequestRequestTypeDef(
     _RequiredListUserHierarchyGroupsRequestRequestTypeDef,
     _OptionalListUserHierarchyGroupsRequestRequestTypeDef,
 ):
     pass
 
 
-ListUserHierarchyGroupsResponseOutputTypeDef = TypedDict(
-    "ListUserHierarchyGroupsResponseOutputTypeDef",
+ListUserHierarchyGroupsResponseTypeDef = TypedDict(
+    "ListUserHierarchyGroupsResponseTypeDef",
     {
-        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryOutputTypeDef"],
+        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
@@ -5599,18 +5597,18 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-ListUsersResponseOutputTypeDef = TypedDict(
-    "ListUsersResponseOutputTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "UserSummaryList": List["UserSummaryOutputTypeDef"],
+        "UserSummaryList": List["UserSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaConcurrencyOutputTypeDef = TypedDict(
     "MediaConcurrencyOutputTypeDef",
@@ -5637,16 +5635,16 @@
 )
 
 
 class MediaConcurrencyTypeDef(_RequiredMediaConcurrencyTypeDef, _OptionalMediaConcurrencyTypeDef):
     pass
 
 
-MetricDataV2OutputTypeDef = TypedDict(
-    "MetricDataV2OutputTypeDef",
+MetricDataV2TypeDef = TypedDict(
+    "MetricDataV2TypeDef",
     {
         "Metric": "MetricV2OutputTypeDef",
         "Value": float,
     },
 )
 
 MetricFilterV2OutputTypeDef = TypedDict(
@@ -5662,19 +5660,19 @@
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
     },
     total=False,
 )
 
-MetricResultV2OutputTypeDef = TypedDict(
-    "MetricResultV2OutputTypeDef",
+MetricResultV2TypeDef = TypedDict(
+    "MetricResultV2TypeDef",
     {
         "Dimensions": Dict[str, str],
-        "Collections": List["MetricDataV2OutputTypeDef"],
+        "Collections": List["MetricDataV2TypeDef"],
     },
 )
 
 MetricV2OutputTypeDef = TypedDict(
     "MetricV2OutputTypeDef",
     {
         "Name": str,
@@ -5713,16 +5711,16 @@
 
 class MonitorContactRequestRequestTypeDef(
     _RequiredMonitorContactRequestRequestTypeDef, _OptionalMonitorContactRequestRequestTypeDef
 ):
     pass
 
 
-MonitorContactResponseOutputTypeDef = TypedDict(
-    "MonitorContactResponseOutputTypeDef",
+MonitorContactResponseTypeDef = TypedDict(
+    "MonitorContactResponseTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -5739,16 +5737,16 @@
     {
         "UserTags": Mapping[str, str],
         "UserIds": Sequence[str],
     },
     total=False,
 )
 
-NumberReferenceOutputTypeDef = TypedDict(
-    "NumberReferenceOutputTypeDef",
+NumberReferenceTypeDef = TypedDict(
+    "NumberReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 NumericQuestionPropertyValueAutomationOutputTypeDef = TypedDict(
@@ -5824,16 +5822,16 @@
     {
         "ParticipantTimerAction": Literal["Unset"],
         "ParticipantTimerDurationInMinutes": int,
     },
     total=False,
 )
 
-ParticipantTokenCredentialsOutputTypeDef = TypedDict(
-    "ParticipantTokenCredentialsOutputTypeDef",
+ParticipantTokenCredentialsTypeDef = TypedDict(
+    "ParticipantTokenCredentialsTypeDef",
     {
         "ParticipantToken": str,
         "Expiry": str,
     },
 )
 
 PersistentChatTypeDef = TypedDict(
@@ -5855,44 +5853,33 @@
 PhoneNumberQuickConnectConfigTypeDef = TypedDict(
     "PhoneNumberQuickConnectConfigTypeDef",
     {
         "PhoneNumber": str,
     },
 )
 
-PhoneNumberStatusOutputTypeDef = TypedDict(
-    "PhoneNumberStatusOutputTypeDef",
+PhoneNumberStatusTypeDef = TypedDict(
+    "PhoneNumberStatusTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
 )
 
-PhoneNumberSummaryOutputTypeDef = TypedDict(
-    "PhoneNumberSummaryOutputTypeDef",
+PhoneNumberSummaryTypeDef = TypedDict(
+    "PhoneNumberSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
     },
 )
 
-PromptOutputTypeDef = TypedDict(
-    "PromptOutputTypeDef",
-    {
-        "PromptARN": str,
-        "PromptId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 PromptSearchCriteriaTypeDef = TypedDict(
     "PromptSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -5903,55 +5890,51 @@
     "PromptSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-PromptSummaryOutputTypeDef = TypedDict(
-    "PromptSummaryOutputTypeDef",
+PromptSummaryTypeDef = TypedDict(
+    "PromptSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+PromptTypeDef = TypedDict(
+    "PromptTypeDef",
+    {
+        "PromptARN": str,
+        "PromptId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+    },
+)
+
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-QueueInfoOutputTypeDef = TypedDict(
-    "QueueInfoOutputTypeDef",
+QueueInfoTypeDef = TypedDict(
+    "QueueInfoTypeDef",
     {
         "Id": str,
         "EnqueueTimestamp": datetime,
     },
 )
 
-QueueOutputTypeDef = TypedDict(
-    "QueueOutputTypeDef",
-    {
-        "Name": str,
-        "QueueArn": str,
-        "QueueId": str,
-        "Description": str,
-        "OutboundCallerConfig": "OutboundCallerConfigOutputTypeDef",
-        "HoursOfOperationId": str,
-        "MaxContacts": int,
-        "Status": QueueStatusType,
-        "Tags": Dict[str, str],
-    },
-)
-
 QueueQuickConnectConfigOutputTypeDef = TypedDict(
     "QueueQuickConnectConfigOutputTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
     },
 )
@@ -5960,16 +5943,16 @@
     "QueueQuickConnectConfigTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
     },
 )
 
-QueueReferenceOutputTypeDef = TypedDict(
-    "QueueReferenceOutputTypeDef",
+QueueReferenceTypeDef = TypedDict(
+    "QueueReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 QueueSearchCriteriaTypeDef = TypedDict(
@@ -5987,24 +5970,39 @@
     "QueueSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QueueSummaryOutputTypeDef = TypedDict(
-    "QueueSummaryOutputTypeDef",
+QueueSummaryTypeDef = TypedDict(
+    "QueueSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
     },
 )
 
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
+    {
+        "Name": str,
+        "QueueArn": str,
+        "QueueId": str,
+        "Description": str,
+        "OutboundCallerConfig": "OutboundCallerConfigOutputTypeDef",
+        "HoursOfOperationId": str,
+        "MaxContacts": int,
+        "Status": QueueStatusType,
+        "Tags": Dict[str, str],
+    },
+)
+
 QuickConnectConfigOutputTypeDef = TypedDict(
     "QuickConnectConfigOutputTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
         "UserConfig": "UserQuickConnectConfigOutputTypeDef",
         "QueueConfig": "QueueQuickConnectConfigOutputTypeDef",
         "PhoneConfig": "PhoneNumberQuickConnectConfigOutputTypeDef",
@@ -6030,26 +6028,14 @@
 
 class QuickConnectConfigTypeDef(
     _RequiredQuickConnectConfigTypeDef, _OptionalQuickConnectConfigTypeDef
 ):
     pass
 
 
-QuickConnectOutputTypeDef = TypedDict(
-    "QuickConnectOutputTypeDef",
-    {
-        "QuickConnectARN": str,
-        "QuickConnectId": str,
-        "Name": str,
-        "Description": str,
-        "QuickConnectConfig": "QuickConnectConfigOutputTypeDef",
-        "Tags": Dict[str, str],
-    },
-)
-
 QuickConnectSearchCriteriaTypeDef = TypedDict(
     "QuickConnectSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -6060,24 +6046,36 @@
     "QuickConnectSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QuickConnectSummaryOutputTypeDef = TypedDict(
-    "QuickConnectSummaryOutputTypeDef",
+QuickConnectSummaryTypeDef = TypedDict(
+    "QuickConnectSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
     },
 )
 
+QuickConnectTypeDef = TypedDict(
+    "QuickConnectTypeDef",
+    {
+        "QuickConnectARN": str,
+        "QuickConnectId": str,
+        "Name": str,
+        "Description": str,
+        "QuickConnectConfig": "QuickConnectConfigOutputTypeDef",
+        "Tags": Dict[str, str],
+    },
+)
+
 ReadOnlyFieldInfoOutputTypeDef = TypedDict(
     "ReadOnlyFieldInfoOutputTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
     },
 )
 
@@ -6093,23 +6091,23 @@
     "ReferenceOutputTypeDef",
     {
         "Value": str,
         "Type": ReferenceTypeType,
     },
 )
 
-ReferenceSummaryOutputTypeDef = TypedDict(
-    "ReferenceSummaryOutputTypeDef",
+ReferenceSummaryTypeDef = TypedDict(
+    "ReferenceSummaryTypeDef",
     {
-        "Url": "UrlReferenceOutputTypeDef",
-        "Attachment": "AttachmentReferenceOutputTypeDef",
-        "String": "StringReferenceOutputTypeDef",
-        "Number": "NumberReferenceOutputTypeDef",
-        "Date": "DateReferenceOutputTypeDef",
-        "Email": "EmailReferenceOutputTypeDef",
+        "Url": "UrlReferenceTypeDef",
+        "Attachment": "AttachmentReferenceTypeDef",
+        "String": "StringReferenceTypeDef",
+        "Number": "NumberReferenceTypeDef",
+        "Date": "DateReferenceTypeDef",
+        "Email": "EmailReferenceTypeDef",
     },
 )
 
 ReferenceTypeDef = TypedDict(
     "ReferenceTypeDef",
     {
         "Value": str,
@@ -6158,16 +6156,16 @@
 
 class ReplicateInstanceRequestRequestTypeDef(
     _RequiredReplicateInstanceRequestRequestTypeDef, _OptionalReplicateInstanceRequestRequestTypeDef
 ):
     pass
 
 
-ReplicateInstanceResponseOutputTypeDef = TypedDict(
-    "ReplicateInstanceResponseOutputTypeDef",
+ReplicateInstanceResponseTypeDef = TypedDict(
+    "ReplicateInstanceResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6210,32 +6208,16 @@
     {
         "InstanceId": str,
         "ContactId": str,
         "InitialContactId": str,
     },
 )
 
-RoutingProfileOutputTypeDef = TypedDict(
-    "RoutingProfileOutputTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "RoutingProfileArn": str,
-        "RoutingProfileId": str,
-        "Description": str,
-        "MediaConcurrencies": List["MediaConcurrencyOutputTypeDef"],
-        "DefaultOutboundQueueId": str,
-        "Tags": Dict[str, str],
-        "NumberOfAssociatedQueues": int,
-        "NumberOfAssociatedUsers": int,
-    },
-)
-
-RoutingProfileQueueConfigSummaryOutputTypeDef = TypedDict(
-    "RoutingProfileQueueConfigSummaryOutputTypeDef",
+RoutingProfileQueueConfigSummaryTypeDef = TypedDict(
+    "RoutingProfileQueueConfigSummaryTypeDef",
     {
         "QueueId": str,
         "QueueArn": str,
         "QueueName": str,
         "Priority": int,
         "Delay": int,
         "Channel": ChannelType,
@@ -6255,16 +6237,16 @@
     "RoutingProfileQueueReferenceTypeDef",
     {
         "QueueId": str,
         "Channel": ChannelType,
     },
 )
 
-RoutingProfileReferenceOutputTypeDef = TypedDict(
-    "RoutingProfileReferenceOutputTypeDef",
+RoutingProfileReferenceTypeDef = TypedDict(
+    "RoutingProfileReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 RoutingProfileSearchCriteriaTypeDef = TypedDict(
@@ -6281,23 +6263,39 @@
     "RoutingProfileSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-RoutingProfileSummaryOutputTypeDef = TypedDict(
-    "RoutingProfileSummaryOutputTypeDef",
+RoutingProfileSummaryTypeDef = TypedDict(
+    "RoutingProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+RoutingProfileTypeDef = TypedDict(
+    "RoutingProfileTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "RoutingProfileArn": str,
+        "RoutingProfileId": str,
+        "Description": str,
+        "MediaConcurrencies": List["MediaConcurrencyOutputTypeDef"],
+        "DefaultOutboundQueueId": str,
+        "Tags": Dict[str, str],
+        "NumberOfAssociatedQueues": int,
+        "NumberOfAssociatedUsers": int,
+    },
+)
+
 RuleActionOutputTypeDef = TypedDict(
     "RuleActionOutputTypeDef",
     {
         "ActionType": ActionTypeType,
         "TaskAction": "TaskActionDefinitionOutputTypeDef",
         "EventBridgeAction": "EventBridgeActionDefinitionOutputTypeDef",
         "AssignContactCategoryAction": Dict[str, Any],
@@ -6323,40 +6321,23 @@
 )
 
 
 class RuleActionTypeDef(_RequiredRuleActionTypeDef, _OptionalRuleActionTypeDef):
     pass
 
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "Name": str,
-        "RuleId": str,
-        "RuleArn": str,
-        "TriggerEventSource": "RuleTriggerEventSourceOutputTypeDef",
-        "Function": str,
-        "Actions": List["RuleActionOutputTypeDef"],
-        "PublishStatus": RulePublishStatusType,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "LastUpdatedBy": str,
-        "Tags": Dict[str, str],
-    },
-)
-
-RuleSummaryOutputTypeDef = TypedDict(
-    "RuleSummaryOutputTypeDef",
+RuleSummaryTypeDef = TypedDict(
+    "RuleSummaryTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "EventSourceName": EventSourceNameType,
         "PublishStatus": RulePublishStatusType,
-        "ActionSummaries": List["ActionSummaryOutputTypeDef"],
+        "ActionSummaries": List["ActionSummaryTypeDef"],
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
     },
 )
 
 RuleTriggerEventSourceOutputTypeDef = TypedDict(
     "RuleTriggerEventSourceOutputTypeDef",
@@ -6383,14 +6364,31 @@
 
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
 
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "Name": str,
+        "RuleId": str,
+        "RuleArn": str,
+        "TriggerEventSource": "RuleTriggerEventSourceOutputTypeDef",
+        "Function": str,
+        "Actions": List["RuleActionOutputTypeDef"],
+        "PublishStatus": RulePublishStatusType,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "LastUpdatedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
 S3ConfigOutputTypeDef = TypedDict(
     "S3ConfigOutputTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "EncryptionConfig": "EncryptionConfigOutputTypeDef",
     },
@@ -6463,19 +6461,19 @@
 class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
 ):
     pass
 
 
-SearchAvailablePhoneNumbersResponseOutputTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     {
         "NextToken": str,
-        "AvailableNumbersList": List["AvailableNumberSummaryOutputTypeDef"],
+        "AvailableNumbersList": List["AvailableNumberSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestRequestTypeDef",
     {
@@ -6521,18 +6519,18 @@
 class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(
     _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
     _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
 
-SearchHoursOfOperationsResponseOutputTypeDef = TypedDict(
-    "SearchHoursOfOperationsResponseOutputTypeDef",
+SearchHoursOfOperationsResponseTypeDef = TypedDict(
+    "SearchHoursOfOperationsResponseTypeDef",
     {
-        "HoursOfOperations": List["HoursOfOperationOutputTypeDef"],
+        "HoursOfOperations": List["HoursOfOperationTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchPromptsRequestRequestTypeDef = TypedDict(
@@ -6579,18 +6577,18 @@
 class SearchPromptsRequestSearchPromptsPaginateTypeDef(
     _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef,
     _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef,
 ):
     pass
 
 
-SearchPromptsResponseOutputTypeDef = TypedDict(
-    "SearchPromptsResponseOutputTypeDef",
+SearchPromptsResponseTypeDef = TypedDict(
+    "SearchPromptsResponseTypeDef",
     {
-        "Prompts": List["PromptOutputTypeDef"],
+        "Prompts": List["PromptTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQueuesRequestRequestTypeDef = TypedDict(
@@ -6637,18 +6635,18 @@
 class SearchQueuesRequestSearchQueuesPaginateTypeDef(
     _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef,
     _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef,
 ):
     pass
 
 
-SearchQueuesResponseOutputTypeDef = TypedDict(
-    "SearchQueuesResponseOutputTypeDef",
+SearchQueuesResponseTypeDef = TypedDict(
+    "SearchQueuesResponseTypeDef",
     {
-        "Queues": List["QueueOutputTypeDef"],
+        "Queues": List["QueueTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -6696,18 +6694,18 @@
 class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(
     _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
     _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
 ):
     pass
 
 
-SearchQuickConnectsResponseOutputTypeDef = TypedDict(
-    "SearchQuickConnectsResponseOutputTypeDef",
+SearchQuickConnectsResponseTypeDef = TypedDict(
+    "SearchQuickConnectsResponseTypeDef",
     {
-        "QuickConnects": List["QuickConnectOutputTypeDef"],
+        "QuickConnects": List["QuickConnectTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchResourceTagsRequestRequestTypeDef = TypedDict(
@@ -6755,18 +6753,18 @@
 class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(
     _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
     _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
 ):
     pass
 
 
-SearchResourceTagsResponseOutputTypeDef = TypedDict(
-    "SearchResourceTagsResponseOutputTypeDef",
+SearchResourceTagsResponseTypeDef = TypedDict(
+    "SearchResourceTagsResponseTypeDef",
     {
-        "Tags": List["TagSetOutputTypeDef"],
+        "Tags": List["TagSetTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestRequestTypeDef",
@@ -6813,18 +6811,18 @@
 class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(
     _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
     _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
 ):
     pass
 
 
-SearchRoutingProfilesResponseOutputTypeDef = TypedDict(
-    "SearchRoutingProfilesResponseOutputTypeDef",
+SearchRoutingProfilesResponseTypeDef = TypedDict(
+    "SearchRoutingProfilesResponseTypeDef",
     {
-        "RoutingProfiles": List["RoutingProfileOutputTypeDef"],
+        "RoutingProfiles": List["RoutingProfileTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -6872,18 +6870,18 @@
 class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(
     _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
     _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
 ):
     pass
 
 
-SearchSecurityProfilesResponseOutputTypeDef = TypedDict(
-    "SearchSecurityProfilesResponseOutputTypeDef",
+SearchSecurityProfilesResponseTypeDef = TypedDict(
+    "SearchSecurityProfilesResponseTypeDef",
     {
-        "SecurityProfiles": List["SecurityProfileSearchSummaryOutputTypeDef"],
+        "SecurityProfiles": List["SecurityProfileSearchSummaryTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchUsersRequestRequestTypeDef = TypedDict(
@@ -6905,18 +6903,18 @@
         "SearchFilter": "UserSearchFilterTypeDef",
         "SearchCriteria": "UserSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-SearchUsersResponseOutputTypeDef = TypedDict(
-    "SearchUsersResponseOutputTypeDef",
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
     {
-        "Users": List["UserSearchSummaryOutputTypeDef"],
+        "Users": List["UserSearchSummaryTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchVocabulariesRequestRequestTypeDef = TypedDict(
@@ -6966,77 +6964,77 @@
 class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(
     _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
     _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
 ):
     pass
 
 
-SearchVocabulariesResponseOutputTypeDef = TypedDict(
-    "SearchVocabulariesResponseOutputTypeDef",
+SearchVocabulariesResponseTypeDef = TypedDict(
+    "SearchVocabulariesResponseTypeDef",
     {
-        "VocabularySummaryList": List["VocabularySummaryOutputTypeDef"],
+        "VocabularySummaryList": List["VocabularySummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SecurityKeyOutputTypeDef = TypedDict(
-    "SecurityKeyOutputTypeDef",
+SecurityKeyTypeDef = TypedDict(
+    "SecurityKeyTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
 )
 
-SecurityProfileOutputTypeDef = TypedDict(
-    "SecurityProfileOutputTypeDef",
-    {
-        "Id": str,
-        "OrganizationResourceId": str,
-        "Arn": str,
-        "SecurityProfileName": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "AllowedAccessControlTags": Dict[str, str],
-        "TagRestrictedResources": List[str],
-    },
-)
-
 SecurityProfileSearchCriteriaTypeDef = TypedDict(
     "SecurityProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
     total=False,
 )
 
-SecurityProfileSearchSummaryOutputTypeDef = TypedDict(
-    "SecurityProfileSearchSummaryOutputTypeDef",
+SecurityProfileSearchSummaryTypeDef = TypedDict(
+    "SecurityProfileSearchSummaryTypeDef",
     {
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
 )
 
-SecurityProfileSummaryOutputTypeDef = TypedDict(
-    "SecurityProfileSummaryOutputTypeDef",
+SecurityProfileSummaryTypeDef = TypedDict(
+    "SecurityProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+SecurityProfileTypeDef = TypedDict(
+    "SecurityProfileTypeDef",
+    {
+        "Id": str,
+        "OrganizationResourceId": str,
+        "Arn": str,
+        "SecurityProfileName": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "AllowedAccessControlTags": Dict[str, str],
+        "TagRestrictedResources": List[str],
+    },
+)
+
 SecurityProfilesSearchFilterTypeDef = TypedDict(
     "SecurityProfilesSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
@@ -7120,16 +7118,16 @@
 
 class StartChatContactRequestRequestTypeDef(
     _RequiredStartChatContactRequestRequestTypeDef, _OptionalStartChatContactRequestRequestTypeDef
 ):
     pass
 
 
-StartChatContactResponseOutputTypeDef = TypedDict(
-    "StartChatContactResponseOutputTypeDef",
+StartChatContactResponseTypeDef = TypedDict(
+    "StartChatContactResponseTypeDef",
     {
         "ContactId": str,
         "ParticipantId": str,
         "ParticipantToken": str,
         "ContinuedFromContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7155,16 +7153,16 @@
 class StartContactEvaluationRequestRequestTypeDef(
     _RequiredStartContactEvaluationRequestRequestTypeDef,
     _OptionalStartContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
 
-StartContactEvaluationResponseOutputTypeDef = TypedDict(
-    "StartContactEvaluationResponseOutputTypeDef",
+StartContactEvaluationResponseTypeDef = TypedDict(
+    "StartContactEvaluationResponseTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7184,16 +7182,16 @@
         "InstanceId": str,
         "ContactId": str,
         "ChatStreamingConfiguration": "ChatStreamingConfigurationTypeDef",
         "ClientToken": str,
     },
 )
 
-StartContactStreamingResponseOutputTypeDef = TypedDict(
-    "StartContactStreamingResponseOutputTypeDef",
+StartContactStreamingResponseTypeDef = TypedDict(
+    "StartContactStreamingResponseTypeDef",
     {
         "StreamingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartOutboundVoiceContactRequestRequestTypeDef = TypedDict(
@@ -7222,16 +7220,16 @@
 class StartOutboundVoiceContactRequestRequestTypeDef(
     _RequiredStartOutboundVoiceContactRequestRequestTypeDef,
     _OptionalStartOutboundVoiceContactRequestRequestTypeDef,
 ):
     pass
 
 
-StartOutboundVoiceContactResponseOutputTypeDef = TypedDict(
-    "StartOutboundVoiceContactResponseOutputTypeDef",
+StartOutboundVoiceContactResponseTypeDef = TypedDict(
+    "StartOutboundVoiceContactResponseTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTaskContactRequestRequestTypeDef = TypedDict(
@@ -7261,16 +7259,16 @@
 
 class StartTaskContactRequestRequestTypeDef(
     _RequiredStartTaskContactRequestRequestTypeDef, _OptionalStartTaskContactRequestRequestTypeDef
 ):
     pass
 
 
-StartTaskContactResponseOutputTypeDef = TypedDict(
-    "StartTaskContactResponseOutputTypeDef",
+StartTaskContactResponseTypeDef = TypedDict(
+    "StartTaskContactResponseTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopContactRecordingRequestRequestTypeDef = TypedDict(
@@ -7305,16 +7303,16 @@
         "FieldName": str,
         "Value": str,
         "ComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-StringReferenceOutputTypeDef = TypedDict(
-    "StringReferenceOutputTypeDef",
+StringReferenceTypeDef = TypedDict(
+    "StringReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
@@ -7337,16 +7335,16 @@
 class SubmitContactEvaluationRequestRequestTypeDef(
     _RequiredSubmitContactEvaluationRequestRequestTypeDef,
     _OptionalSubmitContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
 
-SubmitContactEvaluationResponseOutputTypeDef = TypedDict(
-    "SubmitContactEvaluationResponseOutputTypeDef",
+SubmitContactEvaluationResponseTypeDef = TypedDict(
+    "SubmitContactEvaluationResponseTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7383,16 +7381,16 @@
         "tagValue": str,
         "tagKeyComparisonType": StringComparisonTypeType,
         "tagValueComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-TagSetOutputTypeDef = TypedDict(
-    "TagSetOutputTypeDef",
+TagSetTypeDef = TypedDict(
+    "TagSetTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 TaskActionDefinitionOutputTypeDef = TypedDict(
@@ -7523,16 +7521,16 @@
 
 class TaskTemplateFieldTypeDef(
     _RequiredTaskTemplateFieldTypeDef, _OptionalTaskTemplateFieldTypeDef
 ):
     pass
 
 
-TaskTemplateMetadataOutputTypeDef = TypedDict(
-    "TaskTemplateMetadataOutputTypeDef",
+TaskTemplateMetadataTypeDef = TypedDict(
+    "TaskTemplateMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
@@ -7584,35 +7582,35 @@
     {
         "Comparison": str,
         "ThresholdValue": float,
     },
     total=False,
 )
 
-TrafficDistributionGroupOutputTypeDef = TypedDict(
-    "TrafficDistributionGroupOutputTypeDef",
+TrafficDistributionGroupSummaryTypeDef = TypedDict(
+    "TrafficDistributionGroupSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
-        "Tags": Dict[str, str],
     },
 )
 
-TrafficDistributionGroupSummaryOutputTypeDef = TypedDict(
-    "TrafficDistributionGroupSummaryOutputTypeDef",
+TrafficDistributionGroupTypeDef = TypedDict(
+    "TrafficDistributionGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
+        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
+        "Tags": Dict[str, str],
     },
 )
 
 _RequiredTransferContactRequestRequestTypeDef = TypedDict(
     "_RequiredTransferContactRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -7633,16 +7631,16 @@
 
 class TransferContactRequestRequestTypeDef(
     _RequiredTransferContactRequestRequestTypeDef, _OptionalTransferContactRequestRequestTypeDef
 ):
     pass
 
 
-TransferContactResponseOutputTypeDef = TypedDict(
-    "TransferContactResponseOutputTypeDef",
+TransferContactResponseTypeDef = TypedDict(
+    "TransferContactResponseTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7709,16 +7707,16 @@
 class UpdateContactEvaluationRequestRequestTypeDef(
     _RequiredUpdateContactEvaluationRequestRequestTypeDef,
     _OptionalUpdateContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateContactEvaluationResponseOutputTypeDef = TypedDict(
-    "UpdateContactEvaluationResponseOutputTypeDef",
+UpdateContactEvaluationResponseTypeDef = TypedDict(
+    "UpdateContactEvaluationResponseTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7872,16 +7870,16 @@
 class UpdateEvaluationFormRequestRequestTypeDef(
     _RequiredUpdateEvaluationFormRequestRequestTypeDef,
     _OptionalUpdateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "UpdateEvaluationFormResponseOutputTypeDef",
+UpdateEvaluationFormResponseTypeDef = TypedDict(
+    "UpdateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -7966,16 +7964,16 @@
 
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
 
-UpdatePhoneNumberResponseOutputTypeDef = TypedDict(
-    "UpdatePhoneNumberResponseOutputTypeDef",
+UpdatePhoneNumberResponseTypeDef = TypedDict(
+    "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7999,16 +7997,16 @@
 
 class UpdatePromptRequestRequestTypeDef(
     _RequiredUpdatePromptRequestRequestTypeDef, _OptionalUpdatePromptRequestRequestTypeDef
 ):
     pass
 
 
-UpdatePromptResponseOutputTypeDef = TypedDict(
-    "UpdatePromptResponseOutputTypeDef",
+UpdatePromptResponseTypeDef = TypedDict(
+    "UpdatePromptResponseTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -8232,16 +8230,16 @@
 class UpdateTaskTemplateRequestRequestTypeDef(
     _RequiredUpdateTaskTemplateRequestRequestTypeDef,
     _OptionalUpdateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateTaskTemplateResponseOutputTypeDef = TypedDict(
-    "UpdateTaskTemplateResponseOutputTypeDef",
+UpdateTaskTemplateResponseTypeDef = TypedDict(
+    "UpdateTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
@@ -8349,24 +8347,24 @@
     {
         "SecurityProfileIds": Sequence[str],
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-UrlReferenceOutputTypeDef = TypedDict(
-    "UrlReferenceOutputTypeDef",
+UrlReferenceTypeDef = TypedDict(
+    "UrlReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-UseCaseOutputTypeDef = TypedDict(
-    "UseCaseOutputTypeDef",
+UseCaseTypeDef = TypedDict(
+    "UseCaseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
 )
 
@@ -8378,31 +8376,31 @@
         "RoutingProfiles": Sequence[str],
         "Agents": Sequence[str],
         "UserHierarchyGroups": Sequence[str],
     },
     total=False,
 )
 
-UserDataOutputTypeDef = TypedDict(
-    "UserDataOutputTypeDef",
+UserDataTypeDef = TypedDict(
+    "UserDataTypeDef",
     {
-        "User": "UserReferenceOutputTypeDef",
-        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
-        "HierarchyPath": "HierarchyPathReferenceOutputTypeDef",
-        "Status": "AgentStatusReferenceOutputTypeDef",
+        "User": "UserReferenceTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceTypeDef",
+        "HierarchyPath": "HierarchyPathReferenceTypeDef",
+        "Status": "AgentStatusReferenceTypeDef",
         "AvailableSlotsByChannel": Dict[ChannelType, int],
         "MaxSlotsByChannel": Dict[ChannelType, int],
         "ActiveSlotsByChannel": Dict[ChannelType, int],
-        "Contacts": List["AgentContactReferenceOutputTypeDef"],
+        "Contacts": List["AgentContactReferenceTypeDef"],
         "NextStatus": str,
     },
 )
 
-UserIdentityInfoLiteOutputTypeDef = TypedDict(
-    "UserIdentityInfoLiteOutputTypeDef",
+UserIdentityInfoLiteTypeDef = TypedDict(
+    "UserIdentityInfoLiteTypeDef",
     {
         "FirstName": str,
         "LastName": str,
     },
 )
 
 UserIdentityInfoOutputTypeDef = TypedDict(
@@ -8424,30 +8422,14 @@
         "Email": str,
         "SecondaryEmail": str,
         "Mobile": str,
     },
     total=False,
 )
 
-UserOutputTypeDef = TypedDict(
-    "UserOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Username": str,
-        "IdentityInfo": "UserIdentityInfoOutputTypeDef",
-        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
-        "DirectoryUserId": str,
-        "SecurityProfileIds": List[str],
-        "RoutingProfileId": str,
-        "HierarchyGroupId": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 UserPhoneConfigOutputTypeDef = TypedDict(
     "UserPhoneConfigOutputTypeDef",
     {
         "PhoneType": PhoneTypeType,
         "AutoAccept": bool,
         "AfterContactWorkTimeLimit": int,
         "DeskPhoneNumber": str,
@@ -8487,16 +8469,16 @@
     "UserQuickConnectConfigTypeDef",
     {
         "UserId": str,
         "ContactFlowId": str,
     },
 )
 
-UserReferenceOutputTypeDef = TypedDict(
-    "UserReferenceOutputTypeDef",
+UserReferenceTypeDef = TypedDict(
+    "UserReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 UserSearchCriteriaTypeDef = TypedDict(
@@ -8514,74 +8496,90 @@
     "UserSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-UserSearchSummaryOutputTypeDef = TypedDict(
-    "UserSearchSummaryOutputTypeDef",
+UserSearchSummaryTypeDef = TypedDict(
+    "UserSearchSummaryTypeDef",
     {
         "Arn": str,
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Id": str,
-        "IdentityInfo": "UserIdentityInfoLiteOutputTypeDef",
+        "IdentityInfo": "UserIdentityInfoLiteTypeDef",
         "PhoneConfig": "UserPhoneConfigOutputTypeDef",
         "RoutingProfileId": str,
         "SecurityProfileIds": List[str],
         "Tags": Dict[str, str],
         "Username": str,
     },
 )
 
-UserSummaryOutputTypeDef = TypedDict(
-    "UserSummaryOutputTypeDef",
+UserSummaryTypeDef = TypedDict(
+    "UserSummaryTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Username": str,
+    },
+)
+
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
+        "IdentityInfo": "UserIdentityInfoOutputTypeDef",
+        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
+        "DirectoryUserId": str,
+        "SecurityProfileIds": List[str],
+        "RoutingProfileId": str,
+        "HierarchyGroupId": str,
+        "Tags": Dict[str, str],
     },
 )
 
-VocabularyOutputTypeDef = TypedDict(
-    "VocabularyOutputTypeDef",
+VocabularySummaryTypeDef = TypedDict(
+    "VocabularySummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "Content": str,
-        "Tags": Dict[str, str],
     },
 )
 
-VocabularySummaryOutputTypeDef = TypedDict(
-    "VocabularySummaryOutputTypeDef",
+VocabularyTypeDef = TypedDict(
+    "VocabularyTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
+        "Content": str,
+        "Tags": Dict[str, str],
     },
 )
 
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
 
-WisdomInfoOutputTypeDef = TypedDict(
-    "WisdomInfoOutputTypeDef",
+WisdomInfoTypeDef = TypedDict(
+    "WisdomInfoTypeDef",
     {
         "SessionArn": str,
     },
 )
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connect service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connect.type_defs import ActionSummaryOutputTypeDef
+    from mypy_boto3_connect.type_defs import ActionSummaryTypeDef
 
-    data: ActionSummaryOutputTypeDef = {...}
+    data: ActionSummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -84,103 +84,103 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActionSummaryOutputTypeDef",
+    "ActionSummaryTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
-    "ActivateEvaluationFormResponseOutputTypeDef",
-    "AgentContactReferenceOutputTypeDef",
-    "AgentInfoOutputTypeDef",
-    "AgentStatusOutputTypeDef",
-    "AgentStatusReferenceOutputTypeDef",
-    "AgentStatusSummaryOutputTypeDef",
+    "ActivateEvaluationFormResponseTypeDef",
+    "AgentContactReferenceTypeDef",
+    "AgentInfoTypeDef",
+    "AgentStatusReferenceTypeDef",
+    "AgentStatusSummaryTypeDef",
+    "AgentStatusTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "AssociateApprovedOriginRequestRequestTypeDef",
     "AssociateBotRequestRequestTypeDef",
     "AssociateDefaultVocabularyRequestRequestTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
-    "AssociateInstanceStorageConfigResponseOutputTypeDef",
+    "AssociateInstanceStorageConfigResponseTypeDef",
     "AssociateLambdaFunctionRequestRequestTypeDef",
     "AssociateLexBotRequestRequestTypeDef",
     "AssociatePhoneNumberContactFlowRequestRequestTypeDef",
     "AssociateQueueQuickConnectsRequestRequestTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "AssociateSecurityKeyRequestRequestTypeDef",
-    "AssociateSecurityKeyResponseOutputTypeDef",
-    "AttachmentReferenceOutputTypeDef",
-    "AttributeOutputTypeDef",
-    "AvailableNumberSummaryOutputTypeDef",
+    "AssociateSecurityKeyResponseTypeDef",
+    "AttachmentReferenceTypeDef",
+    "AttributeTypeDef",
+    "AvailableNumberSummaryTypeDef",
     "ChatMessageTypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "ChatStreamingConfigurationTypeDef",
     "ClaimPhoneNumberRequestRequestTypeDef",
-    "ClaimPhoneNumberResponseOutputTypeDef",
-    "ClaimedPhoneNumberSummaryOutputTypeDef",
+    "ClaimPhoneNumberResponseTypeDef",
+    "ClaimedPhoneNumberSummaryTypeDef",
     "ContactFilterTypeDef",
-    "ContactFlowModuleOutputTypeDef",
-    "ContactFlowModuleSummaryOutputTypeDef",
-    "ContactFlowOutputTypeDef",
-    "ContactFlowSummaryOutputTypeDef",
-    "ContactOutputTypeDef",
+    "ContactFlowModuleSummaryTypeDef",
+    "ContactFlowModuleTypeDef",
+    "ContactFlowSummaryTypeDef",
+    "ContactFlowTypeDef",
+    "ContactTypeDef",
     "ControlPlaneTagFilterTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
-    "CreateAgentStatusResponseOutputTypeDef",
+    "CreateAgentStatusResponseTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
-    "CreateContactFlowModuleResponseOutputTypeDef",
+    "CreateContactFlowModuleResponseTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
-    "CreateContactFlowResponseOutputTypeDef",
+    "CreateContactFlowResponseTypeDef",
     "CreateEvaluationFormRequestRequestTypeDef",
-    "CreateEvaluationFormResponseOutputTypeDef",
+    "CreateEvaluationFormResponseTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
-    "CreateHoursOfOperationResponseOutputTypeDef",
+    "CreateHoursOfOperationResponseTypeDef",
     "CreateInstanceRequestRequestTypeDef",
-    "CreateInstanceResponseOutputTypeDef",
+    "CreateInstanceResponseTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
-    "CreateIntegrationAssociationResponseOutputTypeDef",
+    "CreateIntegrationAssociationResponseTypeDef",
     "CreateParticipantRequestRequestTypeDef",
-    "CreateParticipantResponseOutputTypeDef",
+    "CreateParticipantResponseTypeDef",
     "CreatePromptRequestRequestTypeDef",
-    "CreatePromptResponseOutputTypeDef",
+    "CreatePromptResponseTypeDef",
     "CreateQueueRequestRequestTypeDef",
-    "CreateQueueResponseOutputTypeDef",
+    "CreateQueueResponseTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
-    "CreateQuickConnectResponseOutputTypeDef",
+    "CreateQuickConnectResponseTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
-    "CreateRoutingProfileResponseOutputTypeDef",
+    "CreateRoutingProfileResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
-    "CreateRuleResponseOutputTypeDef",
+    "CreateRuleResponseTypeDef",
     "CreateSecurityProfileRequestRequestTypeDef",
-    "CreateSecurityProfileResponseOutputTypeDef",
+    "CreateSecurityProfileResponseTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
-    "CreateTaskTemplateResponseOutputTypeDef",
+    "CreateTaskTemplateResponseTypeDef",
     "CreateTrafficDistributionGroupRequestRequestTypeDef",
-    "CreateTrafficDistributionGroupResponseOutputTypeDef",
+    "CreateTrafficDistributionGroupResponseTypeDef",
     "CreateUseCaseRequestRequestTypeDef",
-    "CreateUseCaseResponseOutputTypeDef",
+    "CreateUseCaseResponseTypeDef",
     "CreateUserHierarchyGroupRequestRequestTypeDef",
-    "CreateUserHierarchyGroupResponseOutputTypeDef",
+    "CreateUserHierarchyGroupResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseOutputTypeDef",
+    "CreateUserResponseTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "CreateVocabularyResponseOutputTypeDef",
-    "CredentialsOutputTypeDef",
+    "CreateVocabularyResponseTypeDef",
+    "CredentialsTypeDef",
     "CrossChannelBehaviorOutputTypeDef",
     "CrossChannelBehaviorTypeDef",
-    "CurrentMetricDataOutputTypeDef",
+    "CurrentMetricDataTypeDef",
     "CurrentMetricOutputTypeDef",
-    "CurrentMetricResultOutputTypeDef",
+    "CurrentMetricResultTypeDef",
     "CurrentMetricSortCriteriaTypeDef",
     "CurrentMetricTypeDef",
-    "DateReferenceOutputTypeDef",
+    "DateReferenceTypeDef",
     "DeactivateEvaluationFormRequestRequestTypeDef",
-    "DeactivateEvaluationFormResponseOutputTypeDef",
-    "DefaultVocabularyOutputTypeDef",
+    "DeactivateEvaluationFormResponseTypeDef",
+    "DefaultVocabularyTypeDef",
     "DeleteContactEvaluationRequestRequestTypeDef",
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
@@ -192,90 +192,89 @@
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
-    "DeleteVocabularyResponseOutputTypeDef",
+    "DeleteVocabularyResponseTypeDef",
     "DescribeAgentStatusRequestRequestTypeDef",
-    "DescribeAgentStatusResponseOutputTypeDef",
+    "DescribeAgentStatusResponseTypeDef",
     "DescribeContactEvaluationRequestRequestTypeDef",
-    "DescribeContactEvaluationResponseOutputTypeDef",
+    "DescribeContactEvaluationResponseTypeDef",
     "DescribeContactFlowModuleRequestRequestTypeDef",
-    "DescribeContactFlowModuleResponseOutputTypeDef",
+    "DescribeContactFlowModuleResponseTypeDef",
     "DescribeContactFlowRequestRequestTypeDef",
-    "DescribeContactFlowResponseOutputTypeDef",
+    "DescribeContactFlowResponseTypeDef",
     "DescribeContactRequestRequestTypeDef",
-    "DescribeContactResponseOutputTypeDef",
+    "DescribeContactResponseTypeDef",
     "DescribeEvaluationFormRequestRequestTypeDef",
-    "DescribeEvaluationFormResponseOutputTypeDef",
+    "DescribeEvaluationFormResponseTypeDef",
     "DescribeHoursOfOperationRequestRequestTypeDef",
-    "DescribeHoursOfOperationResponseOutputTypeDef",
+    "DescribeHoursOfOperationResponseTypeDef",
     "DescribeInstanceAttributeRequestRequestTypeDef",
-    "DescribeInstanceAttributeResponseOutputTypeDef",
+    "DescribeInstanceAttributeResponseTypeDef",
     "DescribeInstanceRequestRequestTypeDef",
-    "DescribeInstanceResponseOutputTypeDef",
+    "DescribeInstanceResponseTypeDef",
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
-    "DescribeInstanceStorageConfigResponseOutputTypeDef",
+    "DescribeInstanceStorageConfigResponseTypeDef",
     "DescribePhoneNumberRequestRequestTypeDef",
-    "DescribePhoneNumberResponseOutputTypeDef",
+    "DescribePhoneNumberResponseTypeDef",
     "DescribePromptRequestRequestTypeDef",
-    "DescribePromptResponseOutputTypeDef",
+    "DescribePromptResponseTypeDef",
     "DescribeQueueRequestRequestTypeDef",
-    "DescribeQueueResponseOutputTypeDef",
+    "DescribeQueueResponseTypeDef",
     "DescribeQuickConnectRequestRequestTypeDef",
-    "DescribeQuickConnectResponseOutputTypeDef",
+    "DescribeQuickConnectResponseTypeDef",
     "DescribeRoutingProfileRequestRequestTypeDef",
-    "DescribeRoutingProfileResponseOutputTypeDef",
+    "DescribeRoutingProfileResponseTypeDef",
     "DescribeRuleRequestRequestTypeDef",
-    "DescribeRuleResponseOutputTypeDef",
+    "DescribeRuleResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
-    "DescribeSecurityProfileResponseOutputTypeDef",
+    "DescribeSecurityProfileResponseTypeDef",
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
-    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
+    "DescribeTrafficDistributionGroupResponseTypeDef",
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
-    "DescribeUserHierarchyGroupResponseOutputTypeDef",
+    "DescribeUserHierarchyGroupResponseTypeDef",
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
-    "DescribeUserHierarchyStructureResponseOutputTypeDef",
+    "DescribeUserHierarchyStructureResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "DescribeUserResponseOutputTypeDef",
+    "DescribeUserResponseTypeDef",
     "DescribeVocabularyRequestRequestTypeDef",
-    "DescribeVocabularyResponseOutputTypeDef",
-    "DimensionsOutputTypeDef",
+    "DescribeVocabularyResponseTypeDef",
+    "DimensionsTypeDef",
     "DisassociateApprovedOriginRequestRequestTypeDef",
     "DisassociateBotRequestRequestTypeDef",
     "DisassociateInstanceStorageConfigRequestRequestTypeDef",
     "DisassociateLambdaFunctionRequestRequestTypeDef",
     "DisassociateLexBotRequestRequestTypeDef",
     "DisassociatePhoneNumberContactFlowRequestRequestTypeDef",
     "DisassociateQueueQuickConnectsRequestRequestTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "DisassociateSecurityKeyRequestRequestTypeDef",
     "DismissUserContactRequestRequestTypeDef",
     "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "EmailReferenceOutputTypeDef",
+    "EmailReferenceTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "EvaluationAnswerDataOutputTypeDef",
     "EvaluationAnswerDataTypeDef",
     "EvaluationAnswerInputTypeDef",
-    "EvaluationAnswerOutputOutputTypeDef",
-    "EvaluationFormContentOutputTypeDef",
+    "EvaluationAnswerOutputTypeDef",
+    "EvaluationFormContentTypeDef",
     "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
     "EvaluationFormNumericQuestionAutomationOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
     "EvaluationFormNumericQuestionOptionOutputTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
     "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
-    "EvaluationFormOutputTypeDef",
     "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
     "EvaluationFormQuestionTypePropertiesOutputTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
     "EvaluationFormScoringStrategyOutputTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
     "EvaluationFormSectionOutputTypeDef",
@@ -284,502 +283,503 @@
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionOptionOutputTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
-    "EvaluationFormSummaryOutputTypeDef",
-    "EvaluationFormVersionSummaryOutputTypeDef",
-    "EvaluationMetadataOutputTypeDef",
+    "EvaluationFormSummaryTypeDef",
+    "EvaluationFormTypeDef",
+    "EvaluationFormVersionSummaryTypeDef",
+    "EvaluationMetadataTypeDef",
     "EvaluationNoteOutputTypeDef",
     "EvaluationNoteTypeDef",
-    "EvaluationOutputTypeDef",
-    "EvaluationScoreOutputTypeDef",
-    "EvaluationSummaryOutputTypeDef",
+    "EvaluationScoreTypeDef",
+    "EvaluationSummaryTypeDef",
+    "EvaluationTypeDef",
     "EventBridgeActionDefinitionOutputTypeDef",
     "EventBridgeActionDefinitionTypeDef",
     "FilterV2TypeDef",
     "FiltersTypeDef",
     "GetContactAttributesRequestRequestTypeDef",
-    "GetContactAttributesResponseOutputTypeDef",
+    "GetContactAttributesResponseTypeDef",
     "GetCurrentMetricDataRequestRequestTypeDef",
-    "GetCurrentMetricDataResponseOutputTypeDef",
+    "GetCurrentMetricDataResponseTypeDef",
     "GetCurrentUserDataRequestRequestTypeDef",
-    "GetCurrentUserDataResponseOutputTypeDef",
+    "GetCurrentUserDataResponseTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
-    "GetFederationTokenResponseOutputTypeDef",
+    "GetFederationTokenResponseTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
-    "GetMetricDataResponseOutputTypeDef",
+    "GetMetricDataResponseTypeDef",
     "GetMetricDataV2RequestRequestTypeDef",
-    "GetMetricDataV2ResponseOutputTypeDef",
+    "GetMetricDataV2ResponseTypeDef",
     "GetPromptFileRequestRequestTypeDef",
-    "GetPromptFileResponseOutputTypeDef",
+    "GetPromptFileResponseTypeDef",
     "GetTaskTemplateRequestRequestTypeDef",
-    "GetTaskTemplateResponseOutputTypeDef",
+    "GetTaskTemplateResponseTypeDef",
     "GetTrafficDistributionRequestRequestTypeDef",
-    "GetTrafficDistributionResponseOutputTypeDef",
+    "GetTrafficDistributionResponseTypeDef",
     "HierarchyGroupConditionTypeDef",
-    "HierarchyGroupOutputTypeDef",
-    "HierarchyGroupSummaryOutputTypeDef",
-    "HierarchyGroupSummaryReferenceOutputTypeDef",
-    "HierarchyLevelOutputTypeDef",
+    "HierarchyGroupSummaryReferenceTypeDef",
+    "HierarchyGroupSummaryTypeDef",
+    "HierarchyGroupTypeDef",
+    "HierarchyLevelTypeDef",
     "HierarchyLevelUpdateTypeDef",
-    "HierarchyPathOutputTypeDef",
-    "HierarchyPathReferenceOutputTypeDef",
-    "HierarchyStructureOutputTypeDef",
+    "HierarchyPathReferenceTypeDef",
+    "HierarchyPathTypeDef",
+    "HierarchyStructureTypeDef",
     "HierarchyStructureUpdateTypeDef",
-    "HistoricalMetricDataOutputTypeDef",
+    "HistoricalMetricDataTypeDef",
     "HistoricalMetricOutputTypeDef",
-    "HistoricalMetricResultOutputTypeDef",
+    "HistoricalMetricResultTypeDef",
     "HistoricalMetricTypeDef",
     "HoursOfOperationConfigOutputTypeDef",
     "HoursOfOperationConfigTypeDef",
-    "HoursOfOperationOutputTypeDef",
     "HoursOfOperationSearchCriteriaTypeDef",
     "HoursOfOperationSearchFilterTypeDef",
-    "HoursOfOperationSummaryOutputTypeDef",
+    "HoursOfOperationSummaryTypeDef",
     "HoursOfOperationTimeSliceOutputTypeDef",
     "HoursOfOperationTimeSliceTypeDef",
-    "InstanceOutputTypeDef",
-    "InstanceStatusReasonOutputTypeDef",
+    "HoursOfOperationTypeDef",
+    "InstanceStatusReasonTypeDef",
     "InstanceStorageConfigOutputTypeDef",
     "InstanceStorageConfigTypeDef",
-    "InstanceSummaryOutputTypeDef",
-    "IntegrationAssociationSummaryOutputTypeDef",
+    "InstanceSummaryTypeDef",
+    "InstanceTypeDef",
+    "IntegrationAssociationSummaryTypeDef",
     "InvisibleFieldInfoOutputTypeDef",
     "InvisibleFieldInfoTypeDef",
     "KinesisFirehoseConfigOutputTypeDef",
     "KinesisFirehoseConfigTypeDef",
     "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
     "KinesisVideoStreamConfigOutputTypeDef",
     "KinesisVideoStreamConfigTypeDef",
-    "LexBotConfigOutputTypeDef",
+    "LexBotConfigTypeDef",
     "LexBotOutputTypeDef",
     "LexBotTypeDef",
     "LexV2BotOutputTypeDef",
     "LexV2BotTypeDef",
     "ListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     "ListAgentStatusRequestRequestTypeDef",
-    "ListAgentStatusResponseOutputTypeDef",
+    "ListAgentStatusResponseTypeDef",
     "ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     "ListApprovedOriginsRequestRequestTypeDef",
-    "ListApprovedOriginsResponseOutputTypeDef",
+    "ListApprovedOriginsResponseTypeDef",
     "ListBotsRequestListBotsPaginateTypeDef",
     "ListBotsRequestRequestTypeDef",
-    "ListBotsResponseOutputTypeDef",
+    "ListBotsResponseTypeDef",
     "ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     "ListContactEvaluationsRequestRequestTypeDef",
-    "ListContactEvaluationsResponseOutputTypeDef",
+    "ListContactEvaluationsResponseTypeDef",
     "ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
     "ListContactFlowModulesRequestRequestTypeDef",
-    "ListContactFlowModulesResponseOutputTypeDef",
+    "ListContactFlowModulesResponseTypeDef",
     "ListContactFlowsRequestListContactFlowsPaginateTypeDef",
     "ListContactFlowsRequestRequestTypeDef",
-    "ListContactFlowsResponseOutputTypeDef",
+    "ListContactFlowsResponseTypeDef",
     "ListContactReferencesRequestListContactReferencesPaginateTypeDef",
     "ListContactReferencesRequestRequestTypeDef",
-    "ListContactReferencesResponseOutputTypeDef",
+    "ListContactReferencesResponseTypeDef",
     "ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
     "ListDefaultVocabulariesRequestRequestTypeDef",
-    "ListDefaultVocabulariesResponseOutputTypeDef",
+    "ListDefaultVocabulariesResponseTypeDef",
     "ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     "ListEvaluationFormVersionsRequestRequestTypeDef",
-    "ListEvaluationFormVersionsResponseOutputTypeDef",
+    "ListEvaluationFormVersionsResponseTypeDef",
     "ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     "ListEvaluationFormsRequestRequestTypeDef",
-    "ListEvaluationFormsResponseOutputTypeDef",
+    "ListEvaluationFormsResponseTypeDef",
     "ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     "ListHoursOfOperationsRequestRequestTypeDef",
-    "ListHoursOfOperationsResponseOutputTypeDef",
+    "ListHoursOfOperationsResponseTypeDef",
     "ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     "ListInstanceAttributesRequestRequestTypeDef",
-    "ListInstanceAttributesResponseOutputTypeDef",
+    "ListInstanceAttributesResponseTypeDef",
     "ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     "ListInstanceStorageConfigsRequestRequestTypeDef",
-    "ListInstanceStorageConfigsResponseOutputTypeDef",
+    "ListInstanceStorageConfigsResponseTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
-    "ListInstancesResponseOutputTypeDef",
+    "ListInstancesResponseTypeDef",
     "ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
     "ListIntegrationAssociationsRequestRequestTypeDef",
-    "ListIntegrationAssociationsResponseOutputTypeDef",
+    "ListIntegrationAssociationsResponseTypeDef",
     "ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     "ListLambdaFunctionsRequestRequestTypeDef",
-    "ListLambdaFunctionsResponseOutputTypeDef",
+    "ListLambdaFunctionsResponseTypeDef",
     "ListLexBotsRequestListLexBotsPaginateTypeDef",
     "ListLexBotsRequestRequestTypeDef",
-    "ListLexBotsResponseOutputTypeDef",
+    "ListLexBotsResponseTypeDef",
     "ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
-    "ListPhoneNumbersResponseOutputTypeDef",
-    "ListPhoneNumbersSummaryOutputTypeDef",
+    "ListPhoneNumbersResponseTypeDef",
+    "ListPhoneNumbersSummaryTypeDef",
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     "ListPhoneNumbersV2RequestRequestTypeDef",
-    "ListPhoneNumbersV2ResponseOutputTypeDef",
+    "ListPhoneNumbersV2ResponseTypeDef",
     "ListPromptsRequestListPromptsPaginateTypeDef",
     "ListPromptsRequestRequestTypeDef",
-    "ListPromptsResponseOutputTypeDef",
+    "ListPromptsResponseTypeDef",
     "ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     "ListQueueQuickConnectsRequestRequestTypeDef",
-    "ListQueueQuickConnectsResponseOutputTypeDef",
+    "ListQueueQuickConnectsResponseTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResponseOutputTypeDef",
+    "ListQueuesResponseTypeDef",
     "ListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
     "ListQuickConnectsRequestRequestTypeDef",
-    "ListQuickConnectsResponseOutputTypeDef",
+    "ListQuickConnectsResponseTypeDef",
     "ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     "ListRoutingProfileQueuesRequestRequestTypeDef",
-    "ListRoutingProfileQueuesResponseOutputTypeDef",
+    "ListRoutingProfileQueuesResponseTypeDef",
     "ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     "ListRoutingProfilesRequestRequestTypeDef",
-    "ListRoutingProfilesResponseOutputTypeDef",
+    "ListRoutingProfilesResponseTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListRulesResponseOutputTypeDef",
+    "ListRulesResponseTypeDef",
     "ListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     "ListSecurityKeysRequestRequestTypeDef",
-    "ListSecurityKeysResponseOutputTypeDef",
+    "ListSecurityKeysResponseTypeDef",
     "ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     "ListSecurityProfilePermissionsRequestRequestTypeDef",
-    "ListSecurityProfilePermissionsResponseOutputTypeDef",
+    "ListSecurityProfilePermissionsResponseTypeDef",
     "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
-    "ListSecurityProfilesResponseOutputTypeDef",
+    "ListSecurityProfilesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef",
     "ListTaskTemplatesRequestRequestTypeDef",
-    "ListTaskTemplatesResponseOutputTypeDef",
+    "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
-    "ListTrafficDistributionGroupsResponseOutputTypeDef",
+    "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesRequestListUseCasesPaginateTypeDef",
     "ListUseCasesRequestRequestTypeDef",
-    "ListUseCasesResponseOutputTypeDef",
+    "ListUseCasesResponseTypeDef",
     "ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
-    "ListUserHierarchyGroupsResponseOutputTypeDef",
+    "ListUserHierarchyGroupsResponseTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListUsersResponseOutputTypeDef",
+    "ListUsersResponseTypeDef",
     "MediaConcurrencyOutputTypeDef",
     "MediaConcurrencyTypeDef",
-    "MetricDataV2OutputTypeDef",
+    "MetricDataV2TypeDef",
     "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
-    "MetricResultV2OutputTypeDef",
+    "MetricResultV2TypeDef",
     "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
-    "MonitorContactResponseOutputTypeDef",
+    "MonitorContactResponseTypeDef",
     "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
-    "NumberReferenceOutputTypeDef",
+    "NumberReferenceTypeDef",
     "NumericQuestionPropertyValueAutomationOutputTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
     "OutboundCallerConfigOutputTypeDef",
     "OutboundCallerConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "ParticipantTimerValueTypeDef",
-    "ParticipantTokenCredentialsOutputTypeDef",
+    "ParticipantTokenCredentialsTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigOutputTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
-    "PhoneNumberStatusOutputTypeDef",
-    "PhoneNumberSummaryOutputTypeDef",
-    "PromptOutputTypeDef",
+    "PhoneNumberStatusTypeDef",
+    "PhoneNumberSummaryTypeDef",
     "PromptSearchCriteriaTypeDef",
     "PromptSearchFilterTypeDef",
-    "PromptSummaryOutputTypeDef",
+    "PromptSummaryTypeDef",
+    "PromptTypeDef",
     "PutUserStatusRequestRequestTypeDef",
-    "QueueInfoOutputTypeDef",
-    "QueueOutputTypeDef",
+    "QueueInfoTypeDef",
     "QueueQuickConnectConfigOutputTypeDef",
     "QueueQuickConnectConfigTypeDef",
-    "QueueReferenceOutputTypeDef",
+    "QueueReferenceTypeDef",
     "QueueSearchCriteriaTypeDef",
     "QueueSearchFilterTypeDef",
-    "QueueSummaryOutputTypeDef",
+    "QueueSummaryTypeDef",
+    "QueueTypeDef",
     "QuickConnectConfigOutputTypeDef",
     "QuickConnectConfigTypeDef",
-    "QuickConnectOutputTypeDef",
     "QuickConnectSearchCriteriaTypeDef",
     "QuickConnectSearchFilterTypeDef",
-    "QuickConnectSummaryOutputTypeDef",
+    "QuickConnectSummaryTypeDef",
+    "QuickConnectTypeDef",
     "ReadOnlyFieldInfoOutputTypeDef",
     "ReadOnlyFieldInfoTypeDef",
     "ReferenceOutputTypeDef",
-    "ReferenceSummaryOutputTypeDef",
+    "ReferenceSummaryTypeDef",
     "ReferenceTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReplicateInstanceRequestRequestTypeDef",
-    "ReplicateInstanceResponseOutputTypeDef",
+    "ReplicateInstanceResponseTypeDef",
     "RequiredFieldInfoOutputTypeDef",
     "RequiredFieldInfoTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeContactRecordingRequestRequestTypeDef",
-    "RoutingProfileOutputTypeDef",
-    "RoutingProfileQueueConfigSummaryOutputTypeDef",
+    "RoutingProfileQueueConfigSummaryTypeDef",
     "RoutingProfileQueueConfigTypeDef",
     "RoutingProfileQueueReferenceTypeDef",
-    "RoutingProfileReferenceOutputTypeDef",
+    "RoutingProfileReferenceTypeDef",
     "RoutingProfileSearchCriteriaTypeDef",
     "RoutingProfileSearchFilterTypeDef",
-    "RoutingProfileSummaryOutputTypeDef",
+    "RoutingProfileSummaryTypeDef",
+    "RoutingProfileTypeDef",
     "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
-    "RuleOutputTypeDef",
-    "RuleSummaryOutputTypeDef",
+    "RuleSummaryTypeDef",
     "RuleTriggerEventSourceOutputTypeDef",
     "RuleTriggerEventSourceTypeDef",
+    "RuleTypeDef",
     "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
-    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SearchHoursOfOperationsRequestRequestTypeDef",
     "SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
-    "SearchHoursOfOperationsResponseOutputTypeDef",
+    "SearchHoursOfOperationsResponseTypeDef",
     "SearchPromptsRequestRequestTypeDef",
     "SearchPromptsRequestSearchPromptsPaginateTypeDef",
-    "SearchPromptsResponseOutputTypeDef",
+    "SearchPromptsResponseTypeDef",
     "SearchQueuesRequestRequestTypeDef",
     "SearchQueuesRequestSearchQueuesPaginateTypeDef",
-    "SearchQueuesResponseOutputTypeDef",
+    "SearchQueuesResponseTypeDef",
     "SearchQuickConnectsRequestRequestTypeDef",
     "SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
-    "SearchQuickConnectsResponseOutputTypeDef",
+    "SearchQuickConnectsResponseTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
-    "SearchResourceTagsResponseOutputTypeDef",
+    "SearchResourceTagsResponseTypeDef",
     "SearchRoutingProfilesRequestRequestTypeDef",
     "SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
-    "SearchRoutingProfilesResponseOutputTypeDef",
+    "SearchRoutingProfilesResponseTypeDef",
     "SearchSecurityProfilesRequestRequestTypeDef",
     "SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
-    "SearchSecurityProfilesResponseOutputTypeDef",
+    "SearchSecurityProfilesResponseTypeDef",
     "SearchUsersRequestRequestTypeDef",
     "SearchUsersRequestSearchUsersPaginateTypeDef",
-    "SearchUsersResponseOutputTypeDef",
+    "SearchUsersResponseTypeDef",
     "SearchVocabulariesRequestRequestTypeDef",
     "SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
-    "SearchVocabulariesResponseOutputTypeDef",
-    "SecurityKeyOutputTypeDef",
-    "SecurityProfileOutputTypeDef",
+    "SearchVocabulariesResponseTypeDef",
+    "SecurityKeyTypeDef",
     "SecurityProfileSearchCriteriaTypeDef",
-    "SecurityProfileSearchSummaryOutputTypeDef",
-    "SecurityProfileSummaryOutputTypeDef",
+    "SecurityProfileSearchSummaryTypeDef",
+    "SecurityProfileSummaryTypeDef",
+    "SecurityProfileTypeDef",
     "SecurityProfilesSearchFilterTypeDef",
     "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationOutputTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "StartChatContactRequestRequestTypeDef",
-    "StartChatContactResponseOutputTypeDef",
+    "StartChatContactResponseTypeDef",
     "StartContactEvaluationRequestRequestTypeDef",
-    "StartContactEvaluationResponseOutputTypeDef",
+    "StartContactEvaluationResponseTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
     "StartContactStreamingRequestRequestTypeDef",
-    "StartContactStreamingResponseOutputTypeDef",
+    "StartContactStreamingResponseTypeDef",
     "StartOutboundVoiceContactRequestRequestTypeDef",
-    "StartOutboundVoiceContactResponseOutputTypeDef",
+    "StartOutboundVoiceContactResponseTypeDef",
     "StartTaskContactRequestRequestTypeDef",
-    "StartTaskContactResponseOutputTypeDef",
+    "StartTaskContactResponseTypeDef",
     "StopContactRecordingRequestRequestTypeDef",
     "StopContactRequestRequestTypeDef",
     "StopContactStreamingRequestRequestTypeDef",
     "StringConditionTypeDef",
-    "StringReferenceOutputTypeDef",
+    "StringReferenceTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
-    "SubmitContactEvaluationResponseOutputTypeDef",
+    "SubmitContactEvaluationResponseTypeDef",
     "SuspendContactRecordingRequestRequestTypeDef",
     "TagConditionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagSearchConditionTypeDef",
-    "TagSetOutputTypeDef",
+    "TagSetTypeDef",
     "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
     "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
     "TaskTemplateDefaultFieldValueOutputTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
     "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
     "TaskTemplateFieldIdentifierOutputTypeDef",
     "TaskTemplateFieldIdentifierTypeDef",
     "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
-    "TaskTemplateMetadataOutputTypeDef",
+    "TaskTemplateMetadataTypeDef",
     "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
     "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
     "ThresholdV2OutputTypeDef",
     "ThresholdV2TypeDef",
-    "TrafficDistributionGroupOutputTypeDef",
-    "TrafficDistributionGroupSummaryOutputTypeDef",
+    "TrafficDistributionGroupSummaryTypeDef",
+    "TrafficDistributionGroupTypeDef",
     "TransferContactRequestRequestTypeDef",
-    "TransferContactResponseOutputTypeDef",
+    "TransferContactResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "UpdateContactAttributesRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
-    "UpdateContactEvaluationResponseOutputTypeDef",
+    "UpdateContactEvaluationResponseTypeDef",
     "UpdateContactFlowContentRequestRequestTypeDef",
     "UpdateContactFlowMetadataRequestRequestTypeDef",
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     "UpdateContactFlowModuleMetadataRequestRequestTypeDef",
     "UpdateContactFlowNameRequestRequestTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "UpdateContactScheduleRequestRequestTypeDef",
     "UpdateEvaluationFormRequestRequestTypeDef",
-    "UpdateEvaluationFormResponseOutputTypeDef",
+    "UpdateEvaluationFormResponseTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "UpdateInstanceAttributeRequestRequestTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
-    "UpdatePhoneNumberResponseOutputTypeDef",
+    "UpdatePhoneNumberResponseTypeDef",
     "UpdatePromptRequestRequestTypeDef",
-    "UpdatePromptResponseOutputTypeDef",
+    "UpdatePromptResponseTypeDef",
     "UpdateQueueHoursOfOperationRequestRequestTypeDef",
     "UpdateQueueMaxContactsRequestRequestTypeDef",
     "UpdateQueueNameRequestRequestTypeDef",
     "UpdateQueueOutboundCallerConfigRequestRequestTypeDef",
     "UpdateQueueStatusRequestRequestTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "UpdateQuickConnectNameRequestRequestTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef",
     "UpdateRoutingProfileNameRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
-    "UpdateTaskTemplateResponseOutputTypeDef",
+    "UpdateTaskTemplateResponseTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     "UpdateUserHierarchyRequestRequestTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "UpdateUserIdentityInfoRequestRequestTypeDef",
     "UpdateUserPhoneConfigRequestRequestTypeDef",
     "UpdateUserRoutingProfileRequestRequestTypeDef",
     "UpdateUserSecurityProfilesRequestRequestTypeDef",
-    "UrlReferenceOutputTypeDef",
-    "UseCaseOutputTypeDef",
+    "UrlReferenceTypeDef",
+    "UseCaseTypeDef",
     "UserDataFiltersTypeDef",
-    "UserDataOutputTypeDef",
-    "UserIdentityInfoLiteOutputTypeDef",
+    "UserDataTypeDef",
+    "UserIdentityInfoLiteTypeDef",
     "UserIdentityInfoOutputTypeDef",
     "UserIdentityInfoTypeDef",
-    "UserOutputTypeDef",
     "UserPhoneConfigOutputTypeDef",
     "UserPhoneConfigTypeDef",
     "UserQuickConnectConfigOutputTypeDef",
     "UserQuickConnectConfigTypeDef",
-    "UserReferenceOutputTypeDef",
+    "UserReferenceTypeDef",
     "UserSearchCriteriaTypeDef",
     "UserSearchFilterTypeDef",
-    "UserSearchSummaryOutputTypeDef",
-    "UserSummaryOutputTypeDef",
-    "VocabularyOutputTypeDef",
-    "VocabularySummaryOutputTypeDef",
+    "UserSearchSummaryTypeDef",
+    "UserSummaryTypeDef",
+    "UserTypeDef",
+    "VocabularySummaryTypeDef",
+    "VocabularyTypeDef",
     "VoiceRecordingConfigurationTypeDef",
-    "WisdomInfoOutputTypeDef",
+    "WisdomInfoTypeDef",
 )
 
-ActionSummaryOutputTypeDef = TypedDict(
-    "ActionSummaryOutputTypeDef",
+ActionSummaryTypeDef = TypedDict(
+    "ActionSummaryTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 
 ActivateEvaluationFormRequestRequestTypeDef = TypedDict(
     "ActivateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-ActivateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "ActivateEvaluationFormResponseOutputTypeDef",
+ActivateEvaluationFormResponseTypeDef = TypedDict(
+    "ActivateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentContactReferenceOutputTypeDef = TypedDict(
-    "AgentContactReferenceOutputTypeDef",
+AgentContactReferenceTypeDef = TypedDict(
+    "AgentContactReferenceTypeDef",
     {
         "ContactId": str,
         "Channel": ChannelType,
         "InitiationMethod": ContactInitiationMethodType,
         "AgentContactState": ContactStateType,
         "StateStartTimestamp": datetime,
         "ConnectedToAgentTimestamp": datetime,
-        "Queue": "QueueReferenceOutputTypeDef",
+        "Queue": "QueueReferenceTypeDef",
     },
 )
 
-AgentInfoOutputTypeDef = TypedDict(
-    "AgentInfoOutputTypeDef",
+AgentInfoTypeDef = TypedDict(
+    "AgentInfoTypeDef",
     {
         "Id": str,
         "ConnectedToAgentTimestamp": datetime,
     },
 )
 
-AgentStatusOutputTypeDef = TypedDict(
-    "AgentStatusOutputTypeDef",
-    {
-        "AgentStatusARN": str,
-        "AgentStatusId": str,
-        "Name": str,
-        "Description": str,
-        "Type": AgentStatusTypeType,
-        "DisplayOrder": int,
-        "State": AgentStatusStateType,
-        "Tags": Dict[str, str],
-    },
-)
-
-AgentStatusReferenceOutputTypeDef = TypedDict(
-    "AgentStatusReferenceOutputTypeDef",
+AgentStatusReferenceTypeDef = TypedDict(
+    "AgentStatusReferenceTypeDef",
     {
         "StatusStartTimestamp": datetime,
         "StatusArn": str,
         "StatusName": str,
     },
 )
 
-AgentStatusSummaryOutputTypeDef = TypedDict(
-    "AgentStatusSummaryOutputTypeDef",
+AgentStatusSummaryTypeDef = TypedDict(
+    "AgentStatusSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": AgentStatusTypeType,
     },
 )
 
+AgentStatusTypeDef = TypedDict(
+    "AgentStatusTypeDef",
+    {
+        "AgentStatusARN": str,
+        "AgentStatusId": str,
+        "Name": str,
+        "Description": str,
+        "Type": AgentStatusTypeType,
+        "DisplayOrder": int,
+        "State": AgentStatusStateType,
+        "Tags": Dict[str, str],
+    },
+)
+
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": bool,
         "AwaitAnswerMachinePrompt": bool,
     },
     total=False,
@@ -839,16 +839,16 @@
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": "InstanceStorageConfigTypeDef",
     },
 )
 
-AssociateInstanceStorageConfigResponseOutputTypeDef = TypedDict(
-    "AssociateInstanceStorageConfigResponseOutputTypeDef",
+AssociateInstanceStorageConfigResponseTypeDef = TypedDict(
+    "AssociateInstanceStorageConfigResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateLambdaFunctionRequestRequestTypeDef = TypedDict(
@@ -898,41 +898,41 @@
     "AssociateSecurityKeyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Key": str,
     },
 )
 
-AssociateSecurityKeyResponseOutputTypeDef = TypedDict(
-    "AssociateSecurityKeyResponseOutputTypeDef",
+AssociateSecurityKeyResponseTypeDef = TypedDict(
+    "AssociateSecurityKeyResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachmentReferenceOutputTypeDef = TypedDict(
-    "AttachmentReferenceOutputTypeDef",
+AttachmentReferenceTypeDef = TypedDict(
+    "AttachmentReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
         "Status": ReferenceStatusType,
     },
 )
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
+AttributeTypeDef = TypedDict(
+    "AttributeTypeDef",
     {
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
 )
 
-AvailableNumberSummaryOutputTypeDef = TypedDict(
-    "AvailableNumberSummaryOutputTypeDef",
+AvailableNumberSummaryTypeDef = TypedDict(
+    "AvailableNumberSummaryTypeDef",
     {
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
 )
 
@@ -976,114 +976,114 @@
 )
 
 class ClaimPhoneNumberRequestRequestTypeDef(
     _RequiredClaimPhoneNumberRequestRequestTypeDef, _OptionalClaimPhoneNumberRequestRequestTypeDef
 ):
     pass
 
-ClaimPhoneNumberResponseOutputTypeDef = TypedDict(
-    "ClaimPhoneNumberResponseOutputTypeDef",
+ClaimPhoneNumberResponseTypeDef = TypedDict(
+    "ClaimPhoneNumberResponseTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClaimedPhoneNumberSummaryOutputTypeDef = TypedDict(
-    "ClaimedPhoneNumberSummaryOutputTypeDef",
+ClaimedPhoneNumberSummaryTypeDef = TypedDict(
+    "ClaimedPhoneNumberSummaryTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberDescription": str,
         "TargetArn": str,
         "Tags": Dict[str, str],
-        "PhoneNumberStatus": "PhoneNumberStatusOutputTypeDef",
+        "PhoneNumberStatus": "PhoneNumberStatusTypeDef",
     },
 )
 
 ContactFilterTypeDef = TypedDict(
     "ContactFilterTypeDef",
     {
         "ContactStates": Sequence[ContactStateType],
     },
     total=False,
 )
 
-ContactFlowModuleOutputTypeDef = TypedDict(
-    "ContactFlowModuleOutputTypeDef",
+ContactFlowModuleSummaryTypeDef = TypedDict(
+    "ContactFlowModuleSummaryTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "State": ContactFlowModuleStateType,
+    },
+)
+
+ContactFlowModuleTypeDef = TypedDict(
+    "ContactFlowModuleTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Content": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
         "Status": ContactFlowModuleStatusType,
         "Tags": Dict[str, str],
     },
 )
 
-ContactFlowModuleSummaryOutputTypeDef = TypedDict(
-    "ContactFlowModuleSummaryOutputTypeDef",
+ContactFlowSummaryTypeDef = TypedDict(
+    "ContactFlowSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "State": ContactFlowModuleStateType,
+        "ContactFlowType": ContactFlowTypeType,
+        "ContactFlowState": ContactFlowStateType,
     },
 )
 
-ContactFlowOutputTypeDef = TypedDict(
-    "ContactFlowOutputTypeDef",
+ContactFlowTypeDef = TypedDict(
+    "ContactFlowTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "State": ContactFlowStateType,
         "Description": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
 )
 
-ContactFlowSummaryOutputTypeDef = TypedDict(
-    "ContactFlowSummaryOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "ContactFlowType": ContactFlowTypeType,
-        "ContactFlowState": ContactFlowStateType,
-    },
-)
-
-ContactOutputTypeDef = TypedDict(
-    "ContactOutputTypeDef",
+ContactTypeDef = TypedDict(
+    "ContactTypeDef",
     {
         "Arn": str,
         "Id": str,
         "InitialContactId": str,
         "PreviousContactId": str,
         "InitiationMethod": ContactInitiationMethodType,
         "Name": str,
         "Description": str,
         "Channel": ChannelType,
-        "QueueInfo": "QueueInfoOutputTypeDef",
-        "AgentInfo": "AgentInfoOutputTypeDef",
+        "QueueInfo": "QueueInfoTypeDef",
+        "AgentInfo": "AgentInfoTypeDef",
         "InitiationTimestamp": datetime,
         "DisconnectTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ScheduledTimestamp": datetime,
         "RelatedContactId": str,
-        "WisdomInfo": "WisdomInfoOutputTypeDef",
+        "WisdomInfo": "WisdomInfoTypeDef",
     },
 )
 
 ControlPlaneTagFilterTypeDef = TypedDict(
     "ControlPlaneTagFilterTypeDef",
     {
         "OrConditions": Sequence[Sequence["TagConditionTypeDef"]],
@@ -1112,16 +1112,16 @@
 )
 
 class CreateAgentStatusRequestRequestTypeDef(
     _RequiredCreateAgentStatusRequestRequestTypeDef, _OptionalCreateAgentStatusRequestRequestTypeDef
 ):
     pass
 
-CreateAgentStatusResponseOutputTypeDef = TypedDict(
-    "CreateAgentStatusResponseOutputTypeDef",
+CreateAgentStatusResponseTypeDef = TypedDict(
+    "CreateAgentStatusResponseTypeDef",
     {
         "AgentStatusARN": str,
         "AgentStatusId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1145,16 +1145,16 @@
 
 class CreateContactFlowModuleRequestRequestTypeDef(
     _RequiredCreateContactFlowModuleRequestRequestTypeDef,
     _OptionalCreateContactFlowModuleRequestRequestTypeDef,
 ):
     pass
 
-CreateContactFlowModuleResponseOutputTypeDef = TypedDict(
-    "CreateContactFlowModuleResponseOutputTypeDef",
+CreateContactFlowModuleResponseTypeDef = TypedDict(
+    "CreateContactFlowModuleResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1177,16 +1177,16 @@
 )
 
 class CreateContactFlowRequestRequestTypeDef(
     _RequiredCreateContactFlowRequestRequestTypeDef, _OptionalCreateContactFlowRequestRequestTypeDef
 ):
     pass
 
-CreateContactFlowResponseOutputTypeDef = TypedDict(
-    "CreateContactFlowResponseOutputTypeDef",
+CreateContactFlowResponseTypeDef = TypedDict(
+    "CreateContactFlowResponseTypeDef",
     {
         "ContactFlowId": str,
         "ContactFlowArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1210,16 +1210,16 @@
 
 class CreateEvaluationFormRequestRequestTypeDef(
     _RequiredCreateEvaluationFormRequestRequestTypeDef,
     _OptionalCreateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-CreateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "CreateEvaluationFormResponseOutputTypeDef",
+CreateEvaluationFormResponseTypeDef = TypedDict(
+    "CreateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1243,16 +1243,16 @@
 
 class CreateHoursOfOperationRequestRequestTypeDef(
     _RequiredCreateHoursOfOperationRequestRequestTypeDef,
     _OptionalCreateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
-CreateHoursOfOperationResponseOutputTypeDef = TypedDict(
-    "CreateHoursOfOperationResponseOutputTypeDef",
+CreateHoursOfOperationResponseTypeDef = TypedDict(
+    "CreateHoursOfOperationResponseTypeDef",
     {
         "HoursOfOperationId": str,
         "HoursOfOperationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1275,16 +1275,16 @@
 )
 
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
-CreateInstanceResponseOutputTypeDef = TypedDict(
-    "CreateInstanceResponseOutputTypeDef",
+CreateInstanceResponseTypeDef = TypedDict(
+    "CreateInstanceResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1309,16 +1309,16 @@
 
 class CreateIntegrationAssociationRequestRequestTypeDef(
     _RequiredCreateIntegrationAssociationRequestRequestTypeDef,
     _OptionalCreateIntegrationAssociationRequestRequestTypeDef,
 ):
     pass
 
-CreateIntegrationAssociationResponseOutputTypeDef = TypedDict(
-    "CreateIntegrationAssociationResponseOutputTypeDef",
+CreateIntegrationAssociationResponseTypeDef = TypedDict(
+    "CreateIntegrationAssociationResponseTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1339,18 +1339,18 @@
 )
 
 class CreateParticipantRequestRequestTypeDef(
     _RequiredCreateParticipantRequestRequestTypeDef, _OptionalCreateParticipantRequestRequestTypeDef
 ):
     pass
 
-CreateParticipantResponseOutputTypeDef = TypedDict(
-    "CreateParticipantResponseOutputTypeDef",
+CreateParticipantResponseTypeDef = TypedDict(
+    "CreateParticipantResponseTypeDef",
     {
-        "ParticipantCredentials": "ParticipantTokenCredentialsOutputTypeDef",
+        "ParticipantCredentials": "ParticipantTokenCredentialsTypeDef",
         "ParticipantId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePromptRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePromptRequestRequestTypeDef",
@@ -1370,16 +1370,16 @@
 )
 
 class CreatePromptRequestRequestTypeDef(
     _RequiredCreatePromptRequestRequestTypeDef, _OptionalCreatePromptRequestRequestTypeDef
 ):
     pass
 
-CreatePromptResponseOutputTypeDef = TypedDict(
-    "CreatePromptResponseOutputTypeDef",
+CreatePromptResponseTypeDef = TypedDict(
+    "CreatePromptResponseTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1404,16 +1404,16 @@
 )
 
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
-CreateQueueResponseOutputTypeDef = TypedDict(
-    "CreateQueueResponseOutputTypeDef",
+CreateQueueResponseTypeDef = TypedDict(
+    "CreateQueueResponseTypeDef",
     {
         "QueueArn": str,
         "QueueId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1436,16 +1436,16 @@
 
 class CreateQuickConnectRequestRequestTypeDef(
     _RequiredCreateQuickConnectRequestRequestTypeDef,
     _OptionalCreateQuickConnectRequestRequestTypeDef,
 ):
     pass
 
-CreateQuickConnectResponseOutputTypeDef = TypedDict(
-    "CreateQuickConnectResponseOutputTypeDef",
+CreateQuickConnectResponseTypeDef = TypedDict(
+    "CreateQuickConnectResponseTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1470,16 +1470,16 @@
 
 class CreateRoutingProfileRequestRequestTypeDef(
     _RequiredCreateRoutingProfileRequestRequestTypeDef,
     _OptionalCreateRoutingProfileRequestRequestTypeDef,
 ):
     pass
 
-CreateRoutingProfileResponseOutputTypeDef = TypedDict(
-    "CreateRoutingProfileResponseOutputTypeDef",
+CreateRoutingProfileResponseTypeDef = TypedDict(
+    "CreateRoutingProfileResponseTypeDef",
     {
         "RoutingProfileArn": str,
         "RoutingProfileId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1503,16 +1503,16 @@
 )
 
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
-CreateRuleResponseOutputTypeDef = TypedDict(
-    "CreateRuleResponseOutputTypeDef",
+CreateRuleResponseTypeDef = TypedDict(
+    "CreateRuleResponseTypeDef",
     {
         "RuleArn": str,
         "RuleId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1537,16 +1537,16 @@
 
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-CreateSecurityProfileResponseOutputTypeDef = TypedDict(
-    "CreateSecurityProfileResponseOutputTypeDef",
+CreateSecurityProfileResponseTypeDef = TypedDict(
+    "CreateSecurityProfileResponseTypeDef",
     {
         "SecurityProfileId": str,
         "SecurityProfileArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1573,16 +1573,16 @@
 
 class CreateTaskTemplateRequestRequestTypeDef(
     _RequiredCreateTaskTemplateRequestRequestTypeDef,
     _OptionalCreateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-CreateTaskTemplateResponseOutputTypeDef = TypedDict(
-    "CreateTaskTemplateResponseOutputTypeDef",
+CreateTaskTemplateResponseTypeDef = TypedDict(
+    "CreateTaskTemplateResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1605,16 +1605,16 @@
 
 class CreateTrafficDistributionGroupRequestRequestTypeDef(
     _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef,
     _OptionalCreateTrafficDistributionGroupRequestRequestTypeDef,
 ):
     pass
 
-CreateTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
-    "CreateTrafficDistributionGroupResponseOutputTypeDef",
+CreateTrafficDistributionGroupResponseTypeDef = TypedDict(
+    "CreateTrafficDistributionGroupResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1635,16 +1635,16 @@
 )
 
 class CreateUseCaseRequestRequestTypeDef(
     _RequiredCreateUseCaseRequestRequestTypeDef, _OptionalCreateUseCaseRequestRequestTypeDef
 ):
     pass
 
-CreateUseCaseResponseOutputTypeDef = TypedDict(
-    "CreateUseCaseResponseOutputTypeDef",
+CreateUseCaseResponseTypeDef = TypedDict(
+    "CreateUseCaseResponseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1666,16 +1666,16 @@
 
 class CreateUserHierarchyGroupRequestRequestTypeDef(
     _RequiredCreateUserHierarchyGroupRequestRequestTypeDef,
     _OptionalCreateUserHierarchyGroupRequestRequestTypeDef,
 ):
     pass
 
-CreateUserHierarchyGroupResponseOutputTypeDef = TypedDict(
-    "CreateUserHierarchyGroupResponseOutputTypeDef",
+CreateUserHierarchyGroupResponseTypeDef = TypedDict(
+    "CreateUserHierarchyGroupResponseTypeDef",
     {
         "HierarchyGroupId": str,
         "HierarchyGroupArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1702,16 +1702,16 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-CreateUserResponseOutputTypeDef = TypedDict(
-    "CreateUserResponseOutputTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
         "UserId": str,
         "UserArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1734,26 +1734,26 @@
 )
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-CreateVocabularyResponseOutputTypeDef = TypedDict(
-    "CreateVocabularyResponseOutputTypeDef",
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CredentialsOutputTypeDef = TypedDict(
-    "CredentialsOutputTypeDef",
+CredentialsTypeDef = TypedDict(
+    "CredentialsTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
     },
 )
@@ -1768,35 +1768,35 @@
 CrossChannelBehaviorTypeDef = TypedDict(
     "CrossChannelBehaviorTypeDef",
     {
         "BehaviorType": BehaviorTypeType,
     },
 )
 
-CurrentMetricDataOutputTypeDef = TypedDict(
-    "CurrentMetricDataOutputTypeDef",
+CurrentMetricDataTypeDef = TypedDict(
+    "CurrentMetricDataTypeDef",
     {
         "Metric": "CurrentMetricOutputTypeDef",
         "Value": float,
     },
 )
 
 CurrentMetricOutputTypeDef = TypedDict(
     "CurrentMetricOutputTypeDef",
     {
         "Name": CurrentMetricNameType,
         "Unit": UnitType,
     },
 )
 
-CurrentMetricResultOutputTypeDef = TypedDict(
-    "CurrentMetricResultOutputTypeDef",
+CurrentMetricResultTypeDef = TypedDict(
+    "CurrentMetricResultTypeDef",
     {
-        "Dimensions": "DimensionsOutputTypeDef",
-        "Collections": List["CurrentMetricDataOutputTypeDef"],
+        "Dimensions": "DimensionsTypeDef",
+        "Collections": List["CurrentMetricDataTypeDef"],
     },
 )
 
 CurrentMetricSortCriteriaTypeDef = TypedDict(
     "CurrentMetricSortCriteriaTypeDef",
     {
         "SortByMetric": CurrentMetricNameType,
@@ -1810,16 +1810,16 @@
     {
         "Name": CurrentMetricNameType,
         "Unit": UnitType,
     },
     total=False,
 )
 
-DateReferenceOutputTypeDef = TypedDict(
-    "DateReferenceOutputTypeDef",
+DateReferenceTypeDef = TypedDict(
+    "DateReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 DeactivateEvaluationFormRequestRequestTypeDef = TypedDict(
@@ -1827,26 +1827,26 @@
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
     },
 )
 
-DeactivateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "DeactivateEvaluationFormResponseOutputTypeDef",
+DeactivateEvaluationFormResponseTypeDef = TypedDict(
+    "DeactivateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DefaultVocabularyOutputTypeDef = TypedDict(
-    "DefaultVocabularyOutputTypeDef",
+DefaultVocabularyTypeDef = TypedDict(
+    "DefaultVocabularyTypeDef",
     {
         "InstanceId": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "VocabularyId": str,
         "VocabularyName": str,
     },
 )
@@ -2011,16 +2011,16 @@
     "DeleteVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DeleteVocabularyResponseOutputTypeDef = TypedDict(
-    "DeleteVocabularyResponseOutputTypeDef",
+DeleteVocabularyResponseTypeDef = TypedDict(
+    "DeleteVocabularyResponseTypeDef",
     {
         "VocabularyArn": str,
         "VocabularyId": str,
         "State": VocabularyStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2029,83 +2029,83 @@
     "DescribeAgentStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-DescribeAgentStatusResponseOutputTypeDef = TypedDict(
-    "DescribeAgentStatusResponseOutputTypeDef",
+DescribeAgentStatusResponseTypeDef = TypedDict(
+    "DescribeAgentStatusResponseTypeDef",
     {
-        "AgentStatus": "AgentStatusOutputTypeDef",
+        "AgentStatus": "AgentStatusTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactEvaluationRequestRequestTypeDef = TypedDict(
     "DescribeContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
 
-DescribeContactEvaluationResponseOutputTypeDef = TypedDict(
-    "DescribeContactEvaluationResponseOutputTypeDef",
+DescribeContactEvaluationResponseTypeDef = TypedDict(
+    "DescribeContactEvaluationResponseTypeDef",
     {
-        "Evaluation": "EvaluationOutputTypeDef",
-        "EvaluationForm": "EvaluationFormContentOutputTypeDef",
+        "Evaluation": "EvaluationTypeDef",
+        "EvaluationForm": "EvaluationFormContentTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowModuleRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowModuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
     },
 )
 
-DescribeContactFlowModuleResponseOutputTypeDef = TypedDict(
-    "DescribeContactFlowModuleResponseOutputTypeDef",
+DescribeContactFlowModuleResponseTypeDef = TypedDict(
+    "DescribeContactFlowModuleResponseTypeDef",
     {
-        "ContactFlowModule": "ContactFlowModuleOutputTypeDef",
+        "ContactFlowModule": "ContactFlowModuleTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactFlowRequestRequestTypeDef = TypedDict(
     "DescribeContactFlowRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
 
-DescribeContactFlowResponseOutputTypeDef = TypedDict(
-    "DescribeContactFlowResponseOutputTypeDef",
+DescribeContactFlowResponseTypeDef = TypedDict(
+    "DescribeContactFlowResponseTypeDef",
     {
-        "ContactFlow": "ContactFlowOutputTypeDef",
+        "ContactFlow": "ContactFlowTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContactRequestRequestTypeDef = TypedDict(
     "DescribeContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
 
-DescribeContactResponseOutputTypeDef = TypedDict(
-    "DescribeContactResponseOutputTypeDef",
+DescribeContactResponseTypeDef = TypedDict(
+    "DescribeContactResponseTypeDef",
     {
-        "Contact": "ContactOutputTypeDef",
+        "Contact": "ContactTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEvaluationFormRequestRequestTypeDef",
     {
@@ -2123,281 +2123,281 @@
 
 class DescribeEvaluationFormRequestRequestTypeDef(
     _RequiredDescribeEvaluationFormRequestRequestTypeDef,
     _OptionalDescribeEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-DescribeEvaluationFormResponseOutputTypeDef = TypedDict(
-    "DescribeEvaluationFormResponseOutputTypeDef",
+DescribeEvaluationFormResponseTypeDef = TypedDict(
+    "DescribeEvaluationFormResponseTypeDef",
     {
-        "EvaluationForm": "EvaluationFormOutputTypeDef",
+        "EvaluationForm": "EvaluationFormTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DescribeHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
 
-DescribeHoursOfOperationResponseOutputTypeDef = TypedDict(
-    "DescribeHoursOfOperationResponseOutputTypeDef",
+DescribeHoursOfOperationResponseTypeDef = TypedDict(
+    "DescribeHoursOfOperationResponseTypeDef",
     {
-        "HoursOfOperation": "HoursOfOperationOutputTypeDef",
+        "HoursOfOperation": "HoursOfOperationTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceAttributeRequestRequestTypeDef = TypedDict(
     "DescribeInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
     },
 )
 
-DescribeInstanceAttributeResponseOutputTypeDef = TypedDict(
-    "DescribeInstanceAttributeResponseOutputTypeDef",
+DescribeInstanceAttributeResponseTypeDef = TypedDict(
+    "DescribeInstanceAttributeResponseTypeDef",
     {
-        "Attribute": "AttributeOutputTypeDef",
+        "Attribute": "AttributeTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceRequestRequestTypeDef = TypedDict(
     "DescribeInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeInstanceResponseOutputTypeDef = TypedDict(
-    "DescribeInstanceResponseOutputTypeDef",
+DescribeInstanceResponseTypeDef = TypedDict(
+    "DescribeInstanceResponseTypeDef",
     {
-        "Instance": "InstanceOutputTypeDef",
+        "Instance": "InstanceTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceStorageConfigRequestRequestTypeDef = TypedDict(
     "DescribeInstanceStorageConfigRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
 
-DescribeInstanceStorageConfigResponseOutputTypeDef = TypedDict(
-    "DescribeInstanceStorageConfigResponseOutputTypeDef",
+DescribeInstanceStorageConfigResponseTypeDef = TypedDict(
+    "DescribeInstanceStorageConfigResponseTypeDef",
     {
         "StorageConfig": "InstanceStorageConfigOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePhoneNumberRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-DescribePhoneNumberResponseOutputTypeDef = TypedDict(
-    "DescribePhoneNumberResponseOutputTypeDef",
+DescribePhoneNumberResponseTypeDef = TypedDict(
+    "DescribePhoneNumberResponseTypeDef",
     {
-        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryOutputTypeDef",
+        "ClaimedPhoneNumberSummary": "ClaimedPhoneNumberSummaryTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePromptRequestRequestTypeDef = TypedDict(
     "DescribePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-DescribePromptResponseOutputTypeDef = TypedDict(
-    "DescribePromptResponseOutputTypeDef",
+DescribePromptResponseTypeDef = TypedDict(
+    "DescribePromptResponseTypeDef",
     {
-        "Prompt": "PromptOutputTypeDef",
+        "Prompt": "PromptTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueueRequestRequestTypeDef = TypedDict(
     "DescribeQueueRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
 
-DescribeQueueResponseOutputTypeDef = TypedDict(
-    "DescribeQueueResponseOutputTypeDef",
+DescribeQueueResponseTypeDef = TypedDict(
+    "DescribeQueueResponseTypeDef",
     {
-        "Queue": "QueueOutputTypeDef",
+        "Queue": "QueueTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQuickConnectRequestRequestTypeDef = TypedDict(
     "DescribeQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
-DescribeQuickConnectResponseOutputTypeDef = TypedDict(
-    "DescribeQuickConnectResponseOutputTypeDef",
+DescribeQuickConnectResponseTypeDef = TypedDict(
+    "DescribeQuickConnectResponseTypeDef",
     {
-        "QuickConnect": "QuickConnectOutputTypeDef",
+        "QuickConnect": "QuickConnectTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRoutingProfileRequestRequestTypeDef = TypedDict(
     "DescribeRoutingProfileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
 
-DescribeRoutingProfileResponseOutputTypeDef = TypedDict(
-    "DescribeRoutingProfileResponseOutputTypeDef",
+DescribeRoutingProfileResponseTypeDef = TypedDict(
+    "DescribeRoutingProfileResponseTypeDef",
     {
-        "RoutingProfile": "RoutingProfileOutputTypeDef",
+        "RoutingProfile": "RoutingProfileTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRuleRequestRequestTypeDef = TypedDict(
     "DescribeRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
 
-DescribeRuleResponseOutputTypeDef = TypedDict(
-    "DescribeRuleResponseOutputTypeDef",
+DescribeRuleResponseTypeDef = TypedDict(
+    "DescribeRuleResponseTypeDef",
     {
-        "Rule": "RuleOutputTypeDef",
+        "Rule": "RuleTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
 
-DescribeSecurityProfileResponseOutputTypeDef = TypedDict(
-    "DescribeSecurityProfileResponseOutputTypeDef",
+DescribeSecurityProfileResponseTypeDef = TypedDict(
+    "DescribeSecurityProfileResponseTypeDef",
     {
-        "SecurityProfile": "SecurityProfileOutputTypeDef",
+        "SecurityProfile": "SecurityProfileTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrafficDistributionGroupRequestRequestTypeDef = TypedDict(
     "DescribeTrafficDistributionGroupRequestRequestTypeDef",
     {
         "TrafficDistributionGroupId": str,
     },
 )
 
-DescribeTrafficDistributionGroupResponseOutputTypeDef = TypedDict(
-    "DescribeTrafficDistributionGroupResponseOutputTypeDef",
+DescribeTrafficDistributionGroupResponseTypeDef = TypedDict(
+    "DescribeTrafficDistributionGroupResponseTypeDef",
     {
-        "TrafficDistributionGroup": "TrafficDistributionGroupOutputTypeDef",
+        "TrafficDistributionGroup": "TrafficDistributionGroupTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyGroupRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyGroupRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyGroupResponseOutputTypeDef = TypedDict(
-    "DescribeUserHierarchyGroupResponseOutputTypeDef",
+DescribeUserHierarchyGroupResponseTypeDef = TypedDict(
+    "DescribeUserHierarchyGroupResponseTypeDef",
     {
-        "HierarchyGroup": "HierarchyGroupOutputTypeDef",
+        "HierarchyGroup": "HierarchyGroupTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserHierarchyStructureRequestRequestTypeDef = TypedDict(
     "DescribeUserHierarchyStructureRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-DescribeUserHierarchyStructureResponseOutputTypeDef = TypedDict(
-    "DescribeUserHierarchyStructureResponseOutputTypeDef",
+DescribeUserHierarchyStructureResponseTypeDef = TypedDict(
+    "DescribeUserHierarchyStructureResponseTypeDef",
     {
-        "HierarchyStructure": "HierarchyStructureOutputTypeDef",
+        "HierarchyStructure": "HierarchyStructureTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-DescribeUserResponseOutputTypeDef = TypedDict(
-    "DescribeUserResponseOutputTypeDef",
+DescribeUserResponseTypeDef = TypedDict(
+    "DescribeUserResponseTypeDef",
     {
-        "User": "UserOutputTypeDef",
+        "User": "UserTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVocabularyRequestRequestTypeDef = TypedDict(
     "DescribeVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyId": str,
     },
 )
 
-DescribeVocabularyResponseOutputTypeDef = TypedDict(
-    "DescribeVocabularyResponseOutputTypeDef",
+DescribeVocabularyResponseTypeDef = TypedDict(
+    "DescribeVocabularyResponseTypeDef",
     {
-        "Vocabulary": "VocabularyOutputTypeDef",
+        "Vocabulary": "VocabularyTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DimensionsOutputTypeDef = TypedDict(
-    "DimensionsOutputTypeDef",
+DimensionsTypeDef = TypedDict(
+    "DimensionsTypeDef",
     {
-        "Queue": "QueueReferenceOutputTypeDef",
+        "Queue": "QueueReferenceTypeDef",
         "Channel": ChannelType,
-        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceTypeDef",
     },
 )
 
 DisassociateApprovedOriginRequestRequestTypeDef = TypedDict(
     "DisassociateApprovedOriginRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -2506,16 +2506,16 @@
     "DistributionTypeDef",
     {
         "Region": str,
         "Percentage": int,
     },
 )
 
-EmailReferenceOutputTypeDef = TypedDict(
-    "EmailReferenceOutputTypeDef",
+EmailReferenceTypeDef = TypedDict(
+    "EmailReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
@@ -2564,24 +2564,24 @@
     "EvaluationAnswerInputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
     },
     total=False,
 )
 
-EvaluationAnswerOutputOutputTypeDef = TypedDict(
-    "EvaluationAnswerOutputOutputTypeDef",
+EvaluationAnswerOutputTypeDef = TypedDict(
+    "EvaluationAnswerOutputTypeDef",
     {
         "Value": "EvaluationAnswerDataOutputTypeDef",
         "SystemSuggestedValue": "EvaluationAnswerDataOutputTypeDef",
     },
 )
 
-EvaluationFormContentOutputTypeDef = TypedDict(
-    "EvaluationFormContentOutputTypeDef",
+EvaluationFormContentTypeDef = TypedDict(
+    "EvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "Description": str,
         "Items": List["EvaluationFormItemOutputTypeDef"],
@@ -2681,34 +2681,14 @@
 
 class EvaluationFormNumericQuestionPropertiesTypeDef(
     _RequiredEvaluationFormNumericQuestionPropertiesTypeDef,
     _OptionalEvaluationFormNumericQuestionPropertiesTypeDef,
 ):
     pass
 
-EvaluationFormOutputTypeDef = TypedDict(
-    "EvaluationFormOutputTypeDef",
-    {
-        "EvaluationFormId": str,
-        "EvaluationFormVersion": int,
-        "Locked": bool,
-        "EvaluationFormArn": str,
-        "Title": str,
-        "Description": str,
-        "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemOutputTypeDef"],
-        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
-        "CreatedTime": datetime,
-        "CreatedBy": str,
-        "LastModifiedTime": datetime,
-        "LastModifiedBy": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 EvaluationFormQuestionOutputTypeDef = TypedDict(
     "EvaluationFormQuestionOutputTypeDef",
     {
         "Title": str,
         "Instructions": str,
         "RefId": str,
         "NotApplicableEnabled": bool,
@@ -2909,16 +2889,16 @@
 
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
-EvaluationFormSummaryOutputTypeDef = TypedDict(
-    "EvaluationFormSummaryOutputTypeDef",
+EvaluationFormSummaryTypeDef = TypedDict(
+    "EvaluationFormSummaryTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
@@ -2926,36 +2906,56 @@
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
         "LatestVersion": int,
         "ActiveVersion": int,
     },
 )
 
-EvaluationFormVersionSummaryOutputTypeDef = TypedDict(
-    "EvaluationFormVersionSummaryOutputTypeDef",
+EvaluationFormTypeDef = TypedDict(
+    "EvaluationFormTypeDef",
+    {
+        "EvaluationFormId": str,
+        "EvaluationFormVersion": int,
+        "Locked": bool,
+        "EvaluationFormArn": str,
+        "Title": str,
+        "Description": str,
+        "Status": EvaluationFormVersionStatusType,
+        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyOutputTypeDef",
+        "CreatedTime": datetime,
+        "CreatedBy": str,
+        "LastModifiedTime": datetime,
+        "LastModifiedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
+EvaluationFormVersionSummaryTypeDef = TypedDict(
+    "EvaluationFormVersionSummaryTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "Status": EvaluationFormVersionStatusType,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 
-EvaluationMetadataOutputTypeDef = TypedDict(
-    "EvaluationMetadataOutputTypeDef",
+EvaluationMetadataTypeDef = TypedDict(
+    "EvaluationMetadataTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
         "ContactAgentId": str,
-        "Score": "EvaluationScoreOutputTypeDef",
+        "Score": "EvaluationScoreTypeDef",
     },
 )
 
 EvaluationNoteOutputTypeDef = TypedDict(
     "EvaluationNoteOutputTypeDef",
     {
         "Value": str,
@@ -2966,54 +2966,54 @@
     "EvaluationNoteTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-EvaluationOutputTypeDef = TypedDict(
-    "EvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "EvaluationArn": str,
-        "Metadata": "EvaluationMetadataOutputTypeDef",
-        "Answers": Dict[str, "EvaluationAnswerOutputOutputTypeDef"],
-        "Notes": Dict[str, "EvaluationNoteOutputTypeDef"],
-        "Status": EvaluationStatusType,
-        "Scores": Dict[str, "EvaluationScoreOutputTypeDef"],
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
-        "Tags": Dict[str, str],
-    },
-)
-
-EvaluationScoreOutputTypeDef = TypedDict(
-    "EvaluationScoreOutputTypeDef",
+EvaluationScoreTypeDef = TypedDict(
+    "EvaluationScoreTypeDef",
     {
         "Percentage": float,
         "NotApplicable": bool,
         "AutomaticFail": bool,
     },
 )
 
-EvaluationSummaryOutputTypeDef = TypedDict(
-    "EvaluationSummaryOutputTypeDef",
+EvaluationSummaryTypeDef = TypedDict(
+    "EvaluationSummaryTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
-        "Score": "EvaluationScoreOutputTypeDef",
+        "Score": "EvaluationScoreTypeDef",
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
 )
 
+EvaluationTypeDef = TypedDict(
+    "EvaluationTypeDef",
+    {
+        "EvaluationId": str,
+        "EvaluationArn": str,
+        "Metadata": "EvaluationMetadataTypeDef",
+        "Answers": Dict[str, "EvaluationAnswerOutputTypeDef"],
+        "Notes": Dict[str, "EvaluationNoteOutputTypeDef"],
+        "Status": EvaluationStatusType,
+        "Scores": Dict[str, "EvaluationScoreTypeDef"],
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+        "Tags": Dict[str, str],
+    },
+)
+
 EventBridgeActionDefinitionOutputTypeDef = TypedDict(
     "EventBridgeActionDefinitionOutputTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -3047,16 +3047,16 @@
     "GetContactAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InitialContactId": str,
     },
 )
 
-GetContactAttributesResponseOutputTypeDef = TypedDict(
-    "GetContactAttributesResponseOutputTypeDef",
+GetContactAttributesResponseTypeDef = TypedDict(
+    "GetContactAttributesResponseTypeDef",
     {
         "Attributes": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentMetricDataRequestRequestTypeDef = TypedDict(
@@ -3080,19 +3080,19 @@
 
 class GetCurrentMetricDataRequestRequestTypeDef(
     _RequiredGetCurrentMetricDataRequestRequestTypeDef,
     _OptionalGetCurrentMetricDataRequestRequestTypeDef,
 ):
     pass
 
-GetCurrentMetricDataResponseOutputTypeDef = TypedDict(
-    "GetCurrentMetricDataResponseOutputTypeDef",
+GetCurrentMetricDataResponseTypeDef = TypedDict(
+    "GetCurrentMetricDataResponseTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["CurrentMetricResultOutputTypeDef"],
+        "MetricResults": List["CurrentMetricResultTypeDef"],
         "DataSnapshotTime": datetime,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetCurrentUserDataRequestRequestTypeDef = TypedDict(
@@ -3113,35 +3113,35 @@
 
 class GetCurrentUserDataRequestRequestTypeDef(
     _RequiredGetCurrentUserDataRequestRequestTypeDef,
     _OptionalGetCurrentUserDataRequestRequestTypeDef,
 ):
     pass
 
-GetCurrentUserDataResponseOutputTypeDef = TypedDict(
-    "GetCurrentUserDataResponseOutputTypeDef",
+GetCurrentUserDataResponseTypeDef = TypedDict(
+    "GetCurrentUserDataResponseTypeDef",
     {
         "NextToken": str,
-        "UserDataList": List["UserDataOutputTypeDef"],
+        "UserDataList": List["UserDataTypeDef"],
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFederationTokenRequestRequestTypeDef = TypedDict(
     "GetFederationTokenRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
-GetFederationTokenResponseOutputTypeDef = TypedDict(
-    "GetFederationTokenResponseOutputTypeDef",
+GetFederationTokenResponseTypeDef = TypedDict(
+    "GetFederationTokenResponseTypeDef",
     {
-        "Credentials": "CredentialsOutputTypeDef",
+        "Credentials": "CredentialsTypeDef",
         "SignInUrl": str,
         "UserArn": str,
         "UserId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3191,19 +3191,19 @@
 )
 
 class GetMetricDataRequestRequestTypeDef(
     _RequiredGetMetricDataRequestRequestTypeDef, _OptionalGetMetricDataRequestRequestTypeDef
 ):
     pass
 
-GetMetricDataResponseOutputTypeDef = TypedDict(
-    "GetMetricDataResponseOutputTypeDef",
+GetMetricDataResponseTypeDef = TypedDict(
+    "GetMetricDataResponseTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["HistoricalMetricResultOutputTypeDef"],
+        "MetricResults": List["HistoricalMetricResultTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataV2RequestRequestTypeDef",
     {
@@ -3225,33 +3225,33 @@
 )
 
 class GetMetricDataV2RequestRequestTypeDef(
     _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
 ):
     pass
 
-GetMetricDataV2ResponseOutputTypeDef = TypedDict(
-    "GetMetricDataV2ResponseOutputTypeDef",
+GetMetricDataV2ResponseTypeDef = TypedDict(
+    "GetMetricDataV2ResponseTypeDef",
     {
         "NextToken": str,
-        "MetricResults": List["MetricResultV2OutputTypeDef"],
+        "MetricResults": List["MetricResultV2TypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPromptFileRequestRequestTypeDef = TypedDict(
     "GetPromptFileRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
-GetPromptFileResponseOutputTypeDef = TypedDict(
-    "GetPromptFileResponseOutputTypeDef",
+GetPromptFileResponseTypeDef = TypedDict(
+    "GetPromptFileResponseTypeDef",
     {
         "PromptPresignedUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetTaskTemplateRequestRequestTypeDef = TypedDict(
@@ -3270,16 +3270,16 @@
 )
 
 class GetTaskTemplateRequestRequestTypeDef(
     _RequiredGetTaskTemplateRequestRequestTypeDef, _OptionalGetTaskTemplateRequestRequestTypeDef
 ):
     pass
 
-GetTaskTemplateResponseOutputTypeDef = TypedDict(
-    "GetTaskTemplateResponseOutputTypeDef",
+GetTaskTemplateResponseTypeDef = TypedDict(
+    "GetTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
@@ -3297,16 +3297,16 @@
 GetTrafficDistributionRequestRequestTypeDef = TypedDict(
     "GetTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficDistributionResponseOutputTypeDef = TypedDict(
-    "GetTrafficDistributionResponseOutputTypeDef",
+GetTrafficDistributionResponseTypeDef = TypedDict(
+    "GetTrafficDistributionResponseTypeDef",
     {
         "TelephonyConfig": "TelephonyConfigOutputTypeDef",
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3316,89 +3316,89 @@
     {
         "Value": str,
         "HierarchyGroupMatchType": HierarchyGroupMatchTypeType,
     },
     total=False,
 )
 
-HierarchyGroupOutputTypeDef = TypedDict(
-    "HierarchyGroupOutputTypeDef",
+HierarchyGroupSummaryReferenceTypeDef = TypedDict(
+    "HierarchyGroupSummaryReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
-        "Name": str,
-        "LevelId": str,
-        "HierarchyPath": "HierarchyPathOutputTypeDef",
-        "Tags": Dict[str, str],
     },
 )
 
-HierarchyGroupSummaryOutputTypeDef = TypedDict(
-    "HierarchyGroupSummaryOutputTypeDef",
+HierarchyGroupSummaryTypeDef = TypedDict(
+    "HierarchyGroupSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
-HierarchyGroupSummaryReferenceOutputTypeDef = TypedDict(
-    "HierarchyGroupSummaryReferenceOutputTypeDef",
+HierarchyGroupTypeDef = TypedDict(
+    "HierarchyGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
+        "Name": str,
+        "LevelId": str,
+        "HierarchyPath": "HierarchyPathTypeDef",
+        "Tags": Dict[str, str],
     },
 )
 
-HierarchyLevelOutputTypeDef = TypedDict(
-    "HierarchyLevelOutputTypeDef",
+HierarchyLevelTypeDef = TypedDict(
+    "HierarchyLevelTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
 HierarchyLevelUpdateTypeDef = TypedDict(
     "HierarchyLevelUpdateTypeDef",
     {
         "Name": str,
     },
 )
 
-HierarchyPathOutputTypeDef = TypedDict(
-    "HierarchyPathOutputTypeDef",
+HierarchyPathReferenceTypeDef = TypedDict(
+    "HierarchyPathReferenceTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelThree": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelFour": "HierarchyGroupSummaryOutputTypeDef",
-        "LevelFive": "HierarchyGroupSummaryOutputTypeDef",
+        "LevelOne": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelThree": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelFour": "HierarchyGroupSummaryReferenceTypeDef",
+        "LevelFive": "HierarchyGroupSummaryReferenceTypeDef",
     },
 )
 
-HierarchyPathReferenceOutputTypeDef = TypedDict(
-    "HierarchyPathReferenceOutputTypeDef",
+HierarchyPathTypeDef = TypedDict(
+    "HierarchyPathTypeDef",
     {
-        "LevelOne": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelTwo": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelThree": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelFour": "HierarchyGroupSummaryReferenceOutputTypeDef",
-        "LevelFive": "HierarchyGroupSummaryReferenceOutputTypeDef",
+        "LevelOne": "HierarchyGroupSummaryTypeDef",
+        "LevelTwo": "HierarchyGroupSummaryTypeDef",
+        "LevelThree": "HierarchyGroupSummaryTypeDef",
+        "LevelFour": "HierarchyGroupSummaryTypeDef",
+        "LevelFive": "HierarchyGroupSummaryTypeDef",
     },
 )
 
-HierarchyStructureOutputTypeDef = TypedDict(
-    "HierarchyStructureOutputTypeDef",
+HierarchyStructureTypeDef = TypedDict(
+    "HierarchyStructureTypeDef",
     {
-        "LevelOne": "HierarchyLevelOutputTypeDef",
-        "LevelTwo": "HierarchyLevelOutputTypeDef",
-        "LevelThree": "HierarchyLevelOutputTypeDef",
-        "LevelFour": "HierarchyLevelOutputTypeDef",
-        "LevelFive": "HierarchyLevelOutputTypeDef",
+        "LevelOne": "HierarchyLevelTypeDef",
+        "LevelTwo": "HierarchyLevelTypeDef",
+        "LevelThree": "HierarchyLevelTypeDef",
+        "LevelFour": "HierarchyLevelTypeDef",
+        "LevelFive": "HierarchyLevelTypeDef",
     },
 )
 
 HierarchyStructureUpdateTypeDef = TypedDict(
     "HierarchyStructureUpdateTypeDef",
     {
         "LevelOne": "HierarchyLevelUpdateTypeDef",
@@ -3406,16 +3406,16 @@
         "LevelThree": "HierarchyLevelUpdateTypeDef",
         "LevelFour": "HierarchyLevelUpdateTypeDef",
         "LevelFive": "HierarchyLevelUpdateTypeDef",
     },
     total=False,
 )
 
-HistoricalMetricDataOutputTypeDef = TypedDict(
-    "HistoricalMetricDataOutputTypeDef",
+HistoricalMetricDataTypeDef = TypedDict(
+    "HistoricalMetricDataTypeDef",
     {
         "Metric": "HistoricalMetricOutputTypeDef",
         "Value": float,
     },
 )
 
 HistoricalMetricOutputTypeDef = TypedDict(
@@ -3424,19 +3424,19 @@
         "Name": HistoricalMetricNameType,
         "Threshold": "ThresholdOutputTypeDef",
         "Statistic": StatisticType,
         "Unit": UnitType,
     },
 )
 
-HistoricalMetricResultOutputTypeDef = TypedDict(
-    "HistoricalMetricResultOutputTypeDef",
+HistoricalMetricResultTypeDef = TypedDict(
+    "HistoricalMetricResultTypeDef",
     {
-        "Dimensions": "DimensionsOutputTypeDef",
-        "Collections": List["HistoricalMetricDataOutputTypeDef"],
+        "Dimensions": "DimensionsTypeDef",
+        "Collections": List["HistoricalMetricDataTypeDef"],
     },
 )
 
 HistoricalMetricTypeDef = TypedDict(
     "HistoricalMetricTypeDef",
     {
         "Name": HistoricalMetricNameType,
@@ -3461,27 +3461,14 @@
     {
         "Day": HoursOfOperationDaysType,
         "StartTime": "HoursOfOperationTimeSliceTypeDef",
         "EndTime": "HoursOfOperationTimeSliceTypeDef",
     },
 )
 
-HoursOfOperationOutputTypeDef = TypedDict(
-    "HoursOfOperationOutputTypeDef",
-    {
-        "HoursOfOperationId": str,
-        "HoursOfOperationArn": str,
-        "Name": str,
-        "Description": str,
-        "TimeZone": str,
-        "Config": List["HoursOfOperationConfigOutputTypeDef"],
-        "Tags": Dict[str, str],
-    },
-)
-
 HoursOfOperationSearchCriteriaTypeDef = TypedDict(
     "HoursOfOperationSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -3492,16 +3479,16 @@
     "HoursOfOperationSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-HoursOfOperationSummaryOutputTypeDef = TypedDict(
-    "HoursOfOperationSummaryOutputTypeDef",
+HoursOfOperationSummaryTypeDef = TypedDict(
+    "HoursOfOperationSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
@@ -3517,33 +3504,29 @@
     "HoursOfOperationTimeSliceTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
 
-InstanceOutputTypeDef = TypedDict(
-    "InstanceOutputTypeDef",
+HoursOfOperationTypeDef = TypedDict(
+    "HoursOfOperationTypeDef",
     {
-        "Id": str,
-        "Arn": str,
-        "IdentityManagementType": DirectoryTypeType,
-        "InstanceAlias": str,
-        "CreatedTime": datetime,
-        "ServiceRole": str,
-        "InstanceStatus": InstanceStatusType,
-        "StatusReason": "InstanceStatusReasonOutputTypeDef",
-        "InboundCallsEnabled": bool,
-        "OutboundCallsEnabled": bool,
-        "InstanceAccessUrl": str,
+        "HoursOfOperationId": str,
+        "HoursOfOperationArn": str,
+        "Name": str,
+        "Description": str,
+        "TimeZone": str,
+        "Config": List["HoursOfOperationConfigOutputTypeDef"],
+        "Tags": Dict[str, str],
     },
 )
 
-InstanceStatusReasonOutputTypeDef = TypedDict(
-    "InstanceStatusReasonOutputTypeDef",
+InstanceStatusReasonTypeDef = TypedDict(
+    "InstanceStatusReasonTypeDef",
     {
         "Message": str,
     },
 )
 
 InstanceStorageConfigOutputTypeDef = TypedDict(
     "InstanceStorageConfigOutputTypeDef",
@@ -3576,32 +3559,49 @@
 )
 
 class InstanceStorageConfigTypeDef(
     _RequiredInstanceStorageConfigTypeDef, _OptionalInstanceStorageConfigTypeDef
 ):
     pass
 
-InstanceSummaryOutputTypeDef = TypedDict(
-    "InstanceSummaryOutputTypeDef",
+InstanceSummaryTypeDef = TypedDict(
+    "InstanceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "IdentityManagementType": DirectoryTypeType,
         "InstanceAlias": str,
         "CreatedTime": datetime,
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
 )
 
-IntegrationAssociationSummaryOutputTypeDef = TypedDict(
-    "IntegrationAssociationSummaryOutputTypeDef",
+InstanceTypeDef = TypedDict(
+    "InstanceTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "IdentityManagementType": DirectoryTypeType,
+        "InstanceAlias": str,
+        "CreatedTime": datetime,
+        "ServiceRole": str,
+        "InstanceStatus": InstanceStatusType,
+        "StatusReason": "InstanceStatusReasonTypeDef",
+        "InboundCallsEnabled": bool,
+        "OutboundCallsEnabled": bool,
+        "InstanceAccessUrl": str,
+    },
+)
+
+IntegrationAssociationSummaryTypeDef = TypedDict(
+    "IntegrationAssociationSummaryTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
         "SourceApplicationUrl": str,
@@ -3667,16 +3667,16 @@
     {
         "Prefix": str,
         "RetentionPeriodHours": int,
         "EncryptionConfig": "EncryptionConfigTypeDef",
     },
 )
 
-LexBotConfigOutputTypeDef = TypedDict(
-    "LexBotConfigOutputTypeDef",
+LexBotConfigTypeDef = TypedDict(
+    "LexBotConfigTypeDef",
     {
         "LexBot": "LexBotOutputTypeDef",
         "LexV2Bot": "LexV2BotOutputTypeDef",
     },
 )
 
 LexBotOutputTypeDef = TypedDict(
@@ -3748,19 +3748,19 @@
 )
 
 class ListAgentStatusRequestRequestTypeDef(
     _RequiredListAgentStatusRequestRequestTypeDef, _OptionalListAgentStatusRequestRequestTypeDef
 ):
     pass
 
-ListAgentStatusResponseOutputTypeDef = TypedDict(
-    "ListAgentStatusResponseOutputTypeDef",
+ListAgentStatusResponseTypeDef = TypedDict(
+    "ListAgentStatusResponseTypeDef",
     {
         "NextToken": str,
-        "AgentStatusSummaryList": List["AgentStatusSummaryOutputTypeDef"],
+        "AgentStatusSummaryList": List["AgentStatusSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
@@ -3798,16 +3798,16 @@
 
 class ListApprovedOriginsRequestRequestTypeDef(
     _RequiredListApprovedOriginsRequestRequestTypeDef,
     _OptionalListApprovedOriginsRequestRequestTypeDef,
 ):
     pass
 
-ListApprovedOriginsResponseOutputTypeDef = TypedDict(
-    "ListApprovedOriginsResponseOutputTypeDef",
+ListApprovedOriginsResponseTypeDef = TypedDict(
+    "ListApprovedOriginsResponseTypeDef",
     {
         "Origins": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3848,18 +3848,18 @@
 )
 
 class ListBotsRequestRequestTypeDef(
     _RequiredListBotsRequestRequestTypeDef, _OptionalListBotsRequestRequestTypeDef
 ):
     pass
 
-ListBotsResponseOutputTypeDef = TypedDict(
-    "ListBotsResponseOutputTypeDef",
+ListBotsResponseTypeDef = TypedDict(
+    "ListBotsResponseTypeDef",
     {
-        "LexBots": List["LexBotConfigOutputTypeDef"],
+        "LexBots": List["LexBotConfigTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
@@ -3899,18 +3899,18 @@
 
 class ListContactEvaluationsRequestRequestTypeDef(
     _RequiredListContactEvaluationsRequestRequestTypeDef,
     _OptionalListContactEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-ListContactEvaluationsResponseOutputTypeDef = TypedDict(
-    "ListContactEvaluationsResponseOutputTypeDef",
+ListContactEvaluationsResponseTypeDef = TypedDict(
+    "ListContactEvaluationsResponseTypeDef",
     {
-        "EvaluationSummaryList": List["EvaluationSummaryOutputTypeDef"],
+        "EvaluationSummaryList": List["EvaluationSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
@@ -3951,18 +3951,18 @@
 
 class ListContactFlowModulesRequestRequestTypeDef(
     _RequiredListContactFlowModulesRequestRequestTypeDef,
     _OptionalListContactFlowModulesRequestRequestTypeDef,
 ):
     pass
 
-ListContactFlowModulesResponseOutputTypeDef = TypedDict(
-    "ListContactFlowModulesResponseOutputTypeDef",
+ListContactFlowModulesResponseTypeDef = TypedDict(
+    "ListContactFlowModulesResponseTypeDef",
     {
-        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryOutputTypeDef"],
+        "ContactFlowModulesSummaryList": List["ContactFlowModuleSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef",
@@ -4002,18 +4002,18 @@
 )
 
 class ListContactFlowsRequestRequestTypeDef(
     _RequiredListContactFlowsRequestRequestTypeDef, _OptionalListContactFlowsRequestRequestTypeDef
 ):
     pass
 
-ListContactFlowsResponseOutputTypeDef = TypedDict(
-    "ListContactFlowsResponseOutputTypeDef",
+ListContactFlowsResponseTypeDef = TypedDict(
+    "ListContactFlowsResponseTypeDef",
     {
-        "ContactFlowSummaryList": List["ContactFlowSummaryOutputTypeDef"],
+        "ContactFlowSummaryList": List["ContactFlowSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef",
@@ -4055,18 +4055,18 @@
 
 class ListContactReferencesRequestRequestTypeDef(
     _RequiredListContactReferencesRequestRequestTypeDef,
     _OptionalListContactReferencesRequestRequestTypeDef,
 ):
     pass
 
-ListContactReferencesResponseOutputTypeDef = TypedDict(
-    "ListContactReferencesResponseOutputTypeDef",
+ListContactReferencesResponseTypeDef = TypedDict(
+    "ListContactReferencesResponseTypeDef",
     {
-        "ReferenceSummaryList": List["ReferenceSummaryOutputTypeDef"],
+        "ReferenceSummaryList": List["ReferenceSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
@@ -4107,18 +4107,18 @@
 
 class ListDefaultVocabulariesRequestRequestTypeDef(
     _RequiredListDefaultVocabulariesRequestRequestTypeDef,
     _OptionalListDefaultVocabulariesRequestRequestTypeDef,
 ):
     pass
 
-ListDefaultVocabulariesResponseOutputTypeDef = TypedDict(
-    "ListDefaultVocabulariesResponseOutputTypeDef",
+ListDefaultVocabulariesResponseTypeDef = TypedDict(
+    "ListDefaultVocabulariesResponseTypeDef",
     {
-        "DefaultVocabularyList": List["DefaultVocabularyOutputTypeDef"],
+        "DefaultVocabularyList": List["DefaultVocabularyTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
@@ -4159,18 +4159,18 @@
 
 class ListEvaluationFormVersionsRequestRequestTypeDef(
     _RequiredListEvaluationFormVersionsRequestRequestTypeDef,
     _OptionalListEvaluationFormVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListEvaluationFormVersionsResponseOutputTypeDef = TypedDict(
-    "ListEvaluationFormVersionsResponseOutputTypeDef",
+ListEvaluationFormVersionsResponseTypeDef = TypedDict(
+    "ListEvaluationFormVersionsResponseTypeDef",
     {
-        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryOutputTypeDef"],
+        "EvaluationFormVersionSummaryList": List["EvaluationFormVersionSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
@@ -4209,18 +4209,18 @@
 
 class ListEvaluationFormsRequestRequestTypeDef(
     _RequiredListEvaluationFormsRequestRequestTypeDef,
     _OptionalListEvaluationFormsRequestRequestTypeDef,
 ):
     pass
 
-ListEvaluationFormsResponseOutputTypeDef = TypedDict(
-    "ListEvaluationFormsResponseOutputTypeDef",
+ListEvaluationFormsResponseTypeDef = TypedDict(
+    "ListEvaluationFormsResponseTypeDef",
     {
-        "EvaluationFormSummaryList": List["EvaluationFormSummaryOutputTypeDef"],
+        "EvaluationFormSummaryList": List["EvaluationFormSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
@@ -4259,18 +4259,18 @@
 
 class ListHoursOfOperationsRequestRequestTypeDef(
     _RequiredListHoursOfOperationsRequestRequestTypeDef,
     _OptionalListHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
-ListHoursOfOperationsResponseOutputTypeDef = TypedDict(
-    "ListHoursOfOperationsResponseOutputTypeDef",
+ListHoursOfOperationsResponseTypeDef = TypedDict(
+    "ListHoursOfOperationsResponseTypeDef",
     {
-        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryOutputTypeDef"],
+        "HoursOfOperationSummaryList": List["HoursOfOperationSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
@@ -4309,18 +4309,18 @@
 
 class ListInstanceAttributesRequestRequestTypeDef(
     _RequiredListInstanceAttributesRequestRequestTypeDef,
     _OptionalListInstanceAttributesRequestRequestTypeDef,
 ):
     pass
 
-ListInstanceAttributesResponseOutputTypeDef = TypedDict(
-    "ListInstanceAttributesResponseOutputTypeDef",
+ListInstanceAttributesResponseTypeDef = TypedDict(
+    "ListInstanceAttributesResponseTypeDef",
     {
-        "Attributes": List["AttributeOutputTypeDef"],
+        "Attributes": List["AttributeTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
@@ -4361,16 +4361,16 @@
 
 class ListInstanceStorageConfigsRequestRequestTypeDef(
     _RequiredListInstanceStorageConfigsRequestRequestTypeDef,
     _OptionalListInstanceStorageConfigsRequestRequestTypeDef,
 ):
     pass
 
-ListInstanceStorageConfigsResponseOutputTypeDef = TypedDict(
-    "ListInstanceStorageConfigsResponseOutputTypeDef",
+ListInstanceStorageConfigsResponseTypeDef = TypedDict(
+    "ListInstanceStorageConfigsResponseTypeDef",
     {
         "StorageConfigs": List["InstanceStorageConfigOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4387,18 +4387,18 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListInstancesResponseOutputTypeDef = TypedDict(
-    "ListInstancesResponseOutputTypeDef",
+ListInstancesResponseTypeDef = TypedDict(
+    "ListInstancesResponseTypeDef",
     {
-        "InstanceSummaryList": List["InstanceSummaryOutputTypeDef"],
+        "InstanceSummaryList": List["InstanceSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef",
@@ -4439,18 +4439,18 @@
 
 class ListIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-ListIntegrationAssociationsResponseOutputTypeDef = TypedDict(
-    "ListIntegrationAssociationsResponseOutputTypeDef",
+ListIntegrationAssociationsResponseTypeDef = TypedDict(
+    "ListIntegrationAssociationsResponseTypeDef",
     {
-        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryOutputTypeDef"],
+        "IntegrationAssociationSummaryList": List["IntegrationAssociationSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
@@ -4489,16 +4489,16 @@
 
 class ListLambdaFunctionsRequestRequestTypeDef(
     _RequiredListLambdaFunctionsRequestRequestTypeDef,
     _OptionalListLambdaFunctionsRequestRequestTypeDef,
 ):
     pass
 
-ListLambdaFunctionsResponseOutputTypeDef = TypedDict(
-    "ListLambdaFunctionsResponseOutputTypeDef",
+ListLambdaFunctionsResponseTypeDef = TypedDict(
+    "ListLambdaFunctionsResponseTypeDef",
     {
         "LambdaFunctions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4538,16 +4538,16 @@
 )
 
 class ListLexBotsRequestRequestTypeDef(
     _RequiredListLexBotsRequestRequestTypeDef, _OptionalListLexBotsRequestRequestTypeDef
 ):
     pass
 
-ListLexBotsResponseOutputTypeDef = TypedDict(
-    "ListLexBotsResponseOutputTypeDef",
+ListLexBotsResponseTypeDef = TypedDict(
+    "ListLexBotsResponseTypeDef",
     {
         "LexBots": List["LexBotOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4591,25 +4591,25 @@
 )
 
 class ListPhoneNumbersRequestRequestTypeDef(
     _RequiredListPhoneNumbersRequestRequestTypeDef, _OptionalListPhoneNumbersRequestRequestTypeDef
 ):
     pass
 
-ListPhoneNumbersResponseOutputTypeDef = TypedDict(
-    "ListPhoneNumbersResponseOutputTypeDef",
+ListPhoneNumbersResponseTypeDef = TypedDict(
+    "ListPhoneNumbersResponseTypeDef",
     {
-        "PhoneNumberSummaryList": List["PhoneNumberSummaryOutputTypeDef"],
+        "PhoneNumberSummaryList": List["PhoneNumberSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPhoneNumbersSummaryOutputTypeDef = TypedDict(
-    "ListPhoneNumbersSummaryOutputTypeDef",
+ListPhoneNumbersSummaryTypeDef = TypedDict(
+    "ListPhoneNumbersSummaryTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": str,
@@ -4637,19 +4637,19 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberPrefix": str,
     },
     total=False,
 )
 
-ListPhoneNumbersV2ResponseOutputTypeDef = TypedDict(
-    "ListPhoneNumbersV2ResponseOutputTypeDef",
+ListPhoneNumbersV2ResponseTypeDef = TypedDict(
+    "ListPhoneNumbersV2ResponseTypeDef",
     {
         "NextToken": str,
-        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryOutputTypeDef"],
+        "ListPhoneNumbersSummaryList": List["ListPhoneNumbersSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPromptsRequestListPromptsPaginateTypeDef = TypedDict(
     "_RequiredListPromptsRequestListPromptsPaginateTypeDef",
     {
@@ -4686,18 +4686,18 @@
 )
 
 class ListPromptsRequestRequestTypeDef(
     _RequiredListPromptsRequestRequestTypeDef, _OptionalListPromptsRequestRequestTypeDef
 ):
     pass
 
-ListPromptsResponseOutputTypeDef = TypedDict(
-    "ListPromptsResponseOutputTypeDef",
+ListPromptsResponseTypeDef = TypedDict(
+    "ListPromptsResponseTypeDef",
     {
-        "PromptSummaryList": List["PromptSummaryOutputTypeDef"],
+        "PromptSummaryList": List["PromptSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
@@ -4738,19 +4738,19 @@
 
 class ListQueueQuickConnectsRequestRequestTypeDef(
     _RequiredListQueueQuickConnectsRequestRequestTypeDef,
     _OptionalListQueueQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
-ListQueueQuickConnectsResponseOutputTypeDef = TypedDict(
-    "ListQueueQuickConnectsResponseOutputTypeDef",
+ListQueueQuickConnectsResponseTypeDef = TypedDict(
+    "ListQueueQuickConnectsResponseTypeDef",
     {
         "NextToken": str,
-        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
     "_RequiredListQueuesRequestListQueuesPaginateTypeDef",
     {
@@ -4789,18 +4789,18 @@
 )
 
 class ListQueuesRequestRequestTypeDef(
     _RequiredListQueuesRequestRequestTypeDef, _OptionalListQueuesRequestRequestTypeDef
 ):
     pass
 
-ListQueuesResponseOutputTypeDef = TypedDict(
-    "ListQueuesResponseOutputTypeDef",
+ListQueuesResponseTypeDef = TypedDict(
+    "ListQueuesResponseTypeDef",
     {
-        "QueueSummaryList": List["QueueSummaryOutputTypeDef"],
+        "QueueSummaryList": List["QueueSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
@@ -4840,18 +4840,18 @@
 )
 
 class ListQuickConnectsRequestRequestTypeDef(
     _RequiredListQuickConnectsRequestRequestTypeDef, _OptionalListQuickConnectsRequestRequestTypeDef
 ):
     pass
 
-ListQuickConnectsResponseOutputTypeDef = TypedDict(
-    "ListQuickConnectsResponseOutputTypeDef",
+ListQuickConnectsResponseTypeDef = TypedDict(
+    "ListQuickConnectsResponseTypeDef",
     {
-        "QuickConnectSummaryList": List["QuickConnectSummaryOutputTypeDef"],
+        "QuickConnectSummaryList": List["QuickConnectSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
@@ -4892,21 +4892,19 @@
 
 class ListRoutingProfileQueuesRequestRequestTypeDef(
     _RequiredListRoutingProfileQueuesRequestRequestTypeDef,
     _OptionalListRoutingProfileQueuesRequestRequestTypeDef,
 ):
     pass
 
-ListRoutingProfileQueuesResponseOutputTypeDef = TypedDict(
-    "ListRoutingProfileQueuesResponseOutputTypeDef",
+ListRoutingProfileQueuesResponseTypeDef = TypedDict(
+    "ListRoutingProfileQueuesResponseTypeDef",
     {
         "NextToken": str,
-        "RoutingProfileQueueConfigSummaryList": List[
-            "RoutingProfileQueueConfigSummaryOutputTypeDef"
-        ],
+        "RoutingProfileQueueConfigSummaryList": List["RoutingProfileQueueConfigSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
@@ -4944,18 +4942,18 @@
 
 class ListRoutingProfilesRequestRequestTypeDef(
     _RequiredListRoutingProfilesRequestRequestTypeDef,
     _OptionalListRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListRoutingProfilesResponseOutputTypeDef = TypedDict(
-    "ListRoutingProfilesResponseOutputTypeDef",
+ListRoutingProfilesResponseTypeDef = TypedDict(
+    "ListRoutingProfilesResponseTypeDef",
     {
-        "RoutingProfileSummaryList": List["RoutingProfileSummaryOutputTypeDef"],
+        "RoutingProfileSummaryList": List["RoutingProfileSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
@@ -4997,18 +4995,18 @@
 )
 
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
-ListRulesResponseOutputTypeDef = TypedDict(
-    "ListRulesResponseOutputTypeDef",
+ListRulesResponseTypeDef = TypedDict(
+    "ListRulesResponseTypeDef",
     {
-        "RuleSummaryList": List["RuleSummaryOutputTypeDef"],
+        "RuleSummaryList": List["RuleSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
@@ -5046,18 +5044,18 @@
 )
 
 class ListSecurityKeysRequestRequestTypeDef(
     _RequiredListSecurityKeysRequestRequestTypeDef, _OptionalListSecurityKeysRequestRequestTypeDef
 ):
     pass
 
-ListSecurityKeysResponseOutputTypeDef = TypedDict(
-    "ListSecurityKeysResponseOutputTypeDef",
+ListSecurityKeysResponseTypeDef = TypedDict(
+    "ListSecurityKeysResponseTypeDef",
     {
-        "SecurityKeys": List["SecurityKeyOutputTypeDef"],
+        "SecurityKeys": List["SecurityKeyTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
@@ -5098,16 +5096,16 @@
 
 class ListSecurityProfilePermissionsRequestRequestTypeDef(
     _RequiredListSecurityProfilePermissionsRequestRequestTypeDef,
     _OptionalListSecurityProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
-ListSecurityProfilePermissionsResponseOutputTypeDef = TypedDict(
-    "ListSecurityProfilePermissionsResponseOutputTypeDef",
+ListSecurityProfilePermissionsResponseTypeDef = TypedDict(
+    "ListSecurityProfilePermissionsResponseTypeDef",
     {
         "Permissions": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -5148,32 +5146,32 @@
 
 class ListSecurityProfilesRequestRequestTypeDef(
     _RequiredListSecurityProfilesRequestRequestTypeDef,
     _OptionalListSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListSecurityProfilesResponseOutputTypeDef = TypedDict(
-    "ListSecurityProfilesResponseOutputTypeDef",
+ListSecurityProfilesResponseTypeDef = TypedDict(
+    "ListSecurityProfilesResponseTypeDef",
     {
-        "SecurityProfileSummaryList": List["SecurityProfileSummaryOutputTypeDef"],
+        "SecurityProfileSummaryList": List["SecurityProfileSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
@@ -5216,18 +5214,18 @@
 )
 
 class ListTaskTemplatesRequestRequestTypeDef(
     _RequiredListTaskTemplatesRequestRequestTypeDef, _OptionalListTaskTemplatesRequestRequestTypeDef
 ):
     pass
 
-ListTaskTemplatesResponseOutputTypeDef = TypedDict(
-    "ListTaskTemplatesResponseOutputTypeDef",
+ListTaskTemplatesResponseTypeDef = TypedDict(
+    "ListTaskTemplatesResponseTypeDef",
     {
-        "TaskTemplates": List["TaskTemplateMetadataOutputTypeDef"],
+        "TaskTemplates": List["TaskTemplateMetadataTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef = TypedDict(
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
@@ -5244,19 +5242,19 @@
         "MaxResults": int,
         "NextToken": str,
         "InstanceId": str,
     },
     total=False,
 )
 
-ListTrafficDistributionGroupsResponseOutputTypeDef = TypedDict(
-    "ListTrafficDistributionGroupsResponseOutputTypeDef",
+ListTrafficDistributionGroupsResponseTypeDef = TypedDict(
+    "ListTrafficDistributionGroupsResponseTypeDef",
     {
         "NextToken": str,
-        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryOutputTypeDef"],
+        "TrafficDistributionGroupSummaryList": List["TrafficDistributionGroupSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUseCasesRequestListUseCasesPaginateTypeDef = TypedDict(
     "_RequiredListUseCasesRequestListUseCasesPaginateTypeDef",
     {
@@ -5295,18 +5293,18 @@
 )
 
 class ListUseCasesRequestRequestTypeDef(
     _RequiredListUseCasesRequestRequestTypeDef, _OptionalListUseCasesRequestRequestTypeDef
 ):
     pass
 
-ListUseCasesResponseOutputTypeDef = TypedDict(
-    "ListUseCasesResponseOutputTypeDef",
+ListUseCasesResponseTypeDef = TypedDict(
+    "ListUseCasesResponseTypeDef",
     {
-        "UseCaseSummaryList": List["UseCaseOutputTypeDef"],
+        "UseCaseSummaryList": List["UseCaseTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
@@ -5345,18 +5343,18 @@
 
 class ListUserHierarchyGroupsRequestRequestTypeDef(
     _RequiredListUserHierarchyGroupsRequestRequestTypeDef,
     _OptionalListUserHierarchyGroupsRequestRequestTypeDef,
 ):
     pass
 
-ListUserHierarchyGroupsResponseOutputTypeDef = TypedDict(
-    "ListUserHierarchyGroupsResponseOutputTypeDef",
+ListUserHierarchyGroupsResponseTypeDef = TypedDict(
+    "ListUserHierarchyGroupsResponseTypeDef",
     {
-        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryOutputTypeDef"],
+        "UserHierarchyGroupSummaryList": List["HierarchyGroupSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
@@ -5394,18 +5392,18 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-ListUsersResponseOutputTypeDef = TypedDict(
-    "ListUsersResponseOutputTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "UserSummaryList": List["UserSummaryOutputTypeDef"],
+        "UserSummaryList": List["UserSummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaConcurrencyOutputTypeDef = TypedDict(
     "MediaConcurrencyOutputTypeDef",
@@ -5430,16 +5428,16 @@
     },
     total=False,
 )
 
 class MediaConcurrencyTypeDef(_RequiredMediaConcurrencyTypeDef, _OptionalMediaConcurrencyTypeDef):
     pass
 
-MetricDataV2OutputTypeDef = TypedDict(
-    "MetricDataV2OutputTypeDef",
+MetricDataV2TypeDef = TypedDict(
+    "MetricDataV2TypeDef",
     {
         "Metric": "MetricV2OutputTypeDef",
         "Value": float,
     },
 )
 
 MetricFilterV2OutputTypeDef = TypedDict(
@@ -5455,19 +5453,19 @@
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
     },
     total=False,
 )
 
-MetricResultV2OutputTypeDef = TypedDict(
-    "MetricResultV2OutputTypeDef",
+MetricResultV2TypeDef = TypedDict(
+    "MetricResultV2TypeDef",
     {
         "Dimensions": Dict[str, str],
-        "Collections": List["MetricDataV2OutputTypeDef"],
+        "Collections": List["MetricDataV2TypeDef"],
     },
 )
 
 MetricV2OutputTypeDef = TypedDict(
     "MetricV2OutputTypeDef",
     {
         "Name": str,
@@ -5504,16 +5502,16 @@
 )
 
 class MonitorContactRequestRequestTypeDef(
     _RequiredMonitorContactRequestRequestTypeDef, _OptionalMonitorContactRequestRequestTypeDef
 ):
     pass
 
-MonitorContactResponseOutputTypeDef = TypedDict(
-    "MonitorContactResponseOutputTypeDef",
+MonitorContactResponseTypeDef = TypedDict(
+    "MonitorContactResponseTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -5530,16 +5528,16 @@
     {
         "UserTags": Mapping[str, str],
         "UserIds": Sequence[str],
     },
     total=False,
 )
 
-NumberReferenceOutputTypeDef = TypedDict(
-    "NumberReferenceOutputTypeDef",
+NumberReferenceTypeDef = TypedDict(
+    "NumberReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 NumericQuestionPropertyValueAutomationOutputTypeDef = TypedDict(
@@ -5615,16 +5613,16 @@
     {
         "ParticipantTimerAction": Literal["Unset"],
         "ParticipantTimerDurationInMinutes": int,
     },
     total=False,
 )
 
-ParticipantTokenCredentialsOutputTypeDef = TypedDict(
-    "ParticipantTokenCredentialsOutputTypeDef",
+ParticipantTokenCredentialsTypeDef = TypedDict(
+    "ParticipantTokenCredentialsTypeDef",
     {
         "ParticipantToken": str,
         "Expiry": str,
     },
 )
 
 PersistentChatTypeDef = TypedDict(
@@ -5646,44 +5644,33 @@
 PhoneNumberQuickConnectConfigTypeDef = TypedDict(
     "PhoneNumberQuickConnectConfigTypeDef",
     {
         "PhoneNumber": str,
     },
 )
 
-PhoneNumberStatusOutputTypeDef = TypedDict(
-    "PhoneNumberStatusOutputTypeDef",
+PhoneNumberStatusTypeDef = TypedDict(
+    "PhoneNumberStatusTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
 )
 
-PhoneNumberSummaryOutputTypeDef = TypedDict(
-    "PhoneNumberSummaryOutputTypeDef",
+PhoneNumberSummaryTypeDef = TypedDict(
+    "PhoneNumberSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
     },
 )
 
-PromptOutputTypeDef = TypedDict(
-    "PromptOutputTypeDef",
-    {
-        "PromptARN": str,
-        "PromptId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 PromptSearchCriteriaTypeDef = TypedDict(
     "PromptSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -5694,55 +5681,51 @@
     "PromptSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-PromptSummaryOutputTypeDef = TypedDict(
-    "PromptSummaryOutputTypeDef",
+PromptSummaryTypeDef = TypedDict(
+    "PromptSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+PromptTypeDef = TypedDict(
+    "PromptTypeDef",
+    {
+        "PromptARN": str,
+        "PromptId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+    },
+)
+
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
         "AgentStatusId": str,
     },
 )
 
-QueueInfoOutputTypeDef = TypedDict(
-    "QueueInfoOutputTypeDef",
+QueueInfoTypeDef = TypedDict(
+    "QueueInfoTypeDef",
     {
         "Id": str,
         "EnqueueTimestamp": datetime,
     },
 )
 
-QueueOutputTypeDef = TypedDict(
-    "QueueOutputTypeDef",
-    {
-        "Name": str,
-        "QueueArn": str,
-        "QueueId": str,
-        "Description": str,
-        "OutboundCallerConfig": "OutboundCallerConfigOutputTypeDef",
-        "HoursOfOperationId": str,
-        "MaxContacts": int,
-        "Status": QueueStatusType,
-        "Tags": Dict[str, str],
-    },
-)
-
 QueueQuickConnectConfigOutputTypeDef = TypedDict(
     "QueueQuickConnectConfigOutputTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
     },
 )
@@ -5751,16 +5734,16 @@
     "QueueQuickConnectConfigTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
     },
 )
 
-QueueReferenceOutputTypeDef = TypedDict(
-    "QueueReferenceOutputTypeDef",
+QueueReferenceTypeDef = TypedDict(
+    "QueueReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 QueueSearchCriteriaTypeDef = TypedDict(
@@ -5778,24 +5761,39 @@
     "QueueSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QueueSummaryOutputTypeDef = TypedDict(
-    "QueueSummaryOutputTypeDef",
+QueueSummaryTypeDef = TypedDict(
+    "QueueSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
     },
 )
 
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
+    {
+        "Name": str,
+        "QueueArn": str,
+        "QueueId": str,
+        "Description": str,
+        "OutboundCallerConfig": "OutboundCallerConfigOutputTypeDef",
+        "HoursOfOperationId": str,
+        "MaxContacts": int,
+        "Status": QueueStatusType,
+        "Tags": Dict[str, str],
+    },
+)
+
 QuickConnectConfigOutputTypeDef = TypedDict(
     "QuickConnectConfigOutputTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
         "UserConfig": "UserQuickConnectConfigOutputTypeDef",
         "QueueConfig": "QueueQuickConnectConfigOutputTypeDef",
         "PhoneConfig": "PhoneNumberQuickConnectConfigOutputTypeDef",
@@ -5819,26 +5817,14 @@
 )
 
 class QuickConnectConfigTypeDef(
     _RequiredQuickConnectConfigTypeDef, _OptionalQuickConnectConfigTypeDef
 ):
     pass
 
-QuickConnectOutputTypeDef = TypedDict(
-    "QuickConnectOutputTypeDef",
-    {
-        "QuickConnectARN": str,
-        "QuickConnectId": str,
-        "Name": str,
-        "Description": str,
-        "QuickConnectConfig": "QuickConnectConfigOutputTypeDef",
-        "Tags": Dict[str, str],
-    },
-)
-
 QuickConnectSearchCriteriaTypeDef = TypedDict(
     "QuickConnectSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
@@ -5849,24 +5835,36 @@
     "QuickConnectSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-QuickConnectSummaryOutputTypeDef = TypedDict(
-    "QuickConnectSummaryOutputTypeDef",
+QuickConnectSummaryTypeDef = TypedDict(
+    "QuickConnectSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
     },
 )
 
+QuickConnectTypeDef = TypedDict(
+    "QuickConnectTypeDef",
+    {
+        "QuickConnectARN": str,
+        "QuickConnectId": str,
+        "Name": str,
+        "Description": str,
+        "QuickConnectConfig": "QuickConnectConfigOutputTypeDef",
+        "Tags": Dict[str, str],
+    },
+)
+
 ReadOnlyFieldInfoOutputTypeDef = TypedDict(
     "ReadOnlyFieldInfoOutputTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierOutputTypeDef",
     },
 )
 
@@ -5882,23 +5880,23 @@
     "ReferenceOutputTypeDef",
     {
         "Value": str,
         "Type": ReferenceTypeType,
     },
 )
 
-ReferenceSummaryOutputTypeDef = TypedDict(
-    "ReferenceSummaryOutputTypeDef",
+ReferenceSummaryTypeDef = TypedDict(
+    "ReferenceSummaryTypeDef",
     {
-        "Url": "UrlReferenceOutputTypeDef",
-        "Attachment": "AttachmentReferenceOutputTypeDef",
-        "String": "StringReferenceOutputTypeDef",
-        "Number": "NumberReferenceOutputTypeDef",
-        "Date": "DateReferenceOutputTypeDef",
-        "Email": "EmailReferenceOutputTypeDef",
+        "Url": "UrlReferenceTypeDef",
+        "Attachment": "AttachmentReferenceTypeDef",
+        "String": "StringReferenceTypeDef",
+        "Number": "NumberReferenceTypeDef",
+        "Date": "DateReferenceTypeDef",
+        "Email": "EmailReferenceTypeDef",
     },
 )
 
 ReferenceTypeDef = TypedDict(
     "ReferenceTypeDef",
     {
         "Value": str,
@@ -5943,16 +5941,16 @@
 )
 
 class ReplicateInstanceRequestRequestTypeDef(
     _RequiredReplicateInstanceRequestRequestTypeDef, _OptionalReplicateInstanceRequestRequestTypeDef
 ):
     pass
 
-ReplicateInstanceResponseOutputTypeDef = TypedDict(
-    "ReplicateInstanceResponseOutputTypeDef",
+ReplicateInstanceResponseTypeDef = TypedDict(
+    "ReplicateInstanceResponseTypeDef",
     {
         "Id": str,
         "Arn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -5995,32 +5993,16 @@
     {
         "InstanceId": str,
         "ContactId": str,
         "InitialContactId": str,
     },
 )
 
-RoutingProfileOutputTypeDef = TypedDict(
-    "RoutingProfileOutputTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "RoutingProfileArn": str,
-        "RoutingProfileId": str,
-        "Description": str,
-        "MediaConcurrencies": List["MediaConcurrencyOutputTypeDef"],
-        "DefaultOutboundQueueId": str,
-        "Tags": Dict[str, str],
-        "NumberOfAssociatedQueues": int,
-        "NumberOfAssociatedUsers": int,
-    },
-)
-
-RoutingProfileQueueConfigSummaryOutputTypeDef = TypedDict(
-    "RoutingProfileQueueConfigSummaryOutputTypeDef",
+RoutingProfileQueueConfigSummaryTypeDef = TypedDict(
+    "RoutingProfileQueueConfigSummaryTypeDef",
     {
         "QueueId": str,
         "QueueArn": str,
         "QueueName": str,
         "Priority": int,
         "Delay": int,
         "Channel": ChannelType,
@@ -6040,16 +6022,16 @@
     "RoutingProfileQueueReferenceTypeDef",
     {
         "QueueId": str,
         "Channel": ChannelType,
     },
 )
 
-RoutingProfileReferenceOutputTypeDef = TypedDict(
-    "RoutingProfileReferenceOutputTypeDef",
+RoutingProfileReferenceTypeDef = TypedDict(
+    "RoutingProfileReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 RoutingProfileSearchCriteriaTypeDef = TypedDict(
@@ -6066,23 +6048,39 @@
     "RoutingProfileSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-RoutingProfileSummaryOutputTypeDef = TypedDict(
-    "RoutingProfileSummaryOutputTypeDef",
+RoutingProfileSummaryTypeDef = TypedDict(
+    "RoutingProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+RoutingProfileTypeDef = TypedDict(
+    "RoutingProfileTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "RoutingProfileArn": str,
+        "RoutingProfileId": str,
+        "Description": str,
+        "MediaConcurrencies": List["MediaConcurrencyOutputTypeDef"],
+        "DefaultOutboundQueueId": str,
+        "Tags": Dict[str, str],
+        "NumberOfAssociatedQueues": int,
+        "NumberOfAssociatedUsers": int,
+    },
+)
+
 RuleActionOutputTypeDef = TypedDict(
     "RuleActionOutputTypeDef",
     {
         "ActionType": ActionTypeType,
         "TaskAction": "TaskActionDefinitionOutputTypeDef",
         "EventBridgeAction": "EventBridgeActionDefinitionOutputTypeDef",
         "AssignContactCategoryAction": Dict[str, Any],
@@ -6106,40 +6104,23 @@
     },
     total=False,
 )
 
 class RuleActionTypeDef(_RequiredRuleActionTypeDef, _OptionalRuleActionTypeDef):
     pass
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "Name": str,
-        "RuleId": str,
-        "RuleArn": str,
-        "TriggerEventSource": "RuleTriggerEventSourceOutputTypeDef",
-        "Function": str,
-        "Actions": List["RuleActionOutputTypeDef"],
-        "PublishStatus": RulePublishStatusType,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "LastUpdatedBy": str,
-        "Tags": Dict[str, str],
-    },
-)
-
-RuleSummaryOutputTypeDef = TypedDict(
-    "RuleSummaryOutputTypeDef",
+RuleSummaryTypeDef = TypedDict(
+    "RuleSummaryTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "EventSourceName": EventSourceNameType,
         "PublishStatus": RulePublishStatusType,
-        "ActionSummaries": List["ActionSummaryOutputTypeDef"],
+        "ActionSummaries": List["ActionSummaryTypeDef"],
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
     },
 )
 
 RuleTriggerEventSourceOutputTypeDef = TypedDict(
     "RuleTriggerEventSourceOutputTypeDef",
@@ -6164,14 +6145,31 @@
 )
 
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "Name": str,
+        "RuleId": str,
+        "RuleArn": str,
+        "TriggerEventSource": "RuleTriggerEventSourceOutputTypeDef",
+        "Function": str,
+        "Actions": List["RuleActionOutputTypeDef"],
+        "PublishStatus": RulePublishStatusType,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "LastUpdatedBy": str,
+        "Tags": Dict[str, str],
+    },
+)
+
 S3ConfigOutputTypeDef = TypedDict(
     "S3ConfigOutputTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "EncryptionConfig": "EncryptionConfigOutputTypeDef",
     },
@@ -6238,19 +6236,19 @@
 
 class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
 ):
     pass
 
-SearchAvailablePhoneNumbersResponseOutputTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseOutputTypeDef",
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     {
         "NextToken": str,
-        "AvailableNumbersList": List["AvailableNumberSummaryOutputTypeDef"],
+        "AvailableNumbersList": List["AvailableNumberSummaryTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestRequestTypeDef",
     {
@@ -6292,18 +6290,18 @@
 
 class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(
     _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
     _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
-SearchHoursOfOperationsResponseOutputTypeDef = TypedDict(
-    "SearchHoursOfOperationsResponseOutputTypeDef",
+SearchHoursOfOperationsResponseTypeDef = TypedDict(
+    "SearchHoursOfOperationsResponseTypeDef",
     {
-        "HoursOfOperations": List["HoursOfOperationOutputTypeDef"],
+        "HoursOfOperations": List["HoursOfOperationTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchPromptsRequestRequestTypeDef = TypedDict(
@@ -6346,18 +6344,18 @@
 
 class SearchPromptsRequestSearchPromptsPaginateTypeDef(
     _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef,
     _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef,
 ):
     pass
 
-SearchPromptsResponseOutputTypeDef = TypedDict(
-    "SearchPromptsResponseOutputTypeDef",
+SearchPromptsResponseTypeDef = TypedDict(
+    "SearchPromptsResponseTypeDef",
     {
-        "Prompts": List["PromptOutputTypeDef"],
+        "Prompts": List["PromptTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQueuesRequestRequestTypeDef = TypedDict(
@@ -6400,18 +6398,18 @@
 
 class SearchQueuesRequestSearchQueuesPaginateTypeDef(
     _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef,
     _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef,
 ):
     pass
 
-SearchQueuesResponseOutputTypeDef = TypedDict(
-    "SearchQueuesResponseOutputTypeDef",
+SearchQueuesResponseTypeDef = TypedDict(
+    "SearchQueuesResponseTypeDef",
     {
-        "Queues": List["QueueOutputTypeDef"],
+        "Queues": List["QueueTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -6455,18 +6453,18 @@
 
 class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(
     _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
     _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
 ):
     pass
 
-SearchQuickConnectsResponseOutputTypeDef = TypedDict(
-    "SearchQuickConnectsResponseOutputTypeDef",
+SearchQuickConnectsResponseTypeDef = TypedDict(
+    "SearchQuickConnectsResponseTypeDef",
     {
-        "QuickConnects": List["QuickConnectOutputTypeDef"],
+        "QuickConnects": List["QuickConnectTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchResourceTagsRequestRequestTypeDef = TypedDict(
@@ -6510,18 +6508,18 @@
 
 class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(
     _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
     _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
 ):
     pass
 
-SearchResourceTagsResponseOutputTypeDef = TypedDict(
-    "SearchResourceTagsResponseOutputTypeDef",
+SearchResourceTagsResponseTypeDef = TypedDict(
+    "SearchResourceTagsResponseTypeDef",
     {
-        "Tags": List["TagSetOutputTypeDef"],
+        "Tags": List["TagSetTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestRequestTypeDef",
@@ -6564,18 +6562,18 @@
 
 class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(
     _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
     _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
 ):
     pass
 
-SearchRoutingProfilesResponseOutputTypeDef = TypedDict(
-    "SearchRoutingProfilesResponseOutputTypeDef",
+SearchRoutingProfilesResponseTypeDef = TypedDict(
+    "SearchRoutingProfilesResponseTypeDef",
     {
-        "RoutingProfiles": List["RoutingProfileOutputTypeDef"],
+        "RoutingProfiles": List["RoutingProfileTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -6619,18 +6617,18 @@
 
 class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(
     _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
     _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
 ):
     pass
 
-SearchSecurityProfilesResponseOutputTypeDef = TypedDict(
-    "SearchSecurityProfilesResponseOutputTypeDef",
+SearchSecurityProfilesResponseTypeDef = TypedDict(
+    "SearchSecurityProfilesResponseTypeDef",
     {
-        "SecurityProfiles": List["SecurityProfileSearchSummaryOutputTypeDef"],
+        "SecurityProfiles": List["SecurityProfileSearchSummaryTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchUsersRequestRequestTypeDef = TypedDict(
@@ -6652,18 +6650,18 @@
         "SearchFilter": "UserSearchFilterTypeDef",
         "SearchCriteria": "UserSearchCriteriaTypeDef",
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-SearchUsersResponseOutputTypeDef = TypedDict(
-    "SearchUsersResponseOutputTypeDef",
+SearchUsersResponseTypeDef = TypedDict(
+    "SearchUsersResponseTypeDef",
     {
-        "Users": List["UserSearchSummaryOutputTypeDef"],
+        "Users": List["UserSearchSummaryTypeDef"],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchVocabulariesRequestRequestTypeDef = TypedDict(
@@ -6709,77 +6707,77 @@
 
 class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(
     _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
     _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
 ):
     pass
 
-SearchVocabulariesResponseOutputTypeDef = TypedDict(
-    "SearchVocabulariesResponseOutputTypeDef",
+SearchVocabulariesResponseTypeDef = TypedDict(
+    "SearchVocabulariesResponseTypeDef",
     {
-        "VocabularySummaryList": List["VocabularySummaryOutputTypeDef"],
+        "VocabularySummaryList": List["VocabularySummaryTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SecurityKeyOutputTypeDef = TypedDict(
-    "SecurityKeyOutputTypeDef",
+SecurityKeyTypeDef = TypedDict(
+    "SecurityKeyTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
 )
 
-SecurityProfileOutputTypeDef = TypedDict(
-    "SecurityProfileOutputTypeDef",
-    {
-        "Id": str,
-        "OrganizationResourceId": str,
-        "Arn": str,
-        "SecurityProfileName": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "AllowedAccessControlTags": Dict[str, str],
-        "TagRestrictedResources": List[str],
-    },
-)
-
 SecurityProfileSearchCriteriaTypeDef = TypedDict(
     "SecurityProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
         "StringCondition": "StringConditionTypeDef",
     },
     total=False,
 )
 
-SecurityProfileSearchSummaryOutputTypeDef = TypedDict(
-    "SecurityProfileSearchSummaryOutputTypeDef",
+SecurityProfileSearchSummaryTypeDef = TypedDict(
+    "SecurityProfileSearchSummaryTypeDef",
     {
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
 )
 
-SecurityProfileSummaryOutputTypeDef = TypedDict(
-    "SecurityProfileSummaryOutputTypeDef",
+SecurityProfileSummaryTypeDef = TypedDict(
+    "SecurityProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
 )
 
+SecurityProfileTypeDef = TypedDict(
+    "SecurityProfileTypeDef",
+    {
+        "Id": str,
+        "OrganizationResourceId": str,
+        "Arn": str,
+        "SecurityProfileName": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "AllowedAccessControlTags": Dict[str, str],
+        "TagRestrictedResources": List[str],
+    },
+)
+
 SecurityProfilesSearchFilterTypeDef = TypedDict(
     "SecurityProfilesSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
@@ -6859,16 +6857,16 @@
 )
 
 class StartChatContactRequestRequestTypeDef(
     _RequiredStartChatContactRequestRequestTypeDef, _OptionalStartChatContactRequestRequestTypeDef
 ):
     pass
 
-StartChatContactResponseOutputTypeDef = TypedDict(
-    "StartChatContactResponseOutputTypeDef",
+StartChatContactResponseTypeDef = TypedDict(
+    "StartChatContactResponseTypeDef",
     {
         "ContactId": str,
         "ParticipantId": str,
         "ParticipantToken": str,
         "ContinuedFromContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6892,16 +6890,16 @@
 
 class StartContactEvaluationRequestRequestTypeDef(
     _RequiredStartContactEvaluationRequestRequestTypeDef,
     _OptionalStartContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-StartContactEvaluationResponseOutputTypeDef = TypedDict(
-    "StartContactEvaluationResponseOutputTypeDef",
+StartContactEvaluationResponseTypeDef = TypedDict(
+    "StartContactEvaluationResponseTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -6921,16 +6919,16 @@
         "InstanceId": str,
         "ContactId": str,
         "ChatStreamingConfiguration": "ChatStreamingConfigurationTypeDef",
         "ClientToken": str,
     },
 )
 
-StartContactStreamingResponseOutputTypeDef = TypedDict(
-    "StartContactStreamingResponseOutputTypeDef",
+StartContactStreamingResponseTypeDef = TypedDict(
+    "StartContactStreamingResponseTypeDef",
     {
         "StreamingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartOutboundVoiceContactRequestRequestTypeDef = TypedDict(
@@ -6957,16 +6955,16 @@
 
 class StartOutboundVoiceContactRequestRequestTypeDef(
     _RequiredStartOutboundVoiceContactRequestRequestTypeDef,
     _OptionalStartOutboundVoiceContactRequestRequestTypeDef,
 ):
     pass
 
-StartOutboundVoiceContactResponseOutputTypeDef = TypedDict(
-    "StartOutboundVoiceContactResponseOutputTypeDef",
+StartOutboundVoiceContactResponseTypeDef = TypedDict(
+    "StartOutboundVoiceContactResponseTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTaskContactRequestRequestTypeDef = TypedDict(
@@ -6994,16 +6992,16 @@
 )
 
 class StartTaskContactRequestRequestTypeDef(
     _RequiredStartTaskContactRequestRequestTypeDef, _OptionalStartTaskContactRequestRequestTypeDef
 ):
     pass
 
-StartTaskContactResponseOutputTypeDef = TypedDict(
-    "StartTaskContactResponseOutputTypeDef",
+StartTaskContactResponseTypeDef = TypedDict(
+    "StartTaskContactResponseTypeDef",
     {
         "ContactId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopContactRecordingRequestRequestTypeDef = TypedDict(
@@ -7038,16 +7036,16 @@
         "FieldName": str,
         "Value": str,
         "ComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-StringReferenceOutputTypeDef = TypedDict(
-    "StringReferenceOutputTypeDef",
+StringReferenceTypeDef = TypedDict(
+    "StringReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
@@ -7068,16 +7066,16 @@
 
 class SubmitContactEvaluationRequestRequestTypeDef(
     _RequiredSubmitContactEvaluationRequestRequestTypeDef,
     _OptionalSubmitContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-SubmitContactEvaluationResponseOutputTypeDef = TypedDict(
-    "SubmitContactEvaluationResponseOutputTypeDef",
+SubmitContactEvaluationResponseTypeDef = TypedDict(
+    "SubmitContactEvaluationResponseTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7114,16 +7112,16 @@
         "tagValue": str,
         "tagKeyComparisonType": StringComparisonTypeType,
         "tagValueComparisonType": StringComparisonTypeType,
     },
     total=False,
 )
 
-TagSetOutputTypeDef = TypedDict(
-    "TagSetOutputTypeDef",
+TagSetTypeDef = TypedDict(
+    "TagSetTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 TaskActionDefinitionOutputTypeDef = TypedDict(
@@ -7250,16 +7248,16 @@
 )
 
 class TaskTemplateFieldTypeDef(
     _RequiredTaskTemplateFieldTypeDef, _OptionalTaskTemplateFieldTypeDef
 ):
     pass
 
-TaskTemplateMetadataOutputTypeDef = TypedDict(
-    "TaskTemplateMetadataOutputTypeDef",
+TaskTemplateMetadataTypeDef = TypedDict(
+    "TaskTemplateMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
@@ -7311,35 +7309,35 @@
     {
         "Comparison": str,
         "ThresholdValue": float,
     },
     total=False,
 )
 
-TrafficDistributionGroupOutputTypeDef = TypedDict(
-    "TrafficDistributionGroupOutputTypeDef",
+TrafficDistributionGroupSummaryTypeDef = TypedDict(
+    "TrafficDistributionGroupSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
-        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
-        "Tags": Dict[str, str],
     },
 )
 
-TrafficDistributionGroupSummaryOutputTypeDef = TypedDict(
-    "TrafficDistributionGroupSummaryOutputTypeDef",
+TrafficDistributionGroupTypeDef = TypedDict(
+    "TrafficDistributionGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
+        "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
+        "Tags": Dict[str, str],
     },
 )
 
 _RequiredTransferContactRequestRequestTypeDef = TypedDict(
     "_RequiredTransferContactRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -7358,16 +7356,16 @@
 )
 
 class TransferContactRequestRequestTypeDef(
     _RequiredTransferContactRequestRequestTypeDef, _OptionalTransferContactRequestRequestTypeDef
 ):
     pass
 
-TransferContactResponseOutputTypeDef = TypedDict(
-    "TransferContactResponseOutputTypeDef",
+TransferContactResponseTypeDef = TypedDict(
+    "TransferContactResponseTypeDef",
     {
         "ContactId": str,
         "ContactArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7430,16 +7428,16 @@
 
 class UpdateContactEvaluationRequestRequestTypeDef(
     _RequiredUpdateContactEvaluationRequestRequestTypeDef,
     _OptionalUpdateContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-UpdateContactEvaluationResponseOutputTypeDef = TypedDict(
-    "UpdateContactEvaluationResponseOutputTypeDef",
+UpdateContactEvaluationResponseTypeDef = TypedDict(
+    "UpdateContactEvaluationResponseTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7583,16 +7581,16 @@
 
 class UpdateEvaluationFormRequestRequestTypeDef(
     _RequiredUpdateEvaluationFormRequestRequestTypeDef,
     _OptionalUpdateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-UpdateEvaluationFormResponseOutputTypeDef = TypedDict(
-    "UpdateEvaluationFormResponseOutputTypeDef",
+UpdateEvaluationFormResponseTypeDef = TypedDict(
+    "UpdateEvaluationFormResponseTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "EvaluationFormVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -7673,16 +7671,16 @@
 )
 
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-UpdatePhoneNumberResponseOutputTypeDef = TypedDict(
-    "UpdatePhoneNumberResponseOutputTypeDef",
+UpdatePhoneNumberResponseTypeDef = TypedDict(
+    "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7704,16 +7702,16 @@
 )
 
 class UpdatePromptRequestRequestTypeDef(
     _RequiredUpdatePromptRequestRequestTypeDef, _OptionalUpdatePromptRequestRequestTypeDef
 ):
     pass
 
-UpdatePromptResponseOutputTypeDef = TypedDict(
-    "UpdatePromptResponseOutputTypeDef",
+UpdatePromptResponseTypeDef = TypedDict(
+    "UpdatePromptResponseTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -7925,16 +7923,16 @@
 
 class UpdateTaskTemplateRequestRequestTypeDef(
     _RequiredUpdateTaskTemplateRequestRequestTypeDef,
     _OptionalUpdateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-UpdateTaskTemplateResponseOutputTypeDef = TypedDict(
-    "UpdateTaskTemplateResponseOutputTypeDef",
+UpdateTaskTemplateResponseTypeDef = TypedDict(
+    "UpdateTaskTemplateResponseTypeDef",
     {
         "InstanceId": str,
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
@@ -8038,24 +8036,24 @@
     {
         "SecurityProfileIds": Sequence[str],
         "UserId": str,
         "InstanceId": str,
     },
 )
 
-UrlReferenceOutputTypeDef = TypedDict(
-    "UrlReferenceOutputTypeDef",
+UrlReferenceTypeDef = TypedDict(
+    "UrlReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-UseCaseOutputTypeDef = TypedDict(
-    "UseCaseOutputTypeDef",
+UseCaseTypeDef = TypedDict(
+    "UseCaseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
 )
 
@@ -8067,31 +8065,31 @@
         "RoutingProfiles": Sequence[str],
         "Agents": Sequence[str],
         "UserHierarchyGroups": Sequence[str],
     },
     total=False,
 )
 
-UserDataOutputTypeDef = TypedDict(
-    "UserDataOutputTypeDef",
+UserDataTypeDef = TypedDict(
+    "UserDataTypeDef",
     {
-        "User": "UserReferenceOutputTypeDef",
-        "RoutingProfile": "RoutingProfileReferenceOutputTypeDef",
-        "HierarchyPath": "HierarchyPathReferenceOutputTypeDef",
-        "Status": "AgentStatusReferenceOutputTypeDef",
+        "User": "UserReferenceTypeDef",
+        "RoutingProfile": "RoutingProfileReferenceTypeDef",
+        "HierarchyPath": "HierarchyPathReferenceTypeDef",
+        "Status": "AgentStatusReferenceTypeDef",
         "AvailableSlotsByChannel": Dict[ChannelType, int],
         "MaxSlotsByChannel": Dict[ChannelType, int],
         "ActiveSlotsByChannel": Dict[ChannelType, int],
-        "Contacts": List["AgentContactReferenceOutputTypeDef"],
+        "Contacts": List["AgentContactReferenceTypeDef"],
         "NextStatus": str,
     },
 )
 
-UserIdentityInfoLiteOutputTypeDef = TypedDict(
-    "UserIdentityInfoLiteOutputTypeDef",
+UserIdentityInfoLiteTypeDef = TypedDict(
+    "UserIdentityInfoLiteTypeDef",
     {
         "FirstName": str,
         "LastName": str,
     },
 )
 
 UserIdentityInfoOutputTypeDef = TypedDict(
@@ -8113,30 +8111,14 @@
         "Email": str,
         "SecondaryEmail": str,
         "Mobile": str,
     },
     total=False,
 )
 
-UserOutputTypeDef = TypedDict(
-    "UserOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Username": str,
-        "IdentityInfo": "UserIdentityInfoOutputTypeDef",
-        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
-        "DirectoryUserId": str,
-        "SecurityProfileIds": List[str],
-        "RoutingProfileId": str,
-        "HierarchyGroupId": str,
-        "Tags": Dict[str, str],
-    },
-)
-
 UserPhoneConfigOutputTypeDef = TypedDict(
     "UserPhoneConfigOutputTypeDef",
     {
         "PhoneType": PhoneTypeType,
         "AutoAccept": bool,
         "AfterContactWorkTimeLimit": int,
         "DeskPhoneNumber": str,
@@ -8174,16 +8156,16 @@
     "UserQuickConnectConfigTypeDef",
     {
         "UserId": str,
         "ContactFlowId": str,
     },
 )
 
-UserReferenceOutputTypeDef = TypedDict(
-    "UserReferenceOutputTypeDef",
+UserReferenceTypeDef = TypedDict(
+    "UserReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
 
 UserSearchCriteriaTypeDef = TypedDict(
@@ -8201,74 +8183,90 @@
     "UserSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
     total=False,
 )
 
-UserSearchSummaryOutputTypeDef = TypedDict(
-    "UserSearchSummaryOutputTypeDef",
+UserSearchSummaryTypeDef = TypedDict(
+    "UserSearchSummaryTypeDef",
     {
         "Arn": str,
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Id": str,
-        "IdentityInfo": "UserIdentityInfoLiteOutputTypeDef",
+        "IdentityInfo": "UserIdentityInfoLiteTypeDef",
         "PhoneConfig": "UserPhoneConfigOutputTypeDef",
         "RoutingProfileId": str,
         "SecurityProfileIds": List[str],
         "Tags": Dict[str, str],
         "Username": str,
     },
 )
 
-UserSummaryOutputTypeDef = TypedDict(
-    "UserSummaryOutputTypeDef",
+UserSummaryTypeDef = TypedDict(
+    "UserSummaryTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Username": str,
+    },
+)
+
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
+        "IdentityInfo": "UserIdentityInfoOutputTypeDef",
+        "PhoneConfig": "UserPhoneConfigOutputTypeDef",
+        "DirectoryUserId": str,
+        "SecurityProfileIds": List[str],
+        "RoutingProfileId": str,
+        "HierarchyGroupId": str,
+        "Tags": Dict[str, str],
     },
 )
 
-VocabularyOutputTypeDef = TypedDict(
-    "VocabularyOutputTypeDef",
+VocabularySummaryTypeDef = TypedDict(
+    "VocabularySummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "Content": str,
-        "Tags": Dict[str, str],
     },
 )
 
-VocabularySummaryOutputTypeDef = TypedDict(
-    "VocabularySummaryOutputTypeDef",
+VocabularyTypeDef = TypedDict(
+    "VocabularyTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
+        "Content": str,
+        "Tags": Dict[str, str],
     },
 )
 
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
 
-WisdomInfoOutputTypeDef = TypedDict(
-    "WisdomInfoOutputTypeDef",
+WisdomInfoTypeDef = TypedDict(
+    "WisdomInfoTypeDef",
     {
         "SessionArn": str,
     },
 )
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -578,103 +578,103 @@
 ### Typed dictionaries
 
 `mypy_boto3_connect.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connect.type_defs import (
-    ActionSummaryOutputTypeDef,
+    ActionSummaryTypeDef,
     ActivateEvaluationFormRequestRequestTypeDef,
-    ActivateEvaluationFormResponseOutputTypeDef,
-    AgentContactReferenceOutputTypeDef,
-    AgentInfoOutputTypeDef,
-    AgentStatusOutputTypeDef,
-    AgentStatusReferenceOutputTypeDef,
-    AgentStatusSummaryOutputTypeDef,
+    ActivateEvaluationFormResponseTypeDef,
+    AgentContactReferenceTypeDef,
+    AgentInfoTypeDef,
+    AgentStatusReferenceTypeDef,
+    AgentStatusSummaryTypeDef,
+    AgentStatusTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     AssociateApprovedOriginRequestRequestTypeDef,
     AssociateBotRequestRequestTypeDef,
     AssociateDefaultVocabularyRequestRequestTypeDef,
     AssociateInstanceStorageConfigRequestRequestTypeDef,
-    AssociateInstanceStorageConfigResponseOutputTypeDef,
+    AssociateInstanceStorageConfigResponseTypeDef,
     AssociateLambdaFunctionRequestRequestTypeDef,
     AssociateLexBotRequestRequestTypeDef,
     AssociatePhoneNumberContactFlowRequestRequestTypeDef,
     AssociateQueueQuickConnectsRequestRequestTypeDef,
     AssociateRoutingProfileQueuesRequestRequestTypeDef,
     AssociateSecurityKeyRequestRequestTypeDef,
-    AssociateSecurityKeyResponseOutputTypeDef,
-    AttachmentReferenceOutputTypeDef,
-    AttributeOutputTypeDef,
-    AvailableNumberSummaryOutputTypeDef,
+    AssociateSecurityKeyResponseTypeDef,
+    AttachmentReferenceTypeDef,
+    AttributeTypeDef,
+    AvailableNumberSummaryTypeDef,
     ChatMessageTypeDef,
     ChatParticipantRoleConfigTypeDef,
     ChatStreamingConfigurationTypeDef,
     ClaimPhoneNumberRequestRequestTypeDef,
-    ClaimPhoneNumberResponseOutputTypeDef,
-    ClaimedPhoneNumberSummaryOutputTypeDef,
+    ClaimPhoneNumberResponseTypeDef,
+    ClaimedPhoneNumberSummaryTypeDef,
     ContactFilterTypeDef,
-    ContactFlowModuleOutputTypeDef,
-    ContactFlowModuleSummaryOutputTypeDef,
-    ContactFlowOutputTypeDef,
-    ContactFlowSummaryOutputTypeDef,
-    ContactOutputTypeDef,
+    ContactFlowModuleSummaryTypeDef,
+    ContactFlowModuleTypeDef,
+    ContactFlowSummaryTypeDef,
+    ContactFlowTypeDef,
+    ContactTypeDef,
     ControlPlaneTagFilterTypeDef,
     CreateAgentStatusRequestRequestTypeDef,
-    CreateAgentStatusResponseOutputTypeDef,
+    CreateAgentStatusResponseTypeDef,
     CreateContactFlowModuleRequestRequestTypeDef,
-    CreateContactFlowModuleResponseOutputTypeDef,
+    CreateContactFlowModuleResponseTypeDef,
     CreateContactFlowRequestRequestTypeDef,
-    CreateContactFlowResponseOutputTypeDef,
+    CreateContactFlowResponseTypeDef,
     CreateEvaluationFormRequestRequestTypeDef,
-    CreateEvaluationFormResponseOutputTypeDef,
+    CreateEvaluationFormResponseTypeDef,
     CreateHoursOfOperationRequestRequestTypeDef,
-    CreateHoursOfOperationResponseOutputTypeDef,
+    CreateHoursOfOperationResponseTypeDef,
     CreateInstanceRequestRequestTypeDef,
-    CreateInstanceResponseOutputTypeDef,
+    CreateInstanceResponseTypeDef,
     CreateIntegrationAssociationRequestRequestTypeDef,
-    CreateIntegrationAssociationResponseOutputTypeDef,
+    CreateIntegrationAssociationResponseTypeDef,
     CreateParticipantRequestRequestTypeDef,
-    CreateParticipantResponseOutputTypeDef,
+    CreateParticipantResponseTypeDef,
     CreatePromptRequestRequestTypeDef,
-    CreatePromptResponseOutputTypeDef,
+    CreatePromptResponseTypeDef,
     CreateQueueRequestRequestTypeDef,
-    CreateQueueResponseOutputTypeDef,
+    CreateQueueResponseTypeDef,
     CreateQuickConnectRequestRequestTypeDef,
-    CreateQuickConnectResponseOutputTypeDef,
+    CreateQuickConnectResponseTypeDef,
     CreateRoutingProfileRequestRequestTypeDef,
-    CreateRoutingProfileResponseOutputTypeDef,
+    CreateRoutingProfileResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseOutputTypeDef,
+    CreateRuleResponseTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
-    CreateSecurityProfileResponseOutputTypeDef,
+    CreateSecurityProfileResponseTypeDef,
     CreateTaskTemplateRequestRequestTypeDef,
-    CreateTaskTemplateResponseOutputTypeDef,
+    CreateTaskTemplateResponseTypeDef,
     CreateTrafficDistributionGroupRequestRequestTypeDef,
-    CreateTrafficDistributionGroupResponseOutputTypeDef,
+    CreateTrafficDistributionGroupResponseTypeDef,
     CreateUseCaseRequestRequestTypeDef,
-    CreateUseCaseResponseOutputTypeDef,
+    CreateUseCaseResponseTypeDef,
     CreateUserHierarchyGroupRequestRequestTypeDef,
-    CreateUserHierarchyGroupResponseOutputTypeDef,
+    CreateUserHierarchyGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseOutputTypeDef,
+    CreateUserResponseTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    CreateVocabularyResponseOutputTypeDef,
-    CredentialsOutputTypeDef,
+    CreateVocabularyResponseTypeDef,
+    CredentialsTypeDef,
     CrossChannelBehaviorOutputTypeDef,
     CrossChannelBehaviorTypeDef,
-    CurrentMetricDataOutputTypeDef,
+    CurrentMetricDataTypeDef,
     CurrentMetricOutputTypeDef,
-    CurrentMetricResultOutputTypeDef,
+    CurrentMetricResultTypeDef,
     CurrentMetricSortCriteriaTypeDef,
     CurrentMetricTypeDef,
-    DateReferenceOutputTypeDef,
+    DateReferenceTypeDef,
     DeactivateEvaluationFormRequestRequestTypeDef,
-    DeactivateEvaluationFormResponseOutputTypeDef,
-    DefaultVocabularyOutputTypeDef,
+    DeactivateEvaluationFormResponseTypeDef,
+    DefaultVocabularyTypeDef,
     DeleteContactEvaluationRequestRequestTypeDef,
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
@@ -686,90 +686,89 @@
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
-    DeleteVocabularyResponseOutputTypeDef,
+    DeleteVocabularyResponseTypeDef,
     DescribeAgentStatusRequestRequestTypeDef,
-    DescribeAgentStatusResponseOutputTypeDef,
+    DescribeAgentStatusResponseTypeDef,
     DescribeContactEvaluationRequestRequestTypeDef,
-    DescribeContactEvaluationResponseOutputTypeDef,
+    DescribeContactEvaluationResponseTypeDef,
     DescribeContactFlowModuleRequestRequestTypeDef,
-    DescribeContactFlowModuleResponseOutputTypeDef,
+    DescribeContactFlowModuleResponseTypeDef,
     DescribeContactFlowRequestRequestTypeDef,
-    DescribeContactFlowResponseOutputTypeDef,
+    DescribeContactFlowResponseTypeDef,
     DescribeContactRequestRequestTypeDef,
-    DescribeContactResponseOutputTypeDef,
+    DescribeContactResponseTypeDef,
     DescribeEvaluationFormRequestRequestTypeDef,
-    DescribeEvaluationFormResponseOutputTypeDef,
+    DescribeEvaluationFormResponseTypeDef,
     DescribeHoursOfOperationRequestRequestTypeDef,
-    DescribeHoursOfOperationResponseOutputTypeDef,
+    DescribeHoursOfOperationResponseTypeDef,
     DescribeInstanceAttributeRequestRequestTypeDef,
-    DescribeInstanceAttributeResponseOutputTypeDef,
+    DescribeInstanceAttributeResponseTypeDef,
     DescribeInstanceRequestRequestTypeDef,
-    DescribeInstanceResponseOutputTypeDef,
+    DescribeInstanceResponseTypeDef,
     DescribeInstanceStorageConfigRequestRequestTypeDef,
-    DescribeInstanceStorageConfigResponseOutputTypeDef,
+    DescribeInstanceStorageConfigResponseTypeDef,
     DescribePhoneNumberRequestRequestTypeDef,
-    DescribePhoneNumberResponseOutputTypeDef,
+    DescribePhoneNumberResponseTypeDef,
     DescribePromptRequestRequestTypeDef,
-    DescribePromptResponseOutputTypeDef,
+    DescribePromptResponseTypeDef,
     DescribeQueueRequestRequestTypeDef,
-    DescribeQueueResponseOutputTypeDef,
+    DescribeQueueResponseTypeDef,
     DescribeQuickConnectRequestRequestTypeDef,
-    DescribeQuickConnectResponseOutputTypeDef,
+    DescribeQuickConnectResponseTypeDef,
     DescribeRoutingProfileRequestRequestTypeDef,
-    DescribeRoutingProfileResponseOutputTypeDef,
+    DescribeRoutingProfileResponseTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseOutputTypeDef,
+    DescribeRuleResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
-    DescribeSecurityProfileResponseOutputTypeDef,
+    DescribeSecurityProfileResponseTypeDef,
     DescribeTrafficDistributionGroupRequestRequestTypeDef,
-    DescribeTrafficDistributionGroupResponseOutputTypeDef,
+    DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupRequestRequestTypeDef,
-    DescribeUserHierarchyGroupResponseOutputTypeDef,
+    DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureRequestRequestTypeDef,
-    DescribeUserHierarchyStructureResponseOutputTypeDef,
+    DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseOutputTypeDef,
+    DescribeUserResponseTypeDef,
     DescribeVocabularyRequestRequestTypeDef,
-    DescribeVocabularyResponseOutputTypeDef,
-    DimensionsOutputTypeDef,
+    DescribeVocabularyResponseTypeDef,
+    DimensionsTypeDef,
     DisassociateApprovedOriginRequestRequestTypeDef,
     DisassociateBotRequestRequestTypeDef,
     DisassociateInstanceStorageConfigRequestRequestTypeDef,
     DisassociateLambdaFunctionRequestRequestTypeDef,
     DisassociateLexBotRequestRequestTypeDef,
     DisassociatePhoneNumberContactFlowRequestRequestTypeDef,
     DisassociateQueueQuickConnectsRequestRequestTypeDef,
     DisassociateRoutingProfileQueuesRequestRequestTypeDef,
     DisassociateSecurityKeyRequestRequestTypeDef,
     DismissUserContactRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
-    EmailReferenceOutputTypeDef,
+    EmailReferenceTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     EvaluationAnswerDataOutputTypeDef,
     EvaluationAnswerDataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationAnswerOutputOutputTypeDef,
-    EvaluationFormContentOutputTypeDef,
+    EvaluationAnswerOutputTypeDef,
+    EvaluationFormContentTypeDef,
     EvaluationFormItemOutputTypeDef,
     EvaluationFormItemTypeDef,
     EvaluationFormNumericQuestionAutomationOutputTypeDef,
     EvaluationFormNumericQuestionAutomationTypeDef,
     EvaluationFormNumericQuestionOptionOutputTypeDef,
     EvaluationFormNumericQuestionOptionTypeDef,
     EvaluationFormNumericQuestionPropertiesOutputTypeDef,
     EvaluationFormNumericQuestionPropertiesTypeDef,
-    EvaluationFormOutputTypeDef,
     EvaluationFormQuestionOutputTypeDef,
     EvaluationFormQuestionTypeDef,
     EvaluationFormQuestionTypePropertiesOutputTypeDef,
     EvaluationFormQuestionTypePropertiesTypeDef,
     EvaluationFormScoringStrategyOutputTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationFormSectionOutputTypeDef,
@@ -778,424 +777,425 @@
     EvaluationFormSingleSelectQuestionAutomationOptionTypeDef,
     EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
     EvaluationFormSingleSelectQuestionAutomationTypeDef,
     EvaluationFormSingleSelectQuestionOptionOutputTypeDef,
     EvaluationFormSingleSelectQuestionOptionTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
     EvaluationFormSingleSelectQuestionPropertiesTypeDef,
-    EvaluationFormSummaryOutputTypeDef,
-    EvaluationFormVersionSummaryOutputTypeDef,
-    EvaluationMetadataOutputTypeDef,
+    EvaluationFormSummaryTypeDef,
+    EvaluationFormTypeDef,
+    EvaluationFormVersionSummaryTypeDef,
+    EvaluationMetadataTypeDef,
     EvaluationNoteOutputTypeDef,
     EvaluationNoteTypeDef,
-    EvaluationOutputTypeDef,
-    EvaluationScoreOutputTypeDef,
-    EvaluationSummaryOutputTypeDef,
+    EvaluationScoreTypeDef,
+    EvaluationSummaryTypeDef,
+    EvaluationTypeDef,
     EventBridgeActionDefinitionOutputTypeDef,
     EventBridgeActionDefinitionTypeDef,
     FilterV2TypeDef,
     FiltersTypeDef,
     GetContactAttributesRequestRequestTypeDef,
-    GetContactAttributesResponseOutputTypeDef,
+    GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataRequestRequestTypeDef,
-    GetCurrentMetricDataResponseOutputTypeDef,
+    GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataRequestRequestTypeDef,
-    GetCurrentUserDataResponseOutputTypeDef,
+    GetCurrentUserDataResponseTypeDef,
     GetFederationTokenRequestRequestTypeDef,
-    GetFederationTokenResponseOutputTypeDef,
+    GetFederationTokenResponseTypeDef,
     GetMetricDataRequestGetMetricDataPaginateTypeDef,
     GetMetricDataRequestRequestTypeDef,
-    GetMetricDataResponseOutputTypeDef,
+    GetMetricDataResponseTypeDef,
     GetMetricDataV2RequestRequestTypeDef,
-    GetMetricDataV2ResponseOutputTypeDef,
+    GetMetricDataV2ResponseTypeDef,
     GetPromptFileRequestRequestTypeDef,
-    GetPromptFileResponseOutputTypeDef,
+    GetPromptFileResponseTypeDef,
     GetTaskTemplateRequestRequestTypeDef,
-    GetTaskTemplateResponseOutputTypeDef,
+    GetTaskTemplateResponseTypeDef,
     GetTrafficDistributionRequestRequestTypeDef,
-    GetTrafficDistributionResponseOutputTypeDef,
+    GetTrafficDistributionResponseTypeDef,
     HierarchyGroupConditionTypeDef,
-    HierarchyGroupOutputTypeDef,
-    HierarchyGroupSummaryOutputTypeDef,
-    HierarchyGroupSummaryReferenceOutputTypeDef,
-    HierarchyLevelOutputTypeDef,
+    HierarchyGroupSummaryReferenceTypeDef,
+    HierarchyGroupSummaryTypeDef,
+    HierarchyGroupTypeDef,
+    HierarchyLevelTypeDef,
     HierarchyLevelUpdateTypeDef,
-    HierarchyPathOutputTypeDef,
-    HierarchyPathReferenceOutputTypeDef,
-    HierarchyStructureOutputTypeDef,
+    HierarchyPathReferenceTypeDef,
+    HierarchyPathTypeDef,
+    HierarchyStructureTypeDef,
     HierarchyStructureUpdateTypeDef,
-    HistoricalMetricDataOutputTypeDef,
+    HistoricalMetricDataTypeDef,
     HistoricalMetricOutputTypeDef,
-    HistoricalMetricResultOutputTypeDef,
+    HistoricalMetricResultTypeDef,
     HistoricalMetricTypeDef,
     HoursOfOperationConfigOutputTypeDef,
     HoursOfOperationConfigTypeDef,
-    HoursOfOperationOutputTypeDef,
     HoursOfOperationSearchCriteriaTypeDef,
     HoursOfOperationSearchFilterTypeDef,
-    HoursOfOperationSummaryOutputTypeDef,
+    HoursOfOperationSummaryTypeDef,
     HoursOfOperationTimeSliceOutputTypeDef,
     HoursOfOperationTimeSliceTypeDef,
-    InstanceOutputTypeDef,
-    InstanceStatusReasonOutputTypeDef,
+    HoursOfOperationTypeDef,
+    InstanceStatusReasonTypeDef,
     InstanceStorageConfigOutputTypeDef,
     InstanceStorageConfigTypeDef,
-    InstanceSummaryOutputTypeDef,
-    IntegrationAssociationSummaryOutputTypeDef,
+    InstanceSummaryTypeDef,
+    InstanceTypeDef,
+    IntegrationAssociationSummaryTypeDef,
     InvisibleFieldInfoOutputTypeDef,
     InvisibleFieldInfoTypeDef,
     KinesisFirehoseConfigOutputTypeDef,
     KinesisFirehoseConfigTypeDef,
     KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
     KinesisVideoStreamConfigOutputTypeDef,
     KinesisVideoStreamConfigTypeDef,
-    LexBotConfigOutputTypeDef,
+    LexBotConfigTypeDef,
     LexBotOutputTypeDef,
     LexBotTypeDef,
     LexV2BotOutputTypeDef,
     LexV2BotTypeDef,
     ListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     ListAgentStatusRequestRequestTypeDef,
-    ListAgentStatusResponseOutputTypeDef,
+    ListAgentStatusResponseTypeDef,
     ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     ListApprovedOriginsRequestRequestTypeDef,
-    ListApprovedOriginsResponseOutputTypeDef,
+    ListApprovedOriginsResponseTypeDef,
     ListBotsRequestListBotsPaginateTypeDef,
     ListBotsRequestRequestTypeDef,
-    ListBotsResponseOutputTypeDef,
+    ListBotsResponseTypeDef,
     ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     ListContactEvaluationsRequestRequestTypeDef,
-    ListContactEvaluationsResponseOutputTypeDef,
+    ListContactEvaluationsResponseTypeDef,
     ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     ListContactFlowModulesRequestRequestTypeDef,
-    ListContactFlowModulesResponseOutputTypeDef,
+    ListContactFlowModulesResponseTypeDef,
     ListContactFlowsRequestListContactFlowsPaginateTypeDef,
     ListContactFlowsRequestRequestTypeDef,
-    ListContactFlowsResponseOutputTypeDef,
+    ListContactFlowsResponseTypeDef,
     ListContactReferencesRequestListContactReferencesPaginateTypeDef,
     ListContactReferencesRequestRequestTypeDef,
-    ListContactReferencesResponseOutputTypeDef,
+    ListContactReferencesResponseTypeDef,
     ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     ListDefaultVocabulariesRequestRequestTypeDef,
-    ListDefaultVocabulariesResponseOutputTypeDef,
+    ListDefaultVocabulariesResponseTypeDef,
     ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     ListEvaluationFormVersionsRequestRequestTypeDef,
-    ListEvaluationFormVersionsResponseOutputTypeDef,
+    ListEvaluationFormVersionsResponseTypeDef,
     ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     ListEvaluationFormsRequestRequestTypeDef,
-    ListEvaluationFormsResponseOutputTypeDef,
+    ListEvaluationFormsResponseTypeDef,
     ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     ListHoursOfOperationsRequestRequestTypeDef,
-    ListHoursOfOperationsResponseOutputTypeDef,
+    ListHoursOfOperationsResponseTypeDef,
     ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     ListInstanceAttributesRequestRequestTypeDef,
-    ListInstanceAttributesResponseOutputTypeDef,
+    ListInstanceAttributesResponseTypeDef,
     ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     ListInstanceStorageConfigsRequestRequestTypeDef,
-    ListInstanceStorageConfigsResponseOutputTypeDef,
+    ListInstanceStorageConfigsResponseTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseOutputTypeDef,
+    ListInstancesResponseTypeDef,
     ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     ListIntegrationAssociationsRequestRequestTypeDef,
-    ListIntegrationAssociationsResponseOutputTypeDef,
+    ListIntegrationAssociationsResponseTypeDef,
     ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     ListLambdaFunctionsRequestRequestTypeDef,
-    ListLambdaFunctionsResponseOutputTypeDef,
+    ListLambdaFunctionsResponseTypeDef,
     ListLexBotsRequestListLexBotsPaginateTypeDef,
     ListLexBotsRequestRequestTypeDef,
-    ListLexBotsResponseOutputTypeDef,
+    ListLexBotsResponseTypeDef,
     ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
-    ListPhoneNumbersResponseOutputTypeDef,
-    ListPhoneNumbersSummaryOutputTypeDef,
+    ListPhoneNumbersResponseTypeDef,
+    ListPhoneNumbersSummaryTypeDef,
     ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef,
     ListPhoneNumbersV2RequestRequestTypeDef,
-    ListPhoneNumbersV2ResponseOutputTypeDef,
+    ListPhoneNumbersV2ResponseTypeDef,
     ListPromptsRequestListPromptsPaginateTypeDef,
     ListPromptsRequestRequestTypeDef,
-    ListPromptsResponseOutputTypeDef,
+    ListPromptsResponseTypeDef,
     ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     ListQueueQuickConnectsRequestRequestTypeDef,
-    ListQueueQuickConnectsResponseOutputTypeDef,
+    ListQueueQuickConnectsResponseTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResponseOutputTypeDef,
+    ListQueuesResponseTypeDef,
     ListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     ListQuickConnectsRequestRequestTypeDef,
-    ListQuickConnectsResponseOutputTypeDef,
+    ListQuickConnectsResponseTypeDef,
     ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     ListRoutingProfileQueuesRequestRequestTypeDef,
-    ListRoutingProfileQueuesResponseOutputTypeDef,
+    ListRoutingProfileQueuesResponseTypeDef,
     ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     ListRoutingProfilesRequestRequestTypeDef,
-    ListRoutingProfilesResponseOutputTypeDef,
+    ListRoutingProfilesResponseTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListRulesResponseOutputTypeDef,
+    ListRulesResponseTypeDef,
     ListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     ListSecurityKeysRequestRequestTypeDef,
-    ListSecurityKeysResponseOutputTypeDef,
+    ListSecurityKeysResponseTypeDef,
     ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     ListSecurityProfilePermissionsRequestRequestTypeDef,
-    ListSecurityProfilePermissionsResponseOutputTypeDef,
+    ListSecurityProfilePermissionsResponseTypeDef,
     ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
-    ListSecurityProfilesResponseOutputTypeDef,
+    ListSecurityProfilesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     ListTaskTemplatesRequestRequestTypeDef,
-    ListTaskTemplatesResponseOutputTypeDef,
+    ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef,
     ListTrafficDistributionGroupsRequestRequestTypeDef,
-    ListTrafficDistributionGroupsResponseOutputTypeDef,
+    ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesRequestListUseCasesPaginateTypeDef,
     ListUseCasesRequestRequestTypeDef,
-    ListUseCasesResponseOutputTypeDef,
+    ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     ListUserHierarchyGroupsRequestRequestTypeDef,
-    ListUserHierarchyGroupsResponseOutputTypeDef,
+    ListUserHierarchyGroupsResponseTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListUsersResponseTypeDef,
     MediaConcurrencyOutputTypeDef,
     MediaConcurrencyTypeDef,
-    MetricDataV2OutputTypeDef,
+    MetricDataV2TypeDef,
     MetricFilterV2OutputTypeDef,
     MetricFilterV2TypeDef,
-    MetricResultV2OutputTypeDef,
+    MetricResultV2TypeDef,
     MetricV2OutputTypeDef,
     MetricV2TypeDef,
     MonitorContactRequestRequestTypeDef,
-    MonitorContactResponseOutputTypeDef,
+    MonitorContactResponseTypeDef,
     NotificationRecipientTypeOutputTypeDef,
     NotificationRecipientTypeTypeDef,
-    NumberReferenceOutputTypeDef,
+    NumberReferenceTypeDef,
     NumericQuestionPropertyValueAutomationOutputTypeDef,
     NumericQuestionPropertyValueAutomationTypeDef,
     OutboundCallerConfigOutputTypeDef,
     OutboundCallerConfigTypeDef,
     PaginatorConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     ParticipantTimerConfigurationTypeDef,
     ParticipantTimerValueTypeDef,
-    ParticipantTokenCredentialsOutputTypeDef,
+    ParticipantTokenCredentialsTypeDef,
     PersistentChatTypeDef,
     PhoneNumberQuickConnectConfigOutputTypeDef,
     PhoneNumberQuickConnectConfigTypeDef,
-    PhoneNumberStatusOutputTypeDef,
-    PhoneNumberSummaryOutputTypeDef,
-    PromptOutputTypeDef,
+    PhoneNumberStatusTypeDef,
+    PhoneNumberSummaryTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
-    PromptSummaryOutputTypeDef,
+    PromptSummaryTypeDef,
+    PromptTypeDef,
     PutUserStatusRequestRequestTypeDef,
-    QueueInfoOutputTypeDef,
-    QueueOutputTypeDef,
+    QueueInfoTypeDef,
     QueueQuickConnectConfigOutputTypeDef,
     QueueQuickConnectConfigTypeDef,
-    QueueReferenceOutputTypeDef,
+    QueueReferenceTypeDef,
     QueueSearchCriteriaTypeDef,
     QueueSearchFilterTypeDef,
-    QueueSummaryOutputTypeDef,
+    QueueSummaryTypeDef,
+    QueueTypeDef,
     QuickConnectConfigOutputTypeDef,
     QuickConnectConfigTypeDef,
-    QuickConnectOutputTypeDef,
     QuickConnectSearchCriteriaTypeDef,
     QuickConnectSearchFilterTypeDef,
-    QuickConnectSummaryOutputTypeDef,
+    QuickConnectSummaryTypeDef,
+    QuickConnectTypeDef,
     ReadOnlyFieldInfoOutputTypeDef,
     ReadOnlyFieldInfoTypeDef,
     ReferenceOutputTypeDef,
-    ReferenceSummaryOutputTypeDef,
+    ReferenceSummaryTypeDef,
     ReferenceTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     ReplicateInstanceRequestRequestTypeDef,
-    ReplicateInstanceResponseOutputTypeDef,
+    ReplicateInstanceResponseTypeDef,
     RequiredFieldInfoOutputTypeDef,
     RequiredFieldInfoTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     ResponseMetadataTypeDef,
     ResumeContactRecordingRequestRequestTypeDef,
-    RoutingProfileOutputTypeDef,
-    RoutingProfileQueueConfigSummaryOutputTypeDef,
+    RoutingProfileQueueConfigSummaryTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
-    RoutingProfileReferenceOutputTypeDef,
+    RoutingProfileReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RoutingProfileSummaryOutputTypeDef,
+    RoutingProfileSummaryTypeDef,
+    RoutingProfileTypeDef,
     RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    RuleOutputTypeDef,
-    RuleSummaryOutputTypeDef,
+    RuleSummaryTypeDef,
     RuleTriggerEventSourceOutputTypeDef,
     RuleTriggerEventSourceTypeDef,
+    RuleTypeDef,
     S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
-    SearchAvailablePhoneNumbersResponseOutputTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SearchHoursOfOperationsRequestRequestTypeDef,
     SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
-    SearchHoursOfOperationsResponseOutputTypeDef,
+    SearchHoursOfOperationsResponseTypeDef,
     SearchPromptsRequestRequestTypeDef,
     SearchPromptsRequestSearchPromptsPaginateTypeDef,
-    SearchPromptsResponseOutputTypeDef,
+    SearchPromptsResponseTypeDef,
     SearchQueuesRequestRequestTypeDef,
     SearchQueuesRequestSearchQueuesPaginateTypeDef,
-    SearchQueuesResponseOutputTypeDef,
+    SearchQueuesResponseTypeDef,
     SearchQuickConnectsRequestRequestTypeDef,
     SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
-    SearchQuickConnectsResponseOutputTypeDef,
+    SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsRequestRequestTypeDef,
     SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
-    SearchResourceTagsResponseOutputTypeDef,
+    SearchResourceTagsResponseTypeDef,
     SearchRoutingProfilesRequestRequestTypeDef,
     SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
-    SearchRoutingProfilesResponseOutputTypeDef,
+    SearchRoutingProfilesResponseTypeDef,
     SearchSecurityProfilesRequestRequestTypeDef,
     SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
-    SearchSecurityProfilesResponseOutputTypeDef,
+    SearchSecurityProfilesResponseTypeDef,
     SearchUsersRequestRequestTypeDef,
     SearchUsersRequestSearchUsersPaginateTypeDef,
-    SearchUsersResponseOutputTypeDef,
+    SearchUsersResponseTypeDef,
     SearchVocabulariesRequestRequestTypeDef,
     SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
-    SearchVocabulariesResponseOutputTypeDef,
-    SecurityKeyOutputTypeDef,
-    SecurityProfileOutputTypeDef,
+    SearchVocabulariesResponseTypeDef,
+    SecurityKeyTypeDef,
     SecurityProfileSearchCriteriaTypeDef,
-    SecurityProfileSearchSummaryOutputTypeDef,
-    SecurityProfileSummaryOutputTypeDef,
+    SecurityProfileSearchSummaryTypeDef,
+    SecurityProfileSummaryTypeDef,
+    SecurityProfileTypeDef,
     SecurityProfilesSearchFilterTypeDef,
     SendNotificationActionDefinitionOutputTypeDef,
     SendNotificationActionDefinitionTypeDef,
     SingleSelectQuestionRuleCategoryAutomationOutputTypeDef,
     SingleSelectQuestionRuleCategoryAutomationTypeDef,
     StartChatContactRequestRequestTypeDef,
-    StartChatContactResponseOutputTypeDef,
+    StartChatContactResponseTypeDef,
     StartContactEvaluationRequestRequestTypeDef,
-    StartContactEvaluationResponseOutputTypeDef,
+    StartContactEvaluationResponseTypeDef,
     StartContactRecordingRequestRequestTypeDef,
     StartContactStreamingRequestRequestTypeDef,
-    StartContactStreamingResponseOutputTypeDef,
+    StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactRequestRequestTypeDef,
-    StartOutboundVoiceContactResponseOutputTypeDef,
+    StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactRequestRequestTypeDef,
-    StartTaskContactResponseOutputTypeDef,
+    StartTaskContactResponseTypeDef,
     StopContactRecordingRequestRequestTypeDef,
     StopContactRequestRequestTypeDef,
     StopContactStreamingRequestRequestTypeDef,
     StringConditionTypeDef,
-    StringReferenceOutputTypeDef,
+    StringReferenceTypeDef,
     SubmitContactEvaluationRequestRequestTypeDef,
-    SubmitContactEvaluationResponseOutputTypeDef,
+    SubmitContactEvaluationResponseTypeDef,
     SuspendContactRecordingRequestRequestTypeDef,
     TagConditionTypeDef,
     TagResourceRequestRequestTypeDef,
     TagSearchConditionTypeDef,
-    TagSetOutputTypeDef,
+    TagSetTypeDef,
     TaskActionDefinitionOutputTypeDef,
     TaskActionDefinitionTypeDef,
     TaskTemplateConstraintsOutputTypeDef,
     TaskTemplateConstraintsTypeDef,
     TaskTemplateDefaultFieldValueOutputTypeDef,
     TaskTemplateDefaultFieldValueTypeDef,
     TaskTemplateDefaultsOutputTypeDef,
     TaskTemplateDefaultsTypeDef,
     TaskTemplateFieldIdentifierOutputTypeDef,
     TaskTemplateFieldIdentifierTypeDef,
     TaskTemplateFieldOutputTypeDef,
     TaskTemplateFieldTypeDef,
-    TaskTemplateMetadataOutputTypeDef,
+    TaskTemplateMetadataTypeDef,
     TelephonyConfigOutputTypeDef,
     TelephonyConfigTypeDef,
     ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ThresholdV2OutputTypeDef,
     ThresholdV2TypeDef,
-    TrafficDistributionGroupOutputTypeDef,
-    TrafficDistributionGroupSummaryOutputTypeDef,
+    TrafficDistributionGroupSummaryTypeDef,
+    TrafficDistributionGroupTypeDef,
     TransferContactRequestRequestTypeDef,
-    TransferContactResponseOutputTypeDef,
+    TransferContactResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     UpdateContactAttributesRequestRequestTypeDef,
     UpdateContactEvaluationRequestRequestTypeDef,
-    UpdateContactEvaluationResponseOutputTypeDef,
+    UpdateContactEvaluationResponseTypeDef,
     UpdateContactFlowContentRequestRequestTypeDef,
     UpdateContactFlowMetadataRequestRequestTypeDef,
     UpdateContactFlowModuleContentRequestRequestTypeDef,
     UpdateContactFlowModuleMetadataRequestRequestTypeDef,
     UpdateContactFlowNameRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     UpdateContactScheduleRequestRequestTypeDef,
     UpdateEvaluationFormRequestRequestTypeDef,
-    UpdateEvaluationFormResponseOutputTypeDef,
+    UpdateEvaluationFormResponseTypeDef,
     UpdateHoursOfOperationRequestRequestTypeDef,
     UpdateInstanceAttributeRequestRequestTypeDef,
     UpdateInstanceStorageConfigRequestRequestTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdateParticipantRoleConfigRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
-    UpdatePhoneNumberResponseOutputTypeDef,
+    UpdatePhoneNumberResponseTypeDef,
     UpdatePromptRequestRequestTypeDef,
-    UpdatePromptResponseOutputTypeDef,
+    UpdatePromptResponseTypeDef,
     UpdateQueueHoursOfOperationRequestRequestTypeDef,
     UpdateQueueMaxContactsRequestRequestTypeDef,
     UpdateQueueNameRequestRequestTypeDef,
     UpdateQueueOutboundCallerConfigRequestRequestTypeDef,
     UpdateQueueStatusRequestRequestTypeDef,
     UpdateQuickConnectConfigRequestRequestTypeDef,
     UpdateQuickConnectNameRequestRequestTypeDef,
     UpdateRoutingProfileConcurrencyRequestRequestTypeDef,
     UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef,
     UpdateRoutingProfileNameRequestRequestTypeDef,
     UpdateRoutingProfileQueuesRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     UpdateTaskTemplateRequestRequestTypeDef,
-    UpdateTaskTemplateResponseOutputTypeDef,
+    UpdateTaskTemplateResponseTypeDef,
     UpdateTrafficDistributionRequestRequestTypeDef,
     UpdateUserHierarchyGroupNameRequestRequestTypeDef,
     UpdateUserHierarchyRequestRequestTypeDef,
     UpdateUserHierarchyStructureRequestRequestTypeDef,
     UpdateUserIdentityInfoRequestRequestTypeDef,
     UpdateUserPhoneConfigRequestRequestTypeDef,
     UpdateUserRoutingProfileRequestRequestTypeDef,
     UpdateUserSecurityProfilesRequestRequestTypeDef,
-    UrlReferenceOutputTypeDef,
-    UseCaseOutputTypeDef,
+    UrlReferenceTypeDef,
+    UseCaseTypeDef,
     UserDataFiltersTypeDef,
-    UserDataOutputTypeDef,
-    UserIdentityInfoLiteOutputTypeDef,
+    UserDataTypeDef,
+    UserIdentityInfoLiteTypeDef,
     UserIdentityInfoOutputTypeDef,
     UserIdentityInfoTypeDef,
-    UserOutputTypeDef,
     UserPhoneConfigOutputTypeDef,
     UserPhoneConfigTypeDef,
     UserQuickConnectConfigOutputTypeDef,
     UserQuickConnectConfigTypeDef,
-    UserReferenceOutputTypeDef,
+    UserReferenceTypeDef,
     UserSearchCriteriaTypeDef,
     UserSearchFilterTypeDef,
-    UserSearchSummaryOutputTypeDef,
-    UserSummaryOutputTypeDef,
-    VocabularyOutputTypeDef,
-    VocabularySummaryOutputTypeDef,
+    UserSearchSummaryTypeDef,
+    UserSummaryTypeDef,
+    UserTypeDef,
+    VocabularySummaryTypeDef,
+    VocabularyTypeDef,
     VoiceRecordingConfigurationTypeDef,
-    WisdomInfoOutputTypeDef,
+    WisdomInfoTypeDef,
 )
 
 
-def get_structure() -> ActionSummaryOutputTypeDef:
+def get_structure() -> ActionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connect-1.28.3.post1/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post1/setup.py` & `mypy-boto3-connect-1.28.3.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.7"
+        "Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

