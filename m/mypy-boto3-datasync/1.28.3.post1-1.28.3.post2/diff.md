# Comparing `tmp/mypy-boto3-datasync-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-datasync-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datasync-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+gzip compressed data, was "mypy-boto3-datasync-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
```

## Comparing `mypy-boto3-datasync-1.28.3.post1.tar` & `mypy-boto3-datasync-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45897 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45825 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-14 16:15:33.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-14 16:15:33.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59781 2023-07-14 16:15:34.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59720 2023-07-14 16:15:33.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.322243 mypy-boto3-datasync-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20953 2023-07-15 06:38:32.322243 mypy-boto3-datasync-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.302242 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45373 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45301 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-15 06:36:01.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-15 06:36:01.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58575 2023-07-15 06:36:03.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-15 06:36:02.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.322243 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20953 2023-07-15 06:38:32.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-15 06:38:32.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-15 06:38:32.000000 mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.322243 mypy-boto3-datasync-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-15 06:36:00.000000 mypy-boto3-datasync-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/LICENSE` & `mypy-boto3-datasync-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3.post1/PKG-INFO` & `mypy-boto3-datasync-1.28.3.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
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
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,170 +391,170 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
     CredentialsTypeDef,
     DiscoveryServerConfigurationTypeDef,
     TagListEntryTypeDef,
-    AddStorageSystemResponseOutputTypeDef,
-    AgentListEntryOutputTypeDef,
+    AddStorageSystemResponseTypeDef,
+    AgentListEntryTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    CapacityOutputTypeDef,
-    CreateAgentResponseOutputTypeDef,
+    CapacityTypeDef,
+    CreateAgentResponseTypeDef,
     Ec2ConfigTypeDef,
-    CreateLocationEfsResponseOutputTypeDef,
-    CreateLocationFsxLustreResponseOutputTypeDef,
-    CreateLocationFsxOntapResponseOutputTypeDef,
-    CreateLocationFsxOpenZfsResponseOutputTypeDef,
-    CreateLocationFsxWindowsResponseOutputTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
-    CreateLocationHdfsResponseOutputTypeDef,
+    CreateLocationHdfsResponseTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
-    CreateLocationNfsResponseOutputTypeDef,
-    CreateLocationObjectStorageResponseOutputTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
     S3ConfigTypeDef,
-    CreateLocationS3ResponseOutputTypeDef,
+    CreateLocationS3ResponseTypeDef,
     SmbMountOptionsTypeDef,
-    CreateLocationSmbResponseOutputTypeDef,
+    CreateLocationSmbResponseTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
-    CreateTaskResponseOutputTypeDef,
+    CreateTaskResponseTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
-    PrivateLinkConfigOutputTypeDef,
+    PrivateLinkConfigTypeDef,
     DescribeDiscoveryJobRequestRequestTypeDef,
-    DescribeDiscoveryJobResponseOutputTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
     Ec2ConfigOutputTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
-    DescribeLocationFsxLustreResponseOutputTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
-    DescribeLocationFsxWindowsResponseOutputTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
     HdfsNameNodeOutputTypeDef,
     QopConfigurationOutputTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
     NfsMountOptionsOutputTypeDef,
     OnPremConfigOutputTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
-    DescribeLocationObjectStorageResponseOutputTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
     S3ConfigOutputTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
     SmbMountOptionsOutputTypeDef,
     DescribeStorageSystemRequestRequestTypeDef,
     DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     DescribeStorageSystemResourcesRequestRequestTypeDef,
     DiscoveryServerConfigurationOutputTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
     FilterRuleOutputTypeDef,
     OptionsOutputTypeDef,
-    TaskExecutionResultDetailOutputTypeDef,
+    TaskExecutionResultDetailTypeDef,
     DescribeTaskRequestRequestTypeDef,
     TaskScheduleOutputTypeDef,
-    DiscoveryJobListEntryOutputTypeDef,
+    DiscoveryJobListEntryTypeDef,
     GenerateRecommendationsRequestRequestTypeDef,
-    IOPSOutputTypeDef,
-    LatencyOutputTypeDef,
+    IOPSTypeDef,
+    LatencyTypeDef,
     ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
     ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
     ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
-    LocationListEntryOutputTypeDef,
+    LocationListEntryTypeDef,
     ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
     ListStorageSystemsRequestRequestTypeDef,
-    StorageSystemListEntryOutputTypeDef,
+    StorageSystemListEntryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagListEntryOutputTypeDef,
     ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
-    TaskExecutionListEntryOutputTypeDef,
+    TaskExecutionListEntryTypeDef,
     TaskFilterTypeDef,
-    TaskListEntryOutputTypeDef,
-    MaxP95PerformanceOutputTypeDef,
-    RecommendationOutputTypeDef,
-    ThroughputOutputTypeDef,
+    TaskListEntryTypeDef,
+    MaxP95PerformanceTypeDef,
+    RecommendationTypeDef,
+    ThroughputTypeDef,
     PaginatorConfigTypeDef,
     RemoveStorageSystemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    StartDiscoveryJobResponseOutputTypeDef,
-    StartTaskExecutionResponseOutputTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
     StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
     UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
     UpdateStorageSystemRequestRequestTypeDef,
     AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
     StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAgentsResponseOutputTypeDef,
+    ListAgentsResponseTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
     UpdateLocationNfsRequestRequestTypeDef,
     CreateLocationS3RequestRequestTypeDef,
     CreateLocationSmbRequestRequestTypeDef,
     FsxProtocolSmbTypeDef,
     UpdateLocationSmbRequestRequestTypeDef,
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
     UpdateTaskRequestRequestTypeDef,
-    DescribeAgentResponseOutputTypeDef,
-    DescribeLocationEfsResponseOutputTypeDef,
-    DescribeLocationHdfsResponseOutputTypeDef,
+    DescribeAgentResponseTypeDef,
+    DescribeLocationEfsResponseTypeDef,
+    DescribeLocationHdfsResponseTypeDef,
     FsxProtocolNfsOutputTypeDef,
-    DescribeLocationNfsResponseOutputTypeDef,
-    DescribeLocationS3ResponseOutputTypeDef,
-    DescribeLocationSmbResponseOutputTypeDef,
+    DescribeLocationNfsResponseTypeDef,
+    DescribeLocationS3ResponseTypeDef,
+    DescribeLocationSmbResponseTypeDef,
     FsxProtocolSmbOutputTypeDef,
-    DescribeStorageSystemResponseOutputTypeDef,
-    DescribeTaskExecutionResponseOutputTypeDef,
-    DescribeTaskResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    DescribeTaskExecutionResponseTypeDef,
+    DescribeTaskResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseOutputTypeDef,
-    NetAppONTAPClusterOutputTypeDef,
-    NetAppONTAPSVMOutputTypeDef,
-    NetAppONTAPVolumeOutputTypeDef,
-    P95MetricsOutputTypeDef,
+    ListTasksResponseTypeDef,
+    NetAppONTAPClusterTypeDef,
+    NetAppONTAPSVMTypeDef,
+    NetAppONTAPVolumeTypeDef,
+    P95MetricsTypeDef,
     FsxProtocolTypeDef,
     FsxProtocolOutputTypeDef,
-    ResourceDetailsOutputTypeDef,
-    ResourceMetricsOutputTypeDef,
+    ResourceDetailsTypeDef,
+    ResourceMetricsTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
-    DescribeLocationFsxOntapResponseOutputTypeDef,
-    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
-    DescribeStorageSystemResourcesResponseOutputTypeDef,
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    DescribeLocationFsxOntapResponseTypeDef,
+    DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
 )
 
 
 def get_structure() -> CredentialsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/README.md` & `mypy-boto3-datasync-1.28.3.post2/README.md`

 * *Files 5% similar despite different names*

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
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,170 +359,170 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
     CredentialsTypeDef,
     DiscoveryServerConfigurationTypeDef,
     TagListEntryTypeDef,
-    AddStorageSystemResponseOutputTypeDef,
-    AgentListEntryOutputTypeDef,
+    AddStorageSystemResponseTypeDef,
+    AgentListEntryTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    CapacityOutputTypeDef,
-    CreateAgentResponseOutputTypeDef,
+    CapacityTypeDef,
+    CreateAgentResponseTypeDef,
     Ec2ConfigTypeDef,
-    CreateLocationEfsResponseOutputTypeDef,
-    CreateLocationFsxLustreResponseOutputTypeDef,
-    CreateLocationFsxOntapResponseOutputTypeDef,
-    CreateLocationFsxOpenZfsResponseOutputTypeDef,
-    CreateLocationFsxWindowsResponseOutputTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
-    CreateLocationHdfsResponseOutputTypeDef,
+    CreateLocationHdfsResponseTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
-    CreateLocationNfsResponseOutputTypeDef,
-    CreateLocationObjectStorageResponseOutputTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
     S3ConfigTypeDef,
-    CreateLocationS3ResponseOutputTypeDef,
+    CreateLocationS3ResponseTypeDef,
     SmbMountOptionsTypeDef,
-    CreateLocationSmbResponseOutputTypeDef,
+    CreateLocationSmbResponseTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
-    CreateTaskResponseOutputTypeDef,
+    CreateTaskResponseTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
-    PrivateLinkConfigOutputTypeDef,
+    PrivateLinkConfigTypeDef,
     DescribeDiscoveryJobRequestRequestTypeDef,
-    DescribeDiscoveryJobResponseOutputTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
     Ec2ConfigOutputTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
-    DescribeLocationFsxLustreResponseOutputTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
-    DescribeLocationFsxWindowsResponseOutputTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
     HdfsNameNodeOutputTypeDef,
     QopConfigurationOutputTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
     NfsMountOptionsOutputTypeDef,
     OnPremConfigOutputTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
-    DescribeLocationObjectStorageResponseOutputTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
     S3ConfigOutputTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
     SmbMountOptionsOutputTypeDef,
     DescribeStorageSystemRequestRequestTypeDef,
     DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     DescribeStorageSystemResourcesRequestRequestTypeDef,
     DiscoveryServerConfigurationOutputTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
     FilterRuleOutputTypeDef,
     OptionsOutputTypeDef,
-    TaskExecutionResultDetailOutputTypeDef,
+    TaskExecutionResultDetailTypeDef,
     DescribeTaskRequestRequestTypeDef,
     TaskScheduleOutputTypeDef,
-    DiscoveryJobListEntryOutputTypeDef,
+    DiscoveryJobListEntryTypeDef,
     GenerateRecommendationsRequestRequestTypeDef,
-    IOPSOutputTypeDef,
-    LatencyOutputTypeDef,
+    IOPSTypeDef,
+    LatencyTypeDef,
     ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
     ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
     ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
-    LocationListEntryOutputTypeDef,
+    LocationListEntryTypeDef,
     ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
     ListStorageSystemsRequestRequestTypeDef,
-    StorageSystemListEntryOutputTypeDef,
+    StorageSystemListEntryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagListEntryOutputTypeDef,
     ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
-    TaskExecutionListEntryOutputTypeDef,
+    TaskExecutionListEntryTypeDef,
     TaskFilterTypeDef,
-    TaskListEntryOutputTypeDef,
-    MaxP95PerformanceOutputTypeDef,
-    RecommendationOutputTypeDef,
-    ThroughputOutputTypeDef,
+    TaskListEntryTypeDef,
+    MaxP95PerformanceTypeDef,
+    RecommendationTypeDef,
+    ThroughputTypeDef,
     PaginatorConfigTypeDef,
     RemoveStorageSystemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    StartDiscoveryJobResponseOutputTypeDef,
-    StartTaskExecutionResponseOutputTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
     StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
     UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
     UpdateStorageSystemRequestRequestTypeDef,
     AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
     StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAgentsResponseOutputTypeDef,
+    ListAgentsResponseTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
     UpdateLocationNfsRequestRequestTypeDef,
     CreateLocationS3RequestRequestTypeDef,
     CreateLocationSmbRequestRequestTypeDef,
     FsxProtocolSmbTypeDef,
     UpdateLocationSmbRequestRequestTypeDef,
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
     UpdateTaskRequestRequestTypeDef,
-    DescribeAgentResponseOutputTypeDef,
-    DescribeLocationEfsResponseOutputTypeDef,
-    DescribeLocationHdfsResponseOutputTypeDef,
+    DescribeAgentResponseTypeDef,
+    DescribeLocationEfsResponseTypeDef,
+    DescribeLocationHdfsResponseTypeDef,
     FsxProtocolNfsOutputTypeDef,
-    DescribeLocationNfsResponseOutputTypeDef,
-    DescribeLocationS3ResponseOutputTypeDef,
-    DescribeLocationSmbResponseOutputTypeDef,
+    DescribeLocationNfsResponseTypeDef,
+    DescribeLocationS3ResponseTypeDef,
+    DescribeLocationSmbResponseTypeDef,
     FsxProtocolSmbOutputTypeDef,
-    DescribeStorageSystemResponseOutputTypeDef,
-    DescribeTaskExecutionResponseOutputTypeDef,
-    DescribeTaskResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    DescribeTaskExecutionResponseTypeDef,
+    DescribeTaskResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseOutputTypeDef,
-    NetAppONTAPClusterOutputTypeDef,
-    NetAppONTAPSVMOutputTypeDef,
-    NetAppONTAPVolumeOutputTypeDef,
-    P95MetricsOutputTypeDef,
+    ListTasksResponseTypeDef,
+    NetAppONTAPClusterTypeDef,
+    NetAppONTAPSVMTypeDef,
+    NetAppONTAPVolumeTypeDef,
+    P95MetricsTypeDef,
     FsxProtocolTypeDef,
     FsxProtocolOutputTypeDef,
-    ResourceDetailsOutputTypeDef,
-    ResourceMetricsOutputTypeDef,
+    ResourceDetailsTypeDef,
+    ResourceMetricsTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
-    DescribeLocationFsxOntapResponseOutputTypeDef,
-    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
-    DescribeStorageSystemResourcesResponseOutputTypeDef,
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    DescribeLocationFsxOntapResponseTypeDef,
+    DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
 )
 
 
 def get_structure() -> CredentialsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.py` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.pyi` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__main__.py` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataSync 1.28.3\nVersion:         1.28.3.post1\nBuilder"
