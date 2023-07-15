# Comparing `tmp/mypy-boto3-secretsmanager-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-secretsmanager-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-secretsmanager-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
+gzip compressed data, was "mypy-boto3-secretsmanager-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:35 2023, max compression
```

## Comparing `mypy-boto3-secretsmanager-1.28.3.post1.tar` & `mypy-boto3-secretsmanager-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.095742 mypy-boto3-secretsmanager-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-07-14 16:18:03.091741 mypy-boto3-secretsmanager-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.091741 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-07-14 16:17:44.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.091741 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 16:18:02.000000 mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.095742 mypy-boto3-secretsmanager-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-14 16:17:43.000000 mypy-boto3-secretsmanager-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.282401 mypy-boto3-secretsmanager-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-15 06:38:35.278401 mypy-boto3-secretsmanager-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.270401 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19968 2023-07-15 06:38:19.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-07-15 06:38:19.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.278401 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-15 06:38:35.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-15 06:38:35.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:35.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 06:38:35.000000 mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:35.282401 mypy-boto3-secretsmanager-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-15 06:38:17.000000 mypy-boto3-secretsmanager-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/LICENSE` & `mypy-boto3-secretsmanager-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/PKG-INFO` & `mypy-boto3-secretsmanager-1.28.3.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,69 +324,69 @@
 
 `mypy_boto3_secretsmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_secretsmanager.type_defs import (
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseOutputTypeDef,
+    CancelRotateSecretResponseTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
-    ReplicationStatusTypeOutputTypeDef,
+    ReplicationStatusTypeTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseOutputTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseOutputTypeDef,
+    DeleteSecretResponseTypeDef,
     DescribeSecretRequestRequestTypeDef,
     RotationRulesTypeOutputTypeDef,
     TagOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseOutputTypeDef,
+    GetRandomPasswordResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseOutputTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseOutputTypeDef,
+    GetSecretValueResponseTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryOutputTypeDef,
+    SecretVersionsListEntryTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseOutputTypeDef,
+    PutResourcePolicyResponseTypeDef,
     PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseOutputTypeDef,
+    PutSecretValueResponseTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseOutputTypeDef,
+    RestoreSecretResponseTypeDef,
     RotationRulesTypeTypeDef,
-    RotateSecretResponseOutputTypeDef,
+    RotateSecretResponseTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseOutputTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseOutputTypeDef,
+    UpdateSecretResponseTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseOutputTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryOutputTypeDef,
+    ValidationErrorsEntryTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateSecretResponseOutputTypeDef,
-    RemoveRegionsFromReplicationResponseOutputTypeDef,
-    ReplicateSecretToRegionsResponseOutputTypeDef,
-    DescribeSecretResponseOutputTypeDef,
-    SecretListEntryOutputTypeDef,
+    CreateSecretResponseTypeDef,
+    RemoveRegionsFromReplicationResponseTypeDef,
+    ReplicateSecretToRegionsResponseTypeDef,
+    DescribeSecretResponseTypeDef,
+    SecretListEntryTypeDef,
     ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseOutputTypeDef,
+    ListSecretVersionIdsResponseTypeDef,
     RotateSecretRequestRequestTypeDef,
-    ValidateResourcePolicyResponseOutputTypeDef,
-    ListSecretsResponseOutputTypeDef,
+    ValidateResourcePolicyResponseTypeDef,
+    ListSecretsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/README.md` & `mypy-boto3-secretsmanager-1.28.3.post2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,69 +292,69 @@
 
 `mypy_boto3_secretsmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_secretsmanager.type_defs import (
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseOutputTypeDef,
+    CancelRotateSecretResponseTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
-    ReplicationStatusTypeOutputTypeDef,
+    ReplicationStatusTypeTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseOutputTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseOutputTypeDef,
+    DeleteSecretResponseTypeDef,
     DescribeSecretRequestRequestTypeDef,
     RotationRulesTypeOutputTypeDef,
     TagOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseOutputTypeDef,
+    GetRandomPasswordResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseOutputTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseOutputTypeDef,
+    GetSecretValueResponseTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryOutputTypeDef,
+    SecretVersionsListEntryTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseOutputTypeDef,
+    PutResourcePolicyResponseTypeDef,
     PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseOutputTypeDef,
+    PutSecretValueResponseTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseOutputTypeDef,
+    RestoreSecretResponseTypeDef,
     RotationRulesTypeTypeDef,
-    RotateSecretResponseOutputTypeDef,
+    RotateSecretResponseTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseOutputTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseOutputTypeDef,
+    UpdateSecretResponseTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseOutputTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryOutputTypeDef,
+    ValidationErrorsEntryTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateSecretResponseOutputTypeDef,
-    RemoveRegionsFromReplicationResponseOutputTypeDef,
-    ReplicateSecretToRegionsResponseOutputTypeDef,
-    DescribeSecretResponseOutputTypeDef,
-    SecretListEntryOutputTypeDef,
+    CreateSecretResponseTypeDef,
+    RemoveRegionsFromReplicationResponseTypeDef,
+    ReplicateSecretToRegionsResponseTypeDef,
+    DescribeSecretResponseTypeDef,
+    SecretListEntryTypeDef,
     ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseOutputTypeDef,
+    ListSecretVersionIdsResponseTypeDef,
     RotateSecretRequestRequestTypeDef,
-    ValidateResourcePolicyResponseOutputTypeDef,
-    ListSecretsResponseOutputTypeDef,
+    ValidateResourcePolicyResponseTypeDef,
+    ListSecretsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.py` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__init__.pyi` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/__main__.py` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecretsManager 1.28.3\nVersion:         1.28.3.post1\nBuilder"
-        " version: 7.14.7\nDocs:           "
+        "Type annotations for boto3.SecretsManager 1.28.3\nVersion:         1.28.3.post2\nBuilder"
+        " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.py` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,58 +18,55 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import SortOrderTypeType
 from .paginator import ListSecretsPaginator
 from .type_defs import (
-    CancelRotateSecretResponseOutputTypeDef,
-    CreateSecretResponseOutputTypeDef,
-    DeleteResourcePolicyResponseOutputTypeDef,
-    DeleteSecretResponseOutputTypeDef,
-    DescribeSecretResponseOutputTypeDef,
+    CancelRotateSecretResponseTypeDef,
+    CreateSecretResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteSecretResponseTypeDef,
+    DescribeSecretResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
-    GetRandomPasswordResponseOutputTypeDef,
-    GetResourcePolicyResponseOutputTypeDef,
-    GetSecretValueResponseOutputTypeDef,
-    ListSecretsResponseOutputTypeDef,
-    ListSecretVersionIdsResponseOutputTypeDef,
-    PutResourcePolicyResponseOutputTypeDef,
-    PutSecretValueResponseOutputTypeDef,
-    RemoveRegionsFromReplicationResponseOutputTypeDef,
+    GetRandomPasswordResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSecretValueResponseTypeDef,
+    ListSecretsResponseTypeDef,
+    ListSecretVersionIdsResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSecretValueResponseTypeDef,
+    RemoveRegionsFromReplicationResponseTypeDef,
     ReplicaRegionTypeTypeDef,
-    ReplicateSecretToRegionsResponseOutputTypeDef,
-    RestoreSecretResponseOutputTypeDef,
-    RotateSecretResponseOutputTypeDef,
+    ReplicateSecretToRegionsResponseTypeDef,
+    RestoreSecretResponseTypeDef,
+    RotateSecretResponseTypeDef,
     RotationRulesTypeTypeDef,
-    StopReplicationToReplicaResponseOutputTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
     TagTypeDef,
-    UpdateSecretResponseOutputTypeDef,
-    UpdateSecretVersionStageResponseOutputTypeDef,
-    ValidateResourcePolicyResponseOutputTypeDef,
+    UpdateSecretResponseTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
+    ValidateResourcePolicyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SecretsManagerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DecryptionFailure: Type[BotocoreClientError]
     EncryptionFailure: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -77,15 +74,14 @@
     LimitExceededException: Type[BotocoreClientError]
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     PreconditionNotMetException: Type[BotocoreClientError]
     PublicPolicyException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
-
 class SecretsManagerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/)
     """
 
     meta: ClientMeta
@@ -94,324 +90,298 @@
     def exceptions(self) -> Exceptions:
         """
         SecretsManagerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#can_paginate)
         """
-
-    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseOutputTypeDef:
+    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseTypeDef:
         """
         Turns off automatic rotation, and if a rotation is currently in progress,
         cancels the rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.cancel_rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#cancel_rotate_secret)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#close)
         """
-
     def create_secret(
         self,
         *,
         Name: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> CreateSecretResponseOutputTypeDef:
+    ) -> CreateSecretResponseTypeDef:
         """
         Creates a new secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.create_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#create_secret)
         """
-
-    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseOutputTypeDef:
+    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseTypeDef:
         """
         Deletes the resource-based permission policy attached to the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_resource_policy)
         """
-
     def delete_secret(
         self,
         *,
         SecretId: str,
         RecoveryWindowInDays: int = ...,
         ForceDeleteWithoutRecovery: bool = ...
-    ) -> DeleteSecretResponseOutputTypeDef:
+    ) -> DeleteSecretResponseTypeDef:
         """
         Deletes a secret and all of its versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_secret)
         """
-
-    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseOutputTypeDef:
+    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseTypeDef:
         """
         Retrieves the details of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.describe_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#describe_secret)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#generate_presigned_url)
         """
-
     def get_random_password(
         self,
         *,
         PasswordLength: int = ...,
         ExcludeCharacters: str = ...,
         ExcludeNumbers: bool = ...,
         ExcludePunctuation: bool = ...,
         ExcludeUppercase: bool = ...,
         ExcludeLowercase: bool = ...,
         IncludeSpace: bool = ...,
         RequireEachIncludedType: bool = ...
-    ) -> GetRandomPasswordResponseOutputTypeDef:
+    ) -> GetRandomPasswordResponseTypeDef:
         """
         Generates a random password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_random_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_random_password)
         """
-
-    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseOutputTypeDef:
+    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseTypeDef:
         """
         Retrieves the JSON text of the resource-based policy document attached to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_resource_policy)
         """
-
     def get_secret_value(
         self, *, SecretId: str, VersionId: str = ..., VersionStage: str = ...
-    ) -> GetSecretValueResponseOutputTypeDef:
+    ) -> GetSecretValueResponseTypeDef:
         """
         Retrieves the contents of the encrypted fields `SecretString` or `SecretBinary`
         from the specified version of a secret, whichever contains content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_secret_value)
         """
-
     def list_secret_version_ids(
         self,
         *,
         SecretId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         IncludeDeprecated: bool = ...
-    ) -> ListSecretVersionIdsResponseOutputTypeDef:
+    ) -> ListSecretVersionIdsResponseTypeDef:
         """
         Lists the versions of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secret_version_ids)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secret_version_ids)
         """
-
     def list_secrets(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...
-    ) -> ListSecretsResponseOutputTypeDef:
+    ) -> ListSecretsResponseTypeDef:
         """
         Lists the secrets that are stored by Secrets Manager in the Amazon Web Services
         account, not including secrets that are marked for deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secrets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secrets)
         """
-
     def put_resource_policy(
         self, *, SecretId: str, ResourcePolicy: str, BlockPublicPolicy: bool = ...
-    ) -> PutResourcePolicyResponseOutputTypeDef:
+    ) -> PutResourcePolicyResponseTypeDef:
         """
         Attaches a resource-based permission policy to a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_resource_policy)
         """
-
     def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         VersionStages: Sequence[str] = ...
-    ) -> PutSecretValueResponseOutputTypeDef:
+    ) -> PutSecretValueResponseTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_secret_value)
         """
