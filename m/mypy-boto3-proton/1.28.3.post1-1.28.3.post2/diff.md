# Comparing `tmp/mypy-boto3-proton-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-proton-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-proton-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
+gzip compressed data, was "mypy-boto3-proton-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:35 2023, max compression
```

## Comparing `mypy-boto3-proton-1.28.3.post1.tar` & `mypy-boto3-proton-1.28.3.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32134 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.023733 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75426 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    75301 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-07-14 16:16:59.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26749 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   107926 2023-07-14 16:17:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   107803 2023-07-14 16:17:00.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-14 16:16:58.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32134 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:18:02.000000 mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.031734 mypy-boto3-proton-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-14 16:16:57.000000 mypy-boto3-proton-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.230399 mypy-boto3-proton-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31335 2023-07-15 06:38:35.230399 mypy-boto3-proton-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29848 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.230399 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74390 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74265 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-07-15 06:37:31.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-15 06:37:31.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   104793 2023-07-15 06:37:34.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104670 2023-07-15 06:37:33.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-15 06:37:30.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.230399 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31335 2023-07-15 06:38:35.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-15 06:38:35.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:35.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 06:38:35.000000 mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:35.230399 mypy-boto3-proton-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-15 06:37:29.000000 mypy-boto3-proton-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-proton-1.28.3.post1/LICENSE` & `mypy-boto3-proton-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/PKG-INFO` & `mypy-boto3-proton-1.28.3.post2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-proton
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.7
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 proton type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-proton"></a>
 
 # mypy-boto3-proton
 
 [![PyPI - mypy-boto3-proton](https://img.shields.io/pypi/v/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -494,84 +462,84 @@
 
 `mypy_boto3_proton.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_proton.type_defs import (
     AcceptEnvironmentAccountConnectionInputRequestTypeDef,
-    EnvironmentAccountConnectionOutputTypeDef,
-    RepositoryBranchOutputTypeDef,
+    EnvironmentAccountConnectionTypeDef,
+    RepositoryBranchTypeDef,
     CancelComponentDeploymentInputRequestTypeDef,
-    ComponentOutputTypeDef,
+    ComponentTypeDef,
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
-    ServiceInstanceOutputTypeDef,
+    ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
-    ServicePipelineOutputTypeDef,
+    ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
-    CompatibleEnvironmentTemplateOutputTypeDef,
-    ComponentStateOutputTypeDef,
-    ComponentSummaryOutputTypeDef,
-    ResourceCountsSummaryOutputTypeDef,
+    CompatibleEnvironmentTemplateTypeDef,
+    ComponentStateTypeDef,
+    ComponentSummaryTypeDef,
+    ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
-    EnvironmentTemplateOutputTypeDef,
-    EnvironmentTemplateVersionOutputTypeDef,
-    RepositoryOutputTypeDef,
+    EnvironmentTemplateTypeDef,
+    EnvironmentTemplateVersionTypeDef,
+    RepositoryTypeDef,
     CreateServiceSyncConfigInputRequestTypeDef,
-    ServiceSyncConfigOutputTypeDef,
-    ServiceTemplateOutputTypeDef,
+    ServiceSyncConfigTypeDef,
+    ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
-    TemplateSyncConfigOutputTypeDef,
+    TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
     DeleteDeploymentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
     DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
-    EnvironmentStateOutputTypeDef,
-    ServiceInstanceStateOutputTypeDef,
-    ServicePipelineStateOutputTypeDef,
-    DeploymentSummaryOutputTypeDef,
-    EnvironmentAccountConnectionSummaryOutputTypeDef,
-    EnvironmentSummaryOutputTypeDef,
+    EnvironmentStateTypeDef,
+    ServiceInstanceStateTypeDef,
+    ServicePipelineStateTypeDef,
+    DeploymentSummaryTypeDef,
+    EnvironmentAccountConnectionSummaryTypeDef,
+    EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
-    EnvironmentTemplateSummaryOutputTypeDef,
-    EnvironmentTemplateVersionSummaryOutputTypeDef,
+    EnvironmentTemplateSummaryTypeDef,
+    EnvironmentTemplateVersionSummaryTypeDef,
     WaiterConfigTypeDef,
     GetComponentInputRequestTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetEnvironmentAccountConnectionInputRequestTypeDef,
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
     GetServiceInstanceInputRequestTypeDef,
     GetServiceInstanceSyncStatusInputRequestTypeDef,
-    RevisionOutputTypeDef,
+    RevisionTypeDef,
     GetServiceSyncBlockerSummaryInputRequestTypeDef,
     GetServiceSyncConfigInputRequestTypeDef,
     GetServiceTemplateInputRequestTypeDef,
     GetServiceTemplateVersionInputRequestTypeDef,
     GetTemplateSyncConfigInputRequestTypeDef,
     GetTemplateSyncStatusInputRequestTypeDef,
     ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
     ListComponentOutputsInputRequestTypeDef,
-    OutputOutputTypeDef,
+    OutputTypeDef,
     ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
-    ProvisionedResourceOutputTypeDef,
+    ProvisionedResourceTypeDef,
     ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
     ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
     ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
@@ -580,185 +548,184 @@
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
     ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
     ListEnvironmentTemplateVersionsInputRequestTypeDef,
     ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
     ListEnvironmentTemplatesInputRequestTypeDef,
     ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
-    RepositorySummaryOutputTypeDef,
+    RepositorySummaryTypeDef,
     ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
     ListRepositorySyncDefinitionsInputRequestTypeDef,
-    RepositorySyncDefinitionOutputTypeDef,
+    RepositorySyncDefinitionTypeDef,
     ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
     ListServiceInstanceOutputsInputRequestTypeDef,
     ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
     ListServiceInstanceProvisionedResourcesInputRequestTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ServiceInstanceSummaryOutputTypeDef,
+    ServiceInstanceSummaryTypeDef,
     ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
     ListServicePipelineOutputsInputRequestTypeDef,
     ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
     ListServicePipelineProvisionedResourcesInputRequestTypeDef,
     ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
     ListServiceTemplateVersionsInputRequestTypeDef,
-    ServiceTemplateVersionSummaryOutputTypeDef,
+    ServiceTemplateVersionSummaryTypeDef,
     ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
     ListServiceTemplatesInputRequestTypeDef,
-    ServiceTemplateSummaryOutputTypeDef,
+    ServiceTemplateSummaryTypeDef,
     ListServicesInputListServicesPaginateTypeDef,
     ListServicesInputRequestTypeDef,
-    ServiceSummaryOutputTypeDef,
+    ServiceSummaryTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagOutputTypeDef,
-    OutputTypeDef,
     PaginatorConfigTypeDef,
     RejectEnvironmentAccountConnectionInputRequestTypeDef,
-    RepositorySyncEventOutputTypeDef,
-    ResourceSyncEventOutputTypeDef,
+    RepositorySyncEventTypeDef,
+    ResourceSyncEventTypeDef,
     ResponseMetadataTypeDef,
     S3ObjectSourceTypeDef,
-    SyncBlockerContextOutputTypeDef,
+    SyncBlockerContextTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateComponentInputRequestTypeDef,
     UpdateEnvironmentAccountConnectionInputRequestTypeDef,
     UpdateEnvironmentTemplateInputRequestTypeDef,
     UpdateEnvironmentTemplateVersionInputRequestTypeDef,
     UpdateServiceInputRequestTypeDef,
     UpdateServiceInstanceInputRequestTypeDef,
     UpdateServicePipelineInputRequestTypeDef,
     UpdateServiceSyncBlockerInputRequestTypeDef,
     UpdateServiceSyncConfigInputRequestTypeDef,
     UpdateServiceTemplateInputRequestTypeDef,
     UpdateTemplateSyncConfigInputRequestTypeDef,
-    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputOutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
-    AccountSettingsOutputTypeDef,
-    EnvironmentOutputTypeDef,
-    CancelComponentDeploymentOutputOutputTypeDef,
-    CreateComponentOutputOutputTypeDef,
-    DeleteComponentOutputOutputTypeDef,
-    GetComponentOutputOutputTypeDef,
-    UpdateComponentOutputOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputOutputTypeDef,
-    CreateServiceInstanceOutputOutputTypeDef,
-    GetServiceInstanceOutputOutputTypeDef,
-    UpdateServiceInstanceOutputOutputTypeDef,
-    CancelServicePipelineDeploymentOutputOutputTypeDef,
-    ServiceOutputTypeDef,
-    UpdateServicePipelineOutputOutputTypeDef,
+    AcceptEnvironmentAccountConnectionOutputTypeDef,
+    CreateEnvironmentAccountConnectionOutputTypeDef,
+    DeleteEnvironmentAccountConnectionOutputTypeDef,
+    GetEnvironmentAccountConnectionOutputTypeDef,
+    RejectEnvironmentAccountConnectionOutputTypeDef,
+    UpdateEnvironmentAccountConnectionOutputTypeDef,
+    AccountSettingsTypeDef,
+    EnvironmentTypeDef,
+    CancelComponentDeploymentOutputTypeDef,
+    CreateComponentOutputTypeDef,
+    DeleteComponentOutputTypeDef,
+    GetComponentOutputTypeDef,
+    UpdateComponentOutputTypeDef,
+    CancelServiceInstanceDeploymentOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
+    GetServiceInstanceOutputTypeDef,
+    UpdateServiceInstanceOutputTypeDef,
+    CancelServicePipelineDeploymentOutputTypeDef,
+    ServiceTypeDef,
+    UpdateServicePipelineOutputTypeDef,
     UpdateServiceTemplateVersionInputRequestTypeDef,
-    ServiceTemplateVersionOutputTypeDef,
-    ListComponentsOutputOutputTypeDef,
-    CountsSummaryOutputTypeDef,
+    ServiceTemplateVersionTypeDef,
+    ListComponentsOutputTypeDef,
+    CountsSummaryTypeDef,
     CreateComponentInputRequestTypeDef,
     CreateEnvironmentAccountConnectionInputRequestTypeDef,
     CreateEnvironmentTemplateInputRequestTypeDef,
     CreateRepositoryInputRequestTypeDef,
     CreateServiceInputRequestTypeDef,
     CreateServiceInstanceInputRequestTypeDef,
     CreateServiceTemplateInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
-    CreateEnvironmentTemplateOutputOutputTypeDef,
-    DeleteEnvironmentTemplateOutputOutputTypeDef,
-    GetEnvironmentTemplateOutputOutputTypeDef,
-    UpdateEnvironmentTemplateOutputOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
-    CreateRepositoryOutputOutputTypeDef,
-    DeleteRepositoryOutputOutputTypeDef,
-    GetRepositoryOutputOutputTypeDef,
-    CreateServiceSyncConfigOutputOutputTypeDef,
-    DeleteServiceSyncConfigOutputOutputTypeDef,
-    GetServiceSyncConfigOutputOutputTypeDef,
-    UpdateServiceSyncConfigOutputOutputTypeDef,
-    CreateServiceTemplateOutputOutputTypeDef,
-    DeleteServiceTemplateOutputOutputTypeDef,
-    GetServiceTemplateOutputOutputTypeDef,
-    UpdateServiceTemplateOutputOutputTypeDef,
-    CreateTemplateSyncConfigOutputOutputTypeDef,
-    DeleteTemplateSyncConfigOutputOutputTypeDef,
-    GetTemplateSyncConfigOutputOutputTypeDef,
-    UpdateTemplateSyncConfigOutputOutputTypeDef,
-    DeploymentStateOutputTypeDef,
-    ListDeploymentsOutputOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
-    ListEnvironmentsOutputOutputTypeDef,
+    CreateEnvironmentTemplateOutputTypeDef,
+    DeleteEnvironmentTemplateOutputTypeDef,
+    GetEnvironmentTemplateOutputTypeDef,
+    UpdateEnvironmentTemplateOutputTypeDef,
+    CreateEnvironmentTemplateVersionOutputTypeDef,
+    DeleteEnvironmentTemplateVersionOutputTypeDef,
+    GetEnvironmentTemplateVersionOutputTypeDef,
+    UpdateEnvironmentTemplateVersionOutputTypeDef,
+    CreateRepositoryOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    GetRepositoryOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
+    CreateServiceTemplateOutputTypeDef,
+    DeleteServiceTemplateOutputTypeDef,
+    GetServiceTemplateOutputTypeDef,
+    UpdateServiceTemplateOutputTypeDef,
+    CreateTemplateSyncConfigOutputTypeDef,
+    DeleteTemplateSyncConfigOutputTypeDef,
+    GetTemplateSyncConfigOutputTypeDef,
+    UpdateTemplateSyncConfigOutputTypeDef,
+    DeploymentStateTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputTypeDef,
+    ListEnvironmentsOutputTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentTemplatesOutputOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
+    ListEnvironmentTemplatesOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
     GetComponentInputComponentDeployedWaitTypeDef,
     GetEnvironmentInputEnvironmentDeployedWaitTypeDef,
     GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
     GetServiceInputServiceCreatedWaitTypeDef,
     GetServiceInputServiceDeletedWaitTypeDef,
     GetServiceInputServicePipelineDeployedWaitTypeDef,
     GetServiceInputServiceUpdatedWaitTypeDef,
     GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
     GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
-    ListComponentOutputsOutputOutputTypeDef,
-    ListEnvironmentOutputsOutputOutputTypeDef,
-    ListServiceInstanceOutputsOutputOutputTypeDef,
-    ListServicePipelineOutputsOutputOutputTypeDef,
-    ListComponentProvisionedResourcesOutputOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
-    ListRepositoriesOutputOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputOutputTypeDef,
+    ListComponentOutputsOutputTypeDef,
+    ListEnvironmentOutputsOutputTypeDef,
+    ListServiceInstanceOutputsOutputTypeDef,
+    ListServicePipelineOutputsOutputTypeDef,
+    NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+    ListComponentProvisionedResourcesOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputTypeDef,
+    ListRepositoriesOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputTypeDef,
     ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
     ListServiceInstancesInputRequestTypeDef,
-    ListServiceInstancesOutputOutputTypeDef,
-    ListServiceTemplateVersionsOutputOutputTypeDef,
-    ListServiceTemplatesOutputOutputTypeDef,
-    ListServicesOutputOutputTypeDef,
-    ListTagsForResourceOutputOutputTypeDef,
-    NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    RepositorySyncAttemptOutputTypeDef,
-    ResourceSyncAttemptOutputTypeDef,
+    ListServiceInstancesOutputTypeDef,
+    ListServiceTemplateVersionsOutputTypeDef,
+    ListServiceTemplatesOutputTypeDef,
+    ListServicesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    RepositorySyncAttemptTypeDef,
+    ResourceSyncAttemptTypeDef,
     TemplateVersionSourceInputTypeDef,
-    SyncBlockerOutputTypeDef,
-    GetAccountSettingsOutputOutputTypeDef,
-    UpdateAccountSettingsOutputOutputTypeDef,
-    CancelEnvironmentDeploymentOutputOutputTypeDef,
-    CreateEnvironmentOutputOutputTypeDef,
-    DeleteEnvironmentOutputOutputTypeDef,
-    GetEnvironmentOutputOutputTypeDef,
-    UpdateEnvironmentOutputOutputTypeDef,
-    CreateServiceOutputOutputTypeDef,
-    DeleteServiceOutputOutputTypeDef,
-    GetServiceOutputOutputTypeDef,
-    UpdateServiceOutputOutputTypeDef,
-    CreateServiceTemplateVersionOutputOutputTypeDef,
-    DeleteServiceTemplateVersionOutputOutputTypeDef,
-    GetServiceTemplateVersionOutputOutputTypeDef,
-    UpdateServiceTemplateVersionOutputOutputTypeDef,
-    GetResourcesSummaryOutputOutputTypeDef,
-    DeploymentOutputTypeDef,
-    GetRepositorySyncStatusOutputOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputOutputTypeDef,
-    GetTemplateSyncStatusOutputOutputTypeDef,
+    SyncBlockerTypeDef,
+    GetAccountSettingsOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
+    CancelEnvironmentDeploymentOutputTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    DeleteEnvironmentOutputTypeDef,
+    GetEnvironmentOutputTypeDef,
+    UpdateEnvironmentOutputTypeDef,
+    CreateServiceOutputTypeDef,
+    DeleteServiceOutputTypeDef,
+    GetServiceOutputTypeDef,
+    UpdateServiceOutputTypeDef,
+    CreateServiceTemplateVersionOutputTypeDef,
+    DeleteServiceTemplateVersionOutputTypeDef,
+    GetServiceTemplateVersionOutputTypeDef,
+    UpdateServiceTemplateVersionOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
+    DeploymentTypeDef,
+    GetRepositorySyncStatusOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
+    GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
-    ServiceSyncBlockerSummaryOutputTypeDef,
-    UpdateServiceSyncBlockerOutputOutputTypeDef,
-    DeleteDeploymentOutputOutputTypeDef,
-    GetDeploymentOutputOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
+    ServiceSyncBlockerSummaryTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-proton-1.28.3.post1/README.md` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/paginator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,816 +1,507 @@
-<a id="mypy-boto3-proton"></a>
+"""
+Type annotations for proton service client paginators.
 
-# mypy-boto3-proton
+[Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/)
 
-[![PyPI - mypy-boto3-proton](https://img.shields.io/pypi/v/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
+Usage::
 
-![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
+    ```python
+    from boto3.session import Session
+
+    from mypy_boto3_proton.client import ProtonClient
+    from mypy_boto3_proton.paginator import (
+        ListComponentOutputsPaginator,
+        ListComponentProvisionedResourcesPaginator,
+        ListComponentsPaginator,
+        ListDeploymentsPaginator,
+        ListEnvironmentAccountConnectionsPaginator,
+        ListEnvironmentOutputsPaginator,
+        ListEnvironmentProvisionedResourcesPaginator,
+        ListEnvironmentTemplateVersionsPaginator,
+        ListEnvironmentTemplatesPaginator,
+        ListEnvironmentsPaginator,
+        ListRepositoriesPaginator,
+        ListRepositorySyncDefinitionsPaginator,
+        ListServiceInstanceOutputsPaginator,
+        ListServiceInstanceProvisionedResourcesPaginator,
+        ListServiceInstancesPaginator,
+        ListServicePipelineOutputsPaginator,
+        ListServicePipelineProvisionedResourcesPaginator,
+        ListServiceTemplateVersionsPaginator,
+        ListServiceTemplatesPaginator,
+        ListServicesPaginator,
+        ListTagsForResourcePaginator,
+    )
+
+    session = Session()
+    client: ProtonClient = session.client("proton")
+
+    list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
+    list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
+    list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
+    list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
+    list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
+    list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
+    list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
+    list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
+    list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+    list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
+    list_repository_sync_definitions_paginator: ListRepositorySyncDefinitionsPaginator = client.get_paginator("list_repository_sync_definitions")
+    list_service_instance_outputs_paginator: ListServiceInstanceOutputsPaginator = client.get_paginator("list_service_instance_outputs")
+    list_service_instance_provisioned_resources_paginator: ListServiceInstanceProvisionedResourcesPaginator = client.get_paginator("list_service_instance_provisioned_resources")
+    list_service_instances_paginator: ListServiceInstancesPaginator = client.get_paginator("list_service_instances")
+    list_service_pipeline_outputs_paginator: ListServicePipelineOutputsPaginator = client.get_paginator("list_service_pipeline_outputs")
+    list_service_pipeline_provisioned_resources_paginator: ListServicePipelineProvisionedResourcesPaginator = client.get_paginator("list_service_pipeline_provisioned_resources")
+    list_service_template_versions_paginator: ListServiceTemplateVersionsPaginator = client.get_paginator("list_service_template_versions")
+    list_service_templates_paginator: ListServiceTemplatesPaginator = client.get_paginator("list_service_templates")
+    list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+    list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
+    ```
+"""
+from typing import Generic, Iterator, Sequence, TypeVar
 
-Type annotations for
-[boto3.Proton 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
-service compatible with [VSCode](https://code.visualstudio.com/),
-[PyCharm](https://www.jetbrains.com/pycharm/),
-[Emacs](https://www.gnu.org/software/emacs/),
-[Sublime Text](https://www.sublimetext.com/),
-[mypy](https://github.com/python/mypy),
-[pyright](https://github.com/microsoft/pyright) and other tools.
+from botocore.paginate import PageIterator, Paginator
 
-Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
-
-More information can be found on
-[boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
-[mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
-
-See how it helps to find and fix potential bugs:
-
-![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
-
-- [mypy-boto3-proton](#mypy-boto3-proton)
-  - [How to install](#how-to-install)
-    - [VSCode extension](#vscode-extension)
-    - [From PyPI with pip](#from-pypi-with-pip)
-  - [How to uninstall](#how-to-uninstall)
-  - [Usage](#usage)
-    - [VSCode](#vscode)
-    - [PyCharm](#pycharm)
-    - [Emacs](#emacs)
-    - [Sublime Text](#sublime-text)
-    - [Other IDEs](#other-ides)
-    - [mypy](#mypy)
-    - [pyright](#pyright)
-  - [Explicit type annotations](#explicit-type-annotations)
-    - [Client annotations](#client-annotations)
-    - [Paginators annotations](#paginators-annotations)
-    - [Waiters annotations](#waiters-annotations)
-    - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
-  - [How it works](#how-it-works)
-  - [What's new](#what's-new)
-    - [Implemented features](#implemented-features)
-    - [Latest changes](#latest-changes)
-  - [Versioning](#versioning)
-  - [Thank you](#thank-you)
-  - [Documentation](#documentation)
-  - [Support and contributing](#support-and-contributing)
-
-<a id="how-to-install"></a>
-
-## How to install
-
-<a id="vscode-extension"></a>
-
-### VSCode extension
-
-Add
-[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
-extension to your VSCode and run `AWS boto3: Quick Start` command.
-
-Click `Modify` and select `boto3 common` and `Proton`.
-
-<a id="from-pypi-with-pip"></a>
-
-### From PyPI with pip
-
-Install `boto3-stubs` for `Proton` service.
-
-```bash
-# install with boto3 type annotations
-python -m pip install 'boto3-stubs[proton]'
-
-
-# Lite version does not provide session.client/resource overloads
-# it is more RAM-friendly, but requires explicit type annotations
-python -m pip install 'boto3-stubs-lite[proton]'
-
-
-# standalone installation
-python -m pip install mypy-boto3-proton
-```
-
-<a id="how-to-uninstall"></a>
-
-## How to uninstall
-
-```bash
-python -m pip uninstall -y mypy-boto3-proton
-```
-
-<a id="usage"></a>
-
-## Usage
-
-<a id="vscode"></a>
-
-### VSCode
-
-- Install
-  [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
-- Install
-  [Pylance extension](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
-- Set `Pylance` as your Python Language Server
-- Install `boto3-stubs[proton]` in your environment:
-
-```bash
-python -m pip install 'boto3-stubs[proton]'
-```
-
-Both type checking and code completion should now work. No explicit type
-annotations required, write your `boto3` code as usual.
-
-<a id="pycharm"></a>
-
-### PyCharm
-
-Install `boto3-stubs-lite[proton]` in your environment:
-
-```bash
-python -m pip install 'boto3-stubs-lite[proton]'`
-```
-
-Both type checking and code completion should now work. Explicit type
-annotations **are required**.
-
-Use `boto3-stubs` package instead for implicit type discovery.
-
-<a id="emacs"></a>
-
-### Emacs
-
-- Install `boto3-stubs` with services you use in your environment:
-
-```bash
-python -m pip install 'boto3-stubs[proton]'
-```
-
-- Install [use-package](https://github.com/jwiegley/use-package),
-  [lsp](https://github.com/emacs-lsp/lsp-mode/),
-  [company](https://github.com/company-mode/company-mode) and
-  [flycheck](https://github.com/flycheck/flycheck) packages
-- Install [lsp-pyright](https://github.com/emacs-lsp/lsp-pyright) package
-
-```elisp
-(use-package lsp-pyright
-  :ensure t
-  :hook (python-mode . (lambda ()
-                          (require 'lsp-pyright)
-                          (lsp)))  ; or lsp-deferred
-  :init (when (executable-find "python3")
-          (setq lsp-pyright-python-executable-cmd "python3"))
-  )
-```
-
-- Make sure emacs uses the environment where you have installed `boto3-stubs`
-
-Type checking should now work. No explicit type annotations required, write
-your `boto3` code as usual.
-
-<a id="sublime-text"></a>
-
-### Sublime Text
-
-- Install `boto3-stubs[proton]` with services you use in your environment:
-
-```bash
-python -m pip install 'boto3-stubs[proton]'
-```
-
-- Install [LSP-pyright](https://github.com/sublimelsp/LSP-pyright) package
-
-Type checking should now work. No explicit type annotations required, write
-your `boto3` code as usual.
-
-<a id="other-ides"></a>
-
-### Other IDEs
-
-Not tested, but as long as your IDE supports `mypy` or `pyright`, everything
-should work.
-
-<a id="mypy"></a>
-
-### mypy
-
-- Install `mypy`: `python -m pip install mypy`
-- Install `boto3-stubs[proton]` in your environment:
-
-```bash
-python -m pip install 'boto3-stubs[proton]'`
-```
-
-Type checking should now work. No explicit type annotations required, write
-your `boto3` code as usual.
-
-<a id="pyright"></a>
-
-### pyright
-
-- Install `pyright`: `npm i -g pyright`
-- Install `boto3-stubs[proton]` in your environment:
-
-```bash
-python -m pip install 'boto3-stubs[proton]'
-```
-
-Optionally, you can install `boto3-stubs` to `typings` folder.
-
-Type checking should now work. No explicit type annotations required, write
-your `boto3` code as usual.
-
-<a id="explicit-type-annotations"></a>
-
-## Explicit type annotations
-
-<a id="client-annotations"></a>
-
-### Client annotations
-
-`ProtonClient` provides annotations for `boto3.client("proton")`.
-
-```python
-from boto3.session import Session
-
-from mypy_boto3_proton import ProtonClient
-
-client: ProtonClient = Session().client("proton")
-
-# now client usage is checked by mypy and IDE should provide code completion
-```
-
-<a id="paginators-annotations"></a>
-
-### Paginators annotations
-
-`mypy_boto3_proton.paginator` module contains type annotations for all
-paginators.
-
-```python
-from boto3.session import Session
-
-from mypy_boto3_proton import ProtonClient
-from mypy_boto3_proton.paginator import (
-    ListComponentOutputsPaginator,
-    ListComponentProvisionedResourcesPaginator,
-    ListComponentsPaginator,
-    ListDeploymentsPaginator,
-    ListEnvironmentAccountConnectionsPaginator,
-    ListEnvironmentOutputsPaginator,
-    ListEnvironmentProvisionedResourcesPaginator,
-    ListEnvironmentTemplateVersionsPaginator,
-    ListEnvironmentTemplatesPaginator,
-    ListEnvironmentsPaginator,
-    ListRepositoriesPaginator,
-    ListRepositorySyncDefinitionsPaginator,
-    ListServiceInstanceOutputsPaginator,
-    ListServiceInstanceProvisionedResourcesPaginator,
-    ListServiceInstancesPaginator,
-    ListServicePipelineOutputsPaginator,
-    ListServicePipelineProvisionedResourcesPaginator,
-    ListServiceTemplateVersionsPaginator,
-    ListServiceTemplatesPaginator,
-    ListServicesPaginator,
-    ListTagsForResourcePaginator,
-)
-
-client: ProtonClient = Session().client("proton")
-
-# Explicit type annotations are optional here
-# Types should be correctly discovered by mypy and IDEs
-list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator(
-    "list_component_outputs"
-)
-list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = (
-    client.get_paginator("list_component_provisioned_resources")
-)
-list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
-list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
-list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = (
-    client.get_paginator("list_environment_account_connections")
-)
-list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator(
-    "list_environment_outputs"
-)
-list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = (
-    client.get_paginator("list_environment_provisioned_resources")
-)
-list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = (
-    client.get_paginator("list_environment_template_versions")
-)
-list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator(
-    "list_environment_templates"
-)
-list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
-list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
-list_repository_sync_definitions_paginator: ListRepositorySyncDefinitionsPaginator = (
-    client.get_paginator("list_repository_sync_definitions")
-)
-list_service_instance_outputs_paginator: ListServiceInstanceOutputsPaginator = client.get_paginator(
-    "list_service_instance_outputs"
-)
-list_service_instance_provisioned_resources_paginator: ListServiceInstanceProvisionedResourcesPaginator = client.get_paginator(
-    "list_service_instance_provisioned_resources"
-)
-list_service_instances_paginator: ListServiceInstancesPaginator = client.get_paginator(
-    "list_service_instances"
-)
-list_service_pipeline_outputs_paginator: ListServicePipelineOutputsPaginator = client.get_paginator(
-    "list_service_pipeline_outputs"
-)
-list_service_pipeline_provisioned_resources_paginator: ListServicePipelineProvisionedResourcesPaginator = client.get_paginator(
-    "list_service_pipeline_provisioned_resources"
-)
-list_service_template_versions_paginator: ListServiceTemplateVersionsPaginator = (
-    client.get_paginator("list_service_template_versions")
-)
-list_service_templates_paginator: ListServiceTemplatesPaginator = client.get_paginator(
-    "list_service_templates"
-)
-list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
-list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator(
-    "list_tags_for_resource"
-)
-```
-
-<a id="waiters-annotations"></a>
-
-### Waiters annotations
-
-`mypy_boto3_proton.waiter` module contains type annotations for all waiters.
-
-```python
-from boto3.session import Session
-
-from mypy_boto3_proton import ProtonClient
-from mypy_boto3_proton.waiter import (
-    ComponentDeletedWaiter,
-    ComponentDeployedWaiter,
-    EnvironmentDeployedWaiter,
-    EnvironmentTemplateVersionRegisteredWaiter,
-    ServiceCreatedWaiter,
-    ServiceDeletedWaiter,
-    ServiceInstanceDeployedWaiter,
-    ServicePipelineDeployedWaiter,
-    ServiceTemplateVersionRegisteredWaiter,
-    ServiceUpdatedWaiter,
-)
-
-client: ProtonClient = Session().client("proton")
-
-# Explicit type annotations are optional here
-# Types should be correctly discovered by mypy and IDEs
-component_deleted_waiter: ComponentDeletedWaiter = client.get_waiter("component_deleted")
-component_deployed_waiter: ComponentDeployedWaiter = client.get_waiter("component_deployed")
-environment_deployed_waiter: EnvironmentDeployedWaiter = client.get_waiter("environment_deployed")
-environment_template_version_registered_waiter: EnvironmentTemplateVersionRegisteredWaiter = (
-    client.get_waiter("environment_template_version_registered")
-)
-service_created_waiter: ServiceCreatedWaiter = client.get_waiter("service_created")
-service_deleted_waiter: ServiceDeletedWaiter = client.get_waiter("service_deleted")
-service_instance_deployed_waiter: ServiceInstanceDeployedWaiter = client.get_waiter(
-    "service_instance_deployed"
-)
-service_pipeline_deployed_waiter: ServicePipelineDeployedWaiter = client.get_waiter(
-    "service_pipeline_deployed"
-)
-service_template_version_registered_waiter: ServiceTemplateVersionRegisteredWaiter = (
-    client.get_waiter("service_template_version_registered")
-)
-service_updated_waiter: ServiceUpdatedWaiter = client.get_waiter("service_updated")
-```
-
-<a id="literals"></a>
-
-### Literals
-
-`mypy_boto3_proton.literals` module contains literals extracted from shapes
-that can be used in user code for type checking.
-
-```python
-from mypy_boto3_proton.literals import (
-    BlockerStatusType,
-    BlockerTypeType,
-    ComponentDeletedWaiterName,
-    ComponentDeployedWaiterName,
-    ComponentDeploymentUpdateTypeType,
-    DeploymentStatusType,
-    DeploymentTargetResourceTypeType,
-    DeploymentUpdateTypeType,
+from .literals import (
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
-    EnvironmentDeployedWaiterName,
-    EnvironmentTemplateVersionRegisteredWaiterName,
-    ListComponentOutputsPaginatorName,
-    ListComponentProvisionedResourcesPaginatorName,
-    ListComponentsPaginatorName,
-    ListDeploymentsPaginatorName,
-    ListEnvironmentAccountConnectionsPaginatorName,
-    ListEnvironmentOutputsPaginatorName,
-    ListEnvironmentProvisionedResourcesPaginatorName,
-    ListEnvironmentTemplateVersionsPaginatorName,
-    ListEnvironmentTemplatesPaginatorName,
-    ListEnvironmentsPaginatorName,
-    ListRepositoriesPaginatorName,
-    ListRepositorySyncDefinitionsPaginatorName,
-    ListServiceInstanceOutputsPaginatorName,
-    ListServiceInstanceProvisionedResourcesPaginatorName,
-    ListServiceInstancesFilterByType,
-    ListServiceInstancesPaginatorName,
     ListServiceInstancesSortByType,
-    ListServicePipelineOutputsPaginatorName,
-    ListServicePipelineProvisionedResourcesPaginatorName,
-    ListServiceTemplateVersionsPaginatorName,
-    ListServiceTemplatesPaginatorName,
-    ListServicesPaginatorName,
-    ListTagsForResourcePaginatorName,
-    ProvisionedResourceEngineType,
-    ProvisioningType,
     RepositoryProviderType,
-    RepositorySyncStatusType,
-    ResourceDeploymentStatusType,
-    ResourceSyncStatusType,
-    ServiceCreatedWaiterName,
-    ServiceDeletedWaiterName,
-    ServiceInstanceDeployedWaiterName,
-    ServicePipelineDeployedWaiterName,
-    ServiceStatusType,
-    ServiceTemplateSupportedComponentSourceTypeType,
-    ServiceTemplateVersionRegisteredWaiterName,
-    ServiceUpdatedWaiterName,
     SortOrderType,
     SyncTypeType,
-    TemplateTypeType,
-    TemplateVersionStatusType,
-    ProtonServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
 )
-
-
-def check_value(value: BlockerStatusType) -> bool:
-    ...
-```
-
-<a id="typed-dictionaries"></a>
-
-### Typed dictionaries
-
-`mypy_boto3_proton.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
-
-```python
-from mypy_boto3_proton.type_defs import (
-    AcceptEnvironmentAccountConnectionInputRequestTypeDef,
-    EnvironmentAccountConnectionOutputTypeDef,
-    RepositoryBranchOutputTypeDef,
-    CancelComponentDeploymentInputRequestTypeDef,
-    ComponentOutputTypeDef,
-    CancelEnvironmentDeploymentInputRequestTypeDef,
-    CancelServiceInstanceDeploymentInputRequestTypeDef,
-    ServiceInstanceOutputTypeDef,
-    CancelServicePipelineDeploymentInputRequestTypeDef,
-    ServicePipelineOutputTypeDef,
-    CompatibleEnvironmentTemplateInputTypeDef,
-    CompatibleEnvironmentTemplateOutputTypeDef,
-    ComponentStateOutputTypeDef,
-    ComponentSummaryOutputTypeDef,
-    ResourceCountsSummaryOutputTypeDef,
-    TagTypeDef,
-    RepositoryBranchInputTypeDef,
-    EnvironmentTemplateOutputTypeDef,
-    EnvironmentTemplateVersionOutputTypeDef,
-    RepositoryOutputTypeDef,
-    CreateServiceSyncConfigInputRequestTypeDef,
-    ServiceSyncConfigOutputTypeDef,
-    ServiceTemplateOutputTypeDef,
-    CreateTemplateSyncConfigInputRequestTypeDef,
-    TemplateSyncConfigOutputTypeDef,
-    DeleteComponentInputRequestTypeDef,
-    DeleteDeploymentInputRequestTypeDef,
-    DeleteEnvironmentAccountConnectionInputRequestTypeDef,
-    DeleteEnvironmentInputRequestTypeDef,
-    DeleteEnvironmentTemplateInputRequestTypeDef,
-    DeleteEnvironmentTemplateVersionInputRequestTypeDef,
-    DeleteRepositoryInputRequestTypeDef,
-    DeleteServiceInputRequestTypeDef,
-    DeleteServiceSyncConfigInputRequestTypeDef,
-    DeleteServiceTemplateInputRequestTypeDef,
-    DeleteServiceTemplateVersionInputRequestTypeDef,
-    DeleteTemplateSyncConfigInputRequestTypeDef,
-    EnvironmentStateOutputTypeDef,
-    ServiceInstanceStateOutputTypeDef,
-    ServicePipelineStateOutputTypeDef,
-    DeploymentSummaryOutputTypeDef,
-    EnvironmentAccountConnectionSummaryOutputTypeDef,
-    EnvironmentSummaryOutputTypeDef,
+from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
-    EnvironmentTemplateSummaryOutputTypeDef,
-    EnvironmentTemplateVersionSummaryOutputTypeDef,
-    WaiterConfigTypeDef,
-    GetComponentInputRequestTypeDef,
-    GetDeploymentInputRequestTypeDef,
-    GetEnvironmentAccountConnectionInputRequestTypeDef,
-    GetEnvironmentInputRequestTypeDef,
-    GetEnvironmentTemplateInputRequestTypeDef,
-    GetEnvironmentTemplateVersionInputRequestTypeDef,
-    GetRepositoryInputRequestTypeDef,
-    GetRepositorySyncStatusInputRequestTypeDef,
-    GetServiceInputRequestTypeDef,
-    GetServiceInstanceInputRequestTypeDef,
-    GetServiceInstanceSyncStatusInputRequestTypeDef,
-    RevisionOutputTypeDef,
-    GetServiceSyncBlockerSummaryInputRequestTypeDef,
-    GetServiceSyncConfigInputRequestTypeDef,
-    GetServiceTemplateInputRequestTypeDef,
-    GetServiceTemplateVersionInputRequestTypeDef,
-    GetTemplateSyncConfigInputRequestTypeDef,
-    GetTemplateSyncStatusInputRequestTypeDef,
-    ListComponentOutputsInputListComponentOutputsPaginateTypeDef,
-    ListComponentOutputsInputRequestTypeDef,
-    OutputOutputTypeDef,
-    ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
-    ListComponentProvisionedResourcesInputRequestTypeDef,
-    ProvisionedResourceOutputTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListComponentsInputRequestTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
-    ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
-    ListEnvironmentAccountConnectionsInputRequestTypeDef,
-    ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
-    ListEnvironmentOutputsInputRequestTypeDef,
-    ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
-    ListEnvironmentProvisionedResourcesInputRequestTypeDef,
-    ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
-    ListEnvironmentTemplateVersionsInputRequestTypeDef,
-    ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef,
-    ListEnvironmentTemplatesInputRequestTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
-    ListRepositoriesInputRequestTypeDef,
-    RepositorySummaryOutputTypeDef,
-    ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef,
-    ListRepositorySyncDefinitionsInputRequestTypeDef,
-    RepositorySyncDefinitionOutputTypeDef,
-    ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
-    ListServiceInstanceOutputsInputRequestTypeDef,
-    ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef,
-    ListServiceInstanceProvisionedResourcesInputRequestTypeDef,
+    ListComponentOutputsOutputTypeDef,
+    ListComponentProvisionedResourcesOutputTypeDef,
+    ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputTypeDef,
+    ListEnvironmentOutputsOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListEnvironmentTemplatesOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputTypeDef,
+    ListRepositoriesOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstanceOutputsOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ServiceInstanceSummaryOutputTypeDef,
-    ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
-    ListServicePipelineOutputsInputRequestTypeDef,
-    ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef,
-    ListServicePipelineProvisionedResourcesInputRequestTypeDef,
-    ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef,
-    ListServiceTemplateVersionsInputRequestTypeDef,
-    ServiceTemplateVersionSummaryOutputTypeDef,
-    ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef,
-    ListServiceTemplatesInputRequestTypeDef,
-    ServiceTemplateSummaryOutputTypeDef,
-    ListServicesInputListServicesPaginateTypeDef,
-    ListServicesInputRequestTypeDef,
-    ServiceSummaryOutputTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    OutputTypeDef,
+    ListServiceInstancesOutputTypeDef,
+    ListServicePipelineOutputsOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputTypeDef,
+    ListServicesOutputTypeDef,
+    ListServiceTemplatesOutputTypeDef,
+    ListServiceTemplateVersionsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
-    RejectEnvironmentAccountConnectionInputRequestTypeDef,
-    RepositorySyncEventOutputTypeDef,
-    ResourceSyncEventOutputTypeDef,
-    ResponseMetadataTypeDef,
-    S3ObjectSourceTypeDef,
-    SyncBlockerContextOutputTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateComponentInputRequestTypeDef,
-    UpdateEnvironmentAccountConnectionInputRequestTypeDef,
-    UpdateEnvironmentTemplateInputRequestTypeDef,
-    UpdateEnvironmentTemplateVersionInputRequestTypeDef,
-    UpdateServiceInputRequestTypeDef,
-    UpdateServiceInstanceInputRequestTypeDef,
-    UpdateServicePipelineInputRequestTypeDef,
-    UpdateServiceSyncBlockerInputRequestTypeDef,
-    UpdateServiceSyncConfigInputRequestTypeDef,
-    UpdateServiceTemplateInputRequestTypeDef,
-    UpdateTemplateSyncConfigInputRequestTypeDef,
-    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputOutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
-    AccountSettingsOutputTypeDef,
-    EnvironmentOutputTypeDef,
-    CancelComponentDeploymentOutputOutputTypeDef,
-    CreateComponentOutputOutputTypeDef,
-    DeleteComponentOutputOutputTypeDef,
-    GetComponentOutputOutputTypeDef,
-    UpdateComponentOutputOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputOutputTypeDef,
-    CreateServiceInstanceOutputOutputTypeDef,
-    GetServiceInstanceOutputOutputTypeDef,
-    UpdateServiceInstanceOutputOutputTypeDef,
-    CancelServicePipelineDeploymentOutputOutputTypeDef,
-    ServiceOutputTypeDef,
-    UpdateServicePipelineOutputOutputTypeDef,
-    UpdateServiceTemplateVersionInputRequestTypeDef,
-    ServiceTemplateVersionOutputTypeDef,
-    ListComponentsOutputOutputTypeDef,
-    CountsSummaryOutputTypeDef,
-    CreateComponentInputRequestTypeDef,
-    CreateEnvironmentAccountConnectionInputRequestTypeDef,
-    CreateEnvironmentTemplateInputRequestTypeDef,
-    CreateRepositoryInputRequestTypeDef,
-    CreateServiceInputRequestTypeDef,
-    CreateServiceInstanceInputRequestTypeDef,
-    CreateServiceTemplateInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateEnvironmentInputRequestTypeDef,
-    UpdateAccountSettingsInputRequestTypeDef,
-    UpdateEnvironmentInputRequestTypeDef,
-    CreateEnvironmentTemplateOutputOutputTypeDef,
-    DeleteEnvironmentTemplateOutputOutputTypeDef,
-    GetEnvironmentTemplateOutputOutputTypeDef,
-    UpdateEnvironmentTemplateOutputOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
-    CreateRepositoryOutputOutputTypeDef,
-    DeleteRepositoryOutputOutputTypeDef,
-    GetRepositoryOutputOutputTypeDef,
-    CreateServiceSyncConfigOutputOutputTypeDef,
-    DeleteServiceSyncConfigOutputOutputTypeDef,
-    GetServiceSyncConfigOutputOutputTypeDef,
-    UpdateServiceSyncConfigOutputOutputTypeDef,
-    CreateServiceTemplateOutputOutputTypeDef,
-    DeleteServiceTemplateOutputOutputTypeDef,
-    GetServiceTemplateOutputOutputTypeDef,
-    UpdateServiceTemplateOutputOutputTypeDef,
-    CreateTemplateSyncConfigOutputOutputTypeDef,
-    DeleteTemplateSyncConfigOutputOutputTypeDef,
-    GetTemplateSyncConfigOutputOutputTypeDef,
-    UpdateTemplateSyncConfigOutputOutputTypeDef,
-    DeploymentStateOutputTypeDef,
-    ListDeploymentsOutputOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
-    ListEnvironmentsOutputOutputTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentTemplatesOutputOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
-    GetComponentInputComponentDeletedWaitTypeDef,
-    GetComponentInputComponentDeployedWaitTypeDef,
-    GetEnvironmentInputEnvironmentDeployedWaitTypeDef,
-    GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef,
-    GetServiceInputServiceCreatedWaitTypeDef,
-    GetServiceInputServiceDeletedWaitTypeDef,
-    GetServiceInputServicePipelineDeployedWaitTypeDef,
-    GetServiceInputServiceUpdatedWaitTypeDef,
-    GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef,
-    GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
-    ListComponentOutputsOutputOutputTypeDef,
-    ListEnvironmentOutputsOutputOutputTypeDef,
-    ListServiceInstanceOutputsOutputOutputTypeDef,
-    ListServicePipelineOutputsOutputOutputTypeDef,
-    ListComponentProvisionedResourcesOutputOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
-    ListRepositoriesOutputOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputOutputTypeDef,
-    ListServiceInstancesInputListServiceInstancesPaginateTypeDef,
-    ListServiceInstancesInputRequestTypeDef,
-    ListServiceInstancesOutputOutputTypeDef,
-    ListServiceTemplateVersionsOutputOutputTypeDef,
-    ListServiceTemplatesOutputOutputTypeDef,
-    ListServicesOutputOutputTypeDef,
-    ListTagsForResourceOutputOutputTypeDef,
-    NotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    RepositorySyncAttemptOutputTypeDef,
-    ResourceSyncAttemptOutputTypeDef,
-    TemplateVersionSourceInputTypeDef,
-    SyncBlockerOutputTypeDef,
-    GetAccountSettingsOutputOutputTypeDef,
-    UpdateAccountSettingsOutputOutputTypeDef,
-    CancelEnvironmentDeploymentOutputOutputTypeDef,
-    CreateEnvironmentOutputOutputTypeDef,
-    DeleteEnvironmentOutputOutputTypeDef,
-    GetEnvironmentOutputOutputTypeDef,
-    UpdateEnvironmentOutputOutputTypeDef,
-    CreateServiceOutputOutputTypeDef,
-    DeleteServiceOutputOutputTypeDef,
-    GetServiceOutputOutputTypeDef,
-    UpdateServiceOutputOutputTypeDef,
-    CreateServiceTemplateVersionOutputOutputTypeDef,
-    DeleteServiceTemplateVersionOutputOutputTypeDef,
-    GetServiceTemplateVersionOutputOutputTypeDef,
-    UpdateServiceTemplateVersionOutputOutputTypeDef,
-    GetResourcesSummaryOutputOutputTypeDef,
-    DeploymentOutputTypeDef,
-    GetRepositorySyncStatusOutputOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputOutputTypeDef,
-    GetTemplateSyncStatusOutputOutputTypeDef,
-    CreateEnvironmentTemplateVersionInputRequestTypeDef,
-    CreateServiceTemplateVersionInputRequestTypeDef,
-    ServiceSyncBlockerSummaryOutputTypeDef,
-    UpdateServiceSyncBlockerOutputOutputTypeDef,
-    DeleteDeploymentOutputOutputTypeDef,
-    GetDeploymentOutputOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
 )
 
-
-def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
-    return {...}
-```
-
-<a id="how-it-works"></a>
-
-## How it works
-
-Fully automated
-[mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
-generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
-
-- All available `boto3` services are covered.
-- Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
-- Type annotations include up-to-date documentation.
-- Link to documentation is provided for every method.
-- Code is processed by [black](https://github.com/psf/black) and
-  [isort](https://github.com/PyCQA/isort) for readability.
-
-<a id="what's-new"></a>
-
-## What's new
-
-<a id="implemented-features"></a>
-
-### Implemented features
-
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
-- `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
-  compatibility
-- `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
-  annotations for each service
-- Generated `TypeDefs` for each service
-- Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
-- Auto discovery of types for `client.get_waiter` and `client.get_paginator`
-  calls
-- Auto discovery of types for `ServiceResource` and `Resource` collections
-- Auto discovery of types for `aiobotocore.Session.create_client` calls
-
-<a id="latest-changes"></a>
-
-### Latest changes
-
-Builder changelog can be found in
-[Releases](https://github.com/youtype/mypy_boto3_builder/releases).
-
-<a id="versioning"></a>
-
-## Versioning
-
-`mypy-boto3-proton` version is the same as related `boto3` version and follows
-[PEP 440](https://www.python.org/dev/peps/pep-0440/) format.
-
-<a id="thank-you"></a>
-
-## Thank you
-
-- [Allie Fitter](https://github.com/alliefitter) for
-  [boto3-type-annotations](https://pypi.org/project/boto3-type-annotations/),
-  this package is based on top of his work
-- [black](https://github.com/psf/black) developers for an awesome formatting
-  tool
-- [Timothy Edmund Crosley](https://github.com/timothycrosley) for
-  [isort](https://github.com/PyCQA/isort) and how flexible it is
-- [mypy](https://github.com/python/mypy) developers for doing all dirty work
-  for us
-- [pyright](https://github.com/microsoft/pyright) team for the new era of typed
-  Python
-
-<a id="documentation"></a>
-
-## Documentation
-
-All services type annotations can be found in
-[boto3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
-
-<a id="support-and-contributing"></a>
-
-## Support and contributing
-
-This package is auto-generated. Please reports any bugs or request new features
-in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
-repository.
+__all__ = (
+    "ListComponentOutputsPaginator",
+    "ListComponentProvisionedResourcesPaginator",
+    "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
+    "ListEnvironmentAccountConnectionsPaginator",
+    "ListEnvironmentOutputsPaginator",
+    "ListEnvironmentProvisionedResourcesPaginator",
+    "ListEnvironmentTemplateVersionsPaginator",
+    "ListEnvironmentTemplatesPaginator",
+    "ListEnvironmentsPaginator",
+    "ListRepositoriesPaginator",
+    "ListRepositorySyncDefinitionsPaginator",
+    "ListServiceInstanceOutputsPaginator",
+    "ListServiceInstanceProvisionedResourcesPaginator",
+    "ListServiceInstancesPaginator",
+    "ListServicePipelineOutputsPaginator",
+    "ListServicePipelineProvisionedResourcesPaginator",
+    "ListServiceTemplateVersionsPaginator",
+    "ListServiceTemplatesPaginator",
+    "ListServicesPaginator",
+    "ListTagsForResourcePaginator",
+)
+
+
+_ItemTypeDef = TypeVar("_ItemTypeDef")
+
+
+class _PageIterator(Generic[_ItemTypeDef], PageIterator):
+    def __iter__(self) -> Iterator[_ItemTypeDef]:
+        """
+        Proxy method to specify iterator item type.
+        """
+
+
+class ListComponentOutputsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        componentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
+        """
+
+
+class ListComponentProvisionedResourcesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
+    """
+
+    def paginate(
+        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListComponentProvisionedResourcesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
+        """
+
+
+class ListComponentsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListComponentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
+        """
+
+
+class ListDeploymentsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
+        """
+
+
+class ListEnvironmentAccountConnectionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
+        environmentName: str = ...,
+        statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
+        """
+
+
+class ListEnvironmentOutputsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        environmentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
+        """
+
+
+class ListEnvironmentProvisionedResourcesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
+    """
+
+    def paginate(
+        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
+        """
+
+
+class ListEnvironmentTemplateVersionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        templateName: str,
+        majorVersion: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
+        """
+
+
+class ListEnvironmentTemplatesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEnvironmentTemplatesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
+        """
+
+
+class ListEnvironmentsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
+        """
+
+
+class ListRepositoriesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
+        """
+
+
+class ListRepositorySyncDefinitionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        repositoryName: str,
+        repositoryProvider: RepositoryProviderType,
+        syncType: SyncTypeType,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
+        """
+
+
+class ListServiceInstanceOutputsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        serviceInstanceName: str,
+        serviceName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
+        """
+
+
+class ListServiceInstanceProvisionedResourcesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        serviceInstanceName: str,
+        serviceName: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
+        """
+
+
+class ListServiceInstancesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
+        serviceName: str = ...,
+        sortBy: ListServiceInstancesSortByType = ...,
+        sortOrder: SortOrderType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServiceInstancesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
+        """
+
+
+class ListServicePipelineOutputsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        serviceName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
+        """
+
+
+class ListServicePipelineProvisionedResourcesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
+    """
+
+    def paginate(
+        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
+        """
+
+
+class ListServiceTemplateVersionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        templateName: str,
+        majorVersion: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServiceTemplateVersionsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
+        """
+
+
+class ListServiceTemplatesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServiceTemplatesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
+        """
+
+
+class ListServicesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListServicesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
+        """
+
+
+class ListTagsForResourcePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
+    """
+
+    def paginate(
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
+        """
```

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__init__.pyi` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/__main__.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Proton 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
-        " 7.14.7\nDocs:           "
+        "Type annotations for boto3.Proton 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
+        " 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
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

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,105 +51,105 @@
     ListServicePipelineProvisionedResourcesPaginator,
     ListServicesPaginator,
     ListServiceTemplatesPaginator,
     ListServiceTemplateVersionsPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
-    CancelComponentDeploymentOutputOutputTypeDef,
-    CancelEnvironmentDeploymentOutputOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputOutputTypeDef,
-    CancelServicePipelineDeploymentOutputOutputTypeDef,
+    AcceptEnvironmentAccountConnectionOutputTypeDef,
+    CancelComponentDeploymentOutputTypeDef,
+    CancelEnvironmentDeploymentOutputTypeDef,
+    CancelServiceInstanceDeploymentOutputTypeDef,
+    CancelServicePipelineDeploymentOutputTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
-    CreateComponentOutputOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
-    CreateEnvironmentOutputOutputTypeDef,
-    CreateEnvironmentTemplateOutputOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
-    CreateRepositoryOutputOutputTypeDef,
-    CreateServiceInstanceOutputOutputTypeDef,
-    CreateServiceOutputOutputTypeDef,
-    CreateServiceSyncConfigOutputOutputTypeDef,
-    CreateServiceTemplateOutputOutputTypeDef,
-    CreateServiceTemplateVersionOutputOutputTypeDef,
-    CreateTemplateSyncConfigOutputOutputTypeDef,
-    DeleteComponentOutputOutputTypeDef,
-    DeleteDeploymentOutputOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
-    DeleteEnvironmentOutputOutputTypeDef,
-    DeleteEnvironmentTemplateOutputOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
-    DeleteRepositoryOutputOutputTypeDef,
-    DeleteServiceOutputOutputTypeDef,
-    DeleteServiceSyncConfigOutputOutputTypeDef,
-    DeleteServiceTemplateOutputOutputTypeDef,
-    DeleteServiceTemplateVersionOutputOutputTypeDef,
-    DeleteTemplateSyncConfigOutputOutputTypeDef,
+    CreateComponentOutputTypeDef,
+    CreateEnvironmentAccountConnectionOutputTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateEnvironmentTemplateOutputTypeDef,
+    CreateEnvironmentTemplateVersionOutputTypeDef,
+    CreateRepositoryOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
+    CreateServiceOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
+    CreateServiceTemplateOutputTypeDef,
+    CreateServiceTemplateVersionOutputTypeDef,
+    CreateTemplateSyncConfigOutputTypeDef,
+    DeleteComponentOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
+    DeleteEnvironmentAccountConnectionOutputTypeDef,
+    DeleteEnvironmentOutputTypeDef,
+    DeleteEnvironmentTemplateOutputTypeDef,
+    DeleteEnvironmentTemplateVersionOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    DeleteServiceOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
+    DeleteServiceTemplateOutputTypeDef,
+    DeleteServiceTemplateVersionOutputTypeDef,
+    DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
-    GetAccountSettingsOutputOutputTypeDef,
-    GetComponentOutputOutputTypeDef,
-    GetDeploymentOutputOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputOutputTypeDef,
-    GetEnvironmentOutputOutputTypeDef,
-    GetEnvironmentTemplateOutputOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputOutputTypeDef,
-    GetRepositoryOutputOutputTypeDef,
-    GetRepositorySyncStatusOutputOutputTypeDef,
-    GetResourcesSummaryOutputOutputTypeDef,
-    GetServiceInstanceOutputOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputOutputTypeDef,
-    GetServiceOutputOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
-    GetServiceSyncConfigOutputOutputTypeDef,
-    GetServiceTemplateOutputOutputTypeDef,
-    GetServiceTemplateVersionOutputOutputTypeDef,
-    GetTemplateSyncConfigOutputOutputTypeDef,
-    GetTemplateSyncStatusOutputOutputTypeDef,
-    ListComponentOutputsOutputOutputTypeDef,
-    ListComponentProvisionedResourcesOutputOutputTypeDef,
-    ListComponentsOutputOutputTypeDef,
-    ListDeploymentsOutputOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
-    ListEnvironmentOutputsOutputOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
-    ListEnvironmentsOutputOutputTypeDef,
-    ListEnvironmentTemplatesOutputOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
-    ListRepositoriesOutputOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputOutputTypeDef,
-    ListServiceInstanceOutputsOutputOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
+    GetComponentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
+    GetEnvironmentAccountConnectionOutputTypeDef,
+    GetEnvironmentOutputTypeDef,
+    GetEnvironmentTemplateOutputTypeDef,
+    GetEnvironmentTemplateVersionOutputTypeDef,
+    GetRepositoryOutputTypeDef,
+    GetRepositorySyncStatusOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
+    GetServiceInstanceOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
+    GetServiceOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
+    GetServiceTemplateOutputTypeDef,
+    GetServiceTemplateVersionOutputTypeDef,
+    GetTemplateSyncConfigOutputTypeDef,
+    GetTemplateSyncStatusOutputTypeDef,
+    ListComponentOutputsOutputTypeDef,
+    ListComponentProvisionedResourcesOutputTypeDef,
+    ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputTypeDef,
+    ListEnvironmentOutputsOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListEnvironmentTemplatesOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputTypeDef,
+    ListRepositoriesOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstanceOutputsOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputOutputTypeDef,
-    ListServicePipelineOutputsOutputOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
-    ListServicesOutputOutputTypeDef,
-    ListServiceTemplatesOutputOutputTypeDef,
-    ListServiceTemplateVersionsOutputOutputTypeDef,
-    ListTagsForResourceOutputOutputTypeDef,
+    ListServiceInstancesOutputTypeDef,
+    ListServicePipelineOutputsOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputTypeDef,
+    ListServicesOutputTypeDef,
+    ListServiceTemplatesOutputTypeDef,
+    ListServiceTemplateVersionsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     OutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
+    RejectEnvironmentAccountConnectionOutputTypeDef,
     RepositoryBranchInputTypeDef,
     TagTypeDef,
     TemplateVersionSourceInputTypeDef,
-    UpdateAccountSettingsOutputOutputTypeDef,
-    UpdateComponentOutputOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
-    UpdateEnvironmentOutputOutputTypeDef,
-    UpdateEnvironmentTemplateOutputOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
-    UpdateServiceInstanceOutputOutputTypeDef,
-    UpdateServiceOutputOutputTypeDef,
-    UpdateServicePipelineOutputOutputTypeDef,
-    UpdateServiceSyncBlockerOutputOutputTypeDef,
-    UpdateServiceSyncConfigOutputOutputTypeDef,
-    UpdateServiceTemplateOutputOutputTypeDef,
-    UpdateServiceTemplateVersionOutputOutputTypeDef,
-    UpdateTemplateSyncConfigOutputOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
+    UpdateComponentOutputTypeDef,
+    UpdateEnvironmentAccountConnectionOutputTypeDef,
+    UpdateEnvironmentOutputTypeDef,
+    UpdateEnvironmentTemplateOutputTypeDef,
+    UpdateEnvironmentTemplateVersionOutputTypeDef,
+    UpdateServiceInstanceOutputTypeDef,
+    UpdateServiceOutputTypeDef,
+    UpdateServicePipelineOutputTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
+    UpdateServiceTemplateOutputTypeDef,
+    UpdateServiceTemplateVersionOutputTypeDef,
+    UpdateTemplateSyncConfigOutputTypeDef,
 )
 from .waiter import (
     ComponentDeletedWaiter,
     ComponentDeployedWaiter,
     EnvironmentDeployedWaiter,
     EnvironmentTemplateVersionRegisteredWaiter,
     ServiceCreatedWaiter,
@@ -203,15 +203,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#exceptions)
         """
 
     def accept_environment_account_connection(
         self, *, id: str
-    ) -> AcceptEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> AcceptEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, an environment account connection request is accepted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#accept_environment_account_connection)
         """
 
@@ -221,48 +221,48 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#can_paginate)
         """
 
     def cancel_component_deployment(
         self, *, componentName: str
-    ) -> CancelComponentDeploymentOutputOutputTypeDef:
+    ) -> CancelComponentDeploymentOutputTypeDef:
         """
         Attempts to cancel a component deployment (for a component that is in the
         `IN_PROGRESS` deployment status).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_component_deployment)
         """
 
     def cancel_environment_deployment(
         self, *, environmentName: str
-    ) -> CancelEnvironmentDeploymentOutputOutputTypeDef:
+    ) -> CancelEnvironmentDeploymentOutputTypeDef:
         """
         Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
         the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_environment_deployment)
         """
 
     def cancel_service_instance_deployment(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> CancelServiceInstanceDeploymentOutputOutputTypeDef:
+    ) -> CancelServiceInstanceDeploymentOutputTypeDef:
         """
         Attempts to cancel a service instance deployment on an  UpdateServiceInstance
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_instance_deployment)
         """
 
     def cancel_service_pipeline_deployment(
         self, *, serviceName: str
-    ) -> CancelServicePipelineDeploymentOutputOutputTypeDef:
+    ) -> CancelServicePipelineDeploymentOutputTypeDef:
         """
         Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_pipeline_deployment)
         """
@@ -284,15 +284,15 @@
         clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateComponentOutputOutputTypeDef:
+    ) -> CreateComponentOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_component)
         """
 
@@ -307,15 +307,15 @@
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateEnvironmentOutputOutputTypeDef:
+    ) -> CreateEnvironmentOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment)
         """
 
@@ -325,15 +325,15 @@
         environmentName: str,
         managementAccountId: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_account_connection)
@@ -344,15 +344,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         provisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateOutputOutputTypeDef:
+    ) -> CreateEnvironmentTemplateOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template)
         """
 
@@ -361,15 +361,15 @@
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template_version)
         """
 
@@ -377,15 +377,15 @@
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRepositoryOutputOutputTypeDef:
+    ) -> CreateRepositoryOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_repository)
         """
 
@@ -398,15 +398,15 @@
         templateName: str,
         branchName: str = ...,
         description: str = ...,
         repositoryConnectionArn: str = ...,
         repositoryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceOutputOutputTypeDef:
+    ) -> CreateServiceOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service)
         """
 
@@ -416,15 +416,15 @@
         name: str,
         serviceName: str,
         spec: str,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceInstanceOutputOutputTypeDef:
+    ) -> CreateServiceInstanceOutputTypeDef:
         """
         Create a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_instance)
         """
 
@@ -432,15 +432,15 @@
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> CreateServiceSyncConfigOutputOutputTypeDef:
+    ) -> CreateServiceSyncConfigOutputTypeDef:
         """
         Create the Proton Ops configuration file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_sync_config)
         """
 
@@ -449,15 +449,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         pipelineProvisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateOutputOutputTypeDef:
+    ) -> CreateServiceTemplateOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template)
         """
 
@@ -468,15 +468,15 @@
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateVersionOutputOutputTypeDef:
+    ) -> CreateServiceTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template_version)
         """
 
@@ -485,130 +485,128 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> CreateTemplateSyncConfigOutputOutputTypeDef:
+    ) -> CreateTemplateSyncConfigOutputTypeDef:
         """
         Set up a template to create new template versions automatically by tracking a
         linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_template_sync_config)
         """
 
-    def delete_component(self, *, name: str) -> DeleteComponentOutputOutputTypeDef:
+    def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
 
-    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputOutputTypeDef:
+    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
         """
         Delete the deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_deployment)
         """
 
-    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputOutputTypeDef:
+    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
 
     def delete_environment_account_connection(
         self, *, id: str
-    ) -> DeleteEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> DeleteEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, delete an environment account connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_account_connection)
         """
 
-    def delete_environment_template(
-        self, *, name: str
-    ) -> DeleteEnvironmentTemplateOutputOutputTypeDef:
+    def delete_environment_template(self, *, name: str) -> DeleteEnvironmentTemplateOutputTypeDef:
         """
         If no other major or minor versions of an environment template exist, delete the
         environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template)
         """
 
     def delete_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> DeleteEnvironmentTemplateVersionOutputTypeDef:
         """
         If no other minor versions of an environment template exist, delete a major
         version of the environment template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template_version)
         """
 
     def delete_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> DeleteRepositoryOutputOutputTypeDef:
+    ) -> DeleteRepositoryOutputTypeDef:
         """
         De-register and unlink your repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_repository)
         """
 
-    def delete_service(self, *, name: str) -> DeleteServiceOutputOutputTypeDef:
+    def delete_service(self, *, name: str) -> DeleteServiceOutputTypeDef:
         """
         Delete a service, with its instances and pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service)
         """
 
     def delete_service_sync_config(
         self, *, serviceName: str
-    ) -> DeleteServiceSyncConfigOutputOutputTypeDef:
+    ) -> DeleteServiceSyncConfigOutputTypeDef:
         """
         Delete the Proton Ops file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_sync_config)
         """
 
-    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputOutputTypeDef:
+    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputTypeDef:
         """
         If no other major or minor versions of the service template exist, delete the
         service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template)
         """
 
     def delete_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteServiceTemplateVersionOutputOutputTypeDef:
+    ) -> DeleteServiceTemplateVersionOutputTypeDef:
         """
         If no other minor versions of a service template exist, delete a major version
         of the service template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template_version)
         """
 
     def delete_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> DeleteTemplateSyncConfigOutputOutputTypeDef:
+    ) -> DeleteTemplateSyncConfigOutputTypeDef:
         """
         Delete a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_template_sync_config)
         """
 
@@ -622,23 +620,23 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#generate_presigned_url)
         """
 
-    def get_account_settings(self) -> GetAccountSettingsOutputOutputTypeDef:
+    def get_account_settings(self) -> GetAccountSettingsOutputTypeDef:
         """
         Get detail data for Proton account-wide settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_account_settings)
         """
 
-    def get_component(self, *, name: str) -> GetComponentOutputOutputTypeDef:
+    def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
 
@@ -646,191 +644,189 @@
         self,
         *,
         id: str,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> GetDeploymentOutputOutputTypeDef:
+    ) -> GetDeploymentOutputTypeDef:
         """
         Get detailed data for a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_deployment)
         """
 
-    def get_environment(self, *, name: str) -> GetEnvironmentOutputOutputTypeDef:
+    def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
 
     def get_environment_account_connection(
         self, *, id: str
-    ) -> GetEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> GetEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, get the detailed data for an environment account
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_account_connection)
         """
 
-    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputOutputTypeDef:
+    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputTypeDef:
         """
         Get detailed data for an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template)
         """
 
     def get_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> GetEnvironmentTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template_version)
         """
 
     def get_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> GetRepositoryOutputOutputTypeDef:
+    ) -> GetRepositoryOutputTypeDef:
         """
         Get detail data for a linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository)
         """
 
     def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType
-    ) -> GetRepositorySyncStatusOutputOutputTypeDef:
+    ) -> GetRepositorySyncStatusOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository_sync_status)
         """
 
-    def get_resources_summary(self) -> GetResourcesSummaryOutputOutputTypeDef:
+    def get_resources_summary(self) -> GetResourcesSummaryOutputTypeDef:
         """
         Get counts of Proton resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_resources_summary)
         """
 
-    def get_service(self, *, name: str) -> GetServiceOutputOutputTypeDef:
+    def get_service(self, *, name: str) -> GetServiceOutputTypeDef:
         """
         Get detailed data for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service)
         """
 
     def get_service_instance(
         self, *, name: str, serviceName: str
-    ) -> GetServiceInstanceOutputOutputTypeDef:
+    ) -> GetServiceInstanceOutputTypeDef:
         """
         Get detailed data for a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance)
         """
 
     def get_service_instance_sync_status(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> GetServiceInstanceSyncStatusOutputOutputTypeDef:
+    ) -> GetServiceInstanceSyncStatusOutputTypeDef:
         """
         Get the status of the synced service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance_sync_status)
         """
 
     def get_service_sync_blocker_summary(
         self, *, serviceName: str, serviceInstanceName: str = ...
-    ) -> GetServiceSyncBlockerSummaryOutputOutputTypeDef:
+    ) -> GetServiceSyncBlockerSummaryOutputTypeDef:
         """
         Get detailed data for the service sync blocker summary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_blocker_summary)
         """
 
-    def get_service_sync_config(
-        self, *, serviceName: str
-    ) -> GetServiceSyncConfigOutputOutputTypeDef:
+    def get_service_sync_config(self, *, serviceName: str) -> GetServiceSyncConfigOutputTypeDef:
         """
         Get detailed information for the service sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_config)
         """
 
-    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputOutputTypeDef:
+    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputTypeDef:
         """
         Get detailed data for a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template)
         """
 
     def get_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetServiceTemplateVersionOutputOutputTypeDef:
+    ) -> GetServiceTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template_version)
         """
 
     def get_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> GetTemplateSyncConfigOutputOutputTypeDef:
+    ) -> GetTemplateSyncConfigOutputTypeDef:
         """
         Get detail data for a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_config)
         """
 
     def get_template_sync_status(
         self, *, templateName: str, templateType: TemplateTypeType, templateVersion: str
-    ) -> GetTemplateSyncStatusOutputOutputTypeDef:
+    ) -> GetTemplateSyncStatusOutputTypeDef:
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
 
     def list_component_outputs(
         self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListComponentOutputsOutputOutputTypeDef:
+    ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
 
     def list_component_provisioned_resources(
         self, *, componentName: str, nextToken: str = ...
-    ) -> ListComponentProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListComponentProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a component with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_provisioned_resources)
         """
 
@@ -838,15 +834,15 @@
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListComponentsOutputOutputTypeDef:
+    ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
 
@@ -855,15 +851,15 @@
         *,
         componentName: str = ...,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListDeploymentsOutputOutputTypeDef:
+    ) -> ListDeploymentsOutputTypeDef:
         """
         List deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_deployments)
         """
 
@@ -871,124 +867,124 @@
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...
-    ) -> ListEnvironmentAccountConnectionsOutputOutputTypeDef:
+    ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
 
     def list_environment_outputs(
         self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListEnvironmentOutputsOutputOutputTypeDef:
+    ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
 
     def list_environment_provisioned_resources(
         self, *, environmentName: str, nextToken: str = ...
-    ) -> ListEnvironmentProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListEnvironmentProvisionedResourcesOutputTypeDef:
         """
         List the provisioned resources for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_provisioned_resources)
         """
 
     def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentTemplateVersionsOutputOutputTypeDef:
+    ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_template_versions)
         """
 
     def list_environment_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListEnvironmentTemplatesOutputOutputTypeDef:
+    ) -> ListEnvironmentTemplatesOutputTypeDef:
         """
         List environment templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_templates)
         """
 
     def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentsOutputOutputTypeDef:
+    ) -> ListEnvironmentsOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environments)
         """
 
     def list_repositories(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListRepositoriesOutputOutputTypeDef:
+    ) -> ListRepositoriesOutputTypeDef:
         """
         List linked repositories with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repositories)
         """
 
     def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         nextToken: str = ...
-    ) -> ListRepositorySyncDefinitionsOutputOutputTypeDef:
+    ) -> ListRepositorySyncDefinitionsOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
 
     def list_service_instance_outputs(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         nextToken: str = ...
-    ) -> ListServiceInstanceOutputsOutputOutputTypeDef:
+    ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
 
     def list_service_instance_provisioned_resources(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
-    ) -> ListServiceInstanceProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service instance with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_provisioned_resources)
         """
 
@@ -997,80 +993,80 @@
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...
-    ) -> ListServiceInstancesOutputOutputTypeDef:
+    ) -> ListServiceInstancesOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
 
     def list_service_pipeline_outputs(
         self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListServicePipelineOutputsOutputOutputTypeDef:
+    ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
 
     def list_service_pipeline_provisioned_resources(
         self, *, serviceName: str, nextToken: str = ...
-    ) -> ListServicePipelineProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListServicePipelineProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service and pipeline with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_provisioned_resources)
         """
 
     def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListServiceTemplateVersionsOutputOutputTypeDef:
+    ) -> ListServiceTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_template_versions)
         """
 
     def list_service_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServiceTemplatesOutputOutputTypeDef:
+    ) -> ListServiceTemplatesOutputTypeDef:
         """
         List service templates with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_templates)
         """
 
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServicesOutputOutputTypeDef:
+    ) -> ListServicesOutputTypeDef:
         """
         List services with summaries of detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_services)
         """
 
     def list_tags_for_resource(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListTagsForResourceOutputOutputTypeDef:
+    ) -> ListTagsForResourceOutputTypeDef:
         """
         List tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_tags_for_resource)
         """
 
@@ -1089,15 +1085,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#notify_resource_deployment_status_change)
         """
 
     def reject_environment_account_connection(
         self, *, id: str
-    ) -> RejectEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> RejectEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, reject an environment account connection from another
         environment account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#reject_environment_account_connection)
         """
@@ -1121,15 +1117,15 @@
     def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
         pipelineServiceRoleArn: str = ...
-    ) -> UpdateAccountSettingsOutputOutputTypeDef:
+    ) -> UpdateAccountSettingsOutputTypeDef:
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_account_settings)
         """
@@ -1141,15 +1137,15 @@
         name: str,
         clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         templateFile: str = ...
-    ) -> UpdateComponentOutputOutputTypeDef:
+    ) -> UpdateComponentOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_component)
         """
 
@@ -1163,41 +1159,41 @@
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateEnvironmentOutputOutputTypeDef:
+    ) -> UpdateEnvironmentOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment)
         """
 
     def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...
-    ) -> UpdateEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> UpdateEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, update an environment account connection to use a new
         IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_account_connection)
         """
 
     def update_environment_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateEnvironmentTemplateOutputOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateOutputTypeDef:
         """
         Update an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template)
         """
 
@@ -1205,25 +1201,25 @@
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
         status: TemplateVersionStatusType = ...
-    ) -> UpdateEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template_version)
         """
 
     def update_service(
         self, *, name: str, description: str = ..., spec: str = ...
-    ) -> UpdateServiceOutputOutputTypeDef:
+    ) -> UpdateServiceOutputTypeDef:
         """
         Edit a service description or use a spec to add and delete service instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service)
         """
 
@@ -1233,15 +1229,15 @@
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
         clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServiceInstanceOutputOutputTypeDef:
+    ) -> UpdateServiceInstanceOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_instance)
         """
 
@@ -1249,25 +1245,25 @@
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServicePipelineOutputOutputTypeDef:
+    ) -> UpdateServicePipelineOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_pipeline)
         """
 
     def update_service_sync_blocker(
         self, *, id: str, resolvedReason: str
-    ) -> UpdateServiceSyncBlockerOutputOutputTypeDef:
+    ) -> UpdateServiceSyncBlockerOutputTypeDef:
         """
         Update the service sync blocker by resolving it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_blocker)
         """
 
@@ -1275,25 +1271,25 @@
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> UpdateServiceSyncConfigOutputOutputTypeDef:
+    ) -> UpdateServiceSyncConfigOutputTypeDef:
         """
         Update the Proton Ops config file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_config)
         """
 
     def update_service_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateServiceTemplateOutputOutputTypeDef:
+    ) -> UpdateServiceTemplateOutputTypeDef:
         """
         Update a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template)
         """
 
@@ -1303,15 +1299,15 @@
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
         description: str = ...,
         status: TemplateVersionStatusType = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...
-    ) -> UpdateServiceTemplateVersionOutputOutputTypeDef:
+    ) -> UpdateServiceTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template_version)
         """
 
@@ -1320,15 +1316,15 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> UpdateTemplateSyncConfigOutputOutputTypeDef:
+    ) -> UpdateTemplateSyncConfigOutputTypeDef:
         """
         Update template sync configuration parameters, except for the `templateName` and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_template_sync_config)
         """
```

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/client.pyi` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -51,105 +51,105 @@
     ListServicePipelineProvisionedResourcesPaginator,
     ListServicesPaginator,
     ListServiceTemplatesPaginator,
     ListServiceTemplateVersionsPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AcceptEnvironmentAccountConnectionOutputOutputTypeDef,
-    CancelComponentDeploymentOutputOutputTypeDef,
-    CancelEnvironmentDeploymentOutputOutputTypeDef,
-    CancelServiceInstanceDeploymentOutputOutputTypeDef,
-    CancelServicePipelineDeploymentOutputOutputTypeDef,
+    AcceptEnvironmentAccountConnectionOutputTypeDef,
+    CancelComponentDeploymentOutputTypeDef,
+    CancelEnvironmentDeploymentOutputTypeDef,
+    CancelServiceInstanceDeploymentOutputTypeDef,
+    CancelServicePipelineDeploymentOutputTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
-    CreateComponentOutputOutputTypeDef,
-    CreateEnvironmentAccountConnectionOutputOutputTypeDef,
-    CreateEnvironmentOutputOutputTypeDef,
-    CreateEnvironmentTemplateOutputOutputTypeDef,
-    CreateEnvironmentTemplateVersionOutputOutputTypeDef,
-    CreateRepositoryOutputOutputTypeDef,
-    CreateServiceInstanceOutputOutputTypeDef,
-    CreateServiceOutputOutputTypeDef,
-    CreateServiceSyncConfigOutputOutputTypeDef,
-    CreateServiceTemplateOutputOutputTypeDef,
-    CreateServiceTemplateVersionOutputOutputTypeDef,
-    CreateTemplateSyncConfigOutputOutputTypeDef,
-    DeleteComponentOutputOutputTypeDef,
-    DeleteDeploymentOutputOutputTypeDef,
-    DeleteEnvironmentAccountConnectionOutputOutputTypeDef,
-    DeleteEnvironmentOutputOutputTypeDef,
-    DeleteEnvironmentTemplateOutputOutputTypeDef,
-    DeleteEnvironmentTemplateVersionOutputOutputTypeDef,
-    DeleteRepositoryOutputOutputTypeDef,
-    DeleteServiceOutputOutputTypeDef,
-    DeleteServiceSyncConfigOutputOutputTypeDef,
-    DeleteServiceTemplateOutputOutputTypeDef,
-    DeleteServiceTemplateVersionOutputOutputTypeDef,
-    DeleteTemplateSyncConfigOutputOutputTypeDef,
+    CreateComponentOutputTypeDef,
+    CreateEnvironmentAccountConnectionOutputTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateEnvironmentTemplateOutputTypeDef,
+    CreateEnvironmentTemplateVersionOutputTypeDef,
+    CreateRepositoryOutputTypeDef,
+    CreateServiceInstanceOutputTypeDef,
+    CreateServiceOutputTypeDef,
+    CreateServiceSyncConfigOutputTypeDef,
+    CreateServiceTemplateOutputTypeDef,
+    CreateServiceTemplateVersionOutputTypeDef,
+    CreateTemplateSyncConfigOutputTypeDef,
+    DeleteComponentOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
+    DeleteEnvironmentAccountConnectionOutputTypeDef,
+    DeleteEnvironmentOutputTypeDef,
+    DeleteEnvironmentTemplateOutputTypeDef,
+    DeleteEnvironmentTemplateVersionOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    DeleteServiceOutputTypeDef,
+    DeleteServiceSyncConfigOutputTypeDef,
+    DeleteServiceTemplateOutputTypeDef,
+    DeleteServiceTemplateVersionOutputTypeDef,
+    DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
-    GetAccountSettingsOutputOutputTypeDef,
-    GetComponentOutputOutputTypeDef,
-    GetDeploymentOutputOutputTypeDef,
-    GetEnvironmentAccountConnectionOutputOutputTypeDef,
-    GetEnvironmentOutputOutputTypeDef,
-    GetEnvironmentTemplateOutputOutputTypeDef,
-    GetEnvironmentTemplateVersionOutputOutputTypeDef,
-    GetRepositoryOutputOutputTypeDef,
-    GetRepositorySyncStatusOutputOutputTypeDef,
-    GetResourcesSummaryOutputOutputTypeDef,
-    GetServiceInstanceOutputOutputTypeDef,
-    GetServiceInstanceSyncStatusOutputOutputTypeDef,
-    GetServiceOutputOutputTypeDef,
-    GetServiceSyncBlockerSummaryOutputOutputTypeDef,
-    GetServiceSyncConfigOutputOutputTypeDef,
-    GetServiceTemplateOutputOutputTypeDef,
-    GetServiceTemplateVersionOutputOutputTypeDef,
-    GetTemplateSyncConfigOutputOutputTypeDef,
-    GetTemplateSyncStatusOutputOutputTypeDef,
-    ListComponentOutputsOutputOutputTypeDef,
-    ListComponentProvisionedResourcesOutputOutputTypeDef,
-    ListComponentsOutputOutputTypeDef,
-    ListDeploymentsOutputOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
-    ListEnvironmentOutputsOutputOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
-    ListEnvironmentsOutputOutputTypeDef,
-    ListEnvironmentTemplatesOutputOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
-    ListRepositoriesOutputOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputOutputTypeDef,
-    ListServiceInstanceOutputsOutputOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
+    GetComponentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
+    GetEnvironmentAccountConnectionOutputTypeDef,
+    GetEnvironmentOutputTypeDef,
+    GetEnvironmentTemplateOutputTypeDef,
+    GetEnvironmentTemplateVersionOutputTypeDef,
+    GetRepositoryOutputTypeDef,
+    GetRepositorySyncStatusOutputTypeDef,
+    GetResourcesSummaryOutputTypeDef,
+    GetServiceInstanceOutputTypeDef,
+    GetServiceInstanceSyncStatusOutputTypeDef,
+    GetServiceOutputTypeDef,
+    GetServiceSyncBlockerSummaryOutputTypeDef,
+    GetServiceSyncConfigOutputTypeDef,
+    GetServiceTemplateOutputTypeDef,
+    GetServiceTemplateVersionOutputTypeDef,
+    GetTemplateSyncConfigOutputTypeDef,
+    GetTemplateSyncStatusOutputTypeDef,
+    ListComponentOutputsOutputTypeDef,
+    ListComponentProvisionedResourcesOutputTypeDef,
+    ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputTypeDef,
+    ListEnvironmentOutputsOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListEnvironmentTemplatesOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputTypeDef,
+    ListRepositoriesOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstanceOutputsOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputOutputTypeDef,
-    ListServicePipelineOutputsOutputOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
-    ListServicesOutputOutputTypeDef,
-    ListServiceTemplatesOutputOutputTypeDef,
-    ListServiceTemplateVersionsOutputOutputTypeDef,
-    ListTagsForResourceOutputOutputTypeDef,
+    ListServiceInstancesOutputTypeDef,
+    ListServicePipelineOutputsOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputTypeDef,
+    ListServicesOutputTypeDef,
+    ListServiceTemplatesOutputTypeDef,
+    ListServiceTemplateVersionsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     OutputTypeDef,
-    RejectEnvironmentAccountConnectionOutputOutputTypeDef,
+    RejectEnvironmentAccountConnectionOutputTypeDef,
     RepositoryBranchInputTypeDef,
     TagTypeDef,
     TemplateVersionSourceInputTypeDef,
-    UpdateAccountSettingsOutputOutputTypeDef,
-    UpdateComponentOutputOutputTypeDef,
-    UpdateEnvironmentAccountConnectionOutputOutputTypeDef,
-    UpdateEnvironmentOutputOutputTypeDef,
-    UpdateEnvironmentTemplateOutputOutputTypeDef,
-    UpdateEnvironmentTemplateVersionOutputOutputTypeDef,
-    UpdateServiceInstanceOutputOutputTypeDef,
-    UpdateServiceOutputOutputTypeDef,
-    UpdateServicePipelineOutputOutputTypeDef,
-    UpdateServiceSyncBlockerOutputOutputTypeDef,
-    UpdateServiceSyncConfigOutputOutputTypeDef,
-    UpdateServiceTemplateOutputOutputTypeDef,
-    UpdateServiceTemplateVersionOutputOutputTypeDef,
-    UpdateTemplateSyncConfigOutputOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
+    UpdateComponentOutputTypeDef,
+    UpdateEnvironmentAccountConnectionOutputTypeDef,
+    UpdateEnvironmentOutputTypeDef,
+    UpdateEnvironmentTemplateOutputTypeDef,
+    UpdateEnvironmentTemplateVersionOutputTypeDef,
+    UpdateServiceInstanceOutputTypeDef,
+    UpdateServiceOutputTypeDef,
+    UpdateServicePipelineOutputTypeDef,
+    UpdateServiceSyncBlockerOutputTypeDef,
+    UpdateServiceSyncConfigOutputTypeDef,
+    UpdateServiceTemplateOutputTypeDef,
+    UpdateServiceTemplateVersionOutputTypeDef,
+    UpdateTemplateSyncConfigOutputTypeDef,
 )
 from .waiter import (
     ComponentDeletedWaiter,
     ComponentDeployedWaiter,
     EnvironmentDeployedWaiter,
     EnvironmentTemplateVersionRegisteredWaiter,
     ServiceCreatedWaiter,
@@ -198,15 +198,15 @@
         ProtonClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#exceptions)
         """
     def accept_environment_account_connection(
         self, *, id: str
-    ) -> AcceptEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> AcceptEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, an environment account connection request is accepted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.accept_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#accept_environment_account_connection)
         """
     def can_paginate(self, operation_name: str) -> bool:
@@ -214,45 +214,45 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#can_paginate)
         """
     def cancel_component_deployment(
         self, *, componentName: str
-    ) -> CancelComponentDeploymentOutputOutputTypeDef:
+    ) -> CancelComponentDeploymentOutputTypeDef:
         """
         Attempts to cancel a component deployment (for a component that is in the
         `IN_PROGRESS` deployment status).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_component_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_component_deployment)
         """
     def cancel_environment_deployment(
         self, *, environmentName: str
-    ) -> CancelEnvironmentDeploymentOutputOutputTypeDef:
+    ) -> CancelEnvironmentDeploymentOutputTypeDef:
         """
         Attempts to cancel an environment deployment on an  UpdateEnvironment action, if
         the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_environment_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_environment_deployment)
         """
     def cancel_service_instance_deployment(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> CancelServiceInstanceDeploymentOutputOutputTypeDef:
+    ) -> CancelServiceInstanceDeploymentOutputTypeDef:
         """
         Attempts to cancel a service instance deployment on an  UpdateServiceInstance
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_instance_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_instance_deployment)
         """
     def cancel_service_pipeline_deployment(
         self, *, serviceName: str
-    ) -> CancelServicePipelineDeploymentOutputOutputTypeDef:
+    ) -> CancelServicePipelineDeploymentOutputTypeDef:
         """
         Attempts to cancel a service pipeline deployment on an  UpdateServicePipeline
         action, if the deployment is `IN_PROGRESS`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.cancel_service_pipeline_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#cancel_service_pipeline_deployment)
         """
@@ -272,15 +272,15 @@
         clientToken: str = ...,
         description: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateComponentOutputOutputTypeDef:
+    ) -> CreateComponentOutputTypeDef:
         """
         Create an Proton component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_component)
         """
     def create_environment(
@@ -294,15 +294,15 @@
         componentRoleArn: str = ...,
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateEnvironmentOutputOutputTypeDef:
+    ) -> CreateEnvironmentOutputTypeDef:
         """
         Deploy a new environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment)
         """
     def create_environment_account_connection(
@@ -311,15 +311,15 @@
         environmentName: str,
         managementAccountId: str,
         clientToken: str = ...,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> CreateEnvironmentAccountConnectionOutputTypeDef:
         """
         Create an environment account connection in an environment account so that
         environment infrastructure resources can be provisioned in the environment
         account from a management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_account_connection)
@@ -329,15 +329,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         provisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateOutputOutputTypeDef:
+    ) -> CreateEnvironmentTemplateOutputTypeDef:
         """
         Create an environment template for Proton.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template)
         """
     def create_environment_template_version(
@@ -345,30 +345,30 @@
         *,
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> CreateEnvironmentTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_environment_template_version)
         """
     def create_repository(
         self,
         *,
         connectionArn: str,
         name: str,
         provider: RepositoryProviderType,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRepositoryOutputOutputTypeDef:
+    ) -> CreateRepositoryOutputTypeDef:
         """
         Create and register a link to a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_repository)
         """
     def create_service(
@@ -380,15 +380,15 @@
         templateName: str,
         branchName: str = ...,
         description: str = ...,
         repositoryConnectionArn: str = ...,
         repositoryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceOutputOutputTypeDef:
+    ) -> CreateServiceOutputTypeDef:
         """
         Create an Proton service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service)
         """
     def create_service_instance(
@@ -397,30 +397,30 @@
         name: str,
         serviceName: str,
         spec: str,
         clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> CreateServiceInstanceOutputOutputTypeDef:
+    ) -> CreateServiceInstanceOutputTypeDef:
         """
         Create a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_instance)
         """
     def create_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> CreateServiceSyncConfigOutputOutputTypeDef:
+    ) -> CreateServiceSyncConfigOutputTypeDef:
         """
         Create the Proton Ops configuration file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_sync_config)
         """
     def create_service_template(
@@ -428,15 +428,15 @@
         *,
         name: str,
         description: str = ...,
         displayName: str = ...,
         encryptionKey: str = ...,
         pipelineProvisioning: Literal["CUSTOMER_MANAGED"] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateOutputOutputTypeDef:
+    ) -> CreateServiceTemplateOutputTypeDef:
         """
         Create a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template)
         """
     def create_service_template_version(
@@ -446,15 +446,15 @@
         source: TemplateVersionSourceInputTypeDef,
         templateName: str,
         clientToken: str = ...,
         description: str = ...,
         majorVersion: str = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateServiceTemplateVersionOutputOutputTypeDef:
+    ) -> CreateServiceTemplateVersionOutputTypeDef:
         """
         Create a new major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_service_template_version)
         """
     def create_template_sync_config(
@@ -462,118 +462,116 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> CreateTemplateSyncConfigOutputOutputTypeDef:
+    ) -> CreateTemplateSyncConfigOutputTypeDef:
         """
         Set up a template to create new template versions automatically by tracking a
         linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.create_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#create_template_sync_config)
         """
-    def delete_component(self, *, name: str) -> DeleteComponentOutputOutputTypeDef:
+    def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
-    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputOutputTypeDef:
+    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
         """
         Delete the deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_deployment)
         """
-    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputOutputTypeDef:
+    def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
     def delete_environment_account_connection(
         self, *, id: str
-    ) -> DeleteEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> DeleteEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, delete an environment account connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_account_connection)
         """
-    def delete_environment_template(
-        self, *, name: str
-    ) -> DeleteEnvironmentTemplateOutputOutputTypeDef:
+    def delete_environment_template(self, *, name: str) -> DeleteEnvironmentTemplateOutputTypeDef:
         """
         If no other major or minor versions of an environment template exist, delete the
         environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template)
         """
     def delete_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> DeleteEnvironmentTemplateVersionOutputTypeDef:
         """
         If no other minor versions of an environment template exist, delete a major
         version of the environment template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment_template_version)
         """
     def delete_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> DeleteRepositoryOutputOutputTypeDef:
+    ) -> DeleteRepositoryOutputTypeDef:
         """
         De-register and unlink your repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_repository)
         """
-    def delete_service(self, *, name: str) -> DeleteServiceOutputOutputTypeDef:
+    def delete_service(self, *, name: str) -> DeleteServiceOutputTypeDef:
         """
         Delete a service, with its instances and pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service)
         """
     def delete_service_sync_config(
         self, *, serviceName: str
-    ) -> DeleteServiceSyncConfigOutputOutputTypeDef:
+    ) -> DeleteServiceSyncConfigOutputTypeDef:
         """
         Delete the Proton Ops file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_sync_config)
         """
-    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputOutputTypeDef:
+    def delete_service_template(self, *, name: str) -> DeleteServiceTemplateOutputTypeDef:
         """
         If no other major or minor versions of the service template exist, delete the
         service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template)
         """
     def delete_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> DeleteServiceTemplateVersionOutputOutputTypeDef:
+    ) -> DeleteServiceTemplateVersionOutputTypeDef:
         """
         If no other minor versions of a service template exist, delete a major version
         of the service template if it's not the `Recommended` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_service_template_version)
         """
     def delete_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> DeleteTemplateSyncConfigOutputOutputTypeDef:
+    ) -> DeleteTemplateSyncConfigOutputTypeDef:
         """
         Delete a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_template_sync_config)
         """
     def generate_presigned_url(
@@ -585,210 +583,208 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#generate_presigned_url)
         """
-    def get_account_settings(self) -> GetAccountSettingsOutputOutputTypeDef:
+    def get_account_settings(self) -> GetAccountSettingsOutputTypeDef:
         """
         Get detail data for Proton account-wide settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_account_settings)
         """
-    def get_component(self, *, name: str) -> GetComponentOutputOutputTypeDef:
+    def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
     def get_deployment(
         self,
         *,
         id: str,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> GetDeploymentOutputOutputTypeDef:
+    ) -> GetDeploymentOutputTypeDef:
         """
         Get detailed data for a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_deployment)
         """
-    def get_environment(self, *, name: str) -> GetEnvironmentOutputOutputTypeDef:
+    def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
     def get_environment_account_connection(
         self, *, id: str
-    ) -> GetEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> GetEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, get the detailed data for an environment account
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_account_connection)
         """
-    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputOutputTypeDef:
+    def get_environment_template(self, *, name: str) -> GetEnvironmentTemplateOutputTypeDef:
         """
         Get detailed data for an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template)
         """
     def get_environment_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> GetEnvironmentTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment_template_version)
         """
     def get_repository(
         self, *, name: str, provider: RepositoryProviderType
-    ) -> GetRepositoryOutputOutputTypeDef:
+    ) -> GetRepositoryOutputTypeDef:
         """
         Get detail data for a linked repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository)
         """
     def get_repository_sync_status(
         self,
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType
-    ) -> GetRepositorySyncStatusOutputOutputTypeDef:
+    ) -> GetRepositorySyncStatusOutputTypeDef:
         """
         Get the sync status of a repository used for Proton template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_repository_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_repository_sync_status)
         """
-    def get_resources_summary(self) -> GetResourcesSummaryOutputOutputTypeDef:
+    def get_resources_summary(self) -> GetResourcesSummaryOutputTypeDef:
         """
         Get counts of Proton resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_resources_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_resources_summary)
         """
-    def get_service(self, *, name: str) -> GetServiceOutputOutputTypeDef:
+    def get_service(self, *, name: str) -> GetServiceOutputTypeDef:
         """
         Get detailed data for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service)
         """
     def get_service_instance(
         self, *, name: str, serviceName: str
-    ) -> GetServiceInstanceOutputOutputTypeDef:
+    ) -> GetServiceInstanceOutputTypeDef:
         """
         Get detailed data for a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance)
         """
     def get_service_instance_sync_status(
         self, *, serviceInstanceName: str, serviceName: str
-    ) -> GetServiceInstanceSyncStatusOutputOutputTypeDef:
+    ) -> GetServiceInstanceSyncStatusOutputTypeDef:
         """
         Get the status of the synced service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_instance_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_instance_sync_status)
         """
     def get_service_sync_blocker_summary(
         self, *, serviceName: str, serviceInstanceName: str = ...
-    ) -> GetServiceSyncBlockerSummaryOutputOutputTypeDef:
+    ) -> GetServiceSyncBlockerSummaryOutputTypeDef:
         """
         Get detailed data for the service sync blocker summary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_blocker_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_blocker_summary)
         """
-    def get_service_sync_config(
-        self, *, serviceName: str
-    ) -> GetServiceSyncConfigOutputOutputTypeDef:
+    def get_service_sync_config(self, *, serviceName: str) -> GetServiceSyncConfigOutputTypeDef:
         """
         Get detailed information for the service sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_sync_config)
         """
-    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputOutputTypeDef:
+    def get_service_template(self, *, name: str) -> GetServiceTemplateOutputTypeDef:
         """
         Get detailed data for a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template)
         """
     def get_service_template_version(
         self, *, majorVersion: str, minorVersion: str, templateName: str
-    ) -> GetServiceTemplateVersionOutputOutputTypeDef:
+    ) -> GetServiceTemplateVersionOutputTypeDef:
         """
         Get detailed data for a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_service_template_version)
         """
     def get_template_sync_config(
         self, *, templateName: str, templateType: TemplateTypeType
-    ) -> GetTemplateSyncConfigOutputOutputTypeDef:
+    ) -> GetTemplateSyncConfigOutputTypeDef:
         """
         Get detail data for a template sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_config)
         """
     def get_template_sync_status(
         self, *, templateName: str, templateType: TemplateTypeType, templateVersion: str
-    ) -> GetTemplateSyncStatusOutputOutputTypeDef:
+    ) -> GetTemplateSyncStatusOutputTypeDef:
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
     def list_component_outputs(
         self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListComponentOutputsOutputOutputTypeDef:
+    ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
     def list_component_provisioned_resources(
         self, *, componentName: str, nextToken: str = ...
-    ) -> ListComponentProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListComponentProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a component with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_provisioned_resources)
         """
     def list_components(
         self,
         *,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListComponentsOutputOutputTypeDef:
+    ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
     def list_deployments(
@@ -796,130 +792,130 @@
         *,
         componentName: str = ...,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...
-    ) -> ListDeploymentsOutputOutputTypeDef:
+    ) -> ListDeploymentsOutputTypeDef:
         """
         List deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_deployments)
         """
     def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...
-    ) -> ListEnvironmentAccountConnectionsOutputOutputTypeDef:
+    ) -> ListEnvironmentAccountConnectionsOutputTypeDef:
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
     def list_environment_outputs(
         self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListEnvironmentOutputsOutputOutputTypeDef:
+    ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
     def list_environment_provisioned_resources(
         self, *, environmentName: str, nextToken: str = ...
-    ) -> ListEnvironmentProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListEnvironmentProvisionedResourcesOutputTypeDef:
         """
         List the provisioned resources for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_provisioned_resources)
         """
     def list_environment_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentTemplateVersionsOutputOutputTypeDef:
+    ) -> ListEnvironmentTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of an environment template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_template_versions)
         """
     def list_environment_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListEnvironmentTemplatesOutputOutputTypeDef:
+    ) -> ListEnvironmentTemplatesOutputTypeDef:
         """
         List environment templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_templates)
         """
     def list_environments(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListEnvironmentsOutputOutputTypeDef:
+    ) -> ListEnvironmentsOutputTypeDef:
         """
         List environments with detail data summaries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environments)
         """
     def list_repositories(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListRepositoriesOutputOutputTypeDef:
+    ) -> ListRepositoriesOutputTypeDef:
         """
         List linked repositories with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repositories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repositories)
         """
     def list_repository_sync_definitions(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         nextToken: str = ...
-    ) -> ListRepositorySyncDefinitionsOutputOutputTypeDef:
+    ) -> ListRepositorySyncDefinitionsOutputTypeDef:
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
     def list_service_instance_outputs(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         nextToken: str = ...
-    ) -> ListServiceInstanceOutputsOutputOutputTypeDef:
+    ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
     def list_service_instance_provisioned_resources(
         self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
-    ) -> ListServiceInstanceProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListServiceInstanceProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service instance with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_provisioned_resources)
         """
     def list_service_instances(
@@ -927,74 +923,74 @@
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...
-    ) -> ListServiceInstancesOutputOutputTypeDef:
+    ) -> ListServiceInstancesOutputTypeDef:
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
     def list_service_pipeline_outputs(
         self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
-    ) -> ListServicePipelineOutputsOutputOutputTypeDef:
+    ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
     def list_service_pipeline_provisioned_resources(
         self, *, serviceName: str, nextToken: str = ...
-    ) -> ListServicePipelineProvisionedResourcesOutputOutputTypeDef:
+    ) -> ListServicePipelineProvisionedResourcesOutputTypeDef:
         """
         List provisioned resources for a service and pipeline with details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_provisioned_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_provisioned_resources)
         """
     def list_service_template_versions(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
-    ) -> ListServiceTemplateVersionsOutputOutputTypeDef:
+    ) -> ListServiceTemplateVersionsOutputTypeDef:
         """
         List major or minor versions of a service template with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_template_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_template_versions)
         """
     def list_service_templates(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServiceTemplatesOutputOutputTypeDef:
+    ) -> ListServiceTemplatesOutputTypeDef:
         """
         List service templates with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_templates)
         """
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
-    ) -> ListServicesOutputOutputTypeDef:
+    ) -> ListServicesOutputTypeDef:
         """
         List services with summaries of detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_services)
         """
     def list_tags_for_resource(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListTagsForResourceOutputOutputTypeDef:
+    ) -> ListTagsForResourceOutputTypeDef:
         """
         List tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_tags_for_resource)
         """
     def notify_resource_deployment_status_change(
@@ -1011,15 +1007,15 @@
         managed provisioning.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.notify_resource_deployment_status_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#notify_resource_deployment_status_change)
         """
     def reject_environment_account_connection(
         self, *, id: str
-    ) -> RejectEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> RejectEnvironmentAccountConnectionOutputTypeDef:
         """
         In a management account, reject an environment account connection from another
         environment account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.reject_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#reject_environment_account_connection)
         """
@@ -1040,15 +1036,15 @@
     def update_account_settings(
         self,
         *,
         deletePipelineProvisioningRepository: bool = ...,
         pipelineCodebuildRoleArn: str = ...,
         pipelineProvisioningRepository: RepositoryBranchInputTypeDef = ...,
         pipelineServiceRoleArn: str = ...
-    ) -> UpdateAccountSettingsOutputOutputTypeDef:
+    ) -> UpdateAccountSettingsOutputTypeDef:
         """
         Update Proton settings that are used for multiple services in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_account_settings)
         """
@@ -1059,15 +1055,15 @@
         name: str,
         clientToken: str = ...,
         description: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         serviceSpec: str = ...,
         templateFile: str = ...
-    ) -> UpdateComponentOutputOutputTypeDef:
+    ) -> UpdateComponentOutputTypeDef:
         """
         Update a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_component)
         """
     def update_environment(
@@ -1080,63 +1076,63 @@
         description: str = ...,
         environmentAccountConnectionId: str = ...,
         protonServiceRoleArn: str = ...,
         provisioningRepository: RepositoryBranchInputTypeDef = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateEnvironmentOutputOutputTypeDef:
+    ) -> UpdateEnvironmentOutputTypeDef:
         """
         Update an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment)
         """
     def update_environment_account_connection(
         self,
         *,
         id: str,
         codebuildRoleArn: str = ...,
         componentRoleArn: str = ...,
         roleArn: str = ...
-    ) -> UpdateEnvironmentAccountConnectionOutputOutputTypeDef:
+    ) -> UpdateEnvironmentAccountConnectionOutputTypeDef:
         """
         In an environment account, update an environment account connection to use a new
         IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_account_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_account_connection)
         """
     def update_environment_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateEnvironmentTemplateOutputOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateOutputTypeDef:
         """
         Update an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template)
         """
     def update_environment_template_version(
         self,
         *,
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         description: str = ...,
         status: TemplateVersionStatusType = ...
-    ) -> UpdateEnvironmentTemplateVersionOutputOutputTypeDef:
+    ) -> UpdateEnvironmentTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of an environment template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_environment_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_environment_template_version)
         """
     def update_service(
         self, *, name: str, description: str = ..., spec: str = ...
-    ) -> UpdateServiceOutputOutputTypeDef:
+    ) -> UpdateServiceOutputTypeDef:
         """
         Edit a service description or use a spec to add and delete service instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service)
         """
     def update_service_instance(
@@ -1145,63 +1141,63 @@
         deploymentType: DeploymentUpdateTypeType,
         name: str,
         serviceName: str,
         clientToken: str = ...,
         spec: str = ...,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServiceInstanceOutputOutputTypeDef:
+    ) -> UpdateServiceInstanceOutputTypeDef:
         """
         Update a service instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_instance)
         """
     def update_service_pipeline(
         self,
         *,
         deploymentType: DeploymentUpdateTypeType,
         serviceName: str,
         spec: str,
         templateMajorVersion: str = ...,
         templateMinorVersion: str = ...
-    ) -> UpdateServicePipelineOutputOutputTypeDef:
+    ) -> UpdateServicePipelineOutputTypeDef:
         """
         Update the service pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_pipeline)
         """
     def update_service_sync_blocker(
         self, *, id: str, resolvedReason: str
-    ) -> UpdateServiceSyncBlockerOutputOutputTypeDef:
+    ) -> UpdateServiceSyncBlockerOutputTypeDef:
         """
         Update the service sync blocker by resolving it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_blocker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_blocker)
         """
     def update_service_sync_config(
         self,
         *,
         branch: str,
         filePath: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         serviceName: str
-    ) -> UpdateServiceSyncConfigOutputOutputTypeDef:
+    ) -> UpdateServiceSyncConfigOutputTypeDef:
         """
         Update the Proton Ops config file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_sync_config)
         """
     def update_service_template(
         self, *, name: str, description: str = ..., displayName: str = ...
-    ) -> UpdateServiceTemplateOutputOutputTypeDef:
+    ) -> UpdateServiceTemplateOutputTypeDef:
         """
         Update a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template)
         """
     def update_service_template_version(
@@ -1210,15 +1206,15 @@
         majorVersion: str,
         minorVersion: str,
         templateName: str,
         compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef] = ...,
         description: str = ...,
         status: TemplateVersionStatusType = ...,
         supportedComponentSources: Sequence[Literal["DIRECTLY_DEFINED"]] = ...
-    ) -> UpdateServiceTemplateVersionOutputOutputTypeDef:
+    ) -> UpdateServiceTemplateVersionOutputTypeDef:
         """
         Update a major or minor version of a service template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_service_template_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_service_template_version)
         """
     def update_template_sync_config(
@@ -1226,15 +1222,15 @@
         *,
         branch: str,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         templateName: str,
         templateType: TemplateTypeType,
         subdirectory: str = ...
-    ) -> UpdateTemplateSyncConfigOutputOutputTypeDef:
+    ) -> UpdateTemplateSyncConfigOutputTypeDef:
         """
         Update template sync configuration parameters, except for the `templateName` and
         `templateType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.update_template_sync_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#update_template_sync_config)
         """
```

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/literals.pyi` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/paginator.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,36 @@
     ListServiceInstancesSortByType,
     RepositoryProviderType,
     SortOrderType,
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
-    ListComponentOutputsOutputOutputTypeDef,
-    ListComponentProvisionedResourcesOutputOutputTypeDef,
-    ListComponentsOutputOutputTypeDef,
-    ListDeploymentsOutputOutputTypeDef,
-    ListEnvironmentAccountConnectionsOutputOutputTypeDef,
-    ListEnvironmentOutputsOutputOutputTypeDef,
-    ListEnvironmentProvisionedResourcesOutputOutputTypeDef,
-    ListEnvironmentsOutputOutputTypeDef,
-    ListEnvironmentTemplatesOutputOutputTypeDef,
-    ListEnvironmentTemplateVersionsOutputOutputTypeDef,
-    ListRepositoriesOutputOutputTypeDef,
-    ListRepositorySyncDefinitionsOutputOutputTypeDef,
-    ListServiceInstanceOutputsOutputOutputTypeDef,
-    ListServiceInstanceProvisionedResourcesOutputOutputTypeDef,
+    ListComponentOutputsOutputTypeDef,
+    ListComponentProvisionedResourcesOutputTypeDef,
+    ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListEnvironmentAccountConnectionsOutputTypeDef,
+    ListEnvironmentOutputsOutputTypeDef,
+    ListEnvironmentProvisionedResourcesOutputTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListEnvironmentTemplatesOutputTypeDef,
+    ListEnvironmentTemplateVersionsOutputTypeDef,
+    ListRepositoriesOutputTypeDef,
+    ListRepositorySyncDefinitionsOutputTypeDef,
+    ListServiceInstanceOutputsOutputTypeDef,
+    ListServiceInstanceProvisionedResourcesOutputTypeDef,
     ListServiceInstancesFilterTypeDef,
-    ListServiceInstancesOutputOutputTypeDef,
-    ListServicePipelineOutputsOutputOutputTypeDef,
-    ListServicePipelineProvisionedResourcesOutputOutputTypeDef,
-    ListServicesOutputOutputTypeDef,
-    ListServiceTemplatesOutputOutputTypeDef,
-    ListServiceTemplateVersionsOutputOutputTypeDef,
-    ListTagsForResourceOutputOutputTypeDef,
+    ListServiceInstancesOutputTypeDef,
+    ListServicePipelineOutputsOutputTypeDef,
+    ListServicePipelineProvisionedResourcesOutputTypeDef,
+    ListServicesOutputTypeDef,
+    ListServiceTemplatesOutputTypeDef,
+    ListServiceTemplateVersionsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
@@ -118,390 +118,367 @@
     "ListServicePipelineProvisionedResourcesPaginator",
     "ListServiceTemplateVersionsPaginator",
     "ListServiceTemplatesPaginator",
     "ListServicesPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListComponentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
         self,
         *,
         componentName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentOutputsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
-
 class ListComponentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentProvisionedResourcesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListComponentProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentprovisionedresourcespaginator)
         """
 
-
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListComponentsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
-
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         componentName: str = ...,
         environmentName: str = ...,
         serviceInstanceName: str = ...,
         serviceName: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDeploymentsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
         """
 
-
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         statuses: Sequence[EnvironmentAccountConnectionStatusType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentAccountConnectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
         """
 
-
 class ListEnvironmentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentOutputsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
-
 class ListEnvironmentProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentprovisionedresourcespaginator)
         """
 
-
 class ListEnvironmentTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplateversionspaginator)
         """
 
-
 class ListEnvironmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentTemplatesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmenttemplatespaginator)
         """
 
-
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         environmentTemplates: Sequence[EnvironmentTemplateFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEnvironmentsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentspaginator)
         """
 
-
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRepositoriesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositoriespaginator)
         """
 
-
 class ListRepositorySyncDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         repositoryProvider: RepositoryProviderType,
         syncType: SyncTypeType,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListRepositorySyncDefinitionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListRepositorySyncDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listrepositorysyncdefinitionspaginator)
         """
 
-
 class ListServiceInstanceOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstanceOutputsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
-
 class ListServiceInstanceProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstanceProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceprovisionedresourcespaginator)
         """
 
-
 class ListServiceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[ListServiceInstancesFilterTypeDef] = ...,
         serviceName: str = ...,
         sortBy: ListServiceInstancesSortByType = ...,
         sortOrder: SortOrderType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceInstancesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServiceInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstancespaginator)
         """
 
-
 class ListServicePipelineOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
         self,
         *,
         serviceName: str,
         deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicePipelineOutputsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
-
 class ListServicePipelineProvisionedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
     """
 
     def paginate(
         self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServicePipelineProvisionedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineProvisionedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineprovisionedresourcespaginator)
         """
 
-
 class ListServiceTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
     """
 
     def paginate(
         self,
         *,
         templateName: str,
         majorVersion: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceTemplateVersionsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServiceTemplateVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplateversionspaginator)
         """
 
-
 class ListServiceTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServiceTemplatesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServiceTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicetemplatespaginator)
         """
 
-
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServicesOutputOutputTypeDef]:
+    ) -> _PageIterator[ListServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicespaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceOutputOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,84 +45,84 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
-    "EnvironmentAccountConnectionOutputTypeDef",
-    "RepositoryBranchOutputTypeDef",
+    "EnvironmentAccountConnectionTypeDef",
+    "RepositoryBranchTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
-    "ComponentOutputTypeDef",
+    "ComponentTypeDef",
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
-    "ServiceInstanceOutputTypeDef",
+    "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
-    "ServicePipelineOutputTypeDef",
+    "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
-    "CompatibleEnvironmentTemplateOutputTypeDef",
-    "ComponentStateOutputTypeDef",
-    "ComponentSummaryOutputTypeDef",
-    "ResourceCountsSummaryOutputTypeDef",
+    "CompatibleEnvironmentTemplateTypeDef",
+    "ComponentStateTypeDef",
+    "ComponentSummaryTypeDef",
+    "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
-    "EnvironmentTemplateOutputTypeDef",
-    "EnvironmentTemplateVersionOutputTypeDef",
-    "RepositoryOutputTypeDef",
+    "EnvironmentTemplateTypeDef",
+    "EnvironmentTemplateVersionTypeDef",
+    "RepositoryTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
-    "ServiceSyncConfigOutputTypeDef",
-    "ServiceTemplateOutputTypeDef",
+    "ServiceSyncConfigTypeDef",
+    "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
-    "TemplateSyncConfigOutputTypeDef",
+    "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
-    "EnvironmentStateOutputTypeDef",
-    "ServiceInstanceStateOutputTypeDef",
-    "ServicePipelineStateOutputTypeDef",
-    "DeploymentSummaryOutputTypeDef",
-    "EnvironmentAccountConnectionSummaryOutputTypeDef",
-    "EnvironmentSummaryOutputTypeDef",
+    "EnvironmentStateTypeDef",
+    "ServiceInstanceStateTypeDef",
+    "ServicePipelineStateTypeDef",
+    "DeploymentSummaryTypeDef",
+    "EnvironmentAccountConnectionSummaryTypeDef",
+    "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
-    "EnvironmentTemplateSummaryOutputTypeDef",
-    "EnvironmentTemplateVersionSummaryOutputTypeDef",
+    "EnvironmentTemplateSummaryTypeDef",
+    "EnvironmentTemplateVersionSummaryTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
     "GetServiceInstanceInputRequestTypeDef",
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
-    "RevisionOutputTypeDef",
+    "RevisionTypeDef",
     "GetServiceSyncBlockerSummaryInputRequestTypeDef",
     "GetServiceSyncConfigInputRequestTypeDef",
     "GetServiceTemplateInputRequestTypeDef",
     "GetServiceTemplateVersionInputRequestTypeDef",
     "GetTemplateSyncConfigInputRequestTypeDef",
     "GetTemplateSyncStatusInputRequestTypeDef",
     "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
-    "OutputOutputTypeDef",
+    "OutputTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
-    "ProvisionedResourceOutputTypeDef",
+    "ProvisionedResourceTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
@@ -131,196 +131,195 @@
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
     "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
-    "RepositorySummaryOutputTypeDef",
+    "RepositorySummaryTypeDef",
     "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
     "ListRepositorySyncDefinitionsInputRequestTypeDef",
-    "RepositorySyncDefinitionOutputTypeDef",
+    "RepositorySyncDefinitionTypeDef",
     "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     "ListServiceInstanceOutputsInputRequestTypeDef",
     "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
     "ListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     "ListServiceInstancesFilterTypeDef",
-    "ServiceInstanceSummaryOutputTypeDef",
+    "ServiceInstanceSummaryTypeDef",
     "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     "ListServicePipelineOutputsInputRequestTypeDef",
     "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
     "ListServicePipelineProvisionedResourcesInputRequestTypeDef",
     "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
     "ListServiceTemplateVersionsInputRequestTypeDef",
-    "ServiceTemplateVersionSummaryOutputTypeDef",
+    "ServiceTemplateVersionSummaryTypeDef",
     "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     "ListServiceTemplatesInputRequestTypeDef",
-    "ServiceTemplateSummaryOutputTypeDef",
+    "ServiceTemplateSummaryTypeDef",
     "ListServicesInputListServicesPaginateTypeDef",
     "ListServicesInputRequestTypeDef",
-    "ServiceSummaryOutputTypeDef",
+    "ServiceSummaryTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagOutputTypeDef",
-    "OutputTypeDef",
     "PaginatorConfigTypeDef",
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
-    "RepositorySyncEventOutputTypeDef",
-    "ResourceSyncEventOutputTypeDef",
+    "RepositorySyncEventTypeDef",
+    "ResourceSyncEventTypeDef",
     "ResponseMetadataTypeDef",
     "S3ObjectSourceTypeDef",
-    "SyncBlockerContextOutputTypeDef",
+    "SyncBlockerContextTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateComponentInputRequestTypeDef",
     "UpdateEnvironmentAccountConnectionInputRequestTypeDef",
     "UpdateEnvironmentTemplateInputRequestTypeDef",
     "UpdateEnvironmentTemplateVersionInputRequestTypeDef",
     "UpdateServiceInputRequestTypeDef",
     "UpdateServiceInstanceInputRequestTypeDef",
     "UpdateServicePipelineInputRequestTypeDef",
     "UpdateServiceSyncBlockerInputRequestTypeDef",
     "UpdateServiceSyncConfigInputRequestTypeDef",
     "UpdateServiceTemplateInputRequestTypeDef",
     "UpdateTemplateSyncConfigInputRequestTypeDef",
-    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
-    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
-    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
-    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
-    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
-    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
-    "AccountSettingsOutputTypeDef",
-    "EnvironmentOutputTypeDef",
-    "CancelComponentDeploymentOutputOutputTypeDef",
-    "CreateComponentOutputOutputTypeDef",
-    "DeleteComponentOutputOutputTypeDef",
-    "GetComponentOutputOutputTypeDef",
-    "UpdateComponentOutputOutputTypeDef",
-    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
-    "CreateServiceInstanceOutputOutputTypeDef",
-    "GetServiceInstanceOutputOutputTypeDef",
-    "UpdateServiceInstanceOutputOutputTypeDef",
-    "CancelServicePipelineDeploymentOutputOutputTypeDef",
-    "ServiceOutputTypeDef",
-    "UpdateServicePipelineOutputOutputTypeDef",
+    "AcceptEnvironmentAccountConnectionOutputTypeDef",
+    "CreateEnvironmentAccountConnectionOutputTypeDef",
+    "DeleteEnvironmentAccountConnectionOutputTypeDef",
+    "GetEnvironmentAccountConnectionOutputTypeDef",
+    "RejectEnvironmentAccountConnectionOutputTypeDef",
+    "UpdateEnvironmentAccountConnectionOutputTypeDef",
+    "AccountSettingsTypeDef",
+    "EnvironmentTypeDef",
+    "CancelComponentDeploymentOutputTypeDef",
+    "CreateComponentOutputTypeDef",
+    "DeleteComponentOutputTypeDef",
+    "GetComponentOutputTypeDef",
+    "UpdateComponentOutputTypeDef",
+    "CancelServiceInstanceDeploymentOutputTypeDef",
+    "CreateServiceInstanceOutputTypeDef",
+    "GetServiceInstanceOutputTypeDef",
+    "UpdateServiceInstanceOutputTypeDef",
+    "CancelServicePipelineDeploymentOutputTypeDef",
+    "ServiceTypeDef",
+    "UpdateServicePipelineOutputTypeDef",
     "UpdateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceTemplateVersionOutputTypeDef",
-    "ListComponentsOutputOutputTypeDef",
-    "CountsSummaryOutputTypeDef",
+    "ServiceTemplateVersionTypeDef",
+    "ListComponentsOutputTypeDef",
+    "CountsSummaryTypeDef",
     "CreateComponentInputRequestTypeDef",
     "CreateEnvironmentAccountConnectionInputRequestTypeDef",
     "CreateEnvironmentTemplateInputRequestTypeDef",
     "CreateRepositoryInputRequestTypeDef",
     "CreateServiceInputRequestTypeDef",
     "CreateServiceInstanceInputRequestTypeDef",
     "CreateServiceTemplateInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
-    "CreateEnvironmentTemplateOutputOutputTypeDef",
-    "DeleteEnvironmentTemplateOutputOutputTypeDef",
-    "GetEnvironmentTemplateOutputOutputTypeDef",
-    "UpdateEnvironmentTemplateOutputOutputTypeDef",
-    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
-    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
-    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
-    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
-    "CreateRepositoryOutputOutputTypeDef",
-    "DeleteRepositoryOutputOutputTypeDef",
-    "GetRepositoryOutputOutputTypeDef",
-    "CreateServiceSyncConfigOutputOutputTypeDef",
-    "DeleteServiceSyncConfigOutputOutputTypeDef",
-    "GetServiceSyncConfigOutputOutputTypeDef",
-    "UpdateServiceSyncConfigOutputOutputTypeDef",
-    "CreateServiceTemplateOutputOutputTypeDef",
-    "DeleteServiceTemplateOutputOutputTypeDef",
-    "GetServiceTemplateOutputOutputTypeDef",
-    "UpdateServiceTemplateOutputOutputTypeDef",
-    "CreateTemplateSyncConfigOutputOutputTypeDef",
-    "DeleteTemplateSyncConfigOutputOutputTypeDef",
-    "GetTemplateSyncConfigOutputOutputTypeDef",
-    "UpdateTemplateSyncConfigOutputOutputTypeDef",
-    "DeploymentStateOutputTypeDef",
-    "ListDeploymentsOutputOutputTypeDef",
-    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
-    "ListEnvironmentsOutputOutputTypeDef",
+    "CreateEnvironmentTemplateOutputTypeDef",
+    "DeleteEnvironmentTemplateOutputTypeDef",
+    "GetEnvironmentTemplateOutputTypeDef",
+    "UpdateEnvironmentTemplateOutputTypeDef",
+    "CreateEnvironmentTemplateVersionOutputTypeDef",
+    "DeleteEnvironmentTemplateVersionOutputTypeDef",
+    "GetEnvironmentTemplateVersionOutputTypeDef",
+    "UpdateEnvironmentTemplateVersionOutputTypeDef",
+    "CreateRepositoryOutputTypeDef",
+    "DeleteRepositoryOutputTypeDef",
+    "GetRepositoryOutputTypeDef",
+    "CreateServiceSyncConfigOutputTypeDef",
+    "DeleteServiceSyncConfigOutputTypeDef",
+    "GetServiceSyncConfigOutputTypeDef",
+    "UpdateServiceSyncConfigOutputTypeDef",
+    "CreateServiceTemplateOutputTypeDef",
+    "DeleteServiceTemplateOutputTypeDef",
+    "GetServiceTemplateOutputTypeDef",
+    "UpdateServiceTemplateOutputTypeDef",
+    "CreateTemplateSyncConfigOutputTypeDef",
+    "DeleteTemplateSyncConfigOutputTypeDef",
+    "GetTemplateSyncConfigOutputTypeDef",
+    "UpdateTemplateSyncConfigOutputTypeDef",
+    "DeploymentStateTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListEnvironmentAccountConnectionsOutputTypeDef",
+    "ListEnvironmentsOutputTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentTemplatesOutputOutputTypeDef",
-    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
+    "ListEnvironmentTemplatesOutputTypeDef",
+    "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
     "GetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     "GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     "GetServiceInputServiceCreatedWaitTypeDef",
     "GetServiceInputServiceDeletedWaitTypeDef",
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
-    "ListComponentOutputsOutputOutputTypeDef",
-    "ListEnvironmentOutputsOutputOutputTypeDef",
-    "ListServiceInstanceOutputsOutputOutputTypeDef",
-    "ListServicePipelineOutputsOutputOutputTypeDef",
-    "ListComponentProvisionedResourcesOutputOutputTypeDef",
-    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
-    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
-    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
-    "ListRepositoriesOutputOutputTypeDef",
-    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
+    "ListComponentOutputsOutputTypeDef",
+    "ListEnvironmentOutputsOutputTypeDef",
+    "ListServiceInstanceOutputsOutputTypeDef",
+    "ListServicePipelineOutputsOutputTypeDef",
+    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    "ListComponentProvisionedResourcesOutputTypeDef",
+    "ListEnvironmentProvisionedResourcesOutputTypeDef",
+    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
+    "ListServicePipelineProvisionedResourcesOutputTypeDef",
+    "ListRepositoriesOutputTypeDef",
+    "ListRepositorySyncDefinitionsOutputTypeDef",
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     "ListServiceInstancesInputRequestTypeDef",
-    "ListServiceInstancesOutputOutputTypeDef",
-    "ListServiceTemplateVersionsOutputOutputTypeDef",
-    "ListServiceTemplatesOutputOutputTypeDef",
-    "ListServicesOutputOutputTypeDef",
-    "ListTagsForResourceOutputOutputTypeDef",
-    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    "RepositorySyncAttemptOutputTypeDef",
-    "ResourceSyncAttemptOutputTypeDef",
+    "ListServiceInstancesOutputTypeDef",
+    "ListServiceTemplateVersionsOutputTypeDef",
+    "ListServiceTemplatesOutputTypeDef",
+    "ListServicesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "RepositorySyncAttemptTypeDef",
+    "ResourceSyncAttemptTypeDef",
     "TemplateVersionSourceInputTypeDef",
-    "SyncBlockerOutputTypeDef",
-    "GetAccountSettingsOutputOutputTypeDef",
-    "UpdateAccountSettingsOutputOutputTypeDef",
-    "CancelEnvironmentDeploymentOutputOutputTypeDef",
-    "CreateEnvironmentOutputOutputTypeDef",
-    "DeleteEnvironmentOutputOutputTypeDef",
-    "GetEnvironmentOutputOutputTypeDef",
-    "UpdateEnvironmentOutputOutputTypeDef",
-    "CreateServiceOutputOutputTypeDef",
-    "DeleteServiceOutputOutputTypeDef",
-    "GetServiceOutputOutputTypeDef",
-    "UpdateServiceOutputOutputTypeDef",
-    "CreateServiceTemplateVersionOutputOutputTypeDef",
-    "DeleteServiceTemplateVersionOutputOutputTypeDef",
-    "GetServiceTemplateVersionOutputOutputTypeDef",
-    "UpdateServiceTemplateVersionOutputOutputTypeDef",
-    "GetResourcesSummaryOutputOutputTypeDef",
-    "DeploymentOutputTypeDef",
-    "GetRepositorySyncStatusOutputOutputTypeDef",
-    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
-    "GetTemplateSyncStatusOutputOutputTypeDef",
+    "SyncBlockerTypeDef",
+    "GetAccountSettingsOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
+    "CancelEnvironmentDeploymentOutputTypeDef",
+    "CreateEnvironmentOutputTypeDef",
+    "DeleteEnvironmentOutputTypeDef",
+    "GetEnvironmentOutputTypeDef",
+    "UpdateEnvironmentOutputTypeDef",
+    "CreateServiceOutputTypeDef",
+    "DeleteServiceOutputTypeDef",
+    "GetServiceOutputTypeDef",
+    "UpdateServiceOutputTypeDef",
+    "CreateServiceTemplateVersionOutputTypeDef",
+    "DeleteServiceTemplateVersionOutputTypeDef",
+    "GetServiceTemplateVersionOutputTypeDef",
+    "UpdateServiceTemplateVersionOutputTypeDef",
+    "GetResourcesSummaryOutputTypeDef",
+    "DeploymentTypeDef",
+    "GetRepositorySyncStatusOutputTypeDef",
+    "GetServiceInstanceSyncStatusOutputTypeDef",
+    "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceSyncBlockerSummaryOutputTypeDef",
-    "UpdateServiceSyncBlockerOutputOutputTypeDef",
-    "DeleteDeploymentOutputOutputTypeDef",
-    "GetDeploymentOutputOutputTypeDef",
-    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
+    "ServiceSyncBlockerSummaryTypeDef",
+    "UpdateServiceSyncBlockerOutputTypeDef",
+    "DeleteDeploymentOutputTypeDef",
+    "GetDeploymentOutputTypeDef",
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "EnvironmentAccountConnectionOutputTypeDef",
+EnvironmentAccountConnectionTypeDef = TypedDict(
+    "EnvironmentAccountConnectionTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
@@ -328,16 +327,16 @@
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-RepositoryBranchOutputTypeDef = TypedDict(
-    "RepositoryBranchOutputTypeDef",
+RepositoryBranchTypeDef = TypedDict(
+    "RepositoryBranchTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -345,16 +344,16 @@
 CancelComponentDeploymentInputRequestTypeDef = TypedDict(
     "CancelComponentDeploymentInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 
-ComponentOutputTypeDef = TypedDict(
-    "ComponentOutputTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentName": str,
@@ -382,16 +381,16 @@
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ServiceInstanceOutputTypeDef = TypedDict(
-    "ServiceInstanceOutputTypeDef",
+ServiceInstanceTypeDef = TypedDict(
+    "ServiceInstanceTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -411,16 +410,16 @@
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-ServicePipelineOutputTypeDef = TypedDict(
-    "ServicePipelineOutputTypeDef",
+ServicePipelineTypeDef = TypedDict(
+    "ServicePipelineTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
@@ -437,34 +436,34 @@
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-CompatibleEnvironmentTemplateOutputTypeDef = TypedDict(
-    "CompatibleEnvironmentTemplateOutputTypeDef",
+CompatibleEnvironmentTemplateTypeDef = TypedDict(
+    "CompatibleEnvironmentTemplateTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-ComponentStateOutputTypeDef = TypedDict(
-    "ComponentStateOutputTypeDef",
+ComponentStateTypeDef = TypedDict(
+    "ComponentStateTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "templateFile": str,
     },
 )
 
-ComponentSummaryOutputTypeDef = TypedDict(
-    "ComponentSummaryOutputTypeDef",
+ComponentSummaryTypeDef = TypedDict(
+    "ComponentSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -474,16 +473,16 @@
         "lastSucceededDeploymentId": str,
         "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ResourceCountsSummaryOutputTypeDef = TypedDict(
-    "ResourceCountsSummaryOutputTypeDef",
+ResourceCountsSummaryTypeDef = TypedDict(
+    "ResourceCountsSummaryTypeDef",
     {
         "behindMajor": int,
         "behindMinor": int,
         "failed": int,
         "total": int,
         "upToDate": int,
     },
@@ -502,31 +501,31 @@
     {
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
-EnvironmentTemplateOutputTypeDef = TypedDict(
-    "EnvironmentTemplateOutputTypeDef",
+EnvironmentTemplateTypeDef = TypedDict(
+    "EnvironmentTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "EnvironmentTemplateVersionOutputTypeDef",
+EnvironmentTemplateVersionTypeDef = TypedDict(
+    "EnvironmentTemplateVersionTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -534,16 +533,16 @@
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-RepositoryOutputTypeDef = TypedDict(
-    "RepositoryOutputTypeDef",
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "encryptionKey": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
@@ -556,27 +555,27 @@
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceSyncConfigOutputTypeDef = TypedDict(
-    "ServiceSyncConfigOutputTypeDef",
+ServiceSyncConfigTypeDef = TypedDict(
+    "ServiceSyncConfigTypeDef",
     {
         "branch": str,
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceTemplateOutputTypeDef = TypedDict(
-    "ServiceTemplateOutputTypeDef",
+ServiceTemplateTypeDef = TypedDict(
+    "ServiceTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
@@ -608,16 +607,16 @@
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
 
-TemplateSyncConfigOutputTypeDef = TypedDict(
-    "TemplateSyncConfigOutputTypeDef",
+TemplateSyncConfigTypeDef = TypedDict(
+    "TemplateSyncConfigTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "subdirectory": str,
         "templateName": str,
         "templateType": TemplateTypeType,
@@ -710,49 +709,49 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
-EnvironmentStateOutputTypeDef = TypedDict(
-    "EnvironmentStateOutputTypeDef",
+EnvironmentStateTypeDef = TypedDict(
+    "EnvironmentStateTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServiceInstanceStateOutputTypeDef = TypedDict(
-    "ServiceInstanceStateOutputTypeDef",
+ServiceInstanceStateTypeDef = TypedDict(
+    "ServiceInstanceStateTypeDef",
     {
         "lastSuccessfulComponentDeploymentIds": List[str],
         "lastSuccessfulEnvironmentDeploymentId": str,
         "lastSuccessfulServicePipelineDeploymentId": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServicePipelineStateOutputTypeDef = TypedDict(
-    "ServicePipelineStateOutputTypeDef",
+ServicePipelineStateTypeDef = TypedDict(
+    "ServicePipelineStateTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-DeploymentSummaryOutputTypeDef = TypedDict(
-    "DeploymentSummaryOutputTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "environmentName": str,
@@ -764,32 +763,32 @@
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
     },
 )
 
-EnvironmentAccountConnectionSummaryOutputTypeDef = TypedDict(
-    "EnvironmentAccountConnectionSummaryOutputTypeDef",
+EnvironmentAccountConnectionSummaryTypeDef = TypedDict(
+    "EnvironmentAccountConnectionSummaryTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-EnvironmentSummaryOutputTypeDef = TypedDict(
-    "EnvironmentSummaryOutputTypeDef",
+EnvironmentSummaryTypeDef = TypedDict(
+    "EnvironmentSummaryTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
@@ -812,30 +811,30 @@
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-EnvironmentTemplateSummaryOutputTypeDef = TypedDict(
-    "EnvironmentTemplateSummaryOutputTypeDef",
+EnvironmentTemplateSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionSummaryOutputTypeDef = TypedDict(
-    "EnvironmentTemplateVersionSummaryOutputTypeDef",
+EnvironmentTemplateVersionSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -953,16 +952,16 @@
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-RevisionOutputTypeDef = TypedDict(
-    "RevisionOutputTypeDef",
+RevisionTypeDef = TypedDict(
+    "RevisionTypeDef",
     {
         "branch": str,
         "directory": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "sha": str,
     },
@@ -1072,20 +1071,21 @@
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
     _OptionalListComponentOutputsInputRequestTypeDef,
 ):
     pass
 
 
-OutputOutputTypeDef = TypedDict(
-    "OutputOutputTypeDef",
+OutputTypeDef = TypedDict(
+    "OutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
+    total=False,
 )
 
 _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
     "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     {
         "componentName": str,
     },
@@ -1124,16 +1124,16 @@
 class ListComponentProvisionedResourcesInputRequestTypeDef(
     _RequiredListComponentProvisionedResourcesInputRequestTypeDef,
     _OptionalListComponentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
 
-ProvisionedResourceOutputTypeDef = TypedDict(
-    "ProvisionedResourceOutputTypeDef",
+ProvisionedResourceTypeDef = TypedDict(
+    "ProvisionedResourceTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
 )
 
@@ -1401,16 +1401,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-RepositorySummaryOutputTypeDef = TypedDict(
-    "RepositorySummaryOutputTypeDef",
+RepositorySummaryTypeDef = TypedDict(
+    "RepositorySummaryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -1459,16 +1459,16 @@
 class ListRepositorySyncDefinitionsInputRequestTypeDef(
     _RequiredListRepositorySyncDefinitionsInputRequestTypeDef,
     _OptionalListRepositorySyncDefinitionsInputRequestTypeDef,
 ):
     pass
 
 
-RepositorySyncDefinitionOutputTypeDef = TypedDict(
-    "RepositorySyncDefinitionOutputTypeDef",
+RepositorySyncDefinitionTypeDef = TypedDict(
+    "RepositorySyncDefinitionTypeDef",
     {
         "branch": str,
         "directory": str,
         "parent": str,
         "target": str,
     },
 )
@@ -1572,16 +1572,16 @@
     {
         "key": ListServiceInstancesFilterByType,
         "value": str,
     },
     total=False,
 )
 
-ServiceInstanceSummaryOutputTypeDef = TypedDict(
-    "ServiceInstanceSummaryOutputTypeDef",
+ServiceInstanceSummaryTypeDef = TypedDict(
+    "ServiceInstanceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -1729,16 +1729,16 @@
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
 
-ServiceTemplateVersionSummaryOutputTypeDef = TypedDict(
-    "ServiceTemplateVersionSummaryOutputTypeDef",
+ServiceTemplateVersionSummaryTypeDef = TypedDict(
+    "ServiceTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -1762,16 +1762,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceTemplateSummaryOutputTypeDef = TypedDict(
-    "ServiceTemplateSummaryOutputTypeDef",
+ServiceTemplateSummaryTypeDef = TypedDict(
+    "ServiceTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
@@ -1793,16 +1793,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceSummaryOutputTypeDef = TypedDict(
-    "ServiceSummaryOutputTypeDef",
+ServiceSummaryTypeDef = TypedDict(
+    "ServiceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
@@ -1859,23 +1859,14 @@
     "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-OutputTypeDef = TypedDict(
-    "OutputTypeDef",
-    {
-        "key": str,
-        "valueString": str,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1885,26 +1876,26 @@
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-RepositorySyncEventOutputTypeDef = TypedDict(
-    "RepositorySyncEventOutputTypeDef",
+RepositorySyncEventTypeDef = TypedDict(
+    "RepositorySyncEventTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
 
-ResourceSyncEventOutputTypeDef = TypedDict(
-    "ResourceSyncEventOutputTypeDef",
+ResourceSyncEventTypeDef = TypedDict(
+    "ResourceSyncEventTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
@@ -1924,16 +1915,16 @@
     "S3ObjectSourceTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
 
-SyncBlockerContextOutputTypeDef = TypedDict(
-    "SyncBlockerContextOutputTypeDef",
+SyncBlockerContextTypeDef = TypedDict(
+    "SyncBlockerContextTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 UntagResourceInputRequestTypeDef = TypedDict(
@@ -2181,73 +2172,73 @@
 class UpdateTemplateSyncConfigInputRequestTypeDef(
     _RequiredUpdateTemplateSyncConfigInputRequestTypeDef,
     _OptionalUpdateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
 
-AcceptEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
+AcceptEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "AcceptEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
+CreateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "CreateEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
+DeleteEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "DeleteEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
+GetEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "GetEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RejectEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
+RejectEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "RejectEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
+UpdateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "UpdateEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AccountSettingsOutputTypeDef = TypedDict(
-    "AccountSettingsOutputTypeDef",
+AccountSettingsTypeDef = TypedDict(
+    "AccountSettingsTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
-        "pipelineProvisioningRepository": RepositoryBranchOutputTypeDef,
+        "pipelineProvisioningRepository": RepositoryBranchTypeDef,
         "pipelineServiceRoleArn": str,
     },
 )
 
-EnvironmentOutputTypeDef = TypedDict(
-    "EnvironmentOutputTypeDef",
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
@@ -2257,125 +2248,125 @@
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
         "lastSucceededDeploymentId": str,
         "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
-        "provisioningRepository": RepositoryBranchOutputTypeDef,
+        "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-CancelComponentDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelComponentDeploymentOutputOutputTypeDef",
+CancelComponentDeploymentOutputTypeDef = TypedDict(
+    "CancelComponentDeploymentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateComponentOutputOutputTypeDef = TypedDict(
-    "CreateComponentOutputOutputTypeDef",
+CreateComponentOutputTypeDef = TypedDict(
+    "CreateComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteComponentOutputOutputTypeDef = TypedDict(
-    "DeleteComponentOutputOutputTypeDef",
+DeleteComponentOutputTypeDef = TypedDict(
+    "DeleteComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetComponentOutputOutputTypeDef = TypedDict(
-    "GetComponentOutputOutputTypeDef",
+GetComponentOutputTypeDef = TypedDict(
+    "GetComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateComponentOutputOutputTypeDef = TypedDict(
-    "UpdateComponentOutputOutputTypeDef",
+UpdateComponentOutputTypeDef = TypedDict(
+    "UpdateComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServiceInstanceDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
+CancelServiceInstanceDeploymentOutputTypeDef = TypedDict(
+    "CancelServiceInstanceDeploymentOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceInstanceOutputOutputTypeDef = TypedDict(
-    "CreateServiceInstanceOutputOutputTypeDef",
+CreateServiceInstanceOutputTypeDef = TypedDict(
+    "CreateServiceInstanceOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceOutputOutputTypeDef = TypedDict(
-    "GetServiceInstanceOutputOutputTypeDef",
+GetServiceInstanceOutputTypeDef = TypedDict(
+    "GetServiceInstanceOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceInstanceOutputOutputTypeDef = TypedDict(
-    "UpdateServiceInstanceOutputOutputTypeDef",
+UpdateServiceInstanceOutputTypeDef = TypedDict(
+    "UpdateServiceInstanceOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServicePipelineDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelServicePipelineDeploymentOutputOutputTypeDef",
+CancelServicePipelineDeploymentOutputTypeDef = TypedDict(
+    "CancelServicePipelineDeploymentOutputTypeDef",
     {
-        "pipeline": ServicePipelineOutputTypeDef,
+        "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServiceOutputTypeDef = TypedDict(
-    "ServiceOutputTypeDef",
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
     {
         "arn": str,
         "branchName": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
-        "pipeline": ServicePipelineOutputTypeDef,
+        "pipeline": ServicePipelineTypeDef,
         "repositoryConnectionArn": str,
         "repositoryId": str,
         "spec": str,
         "status": ServiceStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-UpdateServicePipelineOutputOutputTypeDef = TypedDict(
-    "UpdateServicePipelineOutputOutputTypeDef",
+UpdateServicePipelineOutputTypeDef = TypedDict(
+    "UpdateServicePipelineOutputTypeDef",
     {
-        "pipeline": ServicePipelineOutputTypeDef,
+        "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateVersionInputRequestTypeDef",
     {
@@ -2399,52 +2390,52 @@
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
 
-ServiceTemplateVersionOutputTypeDef = TypedDict(
-    "ServiceTemplateVersionOutputTypeDef",
+ServiceTemplateVersionTypeDef = TypedDict(
+    "ServiceTemplateVersionTypeDef",
     {
         "arn": str,
-        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateOutputTypeDef],
+        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
         "recommendedMinorVersion": str,
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
         "templateName": str,
     },
 )
 
-ListComponentsOutputOutputTypeDef = TypedDict(
-    "ListComponentsOutputOutputTypeDef",
+ListComponentsOutputTypeDef = TypedDict(
+    "ListComponentsOutputTypeDef",
     {
-        "components": List[ComponentSummaryOutputTypeDef],
+        "components": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CountsSummaryOutputTypeDef = TypedDict(
-    "CountsSummaryOutputTypeDef",
+CountsSummaryTypeDef = TypedDict(
+    "CountsSummaryTypeDef",
     {
-        "components": ResourceCountsSummaryOutputTypeDef,
-        "environmentTemplates": ResourceCountsSummaryOutputTypeDef,
-        "environments": ResourceCountsSummaryOutputTypeDef,
-        "pipelines": ResourceCountsSummaryOutputTypeDef,
-        "serviceInstances": ResourceCountsSummaryOutputTypeDef,
-        "serviceTemplates": ResourceCountsSummaryOutputTypeDef,
-        "services": ResourceCountsSummaryOutputTypeDef,
+        "components": ResourceCountsSummaryTypeDef,
+        "environmentTemplates": ResourceCountsSummaryTypeDef,
+        "environments": ResourceCountsSummaryTypeDef,
+        "pipelines": ResourceCountsSummaryTypeDef,
+        "serviceInstances": ResourceCountsSummaryTypeDef,
+        "serviceTemplates": ResourceCountsSummaryTypeDef,
+        "services": ResourceCountsSummaryTypeDef,
     },
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
@@ -2708,230 +2699,230 @@
 
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
 
-CreateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateOutputOutputTypeDef",
+CreateEnvironmentTemplateOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateOutputOutputTypeDef",
+DeleteEnvironmentTemplateOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateOutputOutputTypeDef",
+GetEnvironmentTemplateOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateOutputOutputTypeDef",
+UpdateEnvironmentTemplateOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
+CreateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
+DeleteEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
+GetEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
+UpdateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRepositoryOutputOutputTypeDef = TypedDict(
-    "CreateRepositoryOutputOutputTypeDef",
+CreateRepositoryOutputTypeDef = TypedDict(
+    "CreateRepositoryOutputTypeDef",
     {
-        "repository": RepositoryOutputTypeDef,
+        "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRepositoryOutputOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputOutputTypeDef",
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
     {
-        "repository": RepositoryOutputTypeDef,
+        "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRepositoryOutputOutputTypeDef = TypedDict(
-    "GetRepositoryOutputOutputTypeDef",
+GetRepositoryOutputTypeDef = TypedDict(
+    "GetRepositoryOutputTypeDef",
     {
-        "repository": RepositoryOutputTypeDef,
+        "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "CreateServiceSyncConfigOutputOutputTypeDef",
+CreateServiceSyncConfigOutputTypeDef = TypedDict(
+    "CreateServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "DeleteServiceSyncConfigOutputOutputTypeDef",
+DeleteServiceSyncConfigOutputTypeDef = TypedDict(
+    "DeleteServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "GetServiceSyncConfigOutputOutputTypeDef",
+GetServiceSyncConfigOutputTypeDef = TypedDict(
+    "GetServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "UpdateServiceSyncConfigOutputOutputTypeDef",
+UpdateServiceSyncConfigOutputTypeDef = TypedDict(
+    "UpdateServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateOutputOutputTypeDef = TypedDict(
-    "CreateServiceTemplateOutputOutputTypeDef",
+CreateServiceTemplateOutputTypeDef = TypedDict(
+    "CreateServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateOutputOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateOutputOutputTypeDef",
+DeleteServiceTemplateOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateOutputOutputTypeDef = TypedDict(
-    "GetServiceTemplateOutputOutputTypeDef",
+GetServiceTemplateOutputTypeDef = TypedDict(
+    "GetServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateOutputOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateOutputOutputTypeDef",
+UpdateServiceTemplateOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "CreateTemplateSyncConfigOutputOutputTypeDef",
+CreateTemplateSyncConfigOutputTypeDef = TypedDict(
+    "CreateTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "DeleteTemplateSyncConfigOutputOutputTypeDef",
+DeleteTemplateSyncConfigOutputTypeDef = TypedDict(
+    "DeleteTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "GetTemplateSyncConfigOutputOutputTypeDef",
+GetTemplateSyncConfigOutputTypeDef = TypedDict(
+    "GetTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "UpdateTemplateSyncConfigOutputOutputTypeDef",
+UpdateTemplateSyncConfigOutputTypeDef = TypedDict(
+    "UpdateTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentStateOutputTypeDef = TypedDict(
-    "DeploymentStateOutputTypeDef",
+DeploymentStateTypeDef = TypedDict(
+    "DeploymentStateTypeDef",
     {
-        "component": ComponentStateOutputTypeDef,
-        "environment": EnvironmentStateOutputTypeDef,
-        "serviceInstance": ServiceInstanceStateOutputTypeDef,
-        "servicePipeline": ServicePipelineStateOutputTypeDef,
+        "component": ComponentStateTypeDef,
+        "environment": EnvironmentStateTypeDef,
+        "serviceInstance": ServiceInstanceStateTypeDef,
+        "servicePipeline": ServicePipelineStateTypeDef,
     },
 )
 
-ListDeploymentsOutputOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputOutputTypeDef",
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
     {
-        "deployments": List[DeploymentSummaryOutputTypeDef],
+        "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentAccountConnectionsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
+ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
+    "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
-        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryOutputTypeDef],
+        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputOutputTypeDef",
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
     {
-        "environments": List[EnvironmentSummaryOutputTypeDef],
+        "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
@@ -2948,28 +2939,28 @@
         "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentTemplatesOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplatesOutputOutputTypeDef",
+ListEnvironmentTemplatesOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplatesOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[EnvironmentTemplateSummaryOutputTypeDef],
+        "templates": List[EnvironmentTemplateSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentTemplateVersionsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
+ListEnvironmentTemplateVersionsOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[EnvironmentTemplateVersionSummaryOutputTypeDef],
+        "templateVersions": List[EnvironmentTemplateVersionSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetComponentInputComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeletedWaitTypeDef",
     {
@@ -3191,100 +3182,125 @@
 class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
 
-ListComponentOutputsOutputOutputTypeDef = TypedDict(
-    "ListComponentOutputsOutputOutputTypeDef",
+ListComponentOutputsOutputTypeDef = TypedDict(
+    "ListComponentOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentOutputsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentOutputsOutputOutputTypeDef",
+ListEnvironmentOutputsOutputTypeDef = TypedDict(
+    "ListEnvironmentOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceOutputsOutputOutputTypeDef = TypedDict(
-    "ListServiceInstanceOutputsOutputOutputTypeDef",
+ListServiceInstanceOutputsOutputTypeDef = TypedDict(
+    "ListServiceInstanceOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineOutputsOutputOutputTypeDef = TypedDict(
-    "ListServicePipelineOutputsOutputOutputTypeDef",
+ListServicePipelineOutputsOutputTypeDef = TypedDict(
+    "ListServicePipelineOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListComponentProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListComponentProvisionedResourcesOutputOutputTypeDef",
+_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "deploymentId": str,
+        "outputs": Sequence[OutputTypeDef],
+        "status": ResourceDeploymentStatusType,
+        "statusMessage": str,
+    },
+    total=False,
+)
+
+
+class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
+    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+):
+    pass
+
+
+ListComponentProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListComponentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
+ListEnvironmentProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListEnvironmentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
+ListServiceInstanceProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
+ListServicePipelineProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListServicePipelineProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositoriesOutputOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputOutputTypeDef",
+ListRepositoriesOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputTypeDef",
     {
         "nextToken": str,
-        "repositories": List[RepositorySummaryOutputTypeDef],
+        "repositories": List[RepositorySummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositorySyncDefinitionsOutputOutputTypeDef = TypedDict(
-    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
+ListRepositorySyncDefinitionsOutputTypeDef = TypedDict(
+    "ListRepositorySyncDefinitionsOutputTypeDef",
     {
         "nextToken": str,
-        "syncDefinitions": List[RepositorySyncDefinitionOutputTypeDef],
+        "syncDefinitions": List[RepositorySyncDefinitionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     {
@@ -3306,303 +3322,278 @@
         "serviceName": str,
         "sortBy": ListServiceInstancesSortByType,
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListServiceInstancesOutputOutputTypeDef = TypedDict(
-    "ListServiceInstancesOutputOutputTypeDef",
+ListServiceInstancesOutputTypeDef = TypedDict(
+    "ListServiceInstancesOutputTypeDef",
     {
         "nextToken": str,
-        "serviceInstances": List[ServiceInstanceSummaryOutputTypeDef],
+        "serviceInstances": List[ServiceInstanceSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplateVersionsOutputOutputTypeDef = TypedDict(
-    "ListServiceTemplateVersionsOutputOutputTypeDef",
+ListServiceTemplateVersionsOutputTypeDef = TypedDict(
+    "ListServiceTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[ServiceTemplateVersionSummaryOutputTypeDef],
+        "templateVersions": List[ServiceTemplateVersionSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplatesOutputOutputTypeDef = TypedDict(
-    "ListServiceTemplatesOutputOutputTypeDef",
+ListServiceTemplatesOutputTypeDef = TypedDict(
+    "ListServiceTemplatesOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[ServiceTemplateSummaryOutputTypeDef],
+        "templates": List[ServiceTemplateSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicesOutputOutputTypeDef = TypedDict(
-    "ListServicesOutputOutputTypeDef",
+ListServicesOutputTypeDef = TypedDict(
+    "ListServicesOutputTypeDef",
     {
         "nextToken": str,
-        "services": List[ServiceSummaryOutputTypeDef],
+        "services": List[ServiceSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceOutputOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputOutputTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "deploymentId": str,
-        "outputs": Sequence[OutputTypeDef],
-        "status": ResourceDeploymentStatusType,
-        "statusMessage": str,
-    },
-    total=False,
-)
-
-
-class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
-    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-):
-    pass
-
-
-RepositorySyncAttemptOutputTypeDef = TypedDict(
-    "RepositorySyncAttemptOutputTypeDef",
+RepositorySyncAttemptTypeDef = TypedDict(
+    "RepositorySyncAttemptTypeDef",
     {
-        "events": List[RepositorySyncEventOutputTypeDef],
+        "events": List[RepositorySyncEventTypeDef],
         "startedAt": datetime,
         "status": RepositorySyncStatusType,
     },
 )
 
-ResourceSyncAttemptOutputTypeDef = TypedDict(
-    "ResourceSyncAttemptOutputTypeDef",
+ResourceSyncAttemptTypeDef = TypedDict(
+    "ResourceSyncAttemptTypeDef",
     {
-        "events": List[ResourceSyncEventOutputTypeDef],
-        "initialRevision": RevisionOutputTypeDef,
+        "events": List[ResourceSyncEventTypeDef],
+        "initialRevision": RevisionTypeDef,
         "startedAt": datetime,
         "status": ResourceSyncStatusType,
         "target": str,
-        "targetRevision": RevisionOutputTypeDef,
+        "targetRevision": RevisionTypeDef,
     },
 )
 
 TemplateVersionSourceInputTypeDef = TypedDict(
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
-SyncBlockerOutputTypeDef = TypedDict(
-    "SyncBlockerOutputTypeDef",
+SyncBlockerTypeDef = TypedDict(
+    "SyncBlockerTypeDef",
     {
-        "contexts": List[SyncBlockerContextOutputTypeDef],
+        "contexts": List[SyncBlockerContextTypeDef],
         "createdAt": datetime,
         "createdReason": str,
         "id": str,
         "resolvedAt": datetime,
         "resolvedReason": str,
         "status": BlockerStatusType,
         "type": Literal["AUTOMATED"],
     },
 )
 
-GetAccountSettingsOutputOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputOutputTypeDef",
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
     {
-        "accountSettings": AccountSettingsOutputTypeDef,
+        "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAccountSettingsOutputOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputOutputTypeDef",
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
     {
-        "accountSettings": AccountSettingsOutputTypeDef,
+        "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelEnvironmentDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelEnvironmentDeploymentOutputOutputTypeDef",
+CancelEnvironmentDeploymentOutputTypeDef = TypedDict(
+    "CancelEnvironmentDeploymentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputOutputTypeDef",
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentOutputOutputTypeDef",
+DeleteEnvironmentOutputTypeDef = TypedDict(
+    "DeleteEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentOutputOutputTypeDef",
+GetEnvironmentOutputTypeDef = TypedDict(
+    "GetEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentOutputOutputTypeDef",
+UpdateEnvironmentOutputTypeDef = TypedDict(
+    "UpdateEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceOutputOutputTypeDef = TypedDict(
-    "CreateServiceOutputOutputTypeDef",
+CreateServiceOutputTypeDef = TypedDict(
+    "CreateServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceOutputOutputTypeDef = TypedDict(
-    "DeleteServiceOutputOutputTypeDef",
+DeleteServiceOutputTypeDef = TypedDict(
+    "DeleteServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceOutputOutputTypeDef = TypedDict(
-    "GetServiceOutputOutputTypeDef",
+GetServiceOutputTypeDef = TypedDict(
+    "GetServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceOutputOutputTypeDef = TypedDict(
-    "UpdateServiceOutputOutputTypeDef",
+UpdateServiceOutputTypeDef = TypedDict(
+    "UpdateServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "CreateServiceTemplateVersionOutputOutputTypeDef",
+CreateServiceTemplateVersionOutputTypeDef = TypedDict(
+    "CreateServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateVersionOutputOutputTypeDef",
+DeleteServiceTemplateVersionOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "GetServiceTemplateVersionOutputOutputTypeDef",
+GetServiceTemplateVersionOutputTypeDef = TypedDict(
+    "GetServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateVersionOutputOutputTypeDef",
+UpdateServiceTemplateVersionOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetResourcesSummaryOutputOutputTypeDef = TypedDict(
-    "GetResourcesSummaryOutputOutputTypeDef",
+GetResourcesSummaryOutputTypeDef = TypedDict(
+    "GetResourcesSummaryOutputTypeDef",
     {
-        "counts": CountsSummaryOutputTypeDef,
+        "counts": CountsSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentOutputTypeDef = TypedDict(
-    "DeploymentOutputTypeDef",
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "id": str,
-        "initialState": DeploymentStateOutputTypeDef,
+        "initialState": DeploymentStateTypeDef,
         "lastAttemptedDeploymentId": str,
         "lastModifiedAt": datetime,
         "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
-        "targetState": DeploymentStateOutputTypeDef,
+        "targetState": DeploymentStateTypeDef,
     },
 )
 
-GetRepositorySyncStatusOutputOutputTypeDef = TypedDict(
-    "GetRepositorySyncStatusOutputOutputTypeDef",
+GetRepositorySyncStatusOutputTypeDef = TypedDict(
+    "GetRepositorySyncStatusOutputTypeDef",
     {
-        "latestSync": RepositorySyncAttemptOutputTypeDef,
+        "latestSync": RepositorySyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceSyncStatusOutputOutputTypeDef = TypedDict(
-    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
+GetServiceInstanceSyncStatusOutputTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusOutputTypeDef",
     {
-        "desiredState": RevisionOutputTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
-        "latestSync": ResourceSyncAttemptOutputTypeDef,
+        "desiredState": RevisionTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
+        "latestSync": ResourceSyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncStatusOutputOutputTypeDef = TypedDict(
-    "GetTemplateSyncStatusOutputOutputTypeDef",
+GetTemplateSyncStatusOutputTypeDef = TypedDict(
+    "GetTemplateSyncStatusOutputTypeDef",
     {
-        "desiredState": RevisionOutputTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
-        "latestSync": ResourceSyncAttemptOutputTypeDef,
+        "desiredState": RevisionTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
+        "latestSync": ResourceSyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef",
     {
@@ -3653,49 +3644,49 @@
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
 
-ServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
-    "ServiceSyncBlockerSummaryOutputTypeDef",
+ServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "ServiceSyncBlockerSummaryTypeDef",
     {
-        "latestBlockers": List[SyncBlockerOutputTypeDef],
+        "latestBlockers": List[SyncBlockerTypeDef],
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-UpdateServiceSyncBlockerOutputOutputTypeDef = TypedDict(
-    "UpdateServiceSyncBlockerOutputOutputTypeDef",
+UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
-        "serviceSyncBlocker": SyncBlockerOutputTypeDef,
+        "serviceSyncBlocker": SyncBlockerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDeploymentOutputOutputTypeDef = TypedDict(
-    "DeleteDeploymentOutputOutputTypeDef",
+DeleteDeploymentOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputTypeDef",
     {
-        "deployment": DeploymentOutputTypeDef,
+        "deployment": DeploymentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDeploymentOutputOutputTypeDef = TypedDict(
-    "GetDeploymentOutputOutputTypeDef",
+GetDeploymentOutputTypeDef = TypedDict(
+    "GetDeploymentOutputTypeDef",
     {
-        "deployment": DeploymentOutputTypeDef,
+        "deployment": DeploymentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncBlockerSummaryOutputOutputTypeDef = TypedDict(
-    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
+GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
     {
-        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryOutputTypeDef,
+        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/type_defs.pyi` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,84 +44,84 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
-    "EnvironmentAccountConnectionOutputTypeDef",
-    "RepositoryBranchOutputTypeDef",
+    "EnvironmentAccountConnectionTypeDef",
+    "RepositoryBranchTypeDef",
     "CancelComponentDeploymentInputRequestTypeDef",
-    "ComponentOutputTypeDef",
+    "ComponentTypeDef",
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
-    "ServiceInstanceOutputTypeDef",
+    "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
-    "ServicePipelineOutputTypeDef",
+    "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
-    "CompatibleEnvironmentTemplateOutputTypeDef",
-    "ComponentStateOutputTypeDef",
-    "ComponentSummaryOutputTypeDef",
-    "ResourceCountsSummaryOutputTypeDef",
+    "CompatibleEnvironmentTemplateTypeDef",
+    "ComponentStateTypeDef",
+    "ComponentSummaryTypeDef",
+    "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
-    "EnvironmentTemplateOutputTypeDef",
-    "EnvironmentTemplateVersionOutputTypeDef",
-    "RepositoryOutputTypeDef",
+    "EnvironmentTemplateTypeDef",
+    "EnvironmentTemplateVersionTypeDef",
+    "RepositoryTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
-    "ServiceSyncConfigOutputTypeDef",
-    "ServiceTemplateOutputTypeDef",
+    "ServiceSyncConfigTypeDef",
+    "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
-    "TemplateSyncConfigOutputTypeDef",
+    "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
     "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
-    "EnvironmentStateOutputTypeDef",
-    "ServiceInstanceStateOutputTypeDef",
-    "ServicePipelineStateOutputTypeDef",
-    "DeploymentSummaryOutputTypeDef",
-    "EnvironmentAccountConnectionSummaryOutputTypeDef",
-    "EnvironmentSummaryOutputTypeDef",
+    "EnvironmentStateTypeDef",
+    "ServiceInstanceStateTypeDef",
+    "ServicePipelineStateTypeDef",
+    "DeploymentSummaryTypeDef",
+    "EnvironmentAccountConnectionSummaryTypeDef",
+    "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
-    "EnvironmentTemplateSummaryOutputTypeDef",
-    "EnvironmentTemplateVersionSummaryOutputTypeDef",
+    "EnvironmentTemplateSummaryTypeDef",
+    "EnvironmentTemplateVersionSummaryTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
     "GetServiceInstanceInputRequestTypeDef",
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
-    "RevisionOutputTypeDef",
+    "RevisionTypeDef",
     "GetServiceSyncBlockerSummaryInputRequestTypeDef",
     "GetServiceSyncConfigInputRequestTypeDef",
     "GetServiceTemplateInputRequestTypeDef",
     "GetServiceTemplateVersionInputRequestTypeDef",
     "GetTemplateSyncConfigInputRequestTypeDef",
     "GetTemplateSyncStatusInputRequestTypeDef",
     "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
-    "OutputOutputTypeDef",
+    "OutputTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
-    "ProvisionedResourceOutputTypeDef",
+    "ProvisionedResourceTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
@@ -130,196 +130,195 @@
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
     "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
-    "RepositorySummaryOutputTypeDef",
+    "RepositorySummaryTypeDef",
     "ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef",
     "ListRepositorySyncDefinitionsInputRequestTypeDef",
-    "RepositorySyncDefinitionOutputTypeDef",
+    "RepositorySyncDefinitionTypeDef",
     "ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     "ListServiceInstanceOutputsInputRequestTypeDef",
     "ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef",
     "ListServiceInstanceProvisionedResourcesInputRequestTypeDef",
     "ListServiceInstancesFilterTypeDef",
-    "ServiceInstanceSummaryOutputTypeDef",
+    "ServiceInstanceSummaryTypeDef",
     "ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     "ListServicePipelineOutputsInputRequestTypeDef",
     "ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef",
     "ListServicePipelineProvisionedResourcesInputRequestTypeDef",
     "ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef",
     "ListServiceTemplateVersionsInputRequestTypeDef",
-    "ServiceTemplateVersionSummaryOutputTypeDef",
+    "ServiceTemplateVersionSummaryTypeDef",
     "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     "ListServiceTemplatesInputRequestTypeDef",
-    "ServiceTemplateSummaryOutputTypeDef",
+    "ServiceTemplateSummaryTypeDef",
     "ListServicesInputListServicesPaginateTypeDef",
     "ListServicesInputRequestTypeDef",
-    "ServiceSummaryOutputTypeDef",
+    "ServiceSummaryTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagOutputTypeDef",
-    "OutputTypeDef",
     "PaginatorConfigTypeDef",
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
-    "RepositorySyncEventOutputTypeDef",
-    "ResourceSyncEventOutputTypeDef",
+    "RepositorySyncEventTypeDef",
+    "ResourceSyncEventTypeDef",
     "ResponseMetadataTypeDef",
     "S3ObjectSourceTypeDef",
-    "SyncBlockerContextOutputTypeDef",
+    "SyncBlockerContextTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateComponentInputRequestTypeDef",
     "UpdateEnvironmentAccountConnectionInputRequestTypeDef",
     "UpdateEnvironmentTemplateInputRequestTypeDef",
     "UpdateEnvironmentTemplateVersionInputRequestTypeDef",
     "UpdateServiceInputRequestTypeDef",
     "UpdateServiceInstanceInputRequestTypeDef",
     "UpdateServicePipelineInputRequestTypeDef",
     "UpdateServiceSyncBlockerInputRequestTypeDef",
     "UpdateServiceSyncConfigInputRequestTypeDef",
     "UpdateServiceTemplateInputRequestTypeDef",
     "UpdateTemplateSyncConfigInputRequestTypeDef",
-    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
-    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
-    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
-    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
-    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
-    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
-    "AccountSettingsOutputTypeDef",
-    "EnvironmentOutputTypeDef",
-    "CancelComponentDeploymentOutputOutputTypeDef",
-    "CreateComponentOutputOutputTypeDef",
-    "DeleteComponentOutputOutputTypeDef",
-    "GetComponentOutputOutputTypeDef",
-    "UpdateComponentOutputOutputTypeDef",
-    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
-    "CreateServiceInstanceOutputOutputTypeDef",
-    "GetServiceInstanceOutputOutputTypeDef",
-    "UpdateServiceInstanceOutputOutputTypeDef",
-    "CancelServicePipelineDeploymentOutputOutputTypeDef",
-    "ServiceOutputTypeDef",
-    "UpdateServicePipelineOutputOutputTypeDef",
+    "AcceptEnvironmentAccountConnectionOutputTypeDef",
+    "CreateEnvironmentAccountConnectionOutputTypeDef",
+    "DeleteEnvironmentAccountConnectionOutputTypeDef",
+    "GetEnvironmentAccountConnectionOutputTypeDef",
+    "RejectEnvironmentAccountConnectionOutputTypeDef",
+    "UpdateEnvironmentAccountConnectionOutputTypeDef",
+    "AccountSettingsTypeDef",
+    "EnvironmentTypeDef",
+    "CancelComponentDeploymentOutputTypeDef",
+    "CreateComponentOutputTypeDef",
+    "DeleteComponentOutputTypeDef",
+    "GetComponentOutputTypeDef",
+    "UpdateComponentOutputTypeDef",
+    "CancelServiceInstanceDeploymentOutputTypeDef",
+    "CreateServiceInstanceOutputTypeDef",
+    "GetServiceInstanceOutputTypeDef",
+    "UpdateServiceInstanceOutputTypeDef",
+    "CancelServicePipelineDeploymentOutputTypeDef",
+    "ServiceTypeDef",
+    "UpdateServicePipelineOutputTypeDef",
     "UpdateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceTemplateVersionOutputTypeDef",
-    "ListComponentsOutputOutputTypeDef",
-    "CountsSummaryOutputTypeDef",
+    "ServiceTemplateVersionTypeDef",
+    "ListComponentsOutputTypeDef",
+    "CountsSummaryTypeDef",
     "CreateComponentInputRequestTypeDef",
     "CreateEnvironmentAccountConnectionInputRequestTypeDef",
     "CreateEnvironmentTemplateInputRequestTypeDef",
     "CreateRepositoryInputRequestTypeDef",
     "CreateServiceInputRequestTypeDef",
     "CreateServiceInstanceInputRequestTypeDef",
     "CreateServiceTemplateInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
-    "CreateEnvironmentTemplateOutputOutputTypeDef",
-    "DeleteEnvironmentTemplateOutputOutputTypeDef",
-    "GetEnvironmentTemplateOutputOutputTypeDef",
-    "UpdateEnvironmentTemplateOutputOutputTypeDef",
-    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
-    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
-    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
-    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
-    "CreateRepositoryOutputOutputTypeDef",
-    "DeleteRepositoryOutputOutputTypeDef",
-    "GetRepositoryOutputOutputTypeDef",
-    "CreateServiceSyncConfigOutputOutputTypeDef",
-    "DeleteServiceSyncConfigOutputOutputTypeDef",
-    "GetServiceSyncConfigOutputOutputTypeDef",
-    "UpdateServiceSyncConfigOutputOutputTypeDef",
-    "CreateServiceTemplateOutputOutputTypeDef",
-    "DeleteServiceTemplateOutputOutputTypeDef",
-    "GetServiceTemplateOutputOutputTypeDef",
-    "UpdateServiceTemplateOutputOutputTypeDef",
-    "CreateTemplateSyncConfigOutputOutputTypeDef",
-    "DeleteTemplateSyncConfigOutputOutputTypeDef",
-    "GetTemplateSyncConfigOutputOutputTypeDef",
-    "UpdateTemplateSyncConfigOutputOutputTypeDef",
-    "DeploymentStateOutputTypeDef",
-    "ListDeploymentsOutputOutputTypeDef",
-    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
-    "ListEnvironmentsOutputOutputTypeDef",
+    "CreateEnvironmentTemplateOutputTypeDef",
+    "DeleteEnvironmentTemplateOutputTypeDef",
+    "GetEnvironmentTemplateOutputTypeDef",
+    "UpdateEnvironmentTemplateOutputTypeDef",
+    "CreateEnvironmentTemplateVersionOutputTypeDef",
+    "DeleteEnvironmentTemplateVersionOutputTypeDef",
+    "GetEnvironmentTemplateVersionOutputTypeDef",
+    "UpdateEnvironmentTemplateVersionOutputTypeDef",
+    "CreateRepositoryOutputTypeDef",
+    "DeleteRepositoryOutputTypeDef",
+    "GetRepositoryOutputTypeDef",
+    "CreateServiceSyncConfigOutputTypeDef",
+    "DeleteServiceSyncConfigOutputTypeDef",
+    "GetServiceSyncConfigOutputTypeDef",
+    "UpdateServiceSyncConfigOutputTypeDef",
+    "CreateServiceTemplateOutputTypeDef",
+    "DeleteServiceTemplateOutputTypeDef",
+    "GetServiceTemplateOutputTypeDef",
+    "UpdateServiceTemplateOutputTypeDef",
+    "CreateTemplateSyncConfigOutputTypeDef",
+    "DeleteTemplateSyncConfigOutputTypeDef",
+    "GetTemplateSyncConfigOutputTypeDef",
+    "UpdateTemplateSyncConfigOutputTypeDef",
+    "DeploymentStateTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListEnvironmentAccountConnectionsOutputTypeDef",
+    "ListEnvironmentsOutputTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentTemplatesOutputOutputTypeDef",
-    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
+    "ListEnvironmentTemplatesOutputTypeDef",
+    "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
     "GetEnvironmentInputEnvironmentDeployedWaitTypeDef",
     "GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef",
     "GetServiceInputServiceCreatedWaitTypeDef",
     "GetServiceInputServiceDeletedWaitTypeDef",
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
-    "ListComponentOutputsOutputOutputTypeDef",
-    "ListEnvironmentOutputsOutputOutputTypeDef",
-    "ListServiceInstanceOutputsOutputOutputTypeDef",
-    "ListServicePipelineOutputsOutputOutputTypeDef",
-    "ListComponentProvisionedResourcesOutputOutputTypeDef",
-    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
-    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
-    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
-    "ListRepositoriesOutputOutputTypeDef",
-    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
+    "ListComponentOutputsOutputTypeDef",
+    "ListEnvironmentOutputsOutputTypeDef",
+    "ListServiceInstanceOutputsOutputTypeDef",
+    "ListServicePipelineOutputsOutputTypeDef",
+    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    "ListComponentProvisionedResourcesOutputTypeDef",
+    "ListEnvironmentProvisionedResourcesOutputTypeDef",
+    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
+    "ListServicePipelineProvisionedResourcesOutputTypeDef",
+    "ListRepositoriesOutputTypeDef",
+    "ListRepositorySyncDefinitionsOutputTypeDef",
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     "ListServiceInstancesInputRequestTypeDef",
-    "ListServiceInstancesOutputOutputTypeDef",
-    "ListServiceTemplateVersionsOutputOutputTypeDef",
-    "ListServiceTemplatesOutputOutputTypeDef",
-    "ListServicesOutputOutputTypeDef",
-    "ListTagsForResourceOutputOutputTypeDef",
-    "NotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    "RepositorySyncAttemptOutputTypeDef",
-    "ResourceSyncAttemptOutputTypeDef",
+    "ListServiceInstancesOutputTypeDef",
+    "ListServiceTemplateVersionsOutputTypeDef",
+    "ListServiceTemplatesOutputTypeDef",
+    "ListServicesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "RepositorySyncAttemptTypeDef",
+    "ResourceSyncAttemptTypeDef",
     "TemplateVersionSourceInputTypeDef",
-    "SyncBlockerOutputTypeDef",
-    "GetAccountSettingsOutputOutputTypeDef",
-    "UpdateAccountSettingsOutputOutputTypeDef",
-    "CancelEnvironmentDeploymentOutputOutputTypeDef",
-    "CreateEnvironmentOutputOutputTypeDef",
-    "DeleteEnvironmentOutputOutputTypeDef",
-    "GetEnvironmentOutputOutputTypeDef",
-    "UpdateEnvironmentOutputOutputTypeDef",
-    "CreateServiceOutputOutputTypeDef",
-    "DeleteServiceOutputOutputTypeDef",
-    "GetServiceOutputOutputTypeDef",
-    "UpdateServiceOutputOutputTypeDef",
-    "CreateServiceTemplateVersionOutputOutputTypeDef",
-    "DeleteServiceTemplateVersionOutputOutputTypeDef",
-    "GetServiceTemplateVersionOutputOutputTypeDef",
-    "UpdateServiceTemplateVersionOutputOutputTypeDef",
-    "GetResourcesSummaryOutputOutputTypeDef",
-    "DeploymentOutputTypeDef",
-    "GetRepositorySyncStatusOutputOutputTypeDef",
-    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
-    "GetTemplateSyncStatusOutputOutputTypeDef",
+    "SyncBlockerTypeDef",
+    "GetAccountSettingsOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
+    "CancelEnvironmentDeploymentOutputTypeDef",
+    "CreateEnvironmentOutputTypeDef",
+    "DeleteEnvironmentOutputTypeDef",
+    "GetEnvironmentOutputTypeDef",
+    "UpdateEnvironmentOutputTypeDef",
+    "CreateServiceOutputTypeDef",
+    "DeleteServiceOutputTypeDef",
+    "GetServiceOutputTypeDef",
+    "UpdateServiceOutputTypeDef",
+    "CreateServiceTemplateVersionOutputTypeDef",
+    "DeleteServiceTemplateVersionOutputTypeDef",
+    "GetServiceTemplateVersionOutputTypeDef",
+    "UpdateServiceTemplateVersionOutputTypeDef",
+    "GetResourcesSummaryOutputTypeDef",
+    "DeploymentTypeDef",
+    "GetRepositorySyncStatusOutputTypeDef",
+    "GetServiceInstanceSyncStatusOutputTypeDef",
+    "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
-    "ServiceSyncBlockerSummaryOutputTypeDef",
-    "UpdateServiceSyncBlockerOutputOutputTypeDef",
-    "DeleteDeploymentOutputOutputTypeDef",
-    "GetDeploymentOutputOutputTypeDef",
-    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
+    "ServiceSyncBlockerSummaryTypeDef",
+    "UpdateServiceSyncBlockerOutputTypeDef",
+    "DeleteDeploymentOutputTypeDef",
+    "GetDeploymentOutputTypeDef",
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EnvironmentAccountConnectionOutputTypeDef = TypedDict(
-    "EnvironmentAccountConnectionOutputTypeDef",
+EnvironmentAccountConnectionTypeDef = TypedDict(
+    "EnvironmentAccountConnectionTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
@@ -327,16 +326,16 @@
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-RepositoryBranchOutputTypeDef = TypedDict(
-    "RepositoryBranchOutputTypeDef",
+RepositoryBranchTypeDef = TypedDict(
+    "RepositoryBranchTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -344,16 +343,16 @@
 CancelComponentDeploymentInputRequestTypeDef = TypedDict(
     "CancelComponentDeploymentInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 
-ComponentOutputTypeDef = TypedDict(
-    "ComponentOutputTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentName": str,
@@ -381,16 +380,16 @@
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ServiceInstanceOutputTypeDef = TypedDict(
-    "ServiceInstanceOutputTypeDef",
+ServiceInstanceTypeDef = TypedDict(
+    "ServiceInstanceTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -410,16 +409,16 @@
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-ServicePipelineOutputTypeDef = TypedDict(
-    "ServicePipelineOutputTypeDef",
+ServicePipelineTypeDef = TypedDict(
+    "ServicePipelineTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
@@ -436,34 +435,34 @@
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-CompatibleEnvironmentTemplateOutputTypeDef = TypedDict(
-    "CompatibleEnvironmentTemplateOutputTypeDef",
+CompatibleEnvironmentTemplateTypeDef = TypedDict(
+    "CompatibleEnvironmentTemplateTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-ComponentStateOutputTypeDef = TypedDict(
-    "ComponentStateOutputTypeDef",
+ComponentStateTypeDef = TypedDict(
+    "ComponentStateTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
         "templateFile": str,
     },
 )
 
-ComponentSummaryOutputTypeDef = TypedDict(
-    "ComponentSummaryOutputTypeDef",
+ComponentSummaryTypeDef = TypedDict(
+    "ComponentSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -473,16 +472,16 @@
         "lastSucceededDeploymentId": str,
         "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-ResourceCountsSummaryOutputTypeDef = TypedDict(
-    "ResourceCountsSummaryOutputTypeDef",
+ResourceCountsSummaryTypeDef = TypedDict(
+    "ResourceCountsSummaryTypeDef",
     {
         "behindMajor": int,
         "behindMinor": int,
         "failed": int,
         "total": int,
         "upToDate": int,
     },
@@ -501,31 +500,31 @@
     {
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
-EnvironmentTemplateOutputTypeDef = TypedDict(
-    "EnvironmentTemplateOutputTypeDef",
+EnvironmentTemplateTypeDef = TypedDict(
+    "EnvironmentTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionOutputTypeDef = TypedDict(
-    "EnvironmentTemplateVersionOutputTypeDef",
+EnvironmentTemplateVersionTypeDef = TypedDict(
+    "EnvironmentTemplateVersionTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -533,16 +532,16 @@
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-RepositoryOutputTypeDef = TypedDict(
-    "RepositoryOutputTypeDef",
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "encryptionKey": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
@@ -555,27 +554,27 @@
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceSyncConfigOutputTypeDef = TypedDict(
-    "ServiceSyncConfigOutputTypeDef",
+ServiceSyncConfigTypeDef = TypedDict(
+    "ServiceSyncConfigTypeDef",
     {
         "branch": str,
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-ServiceTemplateOutputTypeDef = TypedDict(
-    "ServiceTemplateOutputTypeDef",
+ServiceTemplateTypeDef = TypedDict(
+    "ServiceTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "encryptionKey": str,
         "lastModifiedAt": datetime,
@@ -605,16 +604,16 @@
 
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-TemplateSyncConfigOutputTypeDef = TypedDict(
-    "TemplateSyncConfigOutputTypeDef",
+TemplateSyncConfigTypeDef = TypedDict(
+    "TemplateSyncConfigTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "subdirectory": str,
         "templateName": str,
         "templateType": TemplateTypeType,
@@ -707,49 +706,49 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
-EnvironmentStateOutputTypeDef = TypedDict(
-    "EnvironmentStateOutputTypeDef",
+EnvironmentStateTypeDef = TypedDict(
+    "EnvironmentStateTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServiceInstanceStateOutputTypeDef = TypedDict(
-    "ServiceInstanceStateOutputTypeDef",
+ServiceInstanceStateTypeDef = TypedDict(
+    "ServiceInstanceStateTypeDef",
     {
         "lastSuccessfulComponentDeploymentIds": List[str],
         "lastSuccessfulEnvironmentDeploymentId": str,
         "lastSuccessfulServicePipelineDeploymentId": str,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-ServicePipelineStateOutputTypeDef = TypedDict(
-    "ServicePipelineStateOutputTypeDef",
+ServicePipelineStateTypeDef = TypedDict(
+    "ServicePipelineStateTypeDef",
     {
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-DeploymentSummaryOutputTypeDef = TypedDict(
-    "DeploymentSummaryOutputTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "environmentName": str,
@@ -761,32 +760,32 @@
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
     },
 )
 
-EnvironmentAccountConnectionSummaryOutputTypeDef = TypedDict(
-    "EnvironmentAccountConnectionSummaryOutputTypeDef",
+EnvironmentAccountConnectionSummaryTypeDef = TypedDict(
+    "EnvironmentAccountConnectionSummaryTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
 
-EnvironmentSummaryOutputTypeDef = TypedDict(
-    "EnvironmentSummaryOutputTypeDef",
+EnvironmentSummaryTypeDef = TypedDict(
+    "EnvironmentSummaryTypeDef",
     {
         "arn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
@@ -809,30 +808,30 @@
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-EnvironmentTemplateSummaryOutputTypeDef = TypedDict(
-    "EnvironmentTemplateSummaryOutputTypeDef",
+EnvironmentTemplateSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
 )
 
-EnvironmentTemplateVersionSummaryOutputTypeDef = TypedDict(
-    "EnvironmentTemplateVersionSummaryOutputTypeDef",
+EnvironmentTemplateVersionSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -948,16 +947,16 @@
     "GetServiceInstanceSyncStatusInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-RevisionOutputTypeDef = TypedDict(
-    "RevisionOutputTypeDef",
+RevisionTypeDef = TypedDict(
+    "RevisionTypeDef",
     {
         "branch": str,
         "directory": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "sha": str,
     },
@@ -1061,20 +1060,21 @@
 
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
     _OptionalListComponentOutputsInputRequestTypeDef,
 ):
     pass
 
-OutputOutputTypeDef = TypedDict(
-    "OutputOutputTypeDef",
+OutputTypeDef = TypedDict(
+    "OutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
+    total=False,
 )
 
 _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
     "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     {
         "componentName": str,
     },
@@ -1109,16 +1109,16 @@
 
 class ListComponentProvisionedResourcesInputRequestTypeDef(
     _RequiredListComponentProvisionedResourcesInputRequestTypeDef,
     _OptionalListComponentProvisionedResourcesInputRequestTypeDef,
 ):
     pass
 
-ProvisionedResourceOutputTypeDef = TypedDict(
-    "ProvisionedResourceOutputTypeDef",
+ProvisionedResourceTypeDef = TypedDict(
+    "ProvisionedResourceTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
 )
 
@@ -1370,16 +1370,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-RepositorySummaryOutputTypeDef = TypedDict(
-    "RepositorySummaryOutputTypeDef",
+RepositorySummaryTypeDef = TypedDict(
+    "RepositorySummaryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
@@ -1424,16 +1424,16 @@
 
 class ListRepositorySyncDefinitionsInputRequestTypeDef(
     _RequiredListRepositorySyncDefinitionsInputRequestTypeDef,
     _OptionalListRepositorySyncDefinitionsInputRequestTypeDef,
 ):
     pass
 
-RepositorySyncDefinitionOutputTypeDef = TypedDict(
-    "RepositorySyncDefinitionOutputTypeDef",
+RepositorySyncDefinitionTypeDef = TypedDict(
+    "RepositorySyncDefinitionTypeDef",
     {
         "branch": str,
         "directory": str,
         "parent": str,
         "target": str,
     },
 )
@@ -1529,16 +1529,16 @@
     {
         "key": ListServiceInstancesFilterByType,
         "value": str,
     },
     total=False,
 )
 
-ServiceInstanceSummaryOutputTypeDef = TypedDict(
-    "ServiceInstanceSummaryOutputTypeDef",
+ServiceInstanceSummaryTypeDef = TypedDict(
+    "ServiceInstanceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "lastAttemptedDeploymentId": str,
@@ -1674,16 +1674,16 @@
 
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
-ServiceTemplateVersionSummaryOutputTypeDef = TypedDict(
-    "ServiceTemplateVersionSummaryOutputTypeDef",
+ServiceTemplateVersionSummaryTypeDef = TypedDict(
+    "ServiceTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
@@ -1707,16 +1707,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceTemplateSummaryOutputTypeDef = TypedDict(
-    "ServiceTemplateSummaryOutputTypeDef",
+ServiceTemplateSummaryTypeDef = TypedDict(
+    "ServiceTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "displayName": str,
         "lastModifiedAt": datetime,
         "name": str,
@@ -1738,16 +1738,16 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ServiceSummaryOutputTypeDef = TypedDict(
-    "ServiceSummaryOutputTypeDef",
+ServiceSummaryTypeDef = TypedDict(
+    "ServiceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
@@ -1800,23 +1800,14 @@
     "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-OutputTypeDef = TypedDict(
-    "OutputTypeDef",
-    {
-        "key": str,
-        "valueString": str,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1826,26 +1817,26 @@
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-RepositorySyncEventOutputTypeDef = TypedDict(
-    "RepositorySyncEventOutputTypeDef",
+RepositorySyncEventTypeDef = TypedDict(
+    "RepositorySyncEventTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
 
-ResourceSyncEventOutputTypeDef = TypedDict(
-    "ResourceSyncEventOutputTypeDef",
+ResourceSyncEventTypeDef = TypedDict(
+    "ResourceSyncEventTypeDef",
     {
         "event": str,
         "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
@@ -1865,16 +1856,16 @@
     "S3ObjectSourceTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
 
-SyncBlockerContextOutputTypeDef = TypedDict(
-    "SyncBlockerContextOutputTypeDef",
+SyncBlockerContextTypeDef = TypedDict(
+    "SyncBlockerContextTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 UntagResourceInputRequestTypeDef = TypedDict(
@@ -2104,73 +2095,73 @@
 
 class UpdateTemplateSyncConfigInputRequestTypeDef(
     _RequiredUpdateTemplateSyncConfigInputRequestTypeDef,
     _OptionalUpdateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-AcceptEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "AcceptEnvironmentAccountConnectionOutputOutputTypeDef",
+AcceptEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "AcceptEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentAccountConnectionOutputOutputTypeDef",
+CreateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "CreateEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentAccountConnectionOutputOutputTypeDef",
+DeleteEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "DeleteEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentAccountConnectionOutputOutputTypeDef",
+GetEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "GetEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RejectEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "RejectEnvironmentAccountConnectionOutputOutputTypeDef",
+RejectEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "RejectEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentAccountConnectionOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentAccountConnectionOutputOutputTypeDef",
+UpdateEnvironmentAccountConnectionOutputTypeDef = TypedDict(
+    "UpdateEnvironmentAccountConnectionOutputTypeDef",
     {
-        "environmentAccountConnection": EnvironmentAccountConnectionOutputTypeDef,
+        "environmentAccountConnection": EnvironmentAccountConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AccountSettingsOutputTypeDef = TypedDict(
-    "AccountSettingsOutputTypeDef",
+AccountSettingsTypeDef = TypedDict(
+    "AccountSettingsTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
-        "pipelineProvisioningRepository": RepositoryBranchOutputTypeDef,
+        "pipelineProvisioningRepository": RepositoryBranchTypeDef,
         "pipelineServiceRoleArn": str,
     },
 )
 
-EnvironmentOutputTypeDef = TypedDict(
-    "EnvironmentOutputTypeDef",
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
     {
         "arn": str,
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
@@ -2180,125 +2171,125 @@
         "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
         "lastSucceededDeploymentId": str,
         "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
-        "provisioningRepository": RepositoryBranchOutputTypeDef,
+        "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
 
-CancelComponentDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelComponentDeploymentOutputOutputTypeDef",
+CancelComponentDeploymentOutputTypeDef = TypedDict(
+    "CancelComponentDeploymentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateComponentOutputOutputTypeDef = TypedDict(
-    "CreateComponentOutputOutputTypeDef",
+CreateComponentOutputTypeDef = TypedDict(
+    "CreateComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteComponentOutputOutputTypeDef = TypedDict(
-    "DeleteComponentOutputOutputTypeDef",
+DeleteComponentOutputTypeDef = TypedDict(
+    "DeleteComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetComponentOutputOutputTypeDef = TypedDict(
-    "GetComponentOutputOutputTypeDef",
+GetComponentOutputTypeDef = TypedDict(
+    "GetComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateComponentOutputOutputTypeDef = TypedDict(
-    "UpdateComponentOutputOutputTypeDef",
+UpdateComponentOutputTypeDef = TypedDict(
+    "UpdateComponentOutputTypeDef",
     {
-        "component": ComponentOutputTypeDef,
+        "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServiceInstanceDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelServiceInstanceDeploymentOutputOutputTypeDef",
+CancelServiceInstanceDeploymentOutputTypeDef = TypedDict(
+    "CancelServiceInstanceDeploymentOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceInstanceOutputOutputTypeDef = TypedDict(
-    "CreateServiceInstanceOutputOutputTypeDef",
+CreateServiceInstanceOutputTypeDef = TypedDict(
+    "CreateServiceInstanceOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceOutputOutputTypeDef = TypedDict(
-    "GetServiceInstanceOutputOutputTypeDef",
+GetServiceInstanceOutputTypeDef = TypedDict(
+    "GetServiceInstanceOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceInstanceOutputOutputTypeDef = TypedDict(
-    "UpdateServiceInstanceOutputOutputTypeDef",
+UpdateServiceInstanceOutputTypeDef = TypedDict(
+    "UpdateServiceInstanceOutputTypeDef",
     {
-        "serviceInstance": ServiceInstanceOutputTypeDef,
+        "serviceInstance": ServiceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelServicePipelineDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelServicePipelineDeploymentOutputOutputTypeDef",
+CancelServicePipelineDeploymentOutputTypeDef = TypedDict(
+    "CancelServicePipelineDeploymentOutputTypeDef",
     {
-        "pipeline": ServicePipelineOutputTypeDef,
+        "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServiceOutputTypeDef = TypedDict(
-    "ServiceOutputTypeDef",
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
     {
         "arn": str,
         "branchName": str,
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "name": str,
-        "pipeline": ServicePipelineOutputTypeDef,
+        "pipeline": ServicePipelineTypeDef,
         "repositoryConnectionArn": str,
         "repositoryId": str,
         "spec": str,
         "status": ServiceStatusType,
         "statusMessage": str,
         "templateName": str,
     },
 )
 
-UpdateServicePipelineOutputOutputTypeDef = TypedDict(
-    "UpdateServicePipelineOutputOutputTypeDef",
+UpdateServicePipelineOutputTypeDef = TypedDict(
+    "UpdateServicePipelineOutputTypeDef",
     {
-        "pipeline": ServicePipelineOutputTypeDef,
+        "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateServiceTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceTemplateVersionInputRequestTypeDef",
     {
@@ -2320,52 +2311,52 @@
 
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-ServiceTemplateVersionOutputTypeDef = TypedDict(
-    "ServiceTemplateVersionOutputTypeDef",
+ServiceTemplateVersionTypeDef = TypedDict(
+    "ServiceTemplateVersionTypeDef",
     {
         "arn": str,
-        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateOutputTypeDef],
+        "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
         "createdAt": datetime,
         "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
         "recommendedMinorVersion": str,
         "schema": str,
         "status": TemplateVersionStatusType,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
         "templateName": str,
     },
 )
 
-ListComponentsOutputOutputTypeDef = TypedDict(
-    "ListComponentsOutputOutputTypeDef",
+ListComponentsOutputTypeDef = TypedDict(
+    "ListComponentsOutputTypeDef",
     {
-        "components": List[ComponentSummaryOutputTypeDef],
+        "components": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CountsSummaryOutputTypeDef = TypedDict(
-    "CountsSummaryOutputTypeDef",
+CountsSummaryTypeDef = TypedDict(
+    "CountsSummaryTypeDef",
     {
-        "components": ResourceCountsSummaryOutputTypeDef,
-        "environmentTemplates": ResourceCountsSummaryOutputTypeDef,
-        "environments": ResourceCountsSummaryOutputTypeDef,
-        "pipelines": ResourceCountsSummaryOutputTypeDef,
-        "serviceInstances": ResourceCountsSummaryOutputTypeDef,
-        "serviceTemplates": ResourceCountsSummaryOutputTypeDef,
-        "services": ResourceCountsSummaryOutputTypeDef,
+        "components": ResourceCountsSummaryTypeDef,
+        "environmentTemplates": ResourceCountsSummaryTypeDef,
+        "environments": ResourceCountsSummaryTypeDef,
+        "pipelines": ResourceCountsSummaryTypeDef,
+        "serviceInstances": ResourceCountsSummaryTypeDef,
+        "serviceTemplates": ResourceCountsSummaryTypeDef,
+        "services": ResourceCountsSummaryTypeDef,
     },
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
@@ -2611,230 +2602,230 @@
 )
 
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
-CreateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateOutputOutputTypeDef",
+CreateEnvironmentTemplateOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateOutputOutputTypeDef",
+DeleteEnvironmentTemplateOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateOutputOutputTypeDef",
+GetEnvironmentTemplateOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateOutputOutputTypeDef",
+UpdateEnvironmentTemplateOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateOutputTypeDef",
     {
-        "environmentTemplate": EnvironmentTemplateOutputTypeDef,
+        "environmentTemplate": EnvironmentTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentTemplateVersionOutputOutputTypeDef",
+CreateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "CreateEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentTemplateVersionOutputOutputTypeDef",
+DeleteEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "DeleteEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentTemplateVersionOutputOutputTypeDef",
+GetEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "GetEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentTemplateVersionOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentTemplateVersionOutputOutputTypeDef",
+UpdateEnvironmentTemplateVersionOutputTypeDef = TypedDict(
+    "UpdateEnvironmentTemplateVersionOutputTypeDef",
     {
-        "environmentTemplateVersion": EnvironmentTemplateVersionOutputTypeDef,
+        "environmentTemplateVersion": EnvironmentTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRepositoryOutputOutputTypeDef = TypedDict(
-    "CreateRepositoryOutputOutputTypeDef",
+CreateRepositoryOutputTypeDef = TypedDict(
+    "CreateRepositoryOutputTypeDef",
     {
-        "repository": RepositoryOutputTypeDef,
+        "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRepositoryOutputOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputOutputTypeDef",
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
     {
-        "repository": RepositoryOutputTypeDef,
+        "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRepositoryOutputOutputTypeDef = TypedDict(
-    "GetRepositoryOutputOutputTypeDef",
+GetRepositoryOutputTypeDef = TypedDict(
+    "GetRepositoryOutputTypeDef",
     {
-        "repository": RepositoryOutputTypeDef,
+        "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "CreateServiceSyncConfigOutputOutputTypeDef",
+CreateServiceSyncConfigOutputTypeDef = TypedDict(
+    "CreateServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "DeleteServiceSyncConfigOutputOutputTypeDef",
+DeleteServiceSyncConfigOutputTypeDef = TypedDict(
+    "DeleteServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "GetServiceSyncConfigOutputOutputTypeDef",
+GetServiceSyncConfigOutputTypeDef = TypedDict(
+    "GetServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceSyncConfigOutputOutputTypeDef = TypedDict(
-    "UpdateServiceSyncConfigOutputOutputTypeDef",
+UpdateServiceSyncConfigOutputTypeDef = TypedDict(
+    "UpdateServiceSyncConfigOutputTypeDef",
     {
-        "serviceSyncConfig": ServiceSyncConfigOutputTypeDef,
+        "serviceSyncConfig": ServiceSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateOutputOutputTypeDef = TypedDict(
-    "CreateServiceTemplateOutputOutputTypeDef",
+CreateServiceTemplateOutputTypeDef = TypedDict(
+    "CreateServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateOutputOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateOutputOutputTypeDef",
+DeleteServiceTemplateOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateOutputOutputTypeDef = TypedDict(
-    "GetServiceTemplateOutputOutputTypeDef",
+GetServiceTemplateOutputTypeDef = TypedDict(
+    "GetServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateOutputOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateOutputOutputTypeDef",
+UpdateServiceTemplateOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateOutputTypeDef",
     {
-        "serviceTemplate": ServiceTemplateOutputTypeDef,
+        "serviceTemplate": ServiceTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "CreateTemplateSyncConfigOutputOutputTypeDef",
+CreateTemplateSyncConfigOutputTypeDef = TypedDict(
+    "CreateTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "DeleteTemplateSyncConfigOutputOutputTypeDef",
+DeleteTemplateSyncConfigOutputTypeDef = TypedDict(
+    "DeleteTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "GetTemplateSyncConfigOutputOutputTypeDef",
+GetTemplateSyncConfigOutputTypeDef = TypedDict(
+    "GetTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateTemplateSyncConfigOutputOutputTypeDef = TypedDict(
-    "UpdateTemplateSyncConfigOutputOutputTypeDef",
+UpdateTemplateSyncConfigOutputTypeDef = TypedDict(
+    "UpdateTemplateSyncConfigOutputTypeDef",
     {
-        "templateSyncConfig": TemplateSyncConfigOutputTypeDef,
+        "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentStateOutputTypeDef = TypedDict(
-    "DeploymentStateOutputTypeDef",
+DeploymentStateTypeDef = TypedDict(
+    "DeploymentStateTypeDef",
     {
-        "component": ComponentStateOutputTypeDef,
-        "environment": EnvironmentStateOutputTypeDef,
-        "serviceInstance": ServiceInstanceStateOutputTypeDef,
-        "servicePipeline": ServicePipelineStateOutputTypeDef,
+        "component": ComponentStateTypeDef,
+        "environment": EnvironmentStateTypeDef,
+        "serviceInstance": ServiceInstanceStateTypeDef,
+        "servicePipeline": ServicePipelineStateTypeDef,
     },
 )
 
-ListDeploymentsOutputOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputOutputTypeDef",
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
     {
-        "deployments": List[DeploymentSummaryOutputTypeDef],
+        "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentAccountConnectionsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentAccountConnectionsOutputOutputTypeDef",
+ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
+    "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
-        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryOutputTypeDef],
+        "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputOutputTypeDef",
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
     {
-        "environments": List[EnvironmentSummaryOutputTypeDef],
+        "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
@@ -2851,28 +2842,28 @@
         "environmentTemplates": Sequence[EnvironmentTemplateFilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentTemplatesOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplatesOutputOutputTypeDef",
+ListEnvironmentTemplatesOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplatesOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[EnvironmentTemplateSummaryOutputTypeDef],
+        "templates": List[EnvironmentTemplateSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentTemplateVersionsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentTemplateVersionsOutputOutputTypeDef",
+ListEnvironmentTemplateVersionsOutputTypeDef = TypedDict(
+    "ListEnvironmentTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[EnvironmentTemplateVersionSummaryOutputTypeDef],
+        "templateVersions": List[EnvironmentTemplateVersionSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetComponentInputComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetComponentInputComponentDeletedWaitTypeDef",
     {
@@ -3074,100 +3065,123 @@
 
 class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(
     _RequiredGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
     _OptionalGetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef,
 ):
     pass
 
-ListComponentOutputsOutputOutputTypeDef = TypedDict(
-    "ListComponentOutputsOutputOutputTypeDef",
+ListComponentOutputsOutputTypeDef = TypedDict(
+    "ListComponentOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentOutputsOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentOutputsOutputOutputTypeDef",
+ListEnvironmentOutputsOutputTypeDef = TypedDict(
+    "ListEnvironmentOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceOutputsOutputOutputTypeDef = TypedDict(
-    "ListServiceInstanceOutputsOutputOutputTypeDef",
+ListServiceInstanceOutputsOutputTypeDef = TypedDict(
+    "ListServiceInstanceOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineOutputsOutputOutputTypeDef = TypedDict(
-    "ListServicePipelineOutputsOutputOutputTypeDef",
+ListServicePipelineOutputsOutputTypeDef = TypedDict(
+    "ListServicePipelineOutputsOutputTypeDef",
     {
         "nextToken": str,
-        "outputs": List[OutputOutputTypeDef],
+        "outputs": List[OutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListComponentProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListComponentProvisionedResourcesOutputOutputTypeDef",
+_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
+    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
+    {
+        "deploymentId": str,
+        "outputs": Sequence[OutputTypeDef],
+        "status": ResourceDeploymentStatusType,
+        "statusMessage": str,
+    },
+    total=False,
+)
+
+class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
+    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
+):
+    pass
+
+ListComponentProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListComponentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEnvironmentProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListEnvironmentProvisionedResourcesOutputOutputTypeDef",
+ListEnvironmentProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListEnvironmentProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceInstanceProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListServiceInstanceProvisionedResourcesOutputOutputTypeDef",
+ListServiceInstanceProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListServiceInstanceProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicePipelineProvisionedResourcesOutputOutputTypeDef = TypedDict(
-    "ListServicePipelineProvisionedResourcesOutputOutputTypeDef",
+ListServicePipelineProvisionedResourcesOutputTypeDef = TypedDict(
+    "ListServicePipelineProvisionedResourcesOutputTypeDef",
     {
         "nextToken": str,
-        "provisionedResources": List[ProvisionedResourceOutputTypeDef],
+        "provisionedResources": List[ProvisionedResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositoriesOutputOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputOutputTypeDef",
+ListRepositoriesOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputTypeDef",
     {
         "nextToken": str,
-        "repositories": List[RepositorySummaryOutputTypeDef],
+        "repositories": List[RepositorySummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositorySyncDefinitionsOutputOutputTypeDef = TypedDict(
-    "ListRepositorySyncDefinitionsOutputOutputTypeDef",
+ListRepositorySyncDefinitionsOutputTypeDef = TypedDict(
+    "ListRepositorySyncDefinitionsOutputTypeDef",
     {
         "nextToken": str,
-        "syncDefinitions": List[RepositorySyncDefinitionOutputTypeDef],
+        "syncDefinitions": List[RepositorySyncDefinitionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServiceInstancesInputListServiceInstancesPaginateTypeDef = TypedDict(
     "ListServiceInstancesInputListServiceInstancesPaginateTypeDef",
     {
@@ -3189,301 +3203,278 @@
         "serviceName": str,
         "sortBy": ListServiceInstancesSortByType,
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListServiceInstancesOutputOutputTypeDef = TypedDict(
-    "ListServiceInstancesOutputOutputTypeDef",
+ListServiceInstancesOutputTypeDef = TypedDict(
+    "ListServiceInstancesOutputTypeDef",
     {
         "nextToken": str,
-        "serviceInstances": List[ServiceInstanceSummaryOutputTypeDef],
+        "serviceInstances": List[ServiceInstanceSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplateVersionsOutputOutputTypeDef = TypedDict(
-    "ListServiceTemplateVersionsOutputOutputTypeDef",
+ListServiceTemplateVersionsOutputTypeDef = TypedDict(
+    "ListServiceTemplateVersionsOutputTypeDef",
     {
         "nextToken": str,
-        "templateVersions": List[ServiceTemplateVersionSummaryOutputTypeDef],
+        "templateVersions": List[ServiceTemplateVersionSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceTemplatesOutputOutputTypeDef = TypedDict(
-    "ListServiceTemplatesOutputOutputTypeDef",
+ListServiceTemplatesOutputTypeDef = TypedDict(
+    "ListServiceTemplatesOutputTypeDef",
     {
         "nextToken": str,
-        "templates": List[ServiceTemplateSummaryOutputTypeDef],
+        "templates": List[ServiceTemplateSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServicesOutputOutputTypeDef = TypedDict(
-    "ListServicesOutputOutputTypeDef",
+ListServicesOutputTypeDef = TypedDict(
+    "ListServicesOutputTypeDef",
     {
         "nextToken": str,
-        "services": List[ServiceSummaryOutputTypeDef],
+        "services": List[ServiceSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceOutputOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputOutputTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef",
-    {
-        "deploymentId": str,
-        "outputs": Sequence[OutputTypeDef],
-        "status": ResourceDeploymentStatusType,
-        "statusMessage": str,
-    },
-    total=False,
-)
-
-class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(
-    _RequiredNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-    _OptionalNotifyResourceDeploymentStatusChangeInputRequestTypeDef,
-):
-    pass
-
-RepositorySyncAttemptOutputTypeDef = TypedDict(
-    "RepositorySyncAttemptOutputTypeDef",
+RepositorySyncAttemptTypeDef = TypedDict(
+    "RepositorySyncAttemptTypeDef",
     {
-        "events": List[RepositorySyncEventOutputTypeDef],
+        "events": List[RepositorySyncEventTypeDef],
         "startedAt": datetime,
         "status": RepositorySyncStatusType,
     },
 )
 
-ResourceSyncAttemptOutputTypeDef = TypedDict(
-    "ResourceSyncAttemptOutputTypeDef",
+ResourceSyncAttemptTypeDef = TypedDict(
+    "ResourceSyncAttemptTypeDef",
     {
-        "events": List[ResourceSyncEventOutputTypeDef],
-        "initialRevision": RevisionOutputTypeDef,
+        "events": List[ResourceSyncEventTypeDef],
+        "initialRevision": RevisionTypeDef,
         "startedAt": datetime,
         "status": ResourceSyncStatusType,
         "target": str,
-        "targetRevision": RevisionOutputTypeDef,
+        "targetRevision": RevisionTypeDef,
     },
 )
 
 TemplateVersionSourceInputTypeDef = TypedDict(
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
-SyncBlockerOutputTypeDef = TypedDict(
-    "SyncBlockerOutputTypeDef",
+SyncBlockerTypeDef = TypedDict(
+    "SyncBlockerTypeDef",
     {
-        "contexts": List[SyncBlockerContextOutputTypeDef],
+        "contexts": List[SyncBlockerContextTypeDef],
         "createdAt": datetime,
         "createdReason": str,
         "id": str,
         "resolvedAt": datetime,
         "resolvedReason": str,
         "status": BlockerStatusType,
         "type": Literal["AUTOMATED"],
     },
 )
 
-GetAccountSettingsOutputOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputOutputTypeDef",
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
     {
-        "accountSettings": AccountSettingsOutputTypeDef,
+        "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAccountSettingsOutputOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputOutputTypeDef",
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
     {
-        "accountSettings": AccountSettingsOutputTypeDef,
+        "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelEnvironmentDeploymentOutputOutputTypeDef = TypedDict(
-    "CancelEnvironmentDeploymentOutputOutputTypeDef",
+CancelEnvironmentDeploymentOutputTypeDef = TypedDict(
+    "CancelEnvironmentDeploymentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEnvironmentOutputOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputOutputTypeDef",
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEnvironmentOutputOutputTypeDef = TypedDict(
-    "DeleteEnvironmentOutputOutputTypeDef",
+DeleteEnvironmentOutputTypeDef = TypedDict(
+    "DeleteEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetEnvironmentOutputOutputTypeDef = TypedDict(
-    "GetEnvironmentOutputOutputTypeDef",
+GetEnvironmentOutputTypeDef = TypedDict(
+    "GetEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEnvironmentOutputOutputTypeDef = TypedDict(
-    "UpdateEnvironmentOutputOutputTypeDef",
+UpdateEnvironmentOutputTypeDef = TypedDict(
+    "UpdateEnvironmentOutputTypeDef",
     {
-        "environment": EnvironmentOutputTypeDef,
+        "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceOutputOutputTypeDef = TypedDict(
-    "CreateServiceOutputOutputTypeDef",
+CreateServiceOutputTypeDef = TypedDict(
+    "CreateServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceOutputOutputTypeDef = TypedDict(
-    "DeleteServiceOutputOutputTypeDef",
+DeleteServiceOutputTypeDef = TypedDict(
+    "DeleteServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceOutputOutputTypeDef = TypedDict(
-    "GetServiceOutputOutputTypeDef",
+GetServiceOutputTypeDef = TypedDict(
+    "GetServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceOutputOutputTypeDef = TypedDict(
-    "UpdateServiceOutputOutputTypeDef",
+UpdateServiceOutputTypeDef = TypedDict(
+    "UpdateServiceOutputTypeDef",
     {
-        "service": ServiceOutputTypeDef,
+        "service": ServiceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "CreateServiceTemplateVersionOutputOutputTypeDef",
+CreateServiceTemplateVersionOutputTypeDef = TypedDict(
+    "CreateServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "DeleteServiceTemplateVersionOutputOutputTypeDef",
+DeleteServiceTemplateVersionOutputTypeDef = TypedDict(
+    "DeleteServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "GetServiceTemplateVersionOutputOutputTypeDef",
+GetServiceTemplateVersionOutputTypeDef = TypedDict(
+    "GetServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceTemplateVersionOutputOutputTypeDef = TypedDict(
-    "UpdateServiceTemplateVersionOutputOutputTypeDef",
+UpdateServiceTemplateVersionOutputTypeDef = TypedDict(
+    "UpdateServiceTemplateVersionOutputTypeDef",
     {
-        "serviceTemplateVersion": ServiceTemplateVersionOutputTypeDef,
+        "serviceTemplateVersion": ServiceTemplateVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetResourcesSummaryOutputOutputTypeDef = TypedDict(
-    "GetResourcesSummaryOutputOutputTypeDef",
+GetResourcesSummaryOutputTypeDef = TypedDict(
+    "GetResourcesSummaryOutputTypeDef",
     {
-        "counts": CountsSummaryOutputTypeDef,
+        "counts": CountsSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentOutputTypeDef = TypedDict(
-    "DeploymentOutputTypeDef",
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
     {
         "arn": str,
         "completedAt": datetime,
         "componentName": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "environmentName": str,
         "id": str,
-        "initialState": DeploymentStateOutputTypeDef,
+        "initialState": DeploymentStateTypeDef,
         "lastAttemptedDeploymentId": str,
         "lastModifiedAt": datetime,
         "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "targetArn": str,
         "targetResourceCreatedAt": datetime,
         "targetResourceType": DeploymentTargetResourceTypeType,
-        "targetState": DeploymentStateOutputTypeDef,
+        "targetState": DeploymentStateTypeDef,
     },
 )
 
-GetRepositorySyncStatusOutputOutputTypeDef = TypedDict(
-    "GetRepositorySyncStatusOutputOutputTypeDef",
+GetRepositorySyncStatusOutputTypeDef = TypedDict(
+    "GetRepositorySyncStatusOutputTypeDef",
     {
-        "latestSync": RepositorySyncAttemptOutputTypeDef,
+        "latestSync": RepositorySyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceInstanceSyncStatusOutputOutputTypeDef = TypedDict(
-    "GetServiceInstanceSyncStatusOutputOutputTypeDef",
+GetServiceInstanceSyncStatusOutputTypeDef = TypedDict(
+    "GetServiceInstanceSyncStatusOutputTypeDef",
     {
-        "desiredState": RevisionOutputTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
-        "latestSync": ResourceSyncAttemptOutputTypeDef,
+        "desiredState": RevisionTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
+        "latestSync": ResourceSyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetTemplateSyncStatusOutputOutputTypeDef = TypedDict(
-    "GetTemplateSyncStatusOutputOutputTypeDef",
+GetTemplateSyncStatusOutputTypeDef = TypedDict(
+    "GetTemplateSyncStatusOutputTypeDef",
     {
-        "desiredState": RevisionOutputTypeDef,
-        "latestSuccessfulSync": ResourceSyncAttemptOutputTypeDef,
-        "latestSync": ResourceSyncAttemptOutputTypeDef,
+        "desiredState": RevisionTypeDef,
+        "latestSuccessfulSync": ResourceSyncAttemptTypeDef,
+        "latestSync": ResourceSyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentTemplateVersionInputRequestTypeDef",
     {
@@ -3530,49 +3521,49 @@
 
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-ServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
-    "ServiceSyncBlockerSummaryOutputTypeDef",
+ServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "ServiceSyncBlockerSummaryTypeDef",
     {
-        "latestBlockers": List[SyncBlockerOutputTypeDef],
+        "latestBlockers": List[SyncBlockerTypeDef],
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-UpdateServiceSyncBlockerOutputOutputTypeDef = TypedDict(
-    "UpdateServiceSyncBlockerOutputOutputTypeDef",
+UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
+    "UpdateServiceSyncBlockerOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
-        "serviceSyncBlocker": SyncBlockerOutputTypeDef,
+        "serviceSyncBlocker": SyncBlockerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDeploymentOutputOutputTypeDef = TypedDict(
-    "DeleteDeploymentOutputOutputTypeDef",
+DeleteDeploymentOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputTypeDef",
     {
-        "deployment": DeploymentOutputTypeDef,
+        "deployment": DeploymentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDeploymentOutputOutputTypeDef = TypedDict(
-    "GetDeploymentOutputOutputTypeDef",
+GetDeploymentOutputTypeDef = TypedDict(
+    "GetDeploymentOutputTypeDef",
     {
-        "deployment": DeploymentOutputTypeDef,
+        "deployment": DeploymentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceSyncBlockerSummaryOutputOutputTypeDef = TypedDict(
-    "GetServiceSyncBlockerSummaryOutputOutputTypeDef",
+GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
+    "GetServiceSyncBlockerSummaryOutputTypeDef",
     {
-        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryOutputTypeDef,
+        "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.py` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton/waiter.pyi` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/mypy_boto3_proton.egg-info/SOURCES.txt` & `mypy-boto3-proton-1.28.3.post2/mypy_boto3_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.3.post1/setup.py` & `mypy-boto3-proton-1.28.3.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-proton",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.7"
+        "Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