-        " version: 7.14.7\nDocs:           "
+        "Type annotations for boto3.DataSync 1.28.3\nVersion:         1.28.3.post2\nBuilder"
+        " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
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

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.py` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,66 +34,66 @@
     ListLocationsPaginator,
     ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
-    AddStorageSystemResponseOutputTypeDef,
-    CreateAgentResponseOutputTypeDef,
-    CreateLocationEfsResponseOutputTypeDef,
-    CreateLocationFsxLustreResponseOutputTypeDef,
-    CreateLocationFsxOntapResponseOutputTypeDef,
-    CreateLocationFsxOpenZfsResponseOutputTypeDef,
-    CreateLocationFsxWindowsResponseOutputTypeDef,
-    CreateLocationHdfsResponseOutputTypeDef,
-    CreateLocationNfsResponseOutputTypeDef,
-    CreateLocationObjectStorageResponseOutputTypeDef,
-    CreateLocationS3ResponseOutputTypeDef,
-    CreateLocationSmbResponseOutputTypeDef,
-    CreateTaskResponseOutputTypeDef,
+    AddStorageSystemResponseTypeDef,
+    CreateAgentResponseTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
+    CreateLocationHdfsResponseTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
+    CreateLocationS3ResponseTypeDef,
+    CreateLocationSmbResponseTypeDef,
+    CreateTaskResponseTypeDef,
     CredentialsTypeDef,
-    DescribeAgentResponseOutputTypeDef,
-    DescribeDiscoveryJobResponseOutputTypeDef,
-    DescribeLocationEfsResponseOutputTypeDef,
-    DescribeLocationFsxLustreResponseOutputTypeDef,
-    DescribeLocationFsxOntapResponseOutputTypeDef,
-    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
-    DescribeLocationFsxWindowsResponseOutputTypeDef,
-    DescribeLocationHdfsResponseOutputTypeDef,
-    DescribeLocationNfsResponseOutputTypeDef,
-    DescribeLocationObjectStorageResponseOutputTypeDef,
-    DescribeLocationS3ResponseOutputTypeDef,
-    DescribeLocationSmbResponseOutputTypeDef,
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
-    DescribeStorageSystemResourcesResponseOutputTypeDef,
-    DescribeStorageSystemResponseOutputTypeDef,
-    DescribeTaskExecutionResponseOutputTypeDef,
-    DescribeTaskResponseOutputTypeDef,
+    DescribeAgentResponseTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
+    DescribeLocationEfsResponseTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
+    DescribeLocationFsxOntapResponseTypeDef,
+    DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
+    DescribeLocationHdfsResponseTypeDef,
+    DescribeLocationNfsResponseTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
+    DescribeLocationS3ResponseTypeDef,
+    DescribeLocationSmbResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    DescribeTaskExecutionResponseTypeDef,
+    DescribeTaskResponseTypeDef,
     DiscoveryServerConfigurationTypeDef,
     Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
-    ListAgentsResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
-    ListTasksResponseOutputTypeDef,
+    ListAgentsResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
+    ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
-    StartDiscoveryJobResponseOutputTypeDef,
-    StartTaskExecutionResponseOutputTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
     TaskFilterTypeDef,
     TaskScheduleTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -142,15 +142,15 @@
         SystemType: Literal["NetAppONTAP"],
         AgentArns: Sequence[str],
         ClientToken: str,
         Credentials: CredentialsTypeDef,
         CloudWatchLogGroupArn: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Name: str = ...
-    ) -> AddStorageSystemResponseOutputTypeDef:
+    ) -> AddStorageSystemResponseTypeDef:
         """
         Creates an Amazon Web Services resource for an on-premises storage system that
         you want DataSync Discovery to collect information about.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#add_storage_system)
         """
@@ -184,15 +184,15 @@
         *,
         ActivationKey: str,
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
-    ) -> CreateAgentResponseOutputTypeDef:
+    ) -> CreateAgentResponseTypeDef:
         """
         Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_agent)
         """
 
@@ -202,15 +202,15 @@
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...
-    ) -> CreateLocationEfsResponseOutputTypeDef:
+    ) -> CreateLocationEfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon EFS file system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_efs)
         """
@@ -218,15 +218,15 @@
     def create_location_fsx_lustre(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxLustreResponseOutputTypeDef:
+    ) -> CreateLocationFsxLustreResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_lustre)
         """
 
@@ -234,15 +234,15 @@
         self,
         *,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         StorageVirtualMachineArn: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOntapResponseOutputTypeDef:
+    ) -> CreateLocationFsxOntapResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_ontap)
         """
@@ -251,15 +251,15 @@
         self,
         *,
         FsxFilesystemArn: str,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOpenZfsResponseOutputTypeDef:
+    ) -> CreateLocationFsxOpenZfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can
         access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_open_zfs)
         """
@@ -270,15 +270,15 @@
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         User: str,
         Password: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Domain: str = ...
-    ) -> CreateLocationFsxWindowsResponseOutputTypeDef:
+    ) -> CreateLocationFsxWindowsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_windows)
         """
 
@@ -294,15 +294,15 @@
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: Union[str, bytes, IO[Any], StreamingBody] = ...,
         KerberosKrb5Conf: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationHdfsResponseOutputTypeDef:
+    ) -> CreateLocationHdfsResponseTypeDef:
         """
         Creates an endpoint for a Hadoop Distributed File System (HDFS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_hdfs)
         """
 
@@ -310,15 +310,15 @@
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationNfsResponseOutputTypeDef:
+    ) -> CreateLocationNfsResponseTypeDef:
         """
         Defines a file system on a Network File System (NFS) server that can be read
         from or written to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_nfs)
         """
@@ -332,15 +332,15 @@
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         ServerCertificate: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> CreateLocationObjectStorageResponseOutputTypeDef:
+    ) -> CreateLocationObjectStorageResponseTypeDef:
         """
         Creates an endpoint for an object storage system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_object_storage)
         """
@@ -350,15 +350,15 @@
         *,
         S3BucketArn: str,
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationS3ResponseOutputTypeDef:
+    ) -> CreateLocationS3ResponseTypeDef:
         """
         A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_s3)
         """
 
@@ -369,15 +369,15 @@
         ServerHostname: str,
         User: str,
         Password: str,
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationSmbResponseOutputTypeDef:
+    ) -> CreateLocationSmbResponseTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_smb)
         """
@@ -390,15 +390,15 @@
         CloudWatchLogGroupArn: str = ...,
         Name: str = ...,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...
-    ) -> CreateTaskResponseOutputTypeDef:
+    ) -> CreateTaskResponseTypeDef:
         """
         Configures a task, which defines where and how DataSync transfers your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_task)
         """
 
@@ -422,139 +422,131 @@
         """
         Deletes an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_task)
         """
 
-    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseOutputTypeDef:
+    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseTypeDef:
         """
         Returns metadata about an DataSync agent, such as its name, endpoint type, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_agent)
         """
 
     def describe_discovery_job(
         self, *, DiscoveryJobArn: str
-    ) -> DescribeDiscoveryJobResponseOutputTypeDef:
+    ) -> DescribeDiscoveryJobResponseTypeDef:
         """
         Returns information about a DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_discovery_job)
         """
 
-    def describe_location_efs(
-        self, *, LocationArn: str
-    ) -> DescribeLocationEfsResponseOutputTypeDef:
+    def describe_location_efs(self, *, LocationArn: str) -> DescribeLocationEfsResponseTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_efs)
         """
 
     def describe_location_fsx_lustre(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxLustreResponseOutputTypeDef:
+    ) -> DescribeLocationFsxLustreResponseTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for Lustre
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_lustre)
         """
 
     def describe_location_fsx_ontap(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOntapResponseOutputTypeDef:
+    ) -> DescribeLocationFsxOntapResponseTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for NetApp
         ONTAP file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_ontap)
         """
 
     def describe_location_fsx_open_zfs(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOpenZfsResponseOutputTypeDef:
+    ) -> DescribeLocationFsxOpenZfsResponseTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for OpenZFS
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_open_zfs)
         """
 
     def describe_location_fsx_windows(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxWindowsResponseOutputTypeDef:
+    ) -> DescribeLocationFsxWindowsResponseTypeDef:
         """
         Returns metadata about an Amazon FSx for Windows File Server location, such as
         information about its path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_windows)
         """
 
-    def describe_location_hdfs(
-        self, *, LocationArn: str
-    ) -> DescribeLocationHdfsResponseOutputTypeDef:
+    def describe_location_hdfs(self, *, LocationArn: str) -> DescribeLocationHdfsResponseTypeDef:
         """
         Returns metadata, such as the authentication information about the Hadoop
         Distributed File System (HDFS) location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_hdfs)
         """
 
-    def describe_location_nfs(
-        self, *, LocationArn: str
-    ) -> DescribeLocationNfsResponseOutputTypeDef:
+    def describe_location_nfs(self, *, LocationArn: str) -> DescribeLocationNfsResponseTypeDef:
         """
         Returns metadata, such as the path information, about an NFS location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_nfs)
         """
 
     def describe_location_object_storage(
         self, *, LocationArn: str
-    ) -> DescribeLocationObjectStorageResponseOutputTypeDef:
+    ) -> DescribeLocationObjectStorageResponseTypeDef:
         """
         Returns metadata about your DataSync location for an object storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_object_storage)
         """
 
-    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseOutputTypeDef:
+    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseTypeDef:
         """
         Returns metadata, such as bucket name, about an Amazon S3 bucket location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_s3)
         """
 
-    def describe_location_smb(
-        self, *, LocationArn: str
-    ) -> DescribeLocationSmbResponseOutputTypeDef:
+    def describe_location_smb(self, *, LocationArn: str) -> DescribeLocationSmbResponseTypeDef:
         """
         Returns metadata, such as the path and user information about an SMB location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_smb)
         """
 
     def describe_storage_system(
         self, *, StorageSystemArn: str
-    ) -> DescribeStorageSystemResponseOutputTypeDef:
+    ) -> DescribeStorageSystemResponseTypeDef:
         """
         Returns information about an on-premises storage system that you're using with
         DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system)
         """
@@ -565,15 +557,15 @@
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourceMetricsResponseOutputTypeDef:
+    ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
         """
         Returns information, including performance data and capacity usage, which
         DataSync Discovery collects about a specific resource in your-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resource_metrics)
@@ -584,34 +576,34 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceIds: Sequence[str] = ...,
         Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourcesResponseOutputTypeDef:
+    ) -> DescribeStorageSystemResourcesResponseTypeDef:
         """
         Returns information that DataSync Discovery collects about resources in your on-
         premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
         """
 
-    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseOutputTypeDef:
+    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
         Returns metadata about a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
 
     def describe_task_execution(
         self, *, TaskExecutionArn: str
-    ) -> DescribeTaskExecutionResponseOutputTypeDef:
+    ) -> DescribeTaskExecutionResponseTypeDef:
         """
         Returns detailed metadata about a task that is being executed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task_execution)
         """
 
@@ -642,85 +634,85 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_recommendations)
         """
 
     def list_agents(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAgentsResponseOutputTypeDef:
+    ) -> ListAgentsResponseTypeDef:
         """
         Returns a list of DataSync agents that belong to an Amazon Web Services account
         in the Amazon Web Services Region specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_agents)
         """
 
     def list_discovery_jobs(
         self, *, StorageSystemArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListDiscoveryJobsResponseOutputTypeDef:
+    ) -> ListDiscoveryJobsResponseTypeDef:
         """
         Provides a list of the existing discovery jobs in the Amazon Web Services Region
         and Amazon Web Services account where you're using DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_discovery_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_discovery_jobs)
         """
 
     def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[LocationFilterTypeDef] = ...
-    ) -> ListLocationsResponseOutputTypeDef:
+    ) -> ListLocationsResponseTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_locations)
         """
 
     def list_storage_systems(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListStorageSystemsResponseOutputTypeDef:
+    ) -> ListStorageSystemsResponseTypeDef:
         """
         Lists the on-premises storage systems that you're using with DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_storage_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_storage_systems)
         """
 
     def list_tags_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags associated with an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tags_for_resource)
         """
 
     def list_task_executions(
         self, *, TaskArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTaskExecutionsResponseOutputTypeDef:
+    ) -> ListTaskExecutionsResponseTypeDef:
         """
         Returns a list of executed tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_task_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_task_executions)
         """
 
     def list_tasks(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[TaskFilterTypeDef] = ...
-    ) -> ListTasksResponseOutputTypeDef:
+    ) -> ListTasksResponseTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tasks)
         """
 
@@ -736,15 +728,15 @@
     def start_discovery_job(
         self,
         *,
         StorageSystemArn: str,
         CollectionDurationMinutes: int,
         ClientToken: str,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartDiscoveryJobResponseOutputTypeDef:
+    ) -> StartDiscoveryJobResponseTypeDef:
         """
         Runs a DataSync discovery job on your on-premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_discovery_job)
         """
 
@@ -752,15 +744,15 @@
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartTaskExecutionResponseOutputTypeDef:
+    ) -> StartTaskExecutionResponseTypeDef:
         """
         Starts an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_task_execution)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.pyi` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -34,66 +34,66 @@
     ListLocationsPaginator,
     ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