-
     def remove_regions_from_replication(
         self, *, SecretId: str, RemoveReplicaRegions: Sequence[str]
-    ) -> RemoveRegionsFromReplicationResponseOutputTypeDef:
+    ) -> RemoveRegionsFromReplicationResponseTypeDef:
         """
         For a secret that is replicated to other Regions, deletes the secret replicas
         from the Regions you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.remove_regions_from_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#remove_regions_from_replication)
         """
-
     def replicate_secret_to_regions(
         self,
         *,
         SecretId: str,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> ReplicateSecretToRegionsResponseOutputTypeDef:
+    ) -> ReplicateSecretToRegionsResponseTypeDef:
         """
         Replicates the secret to a new Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.replicate_secret_to_regions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#replicate_secret_to_regions)
         """
-
-    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseOutputTypeDef:
+    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseTypeDef:
         """
         Cancels the scheduled deletion of a secret by removing the `DeletedDate` time
         stamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.restore_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#restore_secret)
         """
-
     def rotate_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         RotationLambdaARN: str = ...,
         RotationRules: RotationRulesTypeTypeDef = ...,
         RotateImmediately: bool = ...
-    ) -> RotateSecretResponseOutputTypeDef:
+    ) -> RotateSecretResponseTypeDef:
         """
         Configures and starts the asynchronous process of rotating the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#rotate_secret)
         """
-
     def stop_replication_to_replica(
         self, *, SecretId: str
-    ) -> StopReplicationToReplicaResponseOutputTypeDef:
+    ) -> StopReplicationToReplicaResponseTypeDef:
         """
         Removes the link between the replica secret and the primary secret and promotes
         the replica to a primary secret in the replica Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.stop_replication_to_replica)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#stop_replication_to_replica)
         """