-    AddStorageSystemResponseOutputTypeDef,
-    CreateAgentResponseOutputTypeDef,
-    CreateLocationEfsResponseOutputTypeDef,
-    CreateLocationFsxLustreResponseOutputTypeDef,
-    CreateLocationFsxOntapResponseOutputTypeDef,
-    CreateLocationFsxOpenZfsResponseOutputTypeDef,
-    CreateLocationFsxWindowsResponseOutputTypeDef,
-    CreateLocationHdfsResponseOutputTypeDef,
-    CreateLocationNfsResponseOutputTypeDef,
-    CreateLocationObjectStorageResponseOutputTypeDef,
-    CreateLocationS3ResponseOutputTypeDef,
-    CreateLocationSmbResponseOutputTypeDef,
-    CreateTaskResponseOutputTypeDef,
+    AddStorageSystemResponseTypeDef,
+    CreateAgentResponseTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
+    CreateLocationHdfsResponseTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
+    CreateLocationS3ResponseTypeDef,
+    CreateLocationSmbResponseTypeDef,
+    CreateTaskResponseTypeDef,
     CredentialsTypeDef,
-    DescribeAgentResponseOutputTypeDef,
-    DescribeDiscoveryJobResponseOutputTypeDef,
-    DescribeLocationEfsResponseOutputTypeDef,
-    DescribeLocationFsxLustreResponseOutputTypeDef,
-    DescribeLocationFsxOntapResponseOutputTypeDef,
-    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
-    DescribeLocationFsxWindowsResponseOutputTypeDef,
-    DescribeLocationHdfsResponseOutputTypeDef,
-    DescribeLocationNfsResponseOutputTypeDef,
-    DescribeLocationObjectStorageResponseOutputTypeDef,
-    DescribeLocationS3ResponseOutputTypeDef,
-    DescribeLocationSmbResponseOutputTypeDef,
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
-    DescribeStorageSystemResourcesResponseOutputTypeDef,
-    DescribeStorageSystemResponseOutputTypeDef,
-    DescribeTaskExecutionResponseOutputTypeDef,
-    DescribeTaskResponseOutputTypeDef,
+    DescribeAgentResponseTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
+    DescribeLocationEfsResponseTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
+    DescribeLocationFsxOntapResponseTypeDef,
+    DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
+    DescribeLocationHdfsResponseTypeDef,
+    DescribeLocationNfsResponseTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
+    DescribeLocationS3ResponseTypeDef,
+    DescribeLocationSmbResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    DescribeTaskExecutionResponseTypeDef,
+    DescribeTaskResponseTypeDef,
     DiscoveryServerConfigurationTypeDef,
     Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
-    ListAgentsResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
-    ListTasksResponseOutputTypeDef,
+    ListAgentsResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
+    ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
-    StartDiscoveryJobResponseOutputTypeDef,
-    StartTaskExecutionResponseOutputTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
     TaskFilterTypeDef,
     TaskScheduleTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -137,15 +137,15 @@
         SystemType: Literal["NetAppONTAP"],
         AgentArns: Sequence[str],
         ClientToken: str,
         Credentials: CredentialsTypeDef,
         CloudWatchLogGroupArn: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Name: str = ...
-    ) -> AddStorageSystemResponseOutputTypeDef:
+    ) -> AddStorageSystemResponseTypeDef:
         """
         Creates an Amazon Web Services resource for an on-premises storage system that
         you want DataSync Discovery to collect information about.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#add_storage_system)
         """
@@ -175,15 +175,15 @@
         *,
         ActivationKey: str,
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
-    ) -> CreateAgentResponseOutputTypeDef:
+    ) -> CreateAgentResponseTypeDef:
         """
         Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_agent)
         """
     def create_location_efs(
@@ -192,45 +192,45 @@
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...
-    ) -> CreateLocationEfsResponseOutputTypeDef:
+    ) -> CreateLocationEfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon EFS file system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_efs)
         """
     def create_location_fsx_lustre(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxLustreResponseOutputTypeDef:
+    ) -> CreateLocationFsxLustreResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_lustre)
         """
     def create_location_fsx_ontap(
         self,
         *,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         StorageVirtualMachineArn: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOntapResponseOutputTypeDef:
+    ) -> CreateLocationFsxOntapResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_ontap)
         """
@@ -238,15 +238,15 @@
         self,
         *,
         FsxFilesystemArn: str,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOpenZfsResponseOutputTypeDef:
+    ) -> CreateLocationFsxOpenZfsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can
         access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_open_zfs)
         """
@@ -256,15 +256,15 @@
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         User: str,
         Password: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Domain: str = ...
-    ) -> CreateLocationFsxWindowsResponseOutputTypeDef:
+    ) -> CreateLocationFsxWindowsResponseTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_windows)
         """
     def create_location_hdfs(
@@ -279,30 +279,30 @@
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: Union[str, bytes, IO[Any], StreamingBody] = ...,
         KerberosKrb5Conf: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationHdfsResponseOutputTypeDef:
+    ) -> CreateLocationHdfsResponseTypeDef:
         """
         Creates an endpoint for a Hadoop Distributed File System (HDFS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_hdfs)
         """
     def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationNfsResponseOutputTypeDef:
+    ) -> CreateLocationNfsResponseTypeDef:
         """
         Defines a file system on a Network File System (NFS) server that can be read
         from or written to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_nfs)
         """
@@ -315,15 +315,15 @@
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         ServerCertificate: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> CreateLocationObjectStorageResponseOutputTypeDef:
+    ) -> CreateLocationObjectStorageResponseTypeDef:
         """
         Creates an endpoint for an object storage system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_object_storage)
         """
@@ -332,15 +332,15 @@
         *,
         S3BucketArn: str,
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationS3ResponseOutputTypeDef:
+    ) -> CreateLocationS3ResponseTypeDef:
         """
         A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_s3)
         """
     def create_location_smb(
@@ -350,15 +350,15 @@
         ServerHostname: str,
         User: str,
         Password: str,
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationSmbResponseOutputTypeDef:
+    ) -> CreateLocationSmbResponseTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_smb)
         """
@@ -370,15 +370,15 @@
         CloudWatchLogGroupArn: str = ...,
         Name: str = ...,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...
-    ) -> CreateTaskResponseOutputTypeDef:
+    ) -> CreateTaskResponseTypeDef:
         """
         Configures a task, which defines where and how DataSync transfers your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_task)
         """
     def delete_agent(self, *, AgentArn: str) -> Dict[str, Any]:
@@ -398,127 +398,119 @@
     def delete_task(self, *, TaskArn: str) -> Dict[str, Any]:
         """
         Deletes an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_task)
         """
-    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseOutputTypeDef:
+    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseTypeDef:
         """
         Returns metadata about an DataSync agent, such as its name, endpoint type, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_agent)
         """
     def describe_discovery_job(
         self, *, DiscoveryJobArn: str
-    ) -> DescribeDiscoveryJobResponseOutputTypeDef:
+    ) -> DescribeDiscoveryJobResponseTypeDef:
         """
         Returns information about a DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_discovery_job)
         """
-    def describe_location_efs(
-        self, *, LocationArn: str
-    ) -> DescribeLocationEfsResponseOutputTypeDef:
+    def describe_location_efs(self, *, LocationArn: str) -> DescribeLocationEfsResponseTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_efs)
         """
     def describe_location_fsx_lustre(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxLustreResponseOutputTypeDef:
+    ) -> DescribeLocationFsxLustreResponseTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for Lustre
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_lustre)
         """
     def describe_location_fsx_ontap(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOntapResponseOutputTypeDef:
+    ) -> DescribeLocationFsxOntapResponseTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for NetApp
         ONTAP file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_ontap)
         """
     def describe_location_fsx_open_zfs(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOpenZfsResponseOutputTypeDef:
+    ) -> DescribeLocationFsxOpenZfsResponseTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for OpenZFS
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_open_zfs)
         """
     def describe_location_fsx_windows(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxWindowsResponseOutputTypeDef:
+    ) -> DescribeLocationFsxWindowsResponseTypeDef:
         """
         Returns metadata about an Amazon FSx for Windows File Server location, such as
         information about its path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_windows)
         """
-    def describe_location_hdfs(
-        self, *, LocationArn: str
-    ) -> DescribeLocationHdfsResponseOutputTypeDef:
+    def describe_location_hdfs(self, *, LocationArn: str) -> DescribeLocationHdfsResponseTypeDef:
         """
         Returns metadata, such as the authentication information about the Hadoop
         Distributed File System (HDFS) location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_hdfs)
         """
-    def describe_location_nfs(
-        self, *, LocationArn: str
-    ) -> DescribeLocationNfsResponseOutputTypeDef:
+    def describe_location_nfs(self, *, LocationArn: str) -> DescribeLocationNfsResponseTypeDef:
         """
         Returns metadata, such as the path information, about an NFS location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_nfs)
         """
     def describe_location_object_storage(
         self, *, LocationArn: str
-    ) -> DescribeLocationObjectStorageResponseOutputTypeDef:
+    ) -> DescribeLocationObjectStorageResponseTypeDef:
         """
         Returns metadata about your DataSync location for an object storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_object_storage)
         """
-    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseOutputTypeDef:
+    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseTypeDef:
         """
         Returns metadata, such as bucket name, about an Amazon S3 bucket location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_s3)
         """
-    def describe_location_smb(
-        self, *, LocationArn: str
-    ) -> DescribeLocationSmbResponseOutputTypeDef:
+    def describe_location_smb(self, *, LocationArn: str) -> DescribeLocationSmbResponseTypeDef:
         """
         Returns metadata, such as the path and user information about an SMB location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_smb)
         """
     def describe_storage_system(
         self, *, StorageSystemArn: str
-    ) -> DescribeStorageSystemResponseOutputTypeDef:
+    ) -> DescribeStorageSystemResponseTypeDef:
         """
         Returns information about an on-premises storage system that you're using with
         DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system)
         """
@@ -528,15 +520,15 @@
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourceMetricsResponseOutputTypeDef:
+    ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
         """
         Returns information, including performance data and capacity usage, which
         DataSync Discovery collects about a specific resource in your-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resource_metrics)
@@ -546,32 +538,32 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceIds: Sequence[str] = ...,
         Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourcesResponseOutputTypeDef:
+    ) -> DescribeStorageSystemResourcesResponseTypeDef:
         """
         Returns information that DataSync Discovery collects about resources in your on-
         premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
         """
-    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseOutputTypeDef:
+    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
         Returns metadata about a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
     def describe_task_execution(
         self, *, TaskExecutionArn: str
-    ) -> DescribeTaskExecutionResponseOutputTypeDef:
+    ) -> DescribeTaskExecutionResponseTypeDef:
         """
         Returns detailed metadata about a task that is being executed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task_execution)
         """
     def generate_presigned_url(
@@ -599,79 +591,79 @@
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_recommendations)
         """
     def list_agents(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAgentsResponseOutputTypeDef:
+    ) -> ListAgentsResponseTypeDef:
         """
         Returns a list of DataSync agents that belong to an Amazon Web Services account
         in the Amazon Web Services Region specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_agents)
         """
     def list_discovery_jobs(
         self, *, StorageSystemArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListDiscoveryJobsResponseOutputTypeDef:
+    ) -> ListDiscoveryJobsResponseTypeDef:
         """
         Provides a list of the existing discovery jobs in the Amazon Web Services Region
         and Amazon Web Services account where you're using DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_discovery_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_discovery_jobs)
         """
     def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[LocationFilterTypeDef] = ...