-
     def tag_resource(
         self, *, SecretId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches tags to a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#tag_resource)
         """
-
     def untag_resource(
         self, *, SecretId: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes specific tags from a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#untag_resource)
         """
-
     def update_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...
-    ) -> UpdateSecretResponseOutputTypeDef:
+    ) -> UpdateSecretResponseTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret)
         """
-
     def update_secret_version_stage(
         self,
         *,
         SecretId: str,
         VersionStage: str,
         RemoveFromVersionId: str = ...,
         MoveToVersionId: str = ...
-    ) -> UpdateSecretVersionStageResponseOutputTypeDef:
+    ) -> UpdateSecretVersionStageResponseTypeDef:
         """
         Modifies the staging labels attached to a version of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret_version_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret_version_stage)
         """
-
     def validate_resource_policy(
         self, *, ResourcePolicy: str, SecretId: str = ...
-    ) -> ValidateResourcePolicyResponseOutputTypeDef:
+    ) -> ValidateResourcePolicyResponseTypeDef:
         """
         Validates that a resource policy does not grant a wide range of principals
         access to your secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.validate_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#validate_resource_policy)
         """
-
     def get_paginator(self, operation_name: Literal["list_secrets"]) -> ListSecretsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/client.pyi` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,55 +18,58 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import SortOrderTypeType
 from .paginator import ListSecretsPaginator
 from .type_defs import (
-    CancelRotateSecretResponseOutputTypeDef,
-    CreateSecretResponseOutputTypeDef,
-    DeleteResourcePolicyResponseOutputTypeDef,
-    DeleteSecretResponseOutputTypeDef,
-    DescribeSecretResponseOutputTypeDef,
+    CancelRotateSecretResponseTypeDef,
+    CreateSecretResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteSecretResponseTypeDef,
+    DescribeSecretResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
-    GetRandomPasswordResponseOutputTypeDef,
-    GetResourcePolicyResponseOutputTypeDef,
-    GetSecretValueResponseOutputTypeDef,
-    ListSecretsResponseOutputTypeDef,
-    ListSecretVersionIdsResponseOutputTypeDef,
-    PutResourcePolicyResponseOutputTypeDef,
-    PutSecretValueResponseOutputTypeDef,
-    RemoveRegionsFromReplicationResponseOutputTypeDef,
+    GetRandomPasswordResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSecretValueResponseTypeDef,
+    ListSecretsResponseTypeDef,
+    ListSecretVersionIdsResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSecretValueResponseTypeDef,
+    RemoveRegionsFromReplicationResponseTypeDef,
     ReplicaRegionTypeTypeDef,
-    ReplicateSecretToRegionsResponseOutputTypeDef,
-    RestoreSecretResponseOutputTypeDef,
-    RotateSecretResponseOutputTypeDef,
+    ReplicateSecretToRegionsResponseTypeDef,
+    RestoreSecretResponseTypeDef,
+    RotateSecretResponseTypeDef,
     RotationRulesTypeTypeDef,
-    StopReplicationToReplicaResponseOutputTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
     TagTypeDef,
-    UpdateSecretResponseOutputTypeDef,
-    UpdateSecretVersionStageResponseOutputTypeDef,
-    ValidateResourcePolicyResponseOutputTypeDef,
+    UpdateSecretResponseTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
+    ValidateResourcePolicyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SecretsManagerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DecryptionFailure: Type[BotocoreClientError]
     EncryptionFailure: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -74,14 +77,15 @@
     LimitExceededException: Type[BotocoreClientError]
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     PreconditionNotMetException: Type[BotocoreClientError]
     PublicPolicyException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
+
 class SecretsManagerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/)
     """
 
     meta: ClientMeta
@@ -90,298 +94,324 @@
     def exceptions(self) -> Exceptions:
         """
         SecretsManagerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#can_paginate)
         """
-    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseOutputTypeDef:
+
+    def cancel_rotate_secret(self, *, SecretId: str) -> CancelRotateSecretResponseTypeDef:
         """
         Turns off automatic rotation, and if a rotation is currently in progress,
         cancels the rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.cancel_rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#cancel_rotate_secret)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#close)
         """
+
     def create_secret(
         self,
         *,
         Name: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> CreateSecretResponseOutputTypeDef:
+    ) -> CreateSecretResponseTypeDef:
         """
         Creates a new secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.create_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#create_secret)
         """
-    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseOutputTypeDef:
+
+    def delete_resource_policy(self, *, SecretId: str) -> DeleteResourcePolicyResponseTypeDef:
         """
         Deletes the resource-based permission policy attached to the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_resource_policy)
         """
+
     def delete_secret(
         self,
         *,
         SecretId: str,
         RecoveryWindowInDays: int = ...,
         ForceDeleteWithoutRecovery: bool = ...
-    ) -> DeleteSecretResponseOutputTypeDef:
+    ) -> DeleteSecretResponseTypeDef:
         """
         Deletes a secret and all of its versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#delete_secret)
         """
-    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseOutputTypeDef:
+
+    def describe_secret(self, *, SecretId: str) -> DescribeSecretResponseTypeDef:
         """
         Retrieves the details of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.describe_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#describe_secret)
         """
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#generate_presigned_url)
         """
+
     def get_random_password(
         self,
         *,
         PasswordLength: int = ...,
         ExcludeCharacters: str = ...,
         ExcludeNumbers: bool = ...,
         ExcludePunctuation: bool = ...,
         ExcludeUppercase: bool = ...,
         ExcludeLowercase: bool = ...,
         IncludeSpace: bool = ...,
         RequireEachIncludedType: bool = ...
-    ) -> GetRandomPasswordResponseOutputTypeDef:
+    ) -> GetRandomPasswordResponseTypeDef:
         """
         Generates a random password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_random_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_random_password)
         """
-    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseOutputTypeDef:
+
+    def get_resource_policy(self, *, SecretId: str) -> GetResourcePolicyResponseTypeDef:
         """
         Retrieves the JSON text of the resource-based policy document attached to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_resource_policy)
         """
+
     def get_secret_value(
         self, *, SecretId: str, VersionId: str = ..., VersionStage: str = ...
-    ) -> GetSecretValueResponseOutputTypeDef:
+    ) -> GetSecretValueResponseTypeDef:
         """
         Retrieves the contents of the encrypted fields `SecretString` or `SecretBinary`
         from the specified version of a secret, whichever contains content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_secret_value)
         """
+
     def list_secret_version_ids(
         self,
         *,
         SecretId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         IncludeDeprecated: bool = ...
-    ) -> ListSecretVersionIdsResponseOutputTypeDef:
+    ) -> ListSecretVersionIdsResponseTypeDef:
         """
         Lists the versions of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secret_version_ids)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secret_version_ids)
         """
+
     def list_secrets(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...
-    ) -> ListSecretsResponseOutputTypeDef:
+    ) -> ListSecretsResponseTypeDef:
         """
         Lists the secrets that are stored by Secrets Manager in the Amazon Web Services
         account, not including secrets that are marked for deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secrets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#list_secrets)
         """
+
     def put_resource_policy(
         self, *, SecretId: str, ResourcePolicy: str, BlockPublicPolicy: bool = ...
-    ) -> PutResourcePolicyResponseOutputTypeDef:
+    ) -> PutResourcePolicyResponseTypeDef:
         """
         Attaches a resource-based permission policy to a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_resource_policy)
         """
+
     def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...,
         VersionStages: Sequence[str] = ...
-    ) -> PutSecretValueResponseOutputTypeDef:
+    ) -> PutSecretValueResponseTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_secret_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#put_secret_value)
         """
+
     def remove_regions_from_replication(
         self, *, SecretId: str, RemoveReplicaRegions: Sequence[str]
-    ) -> RemoveRegionsFromReplicationResponseOutputTypeDef:
+    ) -> RemoveRegionsFromReplicationResponseTypeDef:
         """
         For a secret that is replicated to other Regions, deletes the secret replicas
         from the Regions you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.remove_regions_from_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#remove_regions_from_replication)
         """
+
     def replicate_secret_to_regions(
         self,
         *,
         SecretId: str,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],
         ForceOverwriteReplicaSecret: bool = ...
-    ) -> ReplicateSecretToRegionsResponseOutputTypeDef:
+    ) -> ReplicateSecretToRegionsResponseTypeDef:
         """
         Replicates the secret to a new Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.replicate_secret_to_regions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#replicate_secret_to_regions)
         """
-    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseOutputTypeDef:
+
+    def restore_secret(self, *, SecretId: str) -> RestoreSecretResponseTypeDef:
         """
         Cancels the scheduled deletion of a secret by removing the `DeletedDate` time
         stamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.restore_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#restore_secret)
         """
+
     def rotate_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         RotationLambdaARN: str = ...,
         RotationRules: RotationRulesTypeTypeDef = ...,
         RotateImmediately: bool = ...
-    ) -> RotateSecretResponseOutputTypeDef:
+    ) -> RotateSecretResponseTypeDef:
         """
         Configures and starts the asynchronous process of rotating the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.rotate_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#rotate_secret)
         """
+
     def stop_replication_to_replica(
         self, *, SecretId: str
-    ) -> StopReplicationToReplicaResponseOutputTypeDef:
+    ) -> StopReplicationToReplicaResponseTypeDef:
         """
         Removes the link between the replica secret and the primary secret and promotes
         the replica to a primary secret in the replica Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.stop_replication_to_replica)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#stop_replication_to_replica)
         """