-    ) -> ListLocationsResponseOutputTypeDef:
+    ) -> ListLocationsResponseTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_locations)
         """
     def list_storage_systems(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListStorageSystemsResponseOutputTypeDef:
+    ) -> ListStorageSystemsResponseTypeDef:
         """
         Lists the on-premises storage systems that you're using with DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_storage_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_storage_systems)
         """
     def list_tags_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags associated with an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tags_for_resource)
         """
     def list_task_executions(
         self, *, TaskArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTaskExecutionsResponseOutputTypeDef:
+    ) -> ListTaskExecutionsResponseTypeDef:
         """
         Returns a list of executed tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_task_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_task_executions)
         """
     def list_tasks(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[TaskFilterTypeDef] = ...
-    ) -> ListTasksResponseOutputTypeDef:
+    ) -> ListTasksResponseTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tasks)
         """
     def remove_storage_system(self, *, StorageSystemArn: str) -> Dict[str, Any]:
@@ -685,30 +677,30 @@
     def start_discovery_job(
         self,
         *,
         StorageSystemArn: str,
         CollectionDurationMinutes: int,
         ClientToken: str,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartDiscoveryJobResponseOutputTypeDef:
+    ) -> StartDiscoveryJobResponseTypeDef:
         """
         Runs a DataSync discovery job on your on-premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_discovery_job)
         """
     def start_task_execution(
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartTaskExecutionResponseOutputTypeDef:
+    ) -> StartTaskExecutionResponseTypeDef:
         """
         Starts an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_task_execution)
         """
     def stop_discovery_job(self, *, DiscoveryJobArn: str) -> Dict[str, Any]:
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.py` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.pyi` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.py` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DiscoveryResourceTypeType
 from .type_defs import (
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
-    ListAgentsResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
-    ListTasksResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    ListAgentsResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
+    ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     PaginatorConfigTypeDef,
     TaskFilterTypeDef,
 )
 
 __all__ = (
     "DescribeStorageSystemResourceMetricsPaginator",
@@ -86,45 +86,45 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#describestoragesystemresourcemetricspaginator)
         """
 
 
 class ListAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
         """
 
 
 class ListDiscoveryJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
     """
 
     def paginate(
         self, *, StorageSystemArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDiscoveryJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDiscoveryJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
         """
 
 
 class ListLocationsPaginator(Paginator):
@@ -134,60 +134,60 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLocationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listlocationspaginator)
         """
 
 
 class ListStorageSystemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListStorageSystemsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListStorageSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTaskExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
     """
 
     def paginate(
         self, *, TaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskExecutionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTaskExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
         """
 
 
 class ListTasksPaginator(Paginator):
@@ -197,12 +197,12 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[TaskFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTasksResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.pyi` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DiscoveryResourceTypeType
 from .type_defs import (
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
-    ListAgentsResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
-    ListTasksResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    ListAgentsResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
+    ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     PaginatorConfigTypeDef,
     TaskFilterTypeDef,
 )
 
 __all__ = (
     "DescribeStorageSystemResourceMetricsPaginator",
@@ -83,43 +83,43 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#describestoragesystemresourcemetricspaginator)
         """
 
 class ListAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
         """
 
 class ListDiscoveryJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
     """
 
     def paginate(
         self, *, StorageSystemArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDiscoveryJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDiscoveryJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
         """
 
 class ListLocationsPaginator(Paginator):
     """
@@ -128,57 +128,57 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLocationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listlocationspaginator)
         """
 
 class ListStorageSystemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListStorageSystemsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListStorageSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTaskExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
     """
 
     def paginate(
         self, *, TaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskExecutionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTaskExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
         """
 
 class ListTasksPaginator(Paginator):
     """
@@ -187,12 +187,12 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[TaskFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTasksResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.py` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,170 +64,170 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
-    "AddStorageSystemResponseOutputTypeDef",
-    "AgentListEntryOutputTypeDef",
+    "AddStorageSystemResponseTypeDef",
+    "AgentListEntryTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
-    "CapacityOutputTypeDef",
-    "CreateAgentResponseOutputTypeDef",
+    "CapacityTypeDef",
+    "CreateAgentResponseTypeDef",
     "Ec2ConfigTypeDef",
-    "CreateLocationEfsResponseOutputTypeDef",
-    "CreateLocationFsxLustreResponseOutputTypeDef",
-    "CreateLocationFsxOntapResponseOutputTypeDef",
-    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
-    "CreateLocationFsxWindowsResponseOutputTypeDef",
+    "CreateLocationEfsResponseTypeDef",
+    "CreateLocationFsxLustreResponseTypeDef",
+    "CreateLocationFsxOntapResponseTypeDef",
+    "CreateLocationFsxOpenZfsResponseTypeDef",
+    "CreateLocationFsxWindowsResponseTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
-    "CreateLocationHdfsResponseOutputTypeDef",
+    "CreateLocationHdfsResponseTypeDef",
     "NfsMountOptionsTypeDef",
     "OnPremConfigTypeDef",
-    "CreateLocationNfsResponseOutputTypeDef",
-    "CreateLocationObjectStorageResponseOutputTypeDef",
+    "CreateLocationNfsResponseTypeDef",
+    "CreateLocationObjectStorageResponseTypeDef",
     "S3ConfigTypeDef",
-    "CreateLocationS3ResponseOutputTypeDef",
+    "CreateLocationS3ResponseTypeDef",
     "SmbMountOptionsTypeDef",
-    "CreateLocationSmbResponseOutputTypeDef",
+    "CreateLocationSmbResponseTypeDef",
     "FilterRuleTypeDef",
     "OptionsTypeDef",
     "TaskScheduleTypeDef",
-    "CreateTaskResponseOutputTypeDef",
+    "CreateTaskResponseTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
-    "PrivateLinkConfigOutputTypeDef",
+    "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
-    "DescribeDiscoveryJobResponseOutputTypeDef",
+    "DescribeDiscoveryJobResponseTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
     "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
-    "DescribeLocationFsxLustreResponseOutputTypeDef",
+    "DescribeLocationFsxLustreResponseTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
-    "DescribeLocationFsxWindowsResponseOutputTypeDef",
+    "DescribeLocationFsxWindowsResponseTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "HdfsNameNodeOutputTypeDef",
     "QopConfigurationOutputTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
     "NfsMountOptionsOutputTypeDef",
     "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
-    "DescribeLocationObjectStorageResponseOutputTypeDef",
+    "DescribeLocationObjectStorageResponseTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "S3ConfigOutputTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
     "SmbMountOptionsOutputTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
     "DiscoveryServerConfigurationOutputTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
     "FilterRuleOutputTypeDef",
     "OptionsOutputTypeDef",
-    "TaskExecutionResultDetailOutputTypeDef",
+    "TaskExecutionResultDetailTypeDef",
     "DescribeTaskRequestRequestTypeDef",
     "TaskScheduleOutputTypeDef",
-    "DiscoveryJobListEntryOutputTypeDef",
+    "DiscoveryJobListEntryTypeDef",
     "GenerateRecommendationsRequestRequestTypeDef",
-    "IOPSOutputTypeDef",
-    "LatencyOutputTypeDef",
+    "IOPSTypeDef",
+    "LatencyTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
-    "LocationListEntryOutputTypeDef",
+    "LocationListEntryTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListStorageSystemsRequestRequestTypeDef",
-    "StorageSystemListEntryOutputTypeDef",
+    "StorageSystemListEntryTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagListEntryOutputTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "ListTaskExecutionsRequestRequestTypeDef",
-    "TaskExecutionListEntryOutputTypeDef",
+    "TaskExecutionListEntryTypeDef",
     "TaskFilterTypeDef",
-    "TaskListEntryOutputTypeDef",
-    "MaxP95PerformanceOutputTypeDef",
-    "RecommendationOutputTypeDef",
-    "ThroughputOutputTypeDef",
+    "TaskListEntryTypeDef",
+    "MaxP95PerformanceTypeDef",
+    "RecommendationTypeDef",
+    "ThroughputTypeDef",
     "PaginatorConfigTypeDef",
     "RemoveStorageSystemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "StartDiscoveryJobResponseOutputTypeDef",
-    "StartTaskExecutionResponseOutputTypeDef",
+    "StartDiscoveryJobResponseTypeDef",
+    "StartTaskExecutionResponseTypeDef",
     "StopDiscoveryJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentRequestRequestTypeDef",
     "UpdateDiscoveryJobRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "UpdateStorageSystemRequestRequestTypeDef",
     "AddStorageSystemRequestRequestTypeDef",
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAgentsResponseOutputTypeDef",
+    "ListAgentsResponseTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
     "UpdateTaskRequestRequestTypeDef",
-    "DescribeAgentResponseOutputTypeDef",
-    "DescribeLocationEfsResponseOutputTypeDef",
-    "DescribeLocationHdfsResponseOutputTypeDef",
+    "DescribeAgentResponseTypeDef",
+    "DescribeLocationEfsResponseTypeDef",
+    "DescribeLocationHdfsResponseTypeDef",
     "FsxProtocolNfsOutputTypeDef",
-    "DescribeLocationNfsResponseOutputTypeDef",
-    "DescribeLocationS3ResponseOutputTypeDef",
-    "DescribeLocationSmbResponseOutputTypeDef",
+    "DescribeLocationNfsResponseTypeDef",
+    "DescribeLocationS3ResponseTypeDef",
+    "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbOutputTypeDef",
-    "DescribeStorageSystemResponseOutputTypeDef",
-    "DescribeTaskExecutionResponseOutputTypeDef",
-    "DescribeTaskResponseOutputTypeDef",
-    "ListDiscoveryJobsResponseOutputTypeDef",
+    "DescribeStorageSystemResponseTypeDef",
+    "DescribeTaskExecutionResponseTypeDef",
+    "DescribeTaskResponseTypeDef",
+    "ListDiscoveryJobsResponseTypeDef",
     "ListLocationsRequestListLocationsPaginateTypeDef",
     "ListLocationsRequestRequestTypeDef",
-    "ListLocationsResponseOutputTypeDef",
-    "ListStorageSystemsResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
-    "ListTaskExecutionsResponseOutputTypeDef",
+    "ListLocationsResponseTypeDef",
+    "ListStorageSystemsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTaskExecutionsResponseTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseOutputTypeDef",
-    "NetAppONTAPClusterOutputTypeDef",
-    "NetAppONTAPSVMOutputTypeDef",
-    "NetAppONTAPVolumeOutputTypeDef",
-    "P95MetricsOutputTypeDef",
+    "ListTasksResponseTypeDef",
+    "NetAppONTAPClusterTypeDef",
+    "NetAppONTAPSVMTypeDef",
+    "NetAppONTAPVolumeTypeDef",
+    "P95MetricsTypeDef",
     "FsxProtocolTypeDef",
     "FsxProtocolOutputTypeDef",
-    "ResourceDetailsOutputTypeDef",
-    "ResourceMetricsOutputTypeDef",
+    "ResourceDetailsTypeDef",
+    "ResourceMetricsTypeDef",
     "CreateLocationFsxOntapRequestRequestTypeDef",
     "CreateLocationFsxOpenZfsRequestRequestTypeDef",
-    "DescribeLocationFsxOntapResponseOutputTypeDef",
-    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
-    "DescribeStorageSystemResourcesResponseOutputTypeDef",
-    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
+    "DescribeLocationFsxOntapResponseTypeDef",
+    "DescribeLocationFsxOpenZfsResponseTypeDef",
+    "DescribeStorageSystemResourcesResponseTypeDef",
+    "DescribeStorageSystemResourceMetricsResponseTypeDef",
 )
 
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
@@ -270,97 +270,97 @@
 )
 
 
 class TagListEntryTypeDef(_RequiredTagListEntryTypeDef, _OptionalTagListEntryTypeDef):
     pass
 
 