+
     def tag_resource(
         self, *, SecretId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches tags to a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#tag_resource)
         """
+
     def untag_resource(
         self, *, SecretId: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes specific tags from a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#untag_resource)
         """
+
     def update_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
         SecretString: str = ...
-    ) -> UpdateSecretResponseOutputTypeDef:
+    ) -> UpdateSecretResponseTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret)
         """
+
     def update_secret_version_stage(
         self,
         *,
         SecretId: str,
         VersionStage: str,
         RemoveFromVersionId: str = ...,
         MoveToVersionId: str = ...
-    ) -> UpdateSecretVersionStageResponseOutputTypeDef:
+    ) -> UpdateSecretVersionStageResponseTypeDef:
         """
         Modifies the staging labels attached to a version of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret_version_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#update_secret_version_stage)
         """
+
     def validate_resource_policy(
         self, *, ResourcePolicy: str, SecretId: str = ...
-    ) -> ValidateResourcePolicyResponseOutputTypeDef:
+    ) -> ValidateResourcePolicyResponseTypeDef:
         """
         Validates that a resource policy does not grant a wide range of principals
         access to your secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.validate_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#validate_resource_policy)
         """
+
     def get_paginator(self, operation_name: Literal["list_secrets"]) -> ListSecretsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.py` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/literals.pyi` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.py` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderTypeType
-from .type_defs import FilterTypeDef, ListSecretsResponseOutputTypeDef, PaginatorConfigTypeDef
+from .type_defs import FilterTypeDef, ListSecretsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListSecretsPaginator",)
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
@@ -48,12 +48,12 @@
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecretsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/paginator.pyi` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderTypeType
-from .type_defs import FilterTypeDef, ListSecretsResponseOutputTypeDef, PaginatorConfigTypeDef
+from .type_defs import FilterTypeDef, ListSecretsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListSecretsPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -45,12 +45,12 @@
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSecretsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.py` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -20,83 +20,82 @@
 from .literals import FilterNameStringTypeType, SortOrderTypeType, StatusTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelRotateSecretRequestRequestTypeDef",
-    "CancelRotateSecretResponseOutputTypeDef",
+    "CancelRotateSecretResponseTypeDef",
     "ReplicaRegionTypeTypeDef",
     "TagTypeDef",
-    "ReplicationStatusTypeOutputTypeDef",
+    "ReplicationStatusTypeTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseOutputTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
     "DeleteSecretRequestRequestTypeDef",
-    "DeleteSecretResponseOutputTypeDef",
+    "DeleteSecretResponseTypeDef",
     "DescribeSecretRequestRequestTypeDef",
     "RotationRulesTypeOutputTypeDef",
     "TagOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FilterTypeDef",
     "GetRandomPasswordRequestRequestTypeDef",
-    "GetRandomPasswordResponseOutputTypeDef",
+    "GetRandomPasswordResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseOutputTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetSecretValueRequestRequestTypeDef",
-    "GetSecretValueResponseOutputTypeDef",
+    "GetSecretValueResponseTypeDef",
     "ListSecretVersionIdsRequestRequestTypeDef",
-    "SecretVersionsListEntryOutputTypeDef",
+    "SecretVersionsListEntryTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseOutputTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "PutSecretValueRequestRequestTypeDef",
-    "PutSecretValueResponseOutputTypeDef",
+    "PutSecretValueResponseTypeDef",
     "RemoveRegionsFromReplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreSecretRequestRequestTypeDef",
-    "RestoreSecretResponseOutputTypeDef",
+    "RestoreSecretResponseTypeDef",
     "RotationRulesTypeTypeDef",
-    "RotateSecretResponseOutputTypeDef",
+    "RotateSecretResponseTypeDef",
     "StopReplicationToReplicaRequestRequestTypeDef",
-    "StopReplicationToReplicaResponseOutputTypeDef",
+    "StopReplicationToReplicaResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSecretRequestRequestTypeDef",
-    "UpdateSecretResponseOutputTypeDef",
+    "UpdateSecretResponseTypeDef",
     "UpdateSecretVersionStageRequestRequestTypeDef",
-    "UpdateSecretVersionStageResponseOutputTypeDef",
+    "UpdateSecretVersionStageResponseTypeDef",
     "ValidateResourcePolicyRequestRequestTypeDef",
-    "ValidationErrorsEntryOutputTypeDef",
+    "ValidationErrorsEntryTypeDef",
     "ReplicateSecretToRegionsRequestRequestTypeDef",
     "CreateSecretRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateSecretResponseOutputTypeDef",
-    "RemoveRegionsFromReplicationResponseOutputTypeDef",
-    "ReplicateSecretToRegionsResponseOutputTypeDef",
-    "DescribeSecretResponseOutputTypeDef",
-    "SecretListEntryOutputTypeDef",
+    "CreateSecretResponseTypeDef",
+    "RemoveRegionsFromReplicationResponseTypeDef",
+    "ReplicateSecretToRegionsResponseTypeDef",
+    "DescribeSecretResponseTypeDef",
+    "SecretListEntryTypeDef",
     "ListSecretsRequestListSecretsPaginateTypeDef",
     "ListSecretsRequestRequestTypeDef",
-    "ListSecretVersionIdsResponseOutputTypeDef",
+    "ListSecretVersionIdsResponseTypeDef",
     "RotateSecretRequestRequestTypeDef",
-    "ValidateResourcePolicyResponseOutputTypeDef",
-    "ListSecretsResponseOutputTypeDef",
+    "ValidateResourcePolicyResponseTypeDef",
+    "ListSecretsResponseTypeDef",
 )
 
 CancelRotateSecretRequestRequestTypeDef = TypedDict(
     "CancelRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-CancelRotateSecretResponseOutputTypeDef = TypedDict(
-    "CancelRotateSecretResponseOutputTypeDef",
+CancelRotateSecretResponseTypeDef = TypedDict(
+    "CancelRotateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -115,16 +114,16 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ReplicationStatusTypeOutputTypeDef = TypedDict(
-    "ReplicationStatusTypeOutputTypeDef",
+ReplicationStatusTypeTypeDef = TypedDict(
+    "ReplicationStatusTypeTypeDef",
     {
         "Region": str,
         "KmsKeyId": str,
         "Status": StatusTypeType,
         "StatusMessage": str,
         "LastAccessedDate": datetime,
     },
@@ -133,16 +132,16 @@
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-DeleteResourcePolicyResponseOutputTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseOutputTypeDef",
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -157,23 +156,21 @@
     {
         "RecoveryWindowInDays": int,
         "ForceDeleteWithoutRecovery": bool,
     },
     total=False,
 )
 
-
 class DeleteSecretRequestRequestTypeDef(
     _RequiredDeleteSecretRequestRequestTypeDef, _OptionalDeleteSecretRequestRequestTypeDef
 ):
     pass
 
-
-DeleteSecretResponseOutputTypeDef = TypedDict(
-    "DeleteSecretResponseOutputTypeDef",
+DeleteSecretResponseTypeDef = TypedDict(
+    "DeleteSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "DeletionDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -229,31 +226,31 @@
         "ExcludeLowercase": bool,
         "IncludeSpace": bool,
         "RequireEachIncludedType": bool,
     },
     total=False,
 )
 
-GetRandomPasswordResponseOutputTypeDef = TypedDict(
-    "GetRandomPasswordResponseOutputTypeDef",
+GetRandomPasswordResponseTypeDef = TypedDict(
+    "GetRandomPasswordResponseTypeDef",
     {
         "RandomPassword": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-GetResourcePolicyResponseOutputTypeDef = TypedDict(
-    "GetResourcePolicyResponseOutputTypeDef",
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResourcePolicy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -269,23 +266,21 @@
     {
         "VersionId": str,
         "VersionStage": str,
     },
     total=False,
 )
 
-
 class GetSecretValueRequestRequestTypeDef(
     _RequiredGetSecretValueRequestRequestTypeDef, _OptionalGetSecretValueRequestRequestTypeDef
 ):
     pass
 
-
-GetSecretValueResponseOutputTypeDef = TypedDict(
-    "GetSecretValueResponseOutputTypeDef",
+GetSecretValueResponseTypeDef = TypedDict(
+    "GetSecretValueResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "SecretBinary": bytes,
         "SecretString": str,
         "VersionStages": List[str],
@@ -306,24 +301,22 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeDeprecated": bool,
     },
     total=False,
 )
 
-
 class ListSecretVersionIdsRequestRequestTypeDef(
     _RequiredListSecretVersionIdsRequestRequestTypeDef,
     _OptionalListSecretVersionIdsRequestRequestTypeDef,
 ):
     pass
 
-
-SecretVersionsListEntryOutputTypeDef = TypedDict(
-    "SecretVersionsListEntryOutputTypeDef",
+SecretVersionsListEntryTypeDef = TypedDict(
+    "SecretVersionsListEntryTypeDef",
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
         "KmsKeyIds": List[str],
     },
@@ -350,23 +343,21 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "BlockPublicPolicy": bool,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutResourcePolicyResponseOutputTypeDef = TypedDict(
-    "PutResourcePolicyResponseOutputTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -383,23 +374,21 @@
         "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
         "SecretString": str,
         "VersionStages": Sequence[str],
     },
     total=False,
 )
 
-
 class PutSecretValueRequestRequestTypeDef(
     _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
 ):
     pass
 
-
-PutSecretValueResponseOutputTypeDef = TypedDict(
-    "PutSecretValueResponseOutputTypeDef",
+PutSecretValueResponseTypeDef = TypedDict(
+    "PutSecretValueResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "VersionStages": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -427,16 +416,16 @@
 RestoreSecretRequestRequestTypeDef = TypedDict(
     "RestoreSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-RestoreSecretResponseOutputTypeDef = TypedDict(
-    "RestoreSecretResponseOutputTypeDef",
+RestoreSecretResponseTypeDef = TypedDict(
+    "RestoreSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -446,16 +435,16 @@
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
     },
     total=False,
 )
 
-RotateSecretResponseOutputTypeDef = TypedDict(
-    "RotateSecretResponseOutputTypeDef",
+RotateSecretResponseTypeDef = TypedDict(
+    "RotateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -463,16 +452,16 @@
 StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
     "StopReplicationToReplicaRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-StopReplicationToReplicaResponseOutputTypeDef = TypedDict(
-    "StopReplicationToReplicaResponseOutputTypeDef",
+StopReplicationToReplicaResponseTypeDef = TypedDict(
+    "StopReplicationToReplicaResponseTypeDef",
     {
         "ARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -497,23 +486,21 @@
         "KmsKeyId": str,
         "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
         "SecretString": str,
     },
     total=False,
 )
 
-
 class UpdateSecretRequestRequestTypeDef(
     _RequiredUpdateSecretRequestRequestTypeDef, _OptionalUpdateSecretRequestRequestTypeDef
 ):
     pass
 
-
-UpdateSecretResponseOutputTypeDef = TypedDict(
-    "UpdateSecretResponseOutputTypeDef",
+UpdateSecretResponseTypeDef = TypedDict(
+    "UpdateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -530,24 +517,22 @@
     {
         "RemoveFromVersionId": str,
         "MoveToVersionId": str,
     },
     total=False,
 )
 
-
 class UpdateSecretVersionStageRequestRequestTypeDef(
     _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
     _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateSecretVersionStageResponseOutputTypeDef = TypedDict(
-    "UpdateSecretVersionStageResponseOutputTypeDef",
+UpdateSecretVersionStageResponseTypeDef = TypedDict(
+    "UpdateSecretVersionStageResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -561,24 +546,22 @@
     "_OptionalValidateResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
     total=False,
 )
 
-
 class ValidateResourcePolicyRequestRequestTypeDef(
     _RequiredValidateResourcePolicyRequestRequestTypeDef,
     _OptionalValidateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-ValidationErrorsEntryOutputTypeDef = TypedDict(
-    "ValidationErrorsEntryOutputTypeDef",
+ValidationErrorsEntryTypeDef = TypedDict(
+    "ValidationErrorsEntryTypeDef",
     {
         "CheckName": str,
         "ErrorMessage": str,
     },
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
@@ -592,22 +575,20 @@
     "_OptionalReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
-
 class ReplicateSecretToRegionsRequestRequestTypeDef(
     _RequiredReplicateSecretToRegionsRequestRequestTypeDef,
     _OptionalReplicateSecretToRegionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecretRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateSecretRequestRequestTypeDef = TypedDict(
@@ -621,60 +602,58 @@
         "Tags": Sequence[TagTypeDef],
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
-
 class CreateSecretRequestRequestTypeDef(
     _RequiredCreateSecretRequestRequestTypeDef, _OptionalCreateSecretRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "SecretId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateSecretResponseOutputTypeDef = TypedDict(
-    "CreateSecretResponseOutputTypeDef",
+CreateSecretResponseTypeDef = TypedDict(
+    "CreateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveRegionsFromReplicationResponseOutputTypeDef = TypedDict(
-    "RemoveRegionsFromReplicationResponseOutputTypeDef",
+RemoveRegionsFromReplicationResponseTypeDef = TypedDict(
+    "RemoveRegionsFromReplicationResponseTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicateSecretToRegionsResponseOutputTypeDef = TypedDict(
-    "ReplicateSecretToRegionsResponseOutputTypeDef",
+ReplicateSecretToRegionsResponseTypeDef = TypedDict(
+    "ReplicateSecretToRegionsResponseTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSecretResponseOutputTypeDef = TypedDict(
-    "DescribeSecretResponseOutputTypeDef",
+DescribeSecretResponseTypeDef = TypedDict(
+    "DescribeSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
@@ -685,21 +664,21 @@
         "DeletedDate": datetime,
         "NextRotationDate": datetime,
         "Tags": List[TagOutputTypeDef],
         "VersionIdsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SecretListEntryOutputTypeDef = TypedDict(
-    "SecretListEntryOutputTypeDef",
+SecretListEntryTypeDef = TypedDict(
+    "SecretListEntryTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
@@ -736,18 +715,18 @@
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortOrder": SortOrderTypeType,
     },
     total=False,
 )
 
-ListSecretVersionIdsResponseOutputTypeDef = TypedDict(
-    "ListSecretVersionIdsResponseOutputTypeDef",
+ListSecretVersionIdsResponseTypeDef = TypedDict(
+    "ListSecretVersionIdsResponseTypeDef",
     {
-        "Versions": List[SecretVersionsListEntryOutputTypeDef],
+        "Versions": List[SecretVersionsListEntryTypeDef],
         "NextToken": str,
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -764,31 +743,29 @@
         "RotationLambdaARN": str,
         "RotationRules": RotationRulesTypeTypeDef,
         "RotateImmediately": bool,
     },
     total=False,
 )
 
-
 class RotateSecretRequestRequestTypeDef(
     _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
 ):
     pass
 
-
-ValidateResourcePolicyResponseOutputTypeDef = TypedDict(
-    "ValidateResourcePolicyResponseOutputTypeDef",
+ValidateResourcePolicyResponseTypeDef = TypedDict(
+    "ValidateResourcePolicyResponseTypeDef",
     {
         "PolicyValidationPassed": bool,
-        "ValidationErrors": List[ValidationErrorsEntryOutputTypeDef],
+        "ValidationErrors": List[ValidationErrorsEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSecretsResponseOutputTypeDef = TypedDict(
-    "ListSecretsResponseOutputTypeDef",
+ListSecretsResponseTypeDef = TypedDict(
+    "ListSecretsResponseTypeDef",
     {
-        "SecretList": List[SecretListEntryOutputTypeDef],
+        "SecretList": List[SecretListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager/type_defs.pyi` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,82 +20,83 @@
 from .literals import FilterNameStringTypeType, SortOrderTypeType, StatusTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelRotateSecretRequestRequestTypeDef",
-    "CancelRotateSecretResponseOutputTypeDef",
+    "CancelRotateSecretResponseTypeDef",
     "ReplicaRegionTypeTypeDef",
     "TagTypeDef",
-    "ReplicationStatusTypeOutputTypeDef",
+    "ReplicationStatusTypeTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseOutputTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
     "DeleteSecretRequestRequestTypeDef",
-    "DeleteSecretResponseOutputTypeDef",
+    "DeleteSecretResponseTypeDef",
     "DescribeSecretRequestRequestTypeDef",
     "RotationRulesTypeOutputTypeDef",
     "TagOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FilterTypeDef",
     "GetRandomPasswordRequestRequestTypeDef",
-    "GetRandomPasswordResponseOutputTypeDef",
+    "GetRandomPasswordResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseOutputTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetSecretValueRequestRequestTypeDef",
-    "GetSecretValueResponseOutputTypeDef",
+    "GetSecretValueResponseTypeDef",
     "ListSecretVersionIdsRequestRequestTypeDef",
-    "SecretVersionsListEntryOutputTypeDef",
+    "SecretVersionsListEntryTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseOutputTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "PutSecretValueRequestRequestTypeDef",
-    "PutSecretValueResponseOutputTypeDef",
+    "PutSecretValueResponseTypeDef",
     "RemoveRegionsFromReplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreSecretRequestRequestTypeDef",
-    "RestoreSecretResponseOutputTypeDef",
+    "RestoreSecretResponseTypeDef",
     "RotationRulesTypeTypeDef",
-    "RotateSecretResponseOutputTypeDef",
+    "RotateSecretResponseTypeDef",
     "StopReplicationToReplicaRequestRequestTypeDef",
-    "StopReplicationToReplicaResponseOutputTypeDef",
+    "StopReplicationToReplicaResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSecretRequestRequestTypeDef",
-    "UpdateSecretResponseOutputTypeDef",
+    "UpdateSecretResponseTypeDef",
     "UpdateSecretVersionStageRequestRequestTypeDef",
-    "UpdateSecretVersionStageResponseOutputTypeDef",
+    "UpdateSecretVersionStageResponseTypeDef",
     "ValidateResourcePolicyRequestRequestTypeDef",
-    "ValidationErrorsEntryOutputTypeDef",
+    "ValidationErrorsEntryTypeDef",
     "ReplicateSecretToRegionsRequestRequestTypeDef",
     "CreateSecretRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateSecretResponseOutputTypeDef",
-    "RemoveRegionsFromReplicationResponseOutputTypeDef",
-    "ReplicateSecretToRegionsResponseOutputTypeDef",
-    "DescribeSecretResponseOutputTypeDef",
-    "SecretListEntryOutputTypeDef",
+    "CreateSecretResponseTypeDef",
+    "RemoveRegionsFromReplicationResponseTypeDef",
+    "ReplicateSecretToRegionsResponseTypeDef",
+    "DescribeSecretResponseTypeDef",
+    "SecretListEntryTypeDef",
     "ListSecretsRequestListSecretsPaginateTypeDef",
     "ListSecretsRequestRequestTypeDef",
-    "ListSecretVersionIdsResponseOutputTypeDef",
+    "ListSecretVersionIdsResponseTypeDef",
     "RotateSecretRequestRequestTypeDef",
-    "ValidateResourcePolicyResponseOutputTypeDef",
-    "ListSecretsResponseOutputTypeDef",
+    "ValidateResourcePolicyResponseTypeDef",
+    "ListSecretsResponseTypeDef",
 )
 
 CancelRotateSecretRequestRequestTypeDef = TypedDict(
     "CancelRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-CancelRotateSecretResponseOutputTypeDef = TypedDict(
-    "CancelRotateSecretResponseOutputTypeDef",
+CancelRotateSecretResponseTypeDef = TypedDict(
+    "CancelRotateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -114,16 +115,16 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ReplicationStatusTypeOutputTypeDef = TypedDict(
-    "ReplicationStatusTypeOutputTypeDef",
+ReplicationStatusTypeTypeDef = TypedDict(
+    "ReplicationStatusTypeTypeDef",
     {
         "Region": str,
         "KmsKeyId": str,
         "Status": StatusTypeType,
         "StatusMessage": str,
         "LastAccessedDate": datetime,
     },
@@ -132,16 +133,16 @@
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-DeleteResourcePolicyResponseOutputTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseOutputTypeDef",
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -156,21 +157,23 @@
     {
         "RecoveryWindowInDays": int,
         "ForceDeleteWithoutRecovery": bool,
     },
     total=False,
 )
 
+
 class DeleteSecretRequestRequestTypeDef(
     _RequiredDeleteSecretRequestRequestTypeDef, _OptionalDeleteSecretRequestRequestTypeDef
 ):
     pass
 
-DeleteSecretResponseOutputTypeDef = TypedDict(
-    "DeleteSecretResponseOutputTypeDef",
+
+DeleteSecretResponseTypeDef = TypedDict(
+    "DeleteSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "DeletionDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -226,31 +229,31 @@
         "ExcludeLowercase": bool,
         "IncludeSpace": bool,
         "RequireEachIncludedType": bool,
     },
     total=False,
 )
 
-GetRandomPasswordResponseOutputTypeDef = TypedDict(
-    "GetRandomPasswordResponseOutputTypeDef",
+GetRandomPasswordResponseTypeDef = TypedDict(
+    "GetRandomPasswordResponseTypeDef",
     {
         "RandomPassword": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-GetResourcePolicyResponseOutputTypeDef = TypedDict(
-    "GetResourcePolicyResponseOutputTypeDef",
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResourcePolicy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -266,21 +269,23 @@
     {
         "VersionId": str,
         "VersionStage": str,
     },
     total=False,
 )
 
+
 class GetSecretValueRequestRequestTypeDef(
     _RequiredGetSecretValueRequestRequestTypeDef, _OptionalGetSecretValueRequestRequestTypeDef
 ):
     pass
 
-GetSecretValueResponseOutputTypeDef = TypedDict(
-    "GetSecretValueResponseOutputTypeDef",
+
+GetSecretValueResponseTypeDef = TypedDict(
+    "GetSecretValueResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "SecretBinary": bytes,
         "SecretString": str,
         "VersionStages": List[str],
@@ -301,22 +306,24 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeDeprecated": bool,
     },
     total=False,
 )
 
+
 class ListSecretVersionIdsRequestRequestTypeDef(
     _RequiredListSecretVersionIdsRequestRequestTypeDef,
     _OptionalListSecretVersionIdsRequestRequestTypeDef,
 ):
     pass
 
-SecretVersionsListEntryOutputTypeDef = TypedDict(
-    "SecretVersionsListEntryOutputTypeDef",
+
+SecretVersionsListEntryTypeDef = TypedDict(
+    "SecretVersionsListEntryTypeDef",
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
         "KmsKeyIds": List[str],
     },
@@ -343,21 +350,23 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "BlockPublicPolicy": bool,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseOutputTypeDef = TypedDict(
-    "PutResourcePolicyResponseOutputTypeDef",
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -374,21 +383,23 @@
         "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
         "SecretString": str,
         "VersionStages": Sequence[str],
     },
     total=False,
 )
 
+
 class PutSecretValueRequestRequestTypeDef(
     _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
 ):
     pass
 
-PutSecretValueResponseOutputTypeDef = TypedDict(
-    "PutSecretValueResponseOutputTypeDef",
+
+PutSecretValueResponseTypeDef = TypedDict(
+    "PutSecretValueResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "VersionStages": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -416,16 +427,16 @@
 RestoreSecretRequestRequestTypeDef = TypedDict(
     "RestoreSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-RestoreSecretResponseOutputTypeDef = TypedDict(
-    "RestoreSecretResponseOutputTypeDef",
+RestoreSecretResponseTypeDef = TypedDict(
+    "RestoreSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -435,16 +446,16 @@
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
     },
     total=False,
 )
 
-RotateSecretResponseOutputTypeDef = TypedDict(
-    "RotateSecretResponseOutputTypeDef",
+RotateSecretResponseTypeDef = TypedDict(
+    "RotateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -452,16 +463,16 @@
 StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
     "StopReplicationToReplicaRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-StopReplicationToReplicaResponseOutputTypeDef = TypedDict(
-    "StopReplicationToReplicaResponseOutputTypeDef",
+StopReplicationToReplicaResponseTypeDef = TypedDict(
+    "StopReplicationToReplicaResponseTypeDef",
     {
         "ARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -486,21 +497,23 @@
         "KmsKeyId": str,
         "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
         "SecretString": str,
     },
     total=False,
 )
 
+
 class UpdateSecretRequestRequestTypeDef(
     _RequiredUpdateSecretRequestRequestTypeDef, _OptionalUpdateSecretRequestRequestTypeDef
 ):
     pass
 
-UpdateSecretResponseOutputTypeDef = TypedDict(
-    "UpdateSecretResponseOutputTypeDef",
+
+UpdateSecretResponseTypeDef = TypedDict(
+    "UpdateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -517,22 +530,24 @@
     {
         "RemoveFromVersionId": str,
         "MoveToVersionId": str,
     },
     total=False,
 )
 
+
 class UpdateSecretVersionStageRequestRequestTypeDef(
     _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
     _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
 ):
     pass
 
-UpdateSecretVersionStageResponseOutputTypeDef = TypedDict(
-    "UpdateSecretVersionStageResponseOutputTypeDef",
+
+UpdateSecretVersionStageResponseTypeDef = TypedDict(
+    "UpdateSecretVersionStageResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -546,22 +561,24 @@
     "_OptionalValidateResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
     total=False,
 )
 
+
 class ValidateResourcePolicyRequestRequestTypeDef(
     _RequiredValidateResourcePolicyRequestRequestTypeDef,
     _OptionalValidateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-ValidationErrorsEntryOutputTypeDef = TypedDict(
-    "ValidationErrorsEntryOutputTypeDef",
+
+ValidationErrorsEntryTypeDef = TypedDict(
+    "ValidationErrorsEntryTypeDef",
     {
         "CheckName": str,
         "ErrorMessage": str,
     },
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
@@ -575,20 +592,22 @@
     "_OptionalReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
+
 class ReplicateSecretToRegionsRequestRequestTypeDef(
     _RequiredReplicateSecretToRegionsRequestRequestTypeDef,
     _OptionalReplicateSecretToRegionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecretRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateSecretRequestRequestTypeDef = TypedDict(
@@ -602,58 +621,60 @@
         "Tags": Sequence[TagTypeDef],
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
+
 class CreateSecretRequestRequestTypeDef(
     _RequiredCreateSecretRequestRequestTypeDef, _OptionalCreateSecretRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "SecretId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateSecretResponseOutputTypeDef = TypedDict(
-    "CreateSecretResponseOutputTypeDef",
+CreateSecretResponseTypeDef = TypedDict(
+    "CreateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveRegionsFromReplicationResponseOutputTypeDef = TypedDict(
-    "RemoveRegionsFromReplicationResponseOutputTypeDef",
+RemoveRegionsFromReplicationResponseTypeDef = TypedDict(
+    "RemoveRegionsFromReplicationResponseTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicateSecretToRegionsResponseOutputTypeDef = TypedDict(
-    "ReplicateSecretToRegionsResponseOutputTypeDef",
+ReplicateSecretToRegionsResponseTypeDef = TypedDict(
+    "ReplicateSecretToRegionsResponseTypeDef",
     {
         "ARN": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSecretResponseOutputTypeDef = TypedDict(
-    "DescribeSecretResponseOutputTypeDef",
+DescribeSecretResponseTypeDef = TypedDict(
+    "DescribeSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
@@ -664,21 +685,21 @@
         "DeletedDate": datetime,
         "NextRotationDate": datetime,
         "Tags": List[TagOutputTypeDef],
         "VersionIdsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
-        "ReplicationStatus": List[ReplicationStatusTypeOutputTypeDef],
+        "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SecretListEntryOutputTypeDef = TypedDict(
-    "SecretListEntryOutputTypeDef",
+SecretListEntryTypeDef = TypedDict(
+    "SecretListEntryTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaARN": str,
@@ -715,18 +736,18 @@
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortOrder": SortOrderTypeType,
     },
     total=False,
 )
 
-ListSecretVersionIdsResponseOutputTypeDef = TypedDict(
-    "ListSecretVersionIdsResponseOutputTypeDef",
+ListSecretVersionIdsResponseTypeDef = TypedDict(
+    "ListSecretVersionIdsResponseTypeDef",
     {
-        "Versions": List[SecretVersionsListEntryOutputTypeDef],
+        "Versions": List[SecretVersionsListEntryTypeDef],
         "NextToken": str,
         "ARN": str,
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -743,29 +764,31 @@
         "RotationLambdaARN": str,
         "RotationRules": RotationRulesTypeTypeDef,
         "RotateImmediately": bool,
     },
     total=False,
 )
 
+
 class RotateSecretRequestRequestTypeDef(
     _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
 ):
     pass
 
-ValidateResourcePolicyResponseOutputTypeDef = TypedDict(
-    "ValidateResourcePolicyResponseOutputTypeDef",
+
+ValidateResourcePolicyResponseTypeDef = TypedDict(
+    "ValidateResourcePolicyResponseTypeDef",
     {
         "PolicyValidationPassed": bool,
-        "ValidationErrors": List[ValidationErrorsEntryOutputTypeDef],
+        "ValidationErrors": List[ValidationErrorsEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSecretsResponseOutputTypeDef = TypedDict(
-    "ListSecretsResponseOutputTypeDef",
+ListSecretsResponseTypeDef = TypedDict(
+    "ListSecretsResponseTypeDef",
     {
-        "SecretList": List[SecretListEntryOutputTypeDef],
+        "SecretList": List[SecretListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/PKG-INFO` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,69 +324,69 @@
 
 `mypy_boto3_secretsmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_secretsmanager.type_defs import (
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseOutputTypeDef,
+    CancelRotateSecretResponseTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
-    ReplicationStatusTypeOutputTypeDef,
+    ReplicationStatusTypeTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseOutputTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseOutputTypeDef,
+    DeleteSecretResponseTypeDef,
     DescribeSecretRequestRequestTypeDef,
     RotationRulesTypeOutputTypeDef,
     TagOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseOutputTypeDef,
+    GetRandomPasswordResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseOutputTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseOutputTypeDef,
+    GetSecretValueResponseTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryOutputTypeDef,
+    SecretVersionsListEntryTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseOutputTypeDef,
+    PutResourcePolicyResponseTypeDef,
     PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseOutputTypeDef,
+    PutSecretValueResponseTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseOutputTypeDef,
+    RestoreSecretResponseTypeDef,
     RotationRulesTypeTypeDef,
-    RotateSecretResponseOutputTypeDef,
+    RotateSecretResponseTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseOutputTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseOutputTypeDef,
+    UpdateSecretResponseTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseOutputTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryOutputTypeDef,
+    ValidationErrorsEntryTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateSecretResponseOutputTypeDef,
-    RemoveRegionsFromReplicationResponseOutputTypeDef,
-    ReplicateSecretToRegionsResponseOutputTypeDef,
-    DescribeSecretResponseOutputTypeDef,
-    SecretListEntryOutputTypeDef,
+    CreateSecretResponseTypeDef,
+    RemoveRegionsFromReplicationResponseTypeDef,
+    ReplicateSecretToRegionsResponseTypeDef,
+    DescribeSecretResponseTypeDef,
+    SecretListEntryTypeDef,
     ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseOutputTypeDef,
+    ListSecretVersionIdsResponseTypeDef,
     RotateSecretRequestRequestTypeDef,
-    ValidateResourcePolicyResponseOutputTypeDef,
-    ListSecretsResponseOutputTypeDef,
+    ValidateResourcePolicyResponseTypeDef,
+    ListSecretsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/mypy_boto3_secretsmanager.egg-info/SOURCES.txt` & `mypy-boto3-secretsmanager-1.28.3.post2/mypy_boto3_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.3.post1/setup.py` & `mypy-boto3-secretsmanager-1.28.3.post2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-secretsmanager",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder"
-        " 7.14.7"
+        " 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