-AddStorageSystemResponseOutputTypeDef = TypedDict(
-    "AddStorageSystemResponseOutputTypeDef",
+AddStorageSystemResponseTypeDef = TypedDict(
+    "AddStorageSystemResponseTypeDef",
     {
         "StorageSystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentListEntryOutputTypeDef = TypedDict(
-    "AgentListEntryOutputTypeDef",
+AgentListEntryTypeDef = TypedDict(
+    "AgentListEntryTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
 )
 
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
-CapacityOutputTypeDef = TypedDict(
-    "CapacityOutputTypeDef",
+CapacityTypeDef = TypedDict(
+    "CapacityTypeDef",
     {
         "Used": int,
         "Provisioned": int,
         "LogicalUsed": int,
     },
 )
 
-CreateAgentResponseOutputTypeDef = TypedDict(
-    "CreateAgentResponseOutputTypeDef",
+CreateAgentResponseTypeDef = TypedDict(
+    "CreateAgentResponseTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2ConfigTypeDef = TypedDict(
     "Ec2ConfigTypeDef",
     {
         "SubnetArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
 
-CreateLocationEfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationEfsResponseOutputTypeDef",
+CreateLocationEfsResponseTypeDef = TypedDict(
+    "CreateLocationEfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxLustreResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxLustreResponseOutputTypeDef",
+CreateLocationFsxLustreResponseTypeDef = TypedDict(
+    "CreateLocationFsxLustreResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOntapResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxOntapResponseOutputTypeDef",
+CreateLocationFsxOntapResponseTypeDef = TypedDict(
+    "CreateLocationFsxOntapResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
+CreateLocationFsxOpenZfsResponseTypeDef = TypedDict(
+    "CreateLocationFsxOpenZfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxWindowsResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxWindowsResponseOutputTypeDef",
+CreateLocationFsxWindowsResponseTypeDef = TypedDict(
+    "CreateLocationFsxWindowsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HdfsNameNodeTypeDef = TypedDict(
@@ -376,16 +376,16 @@
     {
         "RpcProtection": HdfsRpcProtectionType,
         "DataTransferProtection": HdfsDataTransferProtectionType,
     },
     total=False,
 )
 
-CreateLocationHdfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationHdfsResponseOutputTypeDef",
+CreateLocationHdfsResponseTypeDef = TypedDict(
+    "CreateLocationHdfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NfsMountOptionsTypeDef = TypedDict(
@@ -399,55 +399,55 @@
 OnPremConfigTypeDef = TypedDict(
     "OnPremConfigTypeDef",
     {
         "AgentArns": Sequence[str],
     },
 )
 
-CreateLocationNfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationNfsResponseOutputTypeDef",
+CreateLocationNfsResponseTypeDef = TypedDict(
+    "CreateLocationNfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationObjectStorageResponseOutputTypeDef = TypedDict(
-    "CreateLocationObjectStorageResponseOutputTypeDef",
+CreateLocationObjectStorageResponseTypeDef = TypedDict(
+    "CreateLocationObjectStorageResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketAccessRoleArn": str,
     },
 )
 
-CreateLocationS3ResponseOutputTypeDef = TypedDict(
-    "CreateLocationS3ResponseOutputTypeDef",
+CreateLocationS3ResponseTypeDef = TypedDict(
+    "CreateLocationS3ResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SmbMountOptionsTypeDef = TypedDict(
     "SmbMountOptionsTypeDef",
     {
         "Version": SmbVersionType,
     },
     total=False,
 )
 
-CreateLocationSmbResponseOutputTypeDef = TypedDict(
-    "CreateLocationSmbResponseOutputTypeDef",
+CreateLocationSmbResponseTypeDef = TypedDict(
+    "CreateLocationSmbResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterRuleTypeDef = TypedDict(
@@ -484,16 +484,16 @@
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
-CreateTaskResponseOutputTypeDef = TypedDict(
-    "CreateTaskResponseOutputTypeDef",
+CreateTaskResponseTypeDef = TypedDict(
+    "CreateTaskResponseTypeDef",
     {
         "TaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAgentRequestRequestTypeDef = TypedDict(
@@ -520,16 +520,16 @@
 DescribeAgentRequestRequestTypeDef = TypedDict(
     "DescribeAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
 )
 
-PrivateLinkConfigOutputTypeDef = TypedDict(
-    "PrivateLinkConfigOutputTypeDef",
+PrivateLinkConfigTypeDef = TypedDict(
+    "PrivateLinkConfigTypeDef",
     {
         "VpcEndpointId": str,
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
 )
@@ -537,16 +537,16 @@
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
 )
 
-DescribeDiscoveryJobResponseOutputTypeDef = TypedDict(
-    "DescribeDiscoveryJobResponseOutputTypeDef",
+DescribeDiscoveryJobResponseTypeDef = TypedDict(
+    "DescribeDiscoveryJobResponseTypeDef",
     {
         "StorageSystemArn": str,
         "DiscoveryJobArn": str,
         "CollectionDurationMinutes": int,
         "Status": DiscoveryJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
@@ -572,16 +572,16 @@
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxLustreResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxLustreResponseOutputTypeDef",
+DescribeLocationFsxLustreResponseTypeDef = TypedDict(
+    "DescribeLocationFsxLustreResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -604,16 +604,16 @@
 DescribeLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxWindowsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxWindowsResponseOutputTypeDef",
+DescribeLocationFsxWindowsResponseTypeDef = TypedDict(
+    "DescribeLocationFsxWindowsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "User": str,
         "Domain": str,
@@ -668,16 +668,16 @@
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationObjectStorageResponseOutputTypeDef = TypedDict(
-    "DescribeLocationObjectStorageResponseOutputTypeDef",
+DescribeLocationObjectStorageResponseTypeDef = TypedDict(
+    "DescribeLocationObjectStorageResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "AccessKey": str,
         "ServerPort": int,
         "ServerProtocol": ObjectStorageServerProtocolType,
         "AgentArns": List[str],
@@ -841,16 +841,16 @@
         "LogLevel": LogLevelType,
         "TransferMode": TransferModeType,
         "SecurityDescriptorCopyFlags": SmbSecurityDescriptorCopyFlagsType,
         "ObjectTags": ObjectTagsType,
     },
 )
 
-TaskExecutionResultDetailOutputTypeDef = TypedDict(
-    "TaskExecutionResultDetailOutputTypeDef",
+TaskExecutionResultDetailTypeDef = TypedDict(
+    "TaskExecutionResultDetailTypeDef",
     {
         "PrepareDuration": int,
         "PrepareStatus": PhaseStatusType,
         "TotalDuration": int,
         "TransferDuration": int,
         "TransferStatus": PhaseStatusType,
         "VerifyDuration": int,
@@ -870,16 +870,16 @@
 TaskScheduleOutputTypeDef = TypedDict(
     "TaskScheduleOutputTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
-DiscoveryJobListEntryOutputTypeDef = TypedDict(
-    "DiscoveryJobListEntryOutputTypeDef",
+DiscoveryJobListEntryTypeDef = TypedDict(
+    "DiscoveryJobListEntryTypeDef",
     {
         "DiscoveryJobArn": str,
         "Status": DiscoveryJobStatusType,
     },
 )
 
 GenerateRecommendationsRequestRequestTypeDef = TypedDict(
@@ -887,26 +887,26 @@
     {
         "DiscoveryJobArn": str,
         "ResourceIds": Sequence[str],
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
-IOPSOutputTypeDef = TypedDict(
-    "IOPSOutputTypeDef",
+IOPSTypeDef = TypedDict(
+    "IOPSTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
 
-LatencyOutputTypeDef = TypedDict(
-    "LatencyOutputTypeDef",
+LatencyTypeDef = TypedDict(
+    "LatencyTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
     },
 )
 
@@ -951,16 +951,16 @@
     {
         "Name": LocationFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-LocationListEntryOutputTypeDef = TypedDict(
-    "LocationListEntryOutputTypeDef",
+LocationListEntryTypeDef = TypedDict(
+    "LocationListEntryTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
     },
 )
 
 ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
@@ -976,16 +976,16 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-StorageSystemListEntryOutputTypeDef = TypedDict(
-    "StorageSystemListEntryOutputTypeDef",
+StorageSystemListEntryTypeDef = TypedDict(
+    "StorageSystemListEntryTypeDef",
     {
         "StorageSystemArn": str,
         "Name": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
@@ -1056,16 +1056,16 @@
         "TaskArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-TaskExecutionListEntryOutputTypeDef = TypedDict(
-    "TaskExecutionListEntryOutputTypeDef",
+TaskExecutionListEntryTypeDef = TypedDict(
+    "TaskExecutionListEntryTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
     },
 )
 
 TaskFilterTypeDef = TypedDict(
@@ -1073,25 +1073,25 @@
     {
         "Name": TaskFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-TaskListEntryOutputTypeDef = TypedDict(
-    "TaskListEntryOutputTypeDef",
+TaskListEntryTypeDef = TypedDict(
+    "TaskListEntryTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
 )
 
-MaxP95PerformanceOutputTypeDef = TypedDict(
-    "MaxP95PerformanceOutputTypeDef",
+MaxP95PerformanceTypeDef = TypedDict(
+    "MaxP95PerformanceTypeDef",
     {
         "IopsRead": float,
         "IopsWrite": float,
         "IopsOther": float,
         "IopsTotal": float,
         "ThroughputRead": float,
         "ThroughputWrite": float,
@@ -1099,25 +1099,25 @@
         "ThroughputTotal": float,
         "LatencyRead": float,
         "LatencyWrite": float,
         "LatencyOther": float,
     },
 )
 
-RecommendationOutputTypeDef = TypedDict(
-    "RecommendationOutputTypeDef",
+RecommendationTypeDef = TypedDict(
+    "RecommendationTypeDef",
     {
         "StorageType": str,
         "StorageConfiguration": Dict[str, str],
         "EstimatedMonthlyStorageCost": str,
     },
 )
 
-ThroughputOutputTypeDef = TypedDict(
-    "ThroughputOutputTypeDef",
+ThroughputTypeDef = TypedDict(
+    "ThroughputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
@@ -1146,24 +1146,24 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StartDiscoveryJobResponseOutputTypeDef = TypedDict(
-    "StartDiscoveryJobResponseOutputTypeDef",
+StartDiscoveryJobResponseTypeDef = TypedDict(
+    "StartDiscoveryJobResponseTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTaskExecutionResponseOutputTypeDef = TypedDict(
-    "StartTaskExecutionResponseOutputTypeDef",
+StartTaskExecutionResponseTypeDef = TypedDict(
+    "StartTaskExecutionResponseTypeDef",
     {
         "TaskExecutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopDiscoveryJobRequestRequestTypeDef = TypedDict(
@@ -1424,18 +1424,18 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
 )
 
-ListAgentsResponseOutputTypeDef = TypedDict(
-    "ListAgentsResponseOutputTypeDef",
+ListAgentsResponseTypeDef = TypedDict(
+    "ListAgentsResponseTypeDef",
     {
-        "Agents": List[AgentListEntryOutputTypeDef],
+        "Agents": List[AgentListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationEfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationEfsRequestRequestTypeDef",
@@ -1766,44 +1766,44 @@
 
 class UpdateTaskRequestRequestTypeDef(
     _RequiredUpdateTaskRequestRequestTypeDef, _OptionalUpdateTaskRequestRequestTypeDef
 ):
     pass
 
 
-DescribeAgentResponseOutputTypeDef = TypedDict(
-    "DescribeAgentResponseOutputTypeDef",
+DescribeAgentResponseTypeDef = TypedDict(
+    "DescribeAgentResponseTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
         "LastConnectionTime": datetime,
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
-        "PrivateLinkConfig": PrivateLinkConfigOutputTypeDef,
+        "PrivateLinkConfig": PrivateLinkConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationEfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationEfsResponseOutputTypeDef",
+DescribeLocationEfsResponseTypeDef = TypedDict(
+    "DescribeLocationEfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "Ec2Config": Ec2ConfigOutputTypeDef,
         "CreationTime": datetime,
         "AccessPointArn": str,
         "FileSystemAccessRoleArn": str,
         "InTransitEncryption": EfsInTransitEncryptionType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationHdfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationHdfsResponseOutputTypeDef",
+DescribeLocationHdfsResponseTypeDef = TypedDict(
+    "DescribeLocationHdfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "NameNodes": List[HdfsNameNodeOutputTypeDef],
         "BlockSize": int,
         "ReplicationFactor": int,
         "KmsKeyProviderUri": str,
@@ -1820,41 +1820,41 @@
 FsxProtocolNfsOutputTypeDef = TypedDict(
     "FsxProtocolNfsOutputTypeDef",
     {
         "MountOptions": NfsMountOptionsOutputTypeDef,
     },
 )
 
-DescribeLocationNfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationNfsResponseOutputTypeDef",
+DescribeLocationNfsResponseTypeDef = TypedDict(
+    "DescribeLocationNfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "OnPremConfig": OnPremConfigOutputTypeDef,
         "MountOptions": NfsMountOptionsOutputTypeDef,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationS3ResponseOutputTypeDef = TypedDict(
-    "DescribeLocationS3ResponseOutputTypeDef",
+DescribeLocationS3ResponseTypeDef = TypedDict(
+    "DescribeLocationS3ResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "S3StorageClass": S3StorageClassType,
         "S3Config": S3ConfigOutputTypeDef,
         "AgentArns": List[str],
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationSmbResponseOutputTypeDef = TypedDict(
-    "DescribeLocationSmbResponseOutputTypeDef",
+DescribeLocationSmbResponseTypeDef = TypedDict(
+    "DescribeLocationSmbResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "AgentArns": List[str],
         "User": str,
         "Domain": str,
         "MountOptions": SmbMountOptionsOutputTypeDef,
@@ -1869,16 +1869,16 @@
         "Domain": str,
         "MountOptions": SmbMountOptionsOutputTypeDef,
         "Password": str,
         "User": str,
     },
 )
 
-DescribeStorageSystemResponseOutputTypeDef = TypedDict(
-    "DescribeStorageSystemResponseOutputTypeDef",
+DescribeStorageSystemResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResponseTypeDef",
     {
         "StorageSystemArn": str,
         "ServerConfiguration": DiscoveryServerConfigurationOutputTypeDef,
         "SystemType": Literal["NetAppONTAP"],
         "AgentArns": List[str],
         "Name": str,
         "ErrorMessage": str,
@@ -1886,36 +1886,36 @@
         "CloudWatchLogGroupArn": str,
         "CreationTime": datetime,
         "SecretsManagerArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTaskExecutionResponseOutputTypeDef = TypedDict(
-    "DescribeTaskExecutionResponseOutputTypeDef",
+DescribeTaskExecutionResponseTypeDef = TypedDict(
+    "DescribeTaskExecutionResponseTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
         "Options": OptionsOutputTypeDef,
         "Excludes": List[FilterRuleOutputTypeDef],
         "Includes": List[FilterRuleOutputTypeDef],
         "StartTime": datetime,
         "EstimatedFilesToTransfer": int,
         "EstimatedBytesToTransfer": int,
         "FilesTransferred": int,
         "BytesWritten": int,
         "BytesTransferred": int,
-        "Result": TaskExecutionResultDetailOutputTypeDef,
+        "Result": TaskExecutionResultDetailTypeDef,
         "BytesCompressed": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTaskResponseOutputTypeDef = TypedDict(
-    "DescribeTaskResponseOutputTypeDef",
+DescribeTaskResponseTypeDef = TypedDict(
+    "DescribeTaskResponseTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
         "CurrentTaskExecutionArn": str,
         "SourceLocationArn": str,
         "DestinationLocationArn": str,
@@ -1929,18 +1929,18 @@
         "ErrorDetail": str,
         "CreationTime": datetime,
         "Includes": List[FilterRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDiscoveryJobsResponseOutputTypeDef = TypedDict(
-    "ListDiscoveryJobsResponseOutputTypeDef",
+ListDiscoveryJobsResponseTypeDef = TypedDict(
+    "ListDiscoveryJobsResponseTypeDef",
     {
-        "DiscoveryJobs": List[DiscoveryJobListEntryOutputTypeDef],
+        "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
@@ -1957,45 +1957,45 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[LocationFilterTypeDef],
     },
     total=False,
 )
 
-ListLocationsResponseOutputTypeDef = TypedDict(
-    "ListLocationsResponseOutputTypeDef",
+ListLocationsResponseTypeDef = TypedDict(
+    "ListLocationsResponseTypeDef",
     {
-        "Locations": List[LocationListEntryOutputTypeDef],
+        "Locations": List[LocationListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListStorageSystemsResponseOutputTypeDef = TypedDict(
-    "ListStorageSystemsResponseOutputTypeDef",
+ListStorageSystemsResponseTypeDef = TypedDict(
+    "ListStorageSystemsResponseTypeDef",
     {
-        "StorageSystems": List[StorageSystemListEntryOutputTypeDef],
+        "StorageSystems": List[StorageSystemListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTaskExecutionsResponseOutputTypeDef = TypedDict(
-    "ListTaskExecutionsResponseOutputTypeDef",
+ListTaskExecutionsResponseTypeDef = TypedDict(
+    "ListTaskExecutionsResponseTypeDef",
     {
-        "TaskExecutions": List[TaskExecutionListEntryOutputTypeDef],
+        "TaskExecutions": List[TaskExecutionListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
@@ -2012,87 +2012,87 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[TaskFilterTypeDef],
     },
     total=False,
 )
 
-ListTasksResponseOutputTypeDef = TypedDict(
-    "ListTasksResponseOutputTypeDef",
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
     {
-        "Tasks": List[TaskListEntryOutputTypeDef],
+        "Tasks": List[TaskListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NetAppONTAPClusterOutputTypeDef = TypedDict(
-    "NetAppONTAPClusterOutputTypeDef",
+NetAppONTAPClusterTypeDef = TypedDict(
+    "NetAppONTAPClusterTypeDef",
     {
         "CifsShareCount": int,
         "NfsExportedVolumes": int,
         "ResourceId": str,
         "ClusterName": str,
-        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-NetAppONTAPSVMOutputTypeDef = TypedDict(
-    "NetAppONTAPSVMOutputTypeDef",
+NetAppONTAPSVMTypeDef = TypedDict(
+    "NetAppONTAPSVMTypeDef",
     {
         "ClusterUuid": str,
         "ResourceId": str,
         "SvmName": str,
         "CifsShareCount": int,
         "EnabledProtocols": List[str],
         "TotalCapacityUsed": int,
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "Recommendations": List[RecommendationTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
         "LunCount": int,
     },
 )
 
-NetAppONTAPVolumeOutputTypeDef = TypedDict(
-    "NetAppONTAPVolumeOutputTypeDef",
+NetAppONTAPVolumeTypeDef = TypedDict(
+    "NetAppONTAPVolumeTypeDef",
     {
         "VolumeName": str,
         "ResourceId": str,
         "CifsShareCount": int,
         "SecurityStyle": str,
         "SvmUuid": str,
         "SvmName": str,
         "CapacityUsed": int,
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-P95MetricsOutputTypeDef = TypedDict(
-    "P95MetricsOutputTypeDef",
+P95MetricsTypeDef = TypedDict(
+    "P95MetricsTypeDef",
     {
-        "IOPS": IOPSOutputTypeDef,
-        "Throughput": ThroughputOutputTypeDef,
-        "Latency": LatencyOutputTypeDef,
+        "IOPS": IOPSTypeDef,
+        "Throughput": ThroughputTypeDef,
+        "Latency": LatencyTypeDef,
     },
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
@@ -2105,29 +2105,29 @@
     "FsxProtocolOutputTypeDef",
     {
         "NFS": FsxProtocolNfsOutputTypeDef,
         "SMB": FsxProtocolSmbOutputTypeDef,
     },
 )
 
-ResourceDetailsOutputTypeDef = TypedDict(
-    "ResourceDetailsOutputTypeDef",
+ResourceDetailsTypeDef = TypedDict(
+    "ResourceDetailsTypeDef",
     {
-        "NetAppONTAPSVMs": List[NetAppONTAPSVMOutputTypeDef],
-        "NetAppONTAPVolumes": List[NetAppONTAPVolumeOutputTypeDef],
-        "NetAppONTAPClusters": List[NetAppONTAPClusterOutputTypeDef],
+        "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
+        "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
+        "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
     },
 )
 
-ResourceMetricsOutputTypeDef = TypedDict(
-    "ResourceMetricsOutputTypeDef",
+ResourceMetricsTypeDef = TypedDict(
+    "ResourceMetricsTypeDef",
     {
         "Timestamp": datetime,
-        "P95Metrics": P95MetricsOutputTypeDef,
-        "Capacity": CapacityOutputTypeDef,
+        "P95Metrics": P95MetricsTypeDef,
+        "Capacity": CapacityTypeDef,
         "ResourceId": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
@@ -2175,50 +2175,50 @@
 class CreateLocationFsxOpenZfsRequestRequestTypeDef(
     _RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef,
     _OptionalCreateLocationFsxOpenZfsRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeLocationFsxOntapResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxOntapResponseOutputTypeDef",
+DescribeLocationFsxOntapResponseTypeDef = TypedDict(
+    "DescribeLocationFsxOntapResponseTypeDef",
     {
         "CreationTime": datetime,
         "LocationArn": str,
         "LocationUri": str,
         "Protocol": FsxProtocolOutputTypeDef,
         "SecurityGroupArns": List[str],
         "StorageVirtualMachineArn": str,
         "FsxFilesystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
+DescribeLocationFsxOpenZfsResponseTypeDef = TypedDict(
+    "DescribeLocationFsxOpenZfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "Protocol": FsxProtocolOutputTypeDef,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourcesResponseOutputTypeDef = TypedDict(
-    "DescribeStorageSystemResourcesResponseOutputTypeDef",
+DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResourcesResponseTypeDef",
     {
-        "ResourceDetails": ResourceDetailsOutputTypeDef,
+        "ResourceDetails": ResourceDetailsTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourceMetricsResponseOutputTypeDef = TypedDict(
-    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
+DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResourceMetricsResponseTypeDef",
     {
-        "Metrics": List[ResourceMetricsOutputTypeDef],
+        "Metrics": List[ResourceMetricsTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.pyi` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -63,170 +63,170 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
-    "AddStorageSystemResponseOutputTypeDef",
-    "AgentListEntryOutputTypeDef",
+    "AddStorageSystemResponseTypeDef",
+    "AgentListEntryTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
-    "CapacityOutputTypeDef",
-    "CreateAgentResponseOutputTypeDef",
+    "CapacityTypeDef",
+    "CreateAgentResponseTypeDef",
     "Ec2ConfigTypeDef",
-    "CreateLocationEfsResponseOutputTypeDef",
-    "CreateLocationFsxLustreResponseOutputTypeDef",
-    "CreateLocationFsxOntapResponseOutputTypeDef",
-    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
-    "CreateLocationFsxWindowsResponseOutputTypeDef",
+    "CreateLocationEfsResponseTypeDef",
+    "CreateLocationFsxLustreResponseTypeDef",
+    "CreateLocationFsxOntapResponseTypeDef",
+    "CreateLocationFsxOpenZfsResponseTypeDef",
+    "CreateLocationFsxWindowsResponseTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
-    "CreateLocationHdfsResponseOutputTypeDef",
+    "CreateLocationHdfsResponseTypeDef",
     "NfsMountOptionsTypeDef",
     "OnPremConfigTypeDef",
-    "CreateLocationNfsResponseOutputTypeDef",
-    "CreateLocationObjectStorageResponseOutputTypeDef",
+    "CreateLocationNfsResponseTypeDef",
+    "CreateLocationObjectStorageResponseTypeDef",
     "S3ConfigTypeDef",
-    "CreateLocationS3ResponseOutputTypeDef",
+    "CreateLocationS3ResponseTypeDef",
     "SmbMountOptionsTypeDef",
-    "CreateLocationSmbResponseOutputTypeDef",
+    "CreateLocationSmbResponseTypeDef",
     "FilterRuleTypeDef",
     "OptionsTypeDef",
     "TaskScheduleTypeDef",
-    "CreateTaskResponseOutputTypeDef",
+    "CreateTaskResponseTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
-    "PrivateLinkConfigOutputTypeDef",
+    "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
-    "DescribeDiscoveryJobResponseOutputTypeDef",
+    "DescribeDiscoveryJobResponseTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
     "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
-    "DescribeLocationFsxLustreResponseOutputTypeDef",
+    "DescribeLocationFsxLustreResponseTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
-    "DescribeLocationFsxWindowsResponseOutputTypeDef",
+    "DescribeLocationFsxWindowsResponseTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "HdfsNameNodeOutputTypeDef",
     "QopConfigurationOutputTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
     "NfsMountOptionsOutputTypeDef",
     "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
-    "DescribeLocationObjectStorageResponseOutputTypeDef",
+    "DescribeLocationObjectStorageResponseTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "S3ConfigOutputTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
     "SmbMountOptionsOutputTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
     "DiscoveryServerConfigurationOutputTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
     "FilterRuleOutputTypeDef",
     "OptionsOutputTypeDef",
-    "TaskExecutionResultDetailOutputTypeDef",
+    "TaskExecutionResultDetailTypeDef",
     "DescribeTaskRequestRequestTypeDef",
     "TaskScheduleOutputTypeDef",
-    "DiscoveryJobListEntryOutputTypeDef",
+    "DiscoveryJobListEntryTypeDef",
     "GenerateRecommendationsRequestRequestTypeDef",
-    "IOPSOutputTypeDef",
-    "LatencyOutputTypeDef",
+    "IOPSTypeDef",
+    "LatencyTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
-    "LocationListEntryOutputTypeDef",
+    "LocationListEntryTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListStorageSystemsRequestRequestTypeDef",
-    "StorageSystemListEntryOutputTypeDef",
+    "StorageSystemListEntryTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagListEntryOutputTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "ListTaskExecutionsRequestRequestTypeDef",
-    "TaskExecutionListEntryOutputTypeDef",
+    "TaskExecutionListEntryTypeDef",
     "TaskFilterTypeDef",
-    "TaskListEntryOutputTypeDef",
-    "MaxP95PerformanceOutputTypeDef",
-    "RecommendationOutputTypeDef",
-    "ThroughputOutputTypeDef",
+    "TaskListEntryTypeDef",
+    "MaxP95PerformanceTypeDef",
+    "RecommendationTypeDef",
+    "ThroughputTypeDef",
     "PaginatorConfigTypeDef",
     "RemoveStorageSystemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "StartDiscoveryJobResponseOutputTypeDef",
-    "StartTaskExecutionResponseOutputTypeDef",
+    "StartDiscoveryJobResponseTypeDef",
+    "StartTaskExecutionResponseTypeDef",
     "StopDiscoveryJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentRequestRequestTypeDef",
     "UpdateDiscoveryJobRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "UpdateStorageSystemRequestRequestTypeDef",
     "AddStorageSystemRequestRequestTypeDef",
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAgentsResponseOutputTypeDef",
+    "ListAgentsResponseTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
     "UpdateTaskRequestRequestTypeDef",
-    "DescribeAgentResponseOutputTypeDef",
-    "DescribeLocationEfsResponseOutputTypeDef",
-    "DescribeLocationHdfsResponseOutputTypeDef",
+    "DescribeAgentResponseTypeDef",
+    "DescribeLocationEfsResponseTypeDef",
+    "DescribeLocationHdfsResponseTypeDef",
     "FsxProtocolNfsOutputTypeDef",
-    "DescribeLocationNfsResponseOutputTypeDef",
-    "DescribeLocationS3ResponseOutputTypeDef",
-    "DescribeLocationSmbResponseOutputTypeDef",
+    "DescribeLocationNfsResponseTypeDef",
+    "DescribeLocationS3ResponseTypeDef",
+    "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbOutputTypeDef",
-    "DescribeStorageSystemResponseOutputTypeDef",
-    "DescribeTaskExecutionResponseOutputTypeDef",
-    "DescribeTaskResponseOutputTypeDef",
-    "ListDiscoveryJobsResponseOutputTypeDef",
+    "DescribeStorageSystemResponseTypeDef",
+    "DescribeTaskExecutionResponseTypeDef",
+    "DescribeTaskResponseTypeDef",
+    "ListDiscoveryJobsResponseTypeDef",
     "ListLocationsRequestListLocationsPaginateTypeDef",
     "ListLocationsRequestRequestTypeDef",
-    "ListLocationsResponseOutputTypeDef",
-    "ListStorageSystemsResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
-    "ListTaskExecutionsResponseOutputTypeDef",
+    "ListLocationsResponseTypeDef",
+    "ListStorageSystemsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTaskExecutionsResponseTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseOutputTypeDef",
-    "NetAppONTAPClusterOutputTypeDef",
-    "NetAppONTAPSVMOutputTypeDef",
-    "NetAppONTAPVolumeOutputTypeDef",
-    "P95MetricsOutputTypeDef",
+    "ListTasksResponseTypeDef",
+    "NetAppONTAPClusterTypeDef",
+    "NetAppONTAPSVMTypeDef",
+    "NetAppONTAPVolumeTypeDef",
+    "P95MetricsTypeDef",
     "FsxProtocolTypeDef",
     "FsxProtocolOutputTypeDef",
-    "ResourceDetailsOutputTypeDef",
-    "ResourceMetricsOutputTypeDef",
+    "ResourceDetailsTypeDef",
+    "ResourceMetricsTypeDef",
     "CreateLocationFsxOntapRequestRequestTypeDef",
     "CreateLocationFsxOpenZfsRequestRequestTypeDef",
-    "DescribeLocationFsxOntapResponseOutputTypeDef",
-    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
-    "DescribeStorageSystemResourcesResponseOutputTypeDef",
-    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
+    "DescribeLocationFsxOntapResponseTypeDef",
+    "DescribeLocationFsxOpenZfsResponseTypeDef",
+    "DescribeStorageSystemResourcesResponseTypeDef",
+    "DescribeStorageSystemResourceMetricsResponseTypeDef",
 )
 
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
@@ -265,97 +265,97 @@
     },
     total=False,
 )
 
 class TagListEntryTypeDef(_RequiredTagListEntryTypeDef, _OptionalTagListEntryTypeDef):
     pass
 
-AddStorageSystemResponseOutputTypeDef = TypedDict(
-    "AddStorageSystemResponseOutputTypeDef",
+AddStorageSystemResponseTypeDef = TypedDict(
+    "AddStorageSystemResponseTypeDef",
     {
         "StorageSystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentListEntryOutputTypeDef = TypedDict(
-    "AgentListEntryOutputTypeDef",
+AgentListEntryTypeDef = TypedDict(
+    "AgentListEntryTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
 )
 
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
-CapacityOutputTypeDef = TypedDict(
-    "CapacityOutputTypeDef",
+CapacityTypeDef = TypedDict(
+    "CapacityTypeDef",
     {
         "Used": int,
         "Provisioned": int,
         "LogicalUsed": int,
     },
 )
 
-CreateAgentResponseOutputTypeDef = TypedDict(
-    "CreateAgentResponseOutputTypeDef",
+CreateAgentResponseTypeDef = TypedDict(
+    "CreateAgentResponseTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2ConfigTypeDef = TypedDict(
     "Ec2ConfigTypeDef",
     {
         "SubnetArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
 
-CreateLocationEfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationEfsResponseOutputTypeDef",
+CreateLocationEfsResponseTypeDef = TypedDict(
+    "CreateLocationEfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxLustreResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxLustreResponseOutputTypeDef",
+CreateLocationFsxLustreResponseTypeDef = TypedDict(
+    "CreateLocationFsxLustreResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOntapResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxOntapResponseOutputTypeDef",
+CreateLocationFsxOntapResponseTypeDef = TypedDict(
+    "CreateLocationFsxOntapResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
+CreateLocationFsxOpenZfsResponseTypeDef = TypedDict(
+    "CreateLocationFsxOpenZfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxWindowsResponseOutputTypeDef = TypedDict(
-    "CreateLocationFsxWindowsResponseOutputTypeDef",
+CreateLocationFsxWindowsResponseTypeDef = TypedDict(
+    "CreateLocationFsxWindowsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HdfsNameNodeTypeDef = TypedDict(
@@ -371,16 +371,16 @@
     {
         "RpcProtection": HdfsRpcProtectionType,
         "DataTransferProtection": HdfsDataTransferProtectionType,
     },
     total=False,
 )
 
-CreateLocationHdfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationHdfsResponseOutputTypeDef",
+CreateLocationHdfsResponseTypeDef = TypedDict(
+    "CreateLocationHdfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NfsMountOptionsTypeDef = TypedDict(
@@ -394,55 +394,55 @@
 OnPremConfigTypeDef = TypedDict(
     "OnPremConfigTypeDef",
     {
         "AgentArns": Sequence[str],
     },
 )
 
-CreateLocationNfsResponseOutputTypeDef = TypedDict(
-    "CreateLocationNfsResponseOutputTypeDef",
+CreateLocationNfsResponseTypeDef = TypedDict(
+    "CreateLocationNfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationObjectStorageResponseOutputTypeDef = TypedDict(
-    "CreateLocationObjectStorageResponseOutputTypeDef",
+CreateLocationObjectStorageResponseTypeDef = TypedDict(
+    "CreateLocationObjectStorageResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketAccessRoleArn": str,
     },
 )
 
-CreateLocationS3ResponseOutputTypeDef = TypedDict(
-    "CreateLocationS3ResponseOutputTypeDef",
+CreateLocationS3ResponseTypeDef = TypedDict(
+    "CreateLocationS3ResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SmbMountOptionsTypeDef = TypedDict(
     "SmbMountOptionsTypeDef",
     {
         "Version": SmbVersionType,
     },
     total=False,
 )
 
-CreateLocationSmbResponseOutputTypeDef = TypedDict(
-    "CreateLocationSmbResponseOutputTypeDef",
+CreateLocationSmbResponseTypeDef = TypedDict(
+    "CreateLocationSmbResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterRuleTypeDef = TypedDict(
@@ -479,16 +479,16 @@
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
-CreateTaskResponseOutputTypeDef = TypedDict(
-    "CreateTaskResponseOutputTypeDef",
+CreateTaskResponseTypeDef = TypedDict(
+    "CreateTaskResponseTypeDef",
     {
         "TaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAgentRequestRequestTypeDef = TypedDict(
@@ -515,16 +515,16 @@
 DescribeAgentRequestRequestTypeDef = TypedDict(
     "DescribeAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
 )
 
-PrivateLinkConfigOutputTypeDef = TypedDict(
-    "PrivateLinkConfigOutputTypeDef",
+PrivateLinkConfigTypeDef = TypedDict(
+    "PrivateLinkConfigTypeDef",
     {
         "VpcEndpointId": str,
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
 )
@@ -532,16 +532,16 @@
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
 )
 
-DescribeDiscoveryJobResponseOutputTypeDef = TypedDict(
-    "DescribeDiscoveryJobResponseOutputTypeDef",
+DescribeDiscoveryJobResponseTypeDef = TypedDict(
+    "DescribeDiscoveryJobResponseTypeDef",
     {
         "StorageSystemArn": str,
         "DiscoveryJobArn": str,
         "CollectionDurationMinutes": int,
         "Status": DiscoveryJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
@@ -567,16 +567,16 @@
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxLustreResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxLustreResponseOutputTypeDef",
+DescribeLocationFsxLustreResponseTypeDef = TypedDict(
+    "DescribeLocationFsxLustreResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -599,16 +599,16 @@
 DescribeLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxWindowsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxWindowsResponseOutputTypeDef",
+DescribeLocationFsxWindowsResponseTypeDef = TypedDict(
+    "DescribeLocationFsxWindowsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "User": str,
         "Domain": str,
@@ -663,16 +663,16 @@
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationObjectStorageResponseOutputTypeDef = TypedDict(
-    "DescribeLocationObjectStorageResponseOutputTypeDef",
+DescribeLocationObjectStorageResponseTypeDef = TypedDict(
+    "DescribeLocationObjectStorageResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "AccessKey": str,
         "ServerPort": int,
         "ServerProtocol": ObjectStorageServerProtocolType,
         "AgentArns": List[str],
@@ -830,16 +830,16 @@
         "LogLevel": LogLevelType,
         "TransferMode": TransferModeType,
         "SecurityDescriptorCopyFlags": SmbSecurityDescriptorCopyFlagsType,
         "ObjectTags": ObjectTagsType,
     },
 )
 
-TaskExecutionResultDetailOutputTypeDef = TypedDict(
-    "TaskExecutionResultDetailOutputTypeDef",
+TaskExecutionResultDetailTypeDef = TypedDict(
+    "TaskExecutionResultDetailTypeDef",
     {
         "PrepareDuration": int,
         "PrepareStatus": PhaseStatusType,
         "TotalDuration": int,
         "TransferDuration": int,
         "TransferStatus": PhaseStatusType,
         "VerifyDuration": int,
@@ -859,16 +859,16 @@
 TaskScheduleOutputTypeDef = TypedDict(
     "TaskScheduleOutputTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
-DiscoveryJobListEntryOutputTypeDef = TypedDict(
-    "DiscoveryJobListEntryOutputTypeDef",
+DiscoveryJobListEntryTypeDef = TypedDict(
+    "DiscoveryJobListEntryTypeDef",
     {
         "DiscoveryJobArn": str,
         "Status": DiscoveryJobStatusType,
     },
 )
 
 GenerateRecommendationsRequestRequestTypeDef = TypedDict(
@@ -876,26 +876,26 @@
     {
         "DiscoveryJobArn": str,
         "ResourceIds": Sequence[str],
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
-IOPSOutputTypeDef = TypedDict(
-    "IOPSOutputTypeDef",
+IOPSTypeDef = TypedDict(
+    "IOPSTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
 
-LatencyOutputTypeDef = TypedDict(
-    "LatencyOutputTypeDef",
+LatencyTypeDef = TypedDict(
+    "LatencyTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
     },
 )
 
@@ -940,16 +940,16 @@
     {
         "Name": LocationFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-LocationListEntryOutputTypeDef = TypedDict(
-    "LocationListEntryOutputTypeDef",
+LocationListEntryTypeDef = TypedDict(
+    "LocationListEntryTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
     },
 )
 
 ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
@@ -965,16 +965,16 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-StorageSystemListEntryOutputTypeDef = TypedDict(
-    "StorageSystemListEntryOutputTypeDef",
+StorageSystemListEntryTypeDef = TypedDict(
+    "StorageSystemListEntryTypeDef",
     {
         "StorageSystemArn": str,
         "Name": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
@@ -1041,16 +1041,16 @@
         "TaskArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-TaskExecutionListEntryOutputTypeDef = TypedDict(
-    "TaskExecutionListEntryOutputTypeDef",
+TaskExecutionListEntryTypeDef = TypedDict(
+    "TaskExecutionListEntryTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
     },
 )
 
 TaskFilterTypeDef = TypedDict(
@@ -1058,25 +1058,25 @@
     {
         "Name": TaskFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-TaskListEntryOutputTypeDef = TypedDict(
-    "TaskListEntryOutputTypeDef",
+TaskListEntryTypeDef = TypedDict(
+    "TaskListEntryTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
 )
 
-MaxP95PerformanceOutputTypeDef = TypedDict(
-    "MaxP95PerformanceOutputTypeDef",
+MaxP95PerformanceTypeDef = TypedDict(
+    "MaxP95PerformanceTypeDef",
     {
         "IopsRead": float,
         "IopsWrite": float,
         "IopsOther": float,
         "IopsTotal": float,
         "ThroughputRead": float,
         "ThroughputWrite": float,
@@ -1084,25 +1084,25 @@
         "ThroughputTotal": float,
         "LatencyRead": float,
         "LatencyWrite": float,
         "LatencyOther": float,
     },
 )
 
-RecommendationOutputTypeDef = TypedDict(
-    "RecommendationOutputTypeDef",
+RecommendationTypeDef = TypedDict(
+    "RecommendationTypeDef",
     {
         "StorageType": str,
         "StorageConfiguration": Dict[str, str],
         "EstimatedMonthlyStorageCost": str,
     },
 )
 
-ThroughputOutputTypeDef = TypedDict(
-    "ThroughputOutputTypeDef",
+ThroughputTypeDef = TypedDict(
+    "ThroughputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
@@ -1131,24 +1131,24 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StartDiscoveryJobResponseOutputTypeDef = TypedDict(
-    "StartDiscoveryJobResponseOutputTypeDef",
+StartDiscoveryJobResponseTypeDef = TypedDict(
+    "StartDiscoveryJobResponseTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTaskExecutionResponseOutputTypeDef = TypedDict(
-    "StartTaskExecutionResponseOutputTypeDef",
+StartTaskExecutionResponseTypeDef = TypedDict(
+    "StartTaskExecutionResponseTypeDef",
     {
         "TaskExecutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopDiscoveryJobRequestRequestTypeDef = TypedDict(
@@ -1391,18 +1391,18 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
 )
 
-ListAgentsResponseOutputTypeDef = TypedDict(
-    "ListAgentsResponseOutputTypeDef",
+ListAgentsResponseTypeDef = TypedDict(
+    "ListAgentsResponseTypeDef",
     {
-        "Agents": List[AgentListEntryOutputTypeDef],
+        "Agents": List[AgentListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationEfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationEfsRequestRequestTypeDef",
@@ -1709,44 +1709,44 @@
 )
 
 class UpdateTaskRequestRequestTypeDef(
     _RequiredUpdateTaskRequestRequestTypeDef, _OptionalUpdateTaskRequestRequestTypeDef
 ):
     pass
 
-DescribeAgentResponseOutputTypeDef = TypedDict(
-    "DescribeAgentResponseOutputTypeDef",
+DescribeAgentResponseTypeDef = TypedDict(
+    "DescribeAgentResponseTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
         "LastConnectionTime": datetime,
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
-        "PrivateLinkConfig": PrivateLinkConfigOutputTypeDef,
+        "PrivateLinkConfig": PrivateLinkConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationEfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationEfsResponseOutputTypeDef",
+DescribeLocationEfsResponseTypeDef = TypedDict(
+    "DescribeLocationEfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "Ec2Config": Ec2ConfigOutputTypeDef,
         "CreationTime": datetime,
         "AccessPointArn": str,
         "FileSystemAccessRoleArn": str,
         "InTransitEncryption": EfsInTransitEncryptionType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationHdfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationHdfsResponseOutputTypeDef",
+DescribeLocationHdfsResponseTypeDef = TypedDict(
+    "DescribeLocationHdfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "NameNodes": List[HdfsNameNodeOutputTypeDef],
         "BlockSize": int,
         "ReplicationFactor": int,
         "KmsKeyProviderUri": str,
@@ -1763,41 +1763,41 @@
 FsxProtocolNfsOutputTypeDef = TypedDict(
     "FsxProtocolNfsOutputTypeDef",
     {
         "MountOptions": NfsMountOptionsOutputTypeDef,
     },
 )
 
-DescribeLocationNfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationNfsResponseOutputTypeDef",
+DescribeLocationNfsResponseTypeDef = TypedDict(
+    "DescribeLocationNfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "OnPremConfig": OnPremConfigOutputTypeDef,
         "MountOptions": NfsMountOptionsOutputTypeDef,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationS3ResponseOutputTypeDef = TypedDict(
-    "DescribeLocationS3ResponseOutputTypeDef",
+DescribeLocationS3ResponseTypeDef = TypedDict(
+    "DescribeLocationS3ResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "S3StorageClass": S3StorageClassType,
         "S3Config": S3ConfigOutputTypeDef,
         "AgentArns": List[str],
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationSmbResponseOutputTypeDef = TypedDict(
-    "DescribeLocationSmbResponseOutputTypeDef",
+DescribeLocationSmbResponseTypeDef = TypedDict(
+    "DescribeLocationSmbResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "AgentArns": List[str],
         "User": str,
         "Domain": str,
         "MountOptions": SmbMountOptionsOutputTypeDef,
@@ -1812,16 +1812,16 @@
         "Domain": str,
         "MountOptions": SmbMountOptionsOutputTypeDef,
         "Password": str,
         "User": str,
     },
 )
 
-DescribeStorageSystemResponseOutputTypeDef = TypedDict(
-    "DescribeStorageSystemResponseOutputTypeDef",
+DescribeStorageSystemResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResponseTypeDef",
     {
         "StorageSystemArn": str,
         "ServerConfiguration": DiscoveryServerConfigurationOutputTypeDef,
         "SystemType": Literal["NetAppONTAP"],
         "AgentArns": List[str],
         "Name": str,
         "ErrorMessage": str,
@@ -1829,36 +1829,36 @@
         "CloudWatchLogGroupArn": str,
         "CreationTime": datetime,
         "SecretsManagerArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTaskExecutionResponseOutputTypeDef = TypedDict(
-    "DescribeTaskExecutionResponseOutputTypeDef",
+DescribeTaskExecutionResponseTypeDef = TypedDict(
+    "DescribeTaskExecutionResponseTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
         "Options": OptionsOutputTypeDef,
         "Excludes": List[FilterRuleOutputTypeDef],
         "Includes": List[FilterRuleOutputTypeDef],
         "StartTime": datetime,
         "EstimatedFilesToTransfer": int,
         "EstimatedBytesToTransfer": int,
         "FilesTransferred": int,
         "BytesWritten": int,
         "BytesTransferred": int,
-        "Result": TaskExecutionResultDetailOutputTypeDef,
+        "Result": TaskExecutionResultDetailTypeDef,
         "BytesCompressed": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTaskResponseOutputTypeDef = TypedDict(
-    "DescribeTaskResponseOutputTypeDef",
+DescribeTaskResponseTypeDef = TypedDict(
+    "DescribeTaskResponseTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
         "CurrentTaskExecutionArn": str,
         "SourceLocationArn": str,
         "DestinationLocationArn": str,
@@ -1872,18 +1872,18 @@
         "ErrorDetail": str,
         "CreationTime": datetime,
         "Includes": List[FilterRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDiscoveryJobsResponseOutputTypeDef = TypedDict(
-    "ListDiscoveryJobsResponseOutputTypeDef",
+ListDiscoveryJobsResponseTypeDef = TypedDict(
+    "ListDiscoveryJobsResponseTypeDef",
     {
-        "DiscoveryJobs": List[DiscoveryJobListEntryOutputTypeDef],
+        "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
@@ -1900,45 +1900,45 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[LocationFilterTypeDef],
     },
     total=False,
 )
 
-ListLocationsResponseOutputTypeDef = TypedDict(
-    "ListLocationsResponseOutputTypeDef",
+ListLocationsResponseTypeDef = TypedDict(
+    "ListLocationsResponseTypeDef",
     {
-        "Locations": List[LocationListEntryOutputTypeDef],
+        "Locations": List[LocationListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListStorageSystemsResponseOutputTypeDef = TypedDict(
-    "ListStorageSystemsResponseOutputTypeDef",
+ListStorageSystemsResponseTypeDef = TypedDict(
+    "ListStorageSystemsResponseTypeDef",
     {
-        "StorageSystems": List[StorageSystemListEntryOutputTypeDef],
+        "StorageSystems": List[StorageSystemListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTaskExecutionsResponseOutputTypeDef = TypedDict(
-    "ListTaskExecutionsResponseOutputTypeDef",
+ListTaskExecutionsResponseTypeDef = TypedDict(
+    "ListTaskExecutionsResponseTypeDef",
     {
-        "TaskExecutions": List[TaskExecutionListEntryOutputTypeDef],
+        "TaskExecutions": List[TaskExecutionListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
@@ -1955,87 +1955,87 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[TaskFilterTypeDef],
     },
     total=False,
 )
 
-ListTasksResponseOutputTypeDef = TypedDict(
-    "ListTasksResponseOutputTypeDef",
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
     {
-        "Tasks": List[TaskListEntryOutputTypeDef],
+        "Tasks": List[TaskListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NetAppONTAPClusterOutputTypeDef = TypedDict(
-    "NetAppONTAPClusterOutputTypeDef",
+NetAppONTAPClusterTypeDef = TypedDict(
+    "NetAppONTAPClusterTypeDef",
     {
         "CifsShareCount": int,
         "NfsExportedVolumes": int,
         "ResourceId": str,
         "ClusterName": str,
-        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-NetAppONTAPSVMOutputTypeDef = TypedDict(
-    "NetAppONTAPSVMOutputTypeDef",
+NetAppONTAPSVMTypeDef = TypedDict(
+    "NetAppONTAPSVMTypeDef",
     {
         "ClusterUuid": str,
         "ResourceId": str,
         "SvmName": str,
         "CifsShareCount": int,
         "EnabledProtocols": List[str],
         "TotalCapacityUsed": int,
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "Recommendations": List[RecommendationTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
         "LunCount": int,
     },
 )
 
-NetAppONTAPVolumeOutputTypeDef = TypedDict(
-    "NetAppONTAPVolumeOutputTypeDef",
+NetAppONTAPVolumeTypeDef = TypedDict(
+    "NetAppONTAPVolumeTypeDef",
     {
         "VolumeName": str,
         "ResourceId": str,
         "CifsShareCount": int,
         "SecurityStyle": str,
         "SvmUuid": str,
         "SvmName": str,
         "CapacityUsed": int,
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-P95MetricsOutputTypeDef = TypedDict(
-    "P95MetricsOutputTypeDef",
+P95MetricsTypeDef = TypedDict(
+    "P95MetricsTypeDef",
     {
-        "IOPS": IOPSOutputTypeDef,
-        "Throughput": ThroughputOutputTypeDef,
-        "Latency": LatencyOutputTypeDef,
+        "IOPS": IOPSTypeDef,
+        "Throughput": ThroughputTypeDef,
+        "Latency": LatencyTypeDef,
     },
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
@@ -2048,29 +2048,29 @@
     "FsxProtocolOutputTypeDef",
     {
         "NFS": FsxProtocolNfsOutputTypeDef,
         "SMB": FsxProtocolSmbOutputTypeDef,
     },
 )
 
-ResourceDetailsOutputTypeDef = TypedDict(
-    "ResourceDetailsOutputTypeDef",
+ResourceDetailsTypeDef = TypedDict(
+    "ResourceDetailsTypeDef",
     {
-        "NetAppONTAPSVMs": List[NetAppONTAPSVMOutputTypeDef],
-        "NetAppONTAPVolumes": List[NetAppONTAPVolumeOutputTypeDef],
-        "NetAppONTAPClusters": List[NetAppONTAPClusterOutputTypeDef],
+        "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
+        "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
+        "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
     },
 )
 
-ResourceMetricsOutputTypeDef = TypedDict(
-    "ResourceMetricsOutputTypeDef",
+ResourceMetricsTypeDef = TypedDict(
+    "ResourceMetricsTypeDef",
     {
         "Timestamp": datetime,
-        "P95Metrics": P95MetricsOutputTypeDef,
-        "Capacity": CapacityOutputTypeDef,
+        "P95Metrics": P95MetricsTypeDef,
+        "Capacity": CapacityTypeDef,
         "ResourceId": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
@@ -2114,50 +2114,50 @@
 
 class CreateLocationFsxOpenZfsRequestRequestTypeDef(
     _RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef,
     _OptionalCreateLocationFsxOpenZfsRequestRequestTypeDef,
 ):
     pass
 
-DescribeLocationFsxOntapResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxOntapResponseOutputTypeDef",
+DescribeLocationFsxOntapResponseTypeDef = TypedDict(
+    "DescribeLocationFsxOntapResponseTypeDef",
     {
         "CreationTime": datetime,
         "LocationArn": str,
         "LocationUri": str,
         "Protocol": FsxProtocolOutputTypeDef,
         "SecurityGroupArns": List[str],
         "StorageVirtualMachineArn": str,
         "FsxFilesystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
-    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
+DescribeLocationFsxOpenZfsResponseTypeDef = TypedDict(
+    "DescribeLocationFsxOpenZfsResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "Protocol": FsxProtocolOutputTypeDef,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourcesResponseOutputTypeDef = TypedDict(
-    "DescribeStorageSystemResourcesResponseOutputTypeDef",
+DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResourcesResponseTypeDef",
     {
-        "ResourceDetails": ResourceDetailsOutputTypeDef,
+        "ResourceDetails": ResourceDetailsTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourceMetricsResponseOutputTypeDef = TypedDict(
-    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
+DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
+    "DescribeStorageSystemResourceMetricsResponseTypeDef",
     {
-        "Metrics": List[ResourceMetricsOutputTypeDef],
+        "Metrics": List[ResourceMetricsTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
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
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,170 +391,170 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
     CredentialsTypeDef,
     DiscoveryServerConfigurationTypeDef,
     TagListEntryTypeDef,
-    AddStorageSystemResponseOutputTypeDef,
-    AgentListEntryOutputTypeDef,
+    AddStorageSystemResponseTypeDef,
+    AgentListEntryTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    CapacityOutputTypeDef,
-    CreateAgentResponseOutputTypeDef,
+    CapacityTypeDef,
+    CreateAgentResponseTypeDef,
     Ec2ConfigTypeDef,
-    CreateLocationEfsResponseOutputTypeDef,
-    CreateLocationFsxLustreResponseOutputTypeDef,
-    CreateLocationFsxOntapResponseOutputTypeDef,
-    CreateLocationFsxOpenZfsResponseOutputTypeDef,
-    CreateLocationFsxWindowsResponseOutputTypeDef,
+    CreateLocationEfsResponseTypeDef,
+    CreateLocationFsxLustreResponseTypeDef,
+    CreateLocationFsxOntapResponseTypeDef,
+    CreateLocationFsxOpenZfsResponseTypeDef,
+    CreateLocationFsxWindowsResponseTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
-    CreateLocationHdfsResponseOutputTypeDef,
+    CreateLocationHdfsResponseTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
-    CreateLocationNfsResponseOutputTypeDef,
-    CreateLocationObjectStorageResponseOutputTypeDef,
+    CreateLocationNfsResponseTypeDef,
+    CreateLocationObjectStorageResponseTypeDef,
     S3ConfigTypeDef,
-    CreateLocationS3ResponseOutputTypeDef,
+    CreateLocationS3ResponseTypeDef,
     SmbMountOptionsTypeDef,
-    CreateLocationSmbResponseOutputTypeDef,
+    CreateLocationSmbResponseTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
-    CreateTaskResponseOutputTypeDef,
+    CreateTaskResponseTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
-    PrivateLinkConfigOutputTypeDef,
+    PrivateLinkConfigTypeDef,
     DescribeDiscoveryJobRequestRequestTypeDef,
-    DescribeDiscoveryJobResponseOutputTypeDef,
+    DescribeDiscoveryJobResponseTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
     Ec2ConfigOutputTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
-    DescribeLocationFsxLustreResponseOutputTypeDef,
+    DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
-    DescribeLocationFsxWindowsResponseOutputTypeDef,
+    DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
     HdfsNameNodeOutputTypeDef,
     QopConfigurationOutputTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
     NfsMountOptionsOutputTypeDef,
     OnPremConfigOutputTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
-    DescribeLocationObjectStorageResponseOutputTypeDef,
+    DescribeLocationObjectStorageResponseTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
     S3ConfigOutputTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
     SmbMountOptionsOutputTypeDef,
     DescribeStorageSystemRequestRequestTypeDef,
     DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     DescribeStorageSystemResourcesRequestRequestTypeDef,
     DiscoveryServerConfigurationOutputTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
     FilterRuleOutputTypeDef,
     OptionsOutputTypeDef,
-    TaskExecutionResultDetailOutputTypeDef,
+    TaskExecutionResultDetailTypeDef,
     DescribeTaskRequestRequestTypeDef,
     TaskScheduleOutputTypeDef,
-    DiscoveryJobListEntryOutputTypeDef,
+    DiscoveryJobListEntryTypeDef,
     GenerateRecommendationsRequestRequestTypeDef,
-    IOPSOutputTypeDef,
-    LatencyOutputTypeDef,
+    IOPSTypeDef,
+    LatencyTypeDef,
     ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
     ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
     ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
-    LocationListEntryOutputTypeDef,
+    LocationListEntryTypeDef,
     ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
     ListStorageSystemsRequestRequestTypeDef,
-    StorageSystemListEntryOutputTypeDef,
+    StorageSystemListEntryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagListEntryOutputTypeDef,
     ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
-    TaskExecutionListEntryOutputTypeDef,
+    TaskExecutionListEntryTypeDef,
     TaskFilterTypeDef,
-    TaskListEntryOutputTypeDef,
-    MaxP95PerformanceOutputTypeDef,
-    RecommendationOutputTypeDef,
-    ThroughputOutputTypeDef,
+    TaskListEntryTypeDef,
+    MaxP95PerformanceTypeDef,
+    RecommendationTypeDef,
+    ThroughputTypeDef,
     PaginatorConfigTypeDef,
     RemoveStorageSystemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    StartDiscoveryJobResponseOutputTypeDef,
-    StartTaskExecutionResponseOutputTypeDef,
+    StartDiscoveryJobResponseTypeDef,
+    StartTaskExecutionResponseTypeDef,
     StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
     UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
     UpdateStorageSystemRequestRequestTypeDef,
     AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
     StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAgentsResponseOutputTypeDef,
+    ListAgentsResponseTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
     UpdateLocationNfsRequestRequestTypeDef,
     CreateLocationS3RequestRequestTypeDef,
     CreateLocationSmbRequestRequestTypeDef,
     FsxProtocolSmbTypeDef,
     UpdateLocationSmbRequestRequestTypeDef,
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
     UpdateTaskRequestRequestTypeDef,
-    DescribeAgentResponseOutputTypeDef,
-    DescribeLocationEfsResponseOutputTypeDef,
-    DescribeLocationHdfsResponseOutputTypeDef,
+    DescribeAgentResponseTypeDef,
+    DescribeLocationEfsResponseTypeDef,
+    DescribeLocationHdfsResponseTypeDef,
     FsxProtocolNfsOutputTypeDef,
-    DescribeLocationNfsResponseOutputTypeDef,
-    DescribeLocationS3ResponseOutputTypeDef,
-    DescribeLocationSmbResponseOutputTypeDef,
+    DescribeLocationNfsResponseTypeDef,
+    DescribeLocationS3ResponseTypeDef,
+    DescribeLocationSmbResponseTypeDef,
     FsxProtocolSmbOutputTypeDef,
-    DescribeStorageSystemResponseOutputTypeDef,
-    DescribeTaskExecutionResponseOutputTypeDef,
-    DescribeTaskResponseOutputTypeDef,
-    ListDiscoveryJobsResponseOutputTypeDef,
+    DescribeStorageSystemResponseTypeDef,
+    DescribeTaskExecutionResponseTypeDef,
+    DescribeTaskResponseTypeDef,
+    ListDiscoveryJobsResponseTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
-    ListLocationsResponseOutputTypeDef,
-    ListStorageSystemsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListTaskExecutionsResponseOutputTypeDef,
+    ListLocationsResponseTypeDef,
+    ListStorageSystemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskExecutionsResponseTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseOutputTypeDef,
-    NetAppONTAPClusterOutputTypeDef,
-    NetAppONTAPSVMOutputTypeDef,
-    NetAppONTAPVolumeOutputTypeDef,
-    P95MetricsOutputTypeDef,
+    ListTasksResponseTypeDef,
+    NetAppONTAPClusterTypeDef,
+    NetAppONTAPSVMTypeDef,
+    NetAppONTAPVolumeTypeDef,
+    P95MetricsTypeDef,
     FsxProtocolTypeDef,
     FsxProtocolOutputTypeDef,
-    ResourceDetailsOutputTypeDef,
-    ResourceMetricsOutputTypeDef,
+    ResourceDetailsTypeDef,
+    ResourceMetricsTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
-    DescribeLocationFsxOntapResponseOutputTypeDef,
-    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
-    DescribeStorageSystemResourcesResponseOutputTypeDef,
-    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    DescribeLocationFsxOntapResponseTypeDef,
+    DescribeLocationFsxOpenZfsResponseTypeDef,
+    DescribeStorageSystemResourcesResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseTypeDef,
 )
 
 
 def get_structure() -> CredentialsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy-boto3-datasync-1.28.3.post2/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3.post1/setup.py` & `mypy-boto3-datasync-1.28.3.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder"
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

