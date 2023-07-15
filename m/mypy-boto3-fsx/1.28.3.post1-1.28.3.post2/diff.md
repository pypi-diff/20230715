# Comparing `tmp/mypy-boto3-fsx-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-fsx-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fsx-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+gzip compressed data, was "mypy-boto3-fsx-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
```

## Comparing `mypy-boto3-fsx-1.28.3.post1.tar` & `mypy-boto3-fsx-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23371 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21896 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39254 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39201 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-14 16:16:38.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-14 16:16:38.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85904 2023-07-14 16:16:40.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85811 2023-07-14 16:16:39.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23371 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.314243 mypy-boto3-fsx-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-15 06:38:32.294242 mypy-boto3-fsx-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.294242 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-15 06:37:09.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-15 06:37:09.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    83900 2023-07-15 06:37:11.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83807 2023-07-15 06:37:10.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.294242 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-15 06:38:32.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-15 06:38:32.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 06:38:32.000000 mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.314243 mypy-boto3-fsx-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-15 06:37:08.000000 mypy-boto3-fsx-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/LICENSE` & `mypy-boto3-fsx-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3.post1/PKG-INFO` & `mypy-boto3-fsx-1.28.3.post2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-fsx
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.7
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 fsx type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,110 +361,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_fsx.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fsx.type_defs import (
-    ActiveDirectoryBackupAttributesOutputTypeDef,
-    AdministrativeActionFailureDetailsOutputTypeDef,
-    AliasOutputTypeDef,
+    ActiveDirectoryBackupAttributesTypeDef,
+    AdministrativeActionFailureDetailsTypeDef,
+    AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
     AutoExportPolicyOutputTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyOutputTypeDef,
     AutoImportPolicyTypeDef,
     AutocommitPeriodOutputTypeDef,
     AutocommitPeriodTypeDef,
-    BackupFailureDetailsOutputTypeDef,
+    BackupFailureDetailsTypeDef,
     TagOutputTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
-    CancelDataRepositoryTaskResponseOutputTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportOutputTypeDef,
     CompletionReportTypeDef,
     TagTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
-    CreateFileSystemFromBackupResponseOutputTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
-    CreateFileSystemResponseOutputTypeDef,
+    CreateFileSystemResponseTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
-    DataRepositoryFailureDetailsOutputTypeDef,
-    DataRepositoryTaskFailureDetailsOutputTypeDef,
+    DataRepositoryFailureDetailsTypeDef,
+    DataRepositoryTaskFailureDetailsTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DataRepositoryTaskStatusOutputTypeDef,
+    DataRepositoryTaskStatusTypeDef,
     DeleteBackupRequestRequestTypeDef,
-    DeleteBackupResponseOutputTypeDef,
+    DeleteBackupResponseTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteDataRepositoryAssociationResponseOutputTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
-    DeleteFileCacheResponseOutputTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResponseOutputTypeDef,
+    DeleteSnapshotResponseTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
-    DeleteStorageVirtualMachineResponseOutputTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeFileSystemsResponseTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
     DiskIopsConfigurationOutputTypeDef,
-    FileCacheFailureDetailsOutputTypeDef,
+    FileCacheFailureDetailsTypeDef,
     FileCacheNFSConfigurationTypeDef,
     FileCacheLustreMetadataConfigurationOutputTypeDef,
-    LustreLogConfigurationOutputTypeDef,
-    FileSystemEndpointOutputTypeDef,
-    FileSystemFailureDetailsOutputTypeDef,
-    LifecycleTransitionReasonOutputTypeDef,
+    LustreLogConfigurationTypeDef,
+    FileSystemEndpointTypeDef,
+    FileSystemFailureDetailsTypeDef,
+    LifecycleTransitionReasonTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LustreRootSquashConfigurationOutputTypeDef,
     TieringPolicyOutputTypeDef,
     OpenZFSClientConfigurationOutputTypeDef,
     OpenZFSClientConfigurationTypeDef,
-    OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+    OpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaOutputTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
-    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     RetentionPeriodOutputTypeDef,
     RetentionPeriodTypeDef,
-    SelfManagedActiveDirectoryAttributesOutputTypeDef,
+    SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
-    SvmEndpointOutputTypeDef,
+    SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileSystemResponseOutputTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
-    WindowsAuditLogConfigurationOutputTypeDef,
-    AssociateFileSystemAliasesResponseOutputTypeDef,
-    DescribeFileSystemAliasesResponseOutputTypeDef,
-    DisassociateFileSystemAliasesResponseOutputTypeDef,
-    NFSDataRepositoryConfigurationOutputTypeDef,
+    WindowsAuditLogConfigurationTypeDef,
+    AssociateFileSystemAliasesResponseTypeDef,
+    DescribeFileSystemAliasesResponseTypeDef,
+    DisassociateFileSystemAliasesResponseTypeDef,
+    NFSDataRepositoryConfigurationTypeDef,
     S3DataRepositoryConfigurationOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
-    DeleteFileSystemLustreResponseOutputTypeDef,
-    DeleteFileSystemOpenZFSResponseOutputTypeDef,
-    DeleteFileSystemWindowsResponseOutputTypeDef,
-    DeleteVolumeOntapResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    DeleteFileSystemLustreResponseTypeDef,
+    DeleteFileSystemOpenZFSResponseTypeDef,
+    DeleteFileSystemWindowsResponseTypeDef,
+    DeleteVolumeOntapResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
@@ -506,101 +474,101 @@
     CreateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    DataRepositoryConfigurationOutputTypeDef,
+    DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
-    DataRepositoryTaskOutputTypeDef,
+    DataRepositoryTaskTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
-    OpenZFSFileSystemConfigurationOutputTypeDef,
+    OpenZFSFileSystemConfigurationTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
-    FileCacheLustreConfigurationOutputTypeDef,
-    FileSystemEndpointsOutputTypeDef,
-    SnapshotOutputTypeDef,
+    FileCacheLustreConfigurationTypeDef,
+    FileSystemEndpointsTypeDef,
+    SnapshotTypeDef,
     OpenZFSNfsExportOutputTypeDef,
     OpenZFSNfsExportTypeDef,
     SnaplockRetentionPeriodOutputTypeDef,
     SnaplockRetentionPeriodTypeDef,
-    SvmActiveDirectoryConfigurationOutputTypeDef,
+    SvmActiveDirectoryConfigurationTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    SvmEndpointsOutputTypeDef,
+    SvmEndpointsTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
-    WindowsFileSystemConfigurationOutputTypeDef,
-    DataRepositoryAssociationOutputTypeDef,
+    WindowsFileSystemConfigurationTypeDef,
+    DataRepositoryAssociationTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteFileSystemResponseOutputTypeDef,
-    DeleteVolumeResponseOutputTypeDef,
+    DeleteFileSystemResponseTypeDef,
+    DeleteVolumeResponseTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteVolumeRequestRequestTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    LustreFileSystemConfigurationOutputTypeDef,
-    CreateDataRepositoryTaskResponseOutputTypeDef,
-    DescribeDataRepositoryTasksResponseOutputTypeDef,
+    LustreFileSystemConfigurationTypeDef,
+    CreateDataRepositoryTaskResponseTypeDef,
+    DescribeDataRepositoryTasksResponseTypeDef,
     CreateFileCacheRequestRequestTypeDef,
-    FileCacheCreatingOutputTypeDef,
-    FileCacheOutputTypeDef,
-    OntapFileSystemConfigurationOutputTypeDef,
-    CreateSnapshotResponseOutputTypeDef,
-    DescribeSnapshotsResponseOutputTypeDef,
-    UpdateSnapshotResponseOutputTypeDef,
-    OpenZFSVolumeConfigurationOutputTypeDef,
+    FileCacheCreatingTypeDef,
+    FileCacheTypeDef,
+    OntapFileSystemConfigurationTypeDef,
+    CreateSnapshotResponseTypeDef,
+    DescribeSnapshotsResponseTypeDef,
+    UpdateSnapshotResponseTypeDef,
+    OpenZFSVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    SnaplockConfigurationOutputTypeDef,
+    SnaplockConfigurationTypeDef,
     CreateSnaplockConfigurationTypeDef,
     UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
-    StorageVirtualMachineOutputTypeDef,
-    CreateDataRepositoryAssociationResponseOutputTypeDef,
-    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
-    UpdateDataRepositoryAssociationResponseOutputTypeDef,
-    CreateFileCacheResponseOutputTypeDef,
-    DescribeFileCachesResponseOutputTypeDef,
-    UpdateFileCacheResponseOutputTypeDef,
-    FileSystemOutputTypeDef,
+    StorageVirtualMachineTypeDef,
+    CreateDataRepositoryAssociationResponseTypeDef,
+    DescribeDataRepositoryAssociationsResponseTypeDef,
+    UpdateDataRepositoryAssociationResponseTypeDef,
+    CreateFileCacheResponseTypeDef,
+    DescribeFileCachesResponseTypeDef,
+    UpdateFileCacheResponseTypeDef,
+    FileSystemTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    OntapVolumeConfigurationOutputTypeDef,
+    OntapVolumeConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
-    CreateStorageVirtualMachineResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    UpdateStorageVirtualMachineResponseOutputTypeDef,
+    CreateStorageVirtualMachineResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    UpdateStorageVirtualMachineResponseTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
-    VolumeOutputTypeDef,
+    VolumeTypeDef,
     CreateVolumeFromBackupRequestRequestTypeDef,
     CreateVolumeRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
-    AdministrativeActionOutputTypeDef,
-    BackupOutputTypeDef,
-    CreateVolumeFromBackupResponseOutputTypeDef,
-    CreateVolumeResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
-    UpdateVolumeResponseOutputTypeDef,
-    CopyBackupResponseOutputTypeDef,
-    CreateBackupResponseOutputTypeDef,
-    DescribeBackupsResponseOutputTypeDef,
+    AdministrativeActionTypeDef,
+    BackupTypeDef,
+    CreateVolumeFromBackupResponseTypeDef,
+    CreateVolumeResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
+    UpdateVolumeResponseTypeDef,
+    CopyBackupResponseTypeDef,
+    CreateBackupResponseTypeDef,
+    DescribeBackupsResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryBackupAttributesOutputTypeDef:
+def get_structure() -> ActiveDirectoryBackupAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/README.md` & `mypy-boto3-fsx-1.28.3.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-fsx
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 fsx type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,110 +393,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_fsx.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fsx.type_defs import (
-    ActiveDirectoryBackupAttributesOutputTypeDef,
-    AdministrativeActionFailureDetailsOutputTypeDef,
-    AliasOutputTypeDef,
+    ActiveDirectoryBackupAttributesTypeDef,
+    AdministrativeActionFailureDetailsTypeDef,
+    AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
     AutoExportPolicyOutputTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyOutputTypeDef,
     AutoImportPolicyTypeDef,
     AutocommitPeriodOutputTypeDef,
     AutocommitPeriodTypeDef,
-    BackupFailureDetailsOutputTypeDef,
+    BackupFailureDetailsTypeDef,
     TagOutputTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
-    CancelDataRepositoryTaskResponseOutputTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportOutputTypeDef,
     CompletionReportTypeDef,
     TagTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
-    CreateFileSystemFromBackupResponseOutputTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
-    CreateFileSystemResponseOutputTypeDef,
+    CreateFileSystemResponseTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
-    DataRepositoryFailureDetailsOutputTypeDef,
-    DataRepositoryTaskFailureDetailsOutputTypeDef,
+    DataRepositoryFailureDetailsTypeDef,
+    DataRepositoryTaskFailureDetailsTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DataRepositoryTaskStatusOutputTypeDef,
+    DataRepositoryTaskStatusTypeDef,
     DeleteBackupRequestRequestTypeDef,
-    DeleteBackupResponseOutputTypeDef,
+    DeleteBackupResponseTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteDataRepositoryAssociationResponseOutputTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
-    DeleteFileCacheResponseOutputTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResponseOutputTypeDef,
+    DeleteSnapshotResponseTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
-    DeleteStorageVirtualMachineResponseOutputTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeFileSystemsResponseTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
     DiskIopsConfigurationOutputTypeDef,
-    FileCacheFailureDetailsOutputTypeDef,
+    FileCacheFailureDetailsTypeDef,
     FileCacheNFSConfigurationTypeDef,
     FileCacheLustreMetadataConfigurationOutputTypeDef,
-    LustreLogConfigurationOutputTypeDef,
-    FileSystemEndpointOutputTypeDef,
-    FileSystemFailureDetailsOutputTypeDef,
-    LifecycleTransitionReasonOutputTypeDef,
+    LustreLogConfigurationTypeDef,
+    FileSystemEndpointTypeDef,
+    FileSystemFailureDetailsTypeDef,
+    LifecycleTransitionReasonTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LustreRootSquashConfigurationOutputTypeDef,
     TieringPolicyOutputTypeDef,
     OpenZFSClientConfigurationOutputTypeDef,
     OpenZFSClientConfigurationTypeDef,
-    OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+    OpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaOutputTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
-    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     RetentionPeriodOutputTypeDef,
     RetentionPeriodTypeDef,
-    SelfManagedActiveDirectoryAttributesOutputTypeDef,
+    SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
-    SvmEndpointOutputTypeDef,
+    SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileSystemResponseOutputTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
-    WindowsAuditLogConfigurationOutputTypeDef,
-    AssociateFileSystemAliasesResponseOutputTypeDef,
-    DescribeFileSystemAliasesResponseOutputTypeDef,
-    DisassociateFileSystemAliasesResponseOutputTypeDef,
-    NFSDataRepositoryConfigurationOutputTypeDef,
+    WindowsAuditLogConfigurationTypeDef,
+    AssociateFileSystemAliasesResponseTypeDef,
+    DescribeFileSystemAliasesResponseTypeDef,
+    DisassociateFileSystemAliasesResponseTypeDef,
+    NFSDataRepositoryConfigurationTypeDef,
     S3DataRepositoryConfigurationOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
-    DeleteFileSystemLustreResponseOutputTypeDef,
-    DeleteFileSystemOpenZFSResponseOutputTypeDef,
-    DeleteFileSystemWindowsResponseOutputTypeDef,
-    DeleteVolumeOntapResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    DeleteFileSystemLustreResponseTypeDef,
+    DeleteFileSystemOpenZFSResponseTypeDef,
+    DeleteFileSystemWindowsResponseTypeDef,
+    DeleteVolumeOntapResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
@@ -474,101 +506,101 @@
     CreateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    DataRepositoryConfigurationOutputTypeDef,
+    DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
-    DataRepositoryTaskOutputTypeDef,
+    DataRepositoryTaskTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
-    OpenZFSFileSystemConfigurationOutputTypeDef,
+    OpenZFSFileSystemConfigurationTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
-    FileCacheLustreConfigurationOutputTypeDef,
-    FileSystemEndpointsOutputTypeDef,
-    SnapshotOutputTypeDef,
+    FileCacheLustreConfigurationTypeDef,
+    FileSystemEndpointsTypeDef,
+    SnapshotTypeDef,
     OpenZFSNfsExportOutputTypeDef,
     OpenZFSNfsExportTypeDef,
     SnaplockRetentionPeriodOutputTypeDef,
     SnaplockRetentionPeriodTypeDef,
-    SvmActiveDirectoryConfigurationOutputTypeDef,
+    SvmActiveDirectoryConfigurationTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    SvmEndpointsOutputTypeDef,
+    SvmEndpointsTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
-    WindowsFileSystemConfigurationOutputTypeDef,
-    DataRepositoryAssociationOutputTypeDef,
+    WindowsFileSystemConfigurationTypeDef,
+    DataRepositoryAssociationTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteFileSystemResponseOutputTypeDef,
-    DeleteVolumeResponseOutputTypeDef,
+    DeleteFileSystemResponseTypeDef,
+    DeleteVolumeResponseTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteVolumeRequestRequestTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    LustreFileSystemConfigurationOutputTypeDef,
-    CreateDataRepositoryTaskResponseOutputTypeDef,
-    DescribeDataRepositoryTasksResponseOutputTypeDef,
+    LustreFileSystemConfigurationTypeDef,
+    CreateDataRepositoryTaskResponseTypeDef,
+    DescribeDataRepositoryTasksResponseTypeDef,
     CreateFileCacheRequestRequestTypeDef,
-    FileCacheCreatingOutputTypeDef,
-    FileCacheOutputTypeDef,
-    OntapFileSystemConfigurationOutputTypeDef,
-    CreateSnapshotResponseOutputTypeDef,
-    DescribeSnapshotsResponseOutputTypeDef,
-    UpdateSnapshotResponseOutputTypeDef,
-    OpenZFSVolumeConfigurationOutputTypeDef,
+    FileCacheCreatingTypeDef,
+    FileCacheTypeDef,
+    OntapFileSystemConfigurationTypeDef,
+    CreateSnapshotResponseTypeDef,
+    DescribeSnapshotsResponseTypeDef,
+    UpdateSnapshotResponseTypeDef,
+    OpenZFSVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    SnaplockConfigurationOutputTypeDef,
+    SnaplockConfigurationTypeDef,
     CreateSnaplockConfigurationTypeDef,
     UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
-    StorageVirtualMachineOutputTypeDef,
-    CreateDataRepositoryAssociationResponseOutputTypeDef,
-    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
-    UpdateDataRepositoryAssociationResponseOutputTypeDef,
-    CreateFileCacheResponseOutputTypeDef,
-    DescribeFileCachesResponseOutputTypeDef,
-    UpdateFileCacheResponseOutputTypeDef,
-    FileSystemOutputTypeDef,
+    StorageVirtualMachineTypeDef,
+    CreateDataRepositoryAssociationResponseTypeDef,
+    DescribeDataRepositoryAssociationsResponseTypeDef,
+    UpdateDataRepositoryAssociationResponseTypeDef,
+    CreateFileCacheResponseTypeDef,
+    DescribeFileCachesResponseTypeDef,
+    UpdateFileCacheResponseTypeDef,
+    FileSystemTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    OntapVolumeConfigurationOutputTypeDef,
+    OntapVolumeConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
-    CreateStorageVirtualMachineResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    UpdateStorageVirtualMachineResponseOutputTypeDef,
+    CreateStorageVirtualMachineResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    UpdateStorageVirtualMachineResponseTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
-    VolumeOutputTypeDef,
+    VolumeTypeDef,
     CreateVolumeFromBackupRequestRequestTypeDef,
     CreateVolumeRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
-    AdministrativeActionOutputTypeDef,
-    BackupOutputTypeDef,
-    CreateVolumeFromBackupResponseOutputTypeDef,
-    CreateVolumeResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
-    UpdateVolumeResponseOutputTypeDef,
-    CopyBackupResponseOutputTypeDef,
-    CreateBackupResponseOutputTypeDef,
-    DescribeBackupsResponseOutputTypeDef,
+    AdministrativeActionTypeDef,
+    BackupTypeDef,
+    CreateVolumeFromBackupResponseTypeDef,
+    CreateVolumeResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
+    UpdateVolumeResponseTypeDef,
+    CopyBackupResponseTypeDef,
+    CreateBackupResponseTypeDef,
+    DescribeBackupsResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryBackupAttributesOutputTypeDef:
+def get_structure() -> ActiveDirectoryBackupAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.py` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.pyi` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__main__.py` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FSx 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
-        " 7.14.7\nDocs:           "
+        "Type annotations for boto3.FSx 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
+        " 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.py` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,102 +30,99 @@
     DescribeBackupsPaginator,
     DescribeFileSystemsPaginator,
     DescribeStorageVirtualMachinesPaginator,
     DescribeVolumesPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AssociateFileSystemAliasesResponseOutputTypeDef,
-    CancelDataRepositoryTaskResponseOutputTypeDef,
+    AssociateFileSystemAliasesResponseTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
-    CopyBackupResponseOutputTypeDef,
-    CreateBackupResponseOutputTypeDef,
-    CreateDataRepositoryAssociationResponseOutputTypeDef,
-    CreateDataRepositoryTaskResponseOutputTypeDef,
+    CopyBackupResponseTypeDef,
+    CreateBackupResponseTypeDef,
+    CreateDataRepositoryAssociationResponseTypeDef,
+    CreateDataRepositoryTaskResponseTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
-    CreateFileCacheResponseOutputTypeDef,
-    CreateFileSystemFromBackupResponseOutputTypeDef,
+    CreateFileCacheResponseTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    CreateFileSystemResponseOutputTypeDef,
+    CreateFileSystemResponseTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
-    CreateSnapshotResponseOutputTypeDef,
-    CreateStorageVirtualMachineResponseOutputTypeDef,
+    CreateSnapshotResponseTypeDef,
+    CreateStorageVirtualMachineResponseTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
-    CreateVolumeFromBackupResponseOutputTypeDef,
-    CreateVolumeResponseOutputTypeDef,
+    CreateVolumeFromBackupResponseTypeDef,
+    CreateVolumeResponseTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DeleteBackupResponseOutputTypeDef,
-    DeleteDataRepositoryAssociationResponseOutputTypeDef,
-    DeleteFileCacheResponseOutputTypeDef,
+    DeleteBackupResponseTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemResponseOutputTypeDef,
+    DeleteFileSystemResponseTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteSnapshotResponseOutputTypeDef,
-    DeleteStorageVirtualMachineResponseOutputTypeDef,
+    DeleteSnapshotResponseTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
-    DeleteVolumeResponseOutputTypeDef,
-    DescribeBackupsResponseOutputTypeDef,
-    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
-    DescribeDataRepositoryTasksResponseOutputTypeDef,
-    DescribeFileCachesResponseOutputTypeDef,
-    DescribeFileSystemAliasesResponseOutputTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
-    DescribeSnapshotsResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
-    DisassociateFileSystemAliasesResponseOutputTypeDef,
+    DeleteVolumeResponseTypeDef,
+    DescribeBackupsResponseTypeDef,
+    DescribeDataRepositoryAssociationsResponseTypeDef,
+    DescribeDataRepositoryTasksResponseTypeDef,
+    DescribeFileCachesResponseTypeDef,
+    DescribeFileSystemAliasesResponseTypeDef,
+    DescribeFileSystemsResponseTypeDef,
+    DescribeSnapshotsResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
+    DisassociateFileSystemAliasesResponseTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
-    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     TagTypeDef,
-    UpdateDataRepositoryAssociationResponseOutputTypeDef,
+    UpdateDataRepositoryAssociationResponseTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileCacheResponseOutputTypeDef,
+    UpdateFileCacheResponseTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
-    UpdateFileSystemResponseOutputTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    UpdateSnapshotResponseOutputTypeDef,
-    UpdateStorageVirtualMachineResponseOutputTypeDef,
+    UpdateSnapshotResponseTypeDef,
+    UpdateStorageVirtualMachineResponseTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    UpdateVolumeResponseOutputTypeDef,
+    UpdateVolumeResponseTypeDef,
     VolumeFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FSxClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ActiveDirectoryError: Type[BotocoreClientError]
     BackupBeingCopied: Type[BotocoreClientError]
     BackupInProgress: Type[BotocoreClientError]
     BackupNotFound: Type[BotocoreClientError]
     BackupRestoring: Type[BotocoreClientError]
     BadRequest: Type[BotocoreClientError]
@@ -156,15 +153,14 @@
     ServiceLimitExceeded: Type[BotocoreClientError]
     SnapshotNotFound: Type[BotocoreClientError]
     SourceBackupUnavailable: Type[BotocoreClientError]
     StorageVirtualMachineNotFound: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
     VolumeNotFound: Type[BotocoreClientError]
 
-
 class FSxClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/)
     """
 
     meta: ClientMeta
@@ -173,148 +169,138 @@
     def exceptions(self) -> Exceptions:
         """
         FSxClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#exceptions)
         """
-
     def associate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> AssociateFileSystemAliasesResponseOutputTypeDef:
+    ) -> AssociateFileSystemAliasesResponseTypeDef:
         """
         Use this action to associate one or more Domain Name Server (DNS) aliases with
         an existing Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.associate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#associate_file_system_aliases)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#can_paginate)
         """
-
     def cancel_data_repository_task(
         self, *, TaskId: str
-    ) -> CancelDataRepositoryTaskResponseOutputTypeDef:
+    ) -> CancelDataRepositoryTaskResponseTypeDef:
         """
         Cancels an existing Amazon FSx for Lustre data repository task if that task is
         in either the `PENDING` or `EXECUTING` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.cancel_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#cancel_data_repository_task)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#close)
         """
-
     def copy_backup(
         self,
         *,
         SourceBackupId: str,
         ClientRequestToken: str = ...,
         SourceRegion: str = ...,
         KmsKeyId: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CopyBackupResponseOutputTypeDef:
+    ) -> CopyBackupResponseTypeDef:
         """
         Copies an existing backup within the same Amazon Web Services account to another
         Amazon Web Services Region (cross-Region copy) or within the same Amazon Web
         Services Region (in-Region copy).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.copy_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#copy_backup)
         """
-
     def create_backup(
         self,
         *,
         FileSystemId: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VolumeId: str = ...
-    ) -> CreateBackupResponseOutputTypeDef:
+    ) -> CreateBackupResponseTypeDef:
         """
         Creates a backup of an existing Amazon FSx for Windows File Server file system,
         Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or Amazon
         FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_backup)
         """
-
     def create_data_repository_association(
         self,
         *,
         FileSystemId: str,
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDataRepositoryAssociationResponseOutputTypeDef:
+    ) -> CreateDataRepositoryAssociationResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_association)
         """
-
     def create_data_repository_task(
         self,
         *,
         Type: DataRepositoryTaskTypeType,
         FileSystemId: str,
         Report: CompletionReportTypeDef,
         Paths: Sequence[str] = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CapacityToRelease: int = ...
-    ) -> CreateDataRepositoryTaskResponseOutputTypeDef:
+    ) -> CreateDataRepositoryTaskResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_task)
         """
-
     def create_file_cache(
         self,
         *,
         FileCacheType: Literal["LUSTRE"],
         FileCacheTypeVersion: str,
         StorageCapacity: int,
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToDataRepositoryAssociations: bool = ...,
         KmsKeyId: str = ...,
         LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,
         DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...
-    ) -> CreateFileCacheResponseOutputTypeDef:
+    ) -> CreateFileCacheResponseTypeDef:
         """
         Creates a new Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_cache)
         """
-
     def create_file_system(
         self,
         *,
         FileSystemType: FileSystemTypeType,
         StorageCapacity: int,
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
@@ -323,22 +309,21 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> CreateFileSystemResponseOutputTypeDef:
+    ) -> CreateFileSystemResponseTypeDef:
         """
         Creates a new, empty Amazon FSx file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system)
         """
-
     def create_file_system_from_backup(
         self,
         *,
         BackupId: str,
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -346,515 +331,477 @@
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         StorageType: StorageTypeType = ...,
         KmsKeyId: str = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
         StorageCapacity: int = ...
-    ) -> CreateFileSystemFromBackupResponseOutputTypeDef:
+    ) -> CreateFileSystemFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
         Amazon FSx for OpenZFS file system from an existing Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system_from_backup)
         """
-
     def create_snapshot(
         self,
         *,
         Name: str,
         VolumeId: str,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSnapshotResponseOutputTypeDef:
+    ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a snapshot of an existing Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_snapshot)
         """
-
     def create_storage_virtual_machine(
         self,
         *,
         FileSystemId: str,
         Name: str,
         ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...
-    ) -> CreateStorageVirtualMachineResponseOutputTypeDef:
+    ) -> CreateStorageVirtualMachineResponseTypeDef:
         """
         Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_storage_virtual_machine)
         """
-
     def create_volume(
         self,
         *,
         VolumeType: VolumeTypeType,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> CreateVolumeResponseOutputTypeDef:
+    ) -> CreateVolumeResponseTypeDef:
         """
         Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume)
         """
-
     def create_volume_from_backup(
         self,
         *,
         BackupId: str,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVolumeFromBackupResponseOutputTypeDef:
+    ) -> CreateVolumeFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
         volume backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume_from_backup)
         """
-
     def delete_backup(
         self, *, BackupId: str, ClientRequestToken: str = ...
-    ) -> DeleteBackupResponseOutputTypeDef:
+    ) -> DeleteBackupResponseTypeDef:
         """
         Deletes an Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_backup)
         """
-
     def delete_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         DeleteDataInFileSystem: bool = ...
-    ) -> DeleteDataRepositoryAssociationResponseOutputTypeDef:
+    ) -> DeleteDataRepositoryAssociationResponseTypeDef:
         """
         Deletes a data repository association on an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_data_repository_association)
         """
-
     def delete_file_cache(
         self, *, FileCacheId: str, ClientRequestToken: str = ...
-    ) -> DeleteFileCacheResponseOutputTypeDef:
+    ) -> DeleteFileCacheResponseTypeDef:
         """
         Deletes an Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_cache)
         """
-
     def delete_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteFileSystemResponseOutputTypeDef:
+    ) -> DeleteFileSystemResponseTypeDef:
         """
         Deletes a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_system)
         """
-
     def delete_snapshot(
         self, *, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> DeleteSnapshotResponseOutputTypeDef:
+    ) -> DeleteSnapshotResponseTypeDef:
         """
         Deletes an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_snapshot)
         """
-
     def delete_storage_virtual_machine(
         self, *, StorageVirtualMachineId: str, ClientRequestToken: str = ...
-    ) -> DeleteStorageVirtualMachineResponseOutputTypeDef:
+    ) -> DeleteStorageVirtualMachineResponseTypeDef:
         """
         Deletes an existing Amazon FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_storage_virtual_machine)
         """
-
     def delete_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteVolumeResponseOutputTypeDef:
+    ) -> DeleteVolumeResponseTypeDef:
         """
         Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_volume)
         """
-
     def describe_backups(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeBackupsResponseOutputTypeDef:
+    ) -> DescribeBackupsResponseTypeDef:
         """
         Returns the description of a specific Amazon FSx backup, if a `BackupIds` value
         is provided for that backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_backups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_backups)
         """
-
     def describe_data_repository_associations(
         self,
         *,
         AssociationIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryAssociationsResponseOutputTypeDef:
+    ) -> DescribeDataRepositoryAssociationsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository associations, if one or more `AssociationIds` values are
         provided in the request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_associations)
         """
-
     def describe_data_repository_tasks(
         self,
         *,
         TaskIds: Sequence[str] = ...,
         Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryTasksResponseOutputTypeDef:
+    ) -> DescribeDataRepositoryTasksResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository tasks, if one or more `TaskIds` values are provided in the
         request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_tasks)
         """
-
     def describe_file_caches(
         self, *, FileCacheIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileCachesResponseOutputTypeDef:
+    ) -> DescribeFileCachesResponseTypeDef:
         """
         Returns the description of a specific Amazon File Cache resource, if a
         `FileCacheIds` value is provided for that cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_caches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_caches)
         """
-
     def describe_file_system_aliases(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeFileSystemAliasesResponseOutputTypeDef:
+    ) -> DescribeFileSystemAliasesResponseTypeDef:
         """
         Returns the DNS aliases that are associated with the specified Amazon FSx for
         Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_system_aliases)
         """
-
     def describe_file_systems(
         self, *, FileSystemIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileSystemsResponseOutputTypeDef:
+    ) -> DescribeFileSystemsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx file systems, if a
         `FileSystemIds` value is provided for that file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_systems)
         """
-
     def describe_snapshots(
         self,
         *,
         SnapshotIds: Sequence[str] = ...,
         Filters: Sequence[SnapshotFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeSnapshotsResponseOutputTypeDef:
+    ) -> DescribeSnapshotsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
         `SnapshotIds` value is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_snapshots)
         """
-
     def describe_storage_virtual_machines(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageVirtualMachinesResponseOutputTypeDef:
+    ) -> DescribeStorageVirtualMachinesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
         (SVMs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_storage_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_storage_virtual_machines)
         """
-
     def describe_volumes(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeVolumesResponseOutputTypeDef:
+    ) -> DescribeVolumesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
         volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_volumes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_volumes)
         """
-
     def disassociate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> DisassociateFileSystemAliasesResponseOutputTypeDef:
+    ) -> DisassociateFileSystemAliasesResponseTypeDef:
         """
         Use this action to disassociate, or remove, one or more Domain Name Service
         (DNS) aliases from an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.disassociate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#disassociate_file_system_aliases)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#generate_presigned_url)
         """
-
     def list_tags_for_resource(
         self, *, ResourceARN: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists tags for Amazon FSx resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#list_tags_for_resource)
         """
-
     def release_file_system_nfs_v3_locks(
         self, *, FileSystemId: str, ClientRequestToken: str = ...
-    ) -> ReleaseFileSystemNfsV3LocksResponseOutputTypeDef:
+    ) -> ReleaseFileSystemNfsV3LocksResponseTypeDef:
         """
         Releases the file system lock from an Amazon FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.release_file_system_nfs_v3_locks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#release_file_system_nfs_v3_locks)
         """
-
     def restore_volume_from_snapshot(
         self,
         *,
         VolumeId: str,
         SnapshotId: str,
         ClientRequestToken: str = ...,
         Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...
-    ) -> RestoreVolumeFromSnapshotResponseOutputTypeDef:
+    ) -> RestoreVolumeFromSnapshotResponseTypeDef:
         """
         Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.restore_volume_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#restore_volume_from_snapshot)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags an Amazon FSx resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         This action removes a tag from an Amazon FSx resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#untag_resource)
         """
-
     def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...
-    ) -> UpdateDataRepositoryAssociationResponseOutputTypeDef:
+    ) -> UpdateDataRepositoryAssociationResponseTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_data_repository_association)
         """
-
     def update_file_cache(
         self,
         *,
         FileCacheId: str,
         ClientRequestToken: str = ...,
         LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...
-    ) -> UpdateFileCacheResponseOutputTypeDef:
+    ) -> UpdateFileCacheResponseTypeDef:
         """
         Updates the configuration of an existing Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_cache)
         """
-
     def update_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         StorageCapacity: int = ...,
         WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> UpdateFileSystemResponseOutputTypeDef:
+    ) -> UpdateFileSystemResponseTypeDef:
         """
         Use this operation to update the configuration of an existing Amazon FSx file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_system)
         """
-
     def update_snapshot(
         self, *, Name: str, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> UpdateSnapshotResponseOutputTypeDef:
+    ) -> UpdateSnapshotResponseTypeDef:
         """
         Updates the name of an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_snapshot)
         """
-
     def update_storage_virtual_machine(
         self,
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...
-    ) -> UpdateStorageVirtualMachineResponseOutputTypeDef:
+    ) -> UpdateStorageVirtualMachineResponseTypeDef:
         """
         Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_storage_virtual_machine)
         """
-
     def update_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,
         Name: str = ...,
         OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> UpdateVolumeResponseOutputTypeDef:
+    ) -> UpdateVolumeResponseTypeDef:
         """
         Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
         OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_volume)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_backups"]
     ) -> DescribeBackupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_file_systems"]
     ) -> DescribeFileSystemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_storage_virtual_machines"]
     ) -> DescribeStorageVirtualMachinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_volumes"]
     ) -> DescribeVolumesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.pyi` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,99 +30,102 @@
     DescribeBackupsPaginator,
     DescribeFileSystemsPaginator,
     DescribeStorageVirtualMachinesPaginator,
     DescribeVolumesPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AssociateFileSystemAliasesResponseOutputTypeDef,
-    CancelDataRepositoryTaskResponseOutputTypeDef,
+    AssociateFileSystemAliasesResponseTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
-    CopyBackupResponseOutputTypeDef,
-    CreateBackupResponseOutputTypeDef,
-    CreateDataRepositoryAssociationResponseOutputTypeDef,
-    CreateDataRepositoryTaskResponseOutputTypeDef,
+    CopyBackupResponseTypeDef,
+    CreateBackupResponseTypeDef,
+    CreateDataRepositoryAssociationResponseTypeDef,
+    CreateDataRepositoryTaskResponseTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
-    CreateFileCacheResponseOutputTypeDef,
-    CreateFileSystemFromBackupResponseOutputTypeDef,
+    CreateFileCacheResponseTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    CreateFileSystemResponseOutputTypeDef,
+    CreateFileSystemResponseTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
-    CreateSnapshotResponseOutputTypeDef,
-    CreateStorageVirtualMachineResponseOutputTypeDef,
+    CreateSnapshotResponseTypeDef,
+    CreateStorageVirtualMachineResponseTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
-    CreateVolumeFromBackupResponseOutputTypeDef,
-    CreateVolumeResponseOutputTypeDef,
+    CreateVolumeFromBackupResponseTypeDef,
+    CreateVolumeResponseTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DeleteBackupResponseOutputTypeDef,
-    DeleteDataRepositoryAssociationResponseOutputTypeDef,
-    DeleteFileCacheResponseOutputTypeDef,
+    DeleteBackupResponseTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemResponseOutputTypeDef,
+    DeleteFileSystemResponseTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteSnapshotResponseOutputTypeDef,
-    DeleteStorageVirtualMachineResponseOutputTypeDef,
+    DeleteSnapshotResponseTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
-    DeleteVolumeResponseOutputTypeDef,
-    DescribeBackupsResponseOutputTypeDef,
-    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
-    DescribeDataRepositoryTasksResponseOutputTypeDef,
-    DescribeFileCachesResponseOutputTypeDef,
-    DescribeFileSystemAliasesResponseOutputTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
-    DescribeSnapshotsResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
-    DisassociateFileSystemAliasesResponseOutputTypeDef,
+    DeleteVolumeResponseTypeDef,
+    DescribeBackupsResponseTypeDef,
+    DescribeDataRepositoryAssociationsResponseTypeDef,
+    DescribeDataRepositoryTasksResponseTypeDef,
+    DescribeFileCachesResponseTypeDef,
+    DescribeFileSystemAliasesResponseTypeDef,
+    DescribeFileSystemsResponseTypeDef,
+    DescribeSnapshotsResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
+    DisassociateFileSystemAliasesResponseTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
-    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     TagTypeDef,
-    UpdateDataRepositoryAssociationResponseOutputTypeDef,
+    UpdateDataRepositoryAssociationResponseTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileCacheResponseOutputTypeDef,
+    UpdateFileCacheResponseTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
-    UpdateFileSystemResponseOutputTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    UpdateSnapshotResponseOutputTypeDef,
-    UpdateStorageVirtualMachineResponseOutputTypeDef,
+    UpdateSnapshotResponseTypeDef,
+    UpdateStorageVirtualMachineResponseTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    UpdateVolumeResponseOutputTypeDef,
+    UpdateVolumeResponseTypeDef,
     VolumeFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("FSxClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ActiveDirectoryError: Type[BotocoreClientError]
     BackupBeingCopied: Type[BotocoreClientError]
     BackupInProgress: Type[BotocoreClientError]
     BackupNotFound: Type[BotocoreClientError]
     BackupRestoring: Type[BotocoreClientError]
     BadRequest: Type[BotocoreClientError]
@@ -153,14 +156,15 @@
     ServiceLimitExceeded: Type[BotocoreClientError]
     SnapshotNotFound: Type[BotocoreClientError]
     SourceBackupUnavailable: Type[BotocoreClientError]
     StorageVirtualMachineNotFound: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
     VolumeNotFound: Type[BotocoreClientError]
 
+
 class FSxClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/)
     """
 
     meta: ClientMeta
@@ -169,138 +173,148 @@
     def exceptions(self) -> Exceptions:
         """
         FSxClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#exceptions)
         """
+
     def associate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> AssociateFileSystemAliasesResponseOutputTypeDef:
+    ) -> AssociateFileSystemAliasesResponseTypeDef:
         """
         Use this action to associate one or more Domain Name Server (DNS) aliases with
         an existing Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.associate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#associate_file_system_aliases)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#can_paginate)
         """
+
     def cancel_data_repository_task(
         self, *, TaskId: str
-    ) -> CancelDataRepositoryTaskResponseOutputTypeDef:
+    ) -> CancelDataRepositoryTaskResponseTypeDef:
         """
         Cancels an existing Amazon FSx for Lustre data repository task if that task is
         in either the `PENDING` or `EXECUTING` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.cancel_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#cancel_data_repository_task)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#close)
         """
+
     def copy_backup(
         self,
         *,
         SourceBackupId: str,
         ClientRequestToken: str = ...,
         SourceRegion: str = ...,
         KmsKeyId: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CopyBackupResponseOutputTypeDef:
+    ) -> CopyBackupResponseTypeDef:
         """
         Copies an existing backup within the same Amazon Web Services account to another
         Amazon Web Services Region (cross-Region copy) or within the same Amazon Web
         Services Region (in-Region copy).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.copy_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#copy_backup)
         """
+
     def create_backup(
         self,
         *,
         FileSystemId: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VolumeId: str = ...
-    ) -> CreateBackupResponseOutputTypeDef:
+    ) -> CreateBackupResponseTypeDef:
         """
         Creates a backup of an existing Amazon FSx for Windows File Server file system,
         Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or Amazon
         FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_backup)
         """
+
     def create_data_repository_association(
         self,
         *,
         FileSystemId: str,
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDataRepositoryAssociationResponseOutputTypeDef:
+    ) -> CreateDataRepositoryAssociationResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_association)
         """
+
     def create_data_repository_task(
         self,
         *,
         Type: DataRepositoryTaskTypeType,
         FileSystemId: str,
         Report: CompletionReportTypeDef,
         Paths: Sequence[str] = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CapacityToRelease: int = ...
-    ) -> CreateDataRepositoryTaskResponseOutputTypeDef:
+    ) -> CreateDataRepositoryTaskResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_task)
         """
+
     def create_file_cache(
         self,
         *,
         FileCacheType: Literal["LUSTRE"],
         FileCacheTypeVersion: str,
         StorageCapacity: int,
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToDataRepositoryAssociations: bool = ...,
         KmsKeyId: str = ...,
         LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,
         DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...
-    ) -> CreateFileCacheResponseOutputTypeDef:
+    ) -> CreateFileCacheResponseTypeDef:
         """
         Creates a new Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_cache)
         """
+
     def create_file_system(
         self,
         *,
         FileSystemType: FileSystemTypeType,
         StorageCapacity: int,
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
@@ -309,21 +323,22 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> CreateFileSystemResponseOutputTypeDef:
+    ) -> CreateFileSystemResponseTypeDef:
         """
         Creates a new, empty Amazon FSx file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system)
         """
+
     def create_file_system_from_backup(
         self,
         *,
         BackupId: str,
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -331,477 +346,515 @@
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         StorageType: StorageTypeType = ...,
         KmsKeyId: str = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
         StorageCapacity: int = ...
-    ) -> CreateFileSystemFromBackupResponseOutputTypeDef:
+    ) -> CreateFileSystemFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
         Amazon FSx for OpenZFS file system from an existing Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system_from_backup)
         """
+
     def create_snapshot(
         self,
         *,
         Name: str,
         VolumeId: str,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSnapshotResponseOutputTypeDef:
+    ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a snapshot of an existing Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_snapshot)
         """
+
     def create_storage_virtual_machine(
         self,
         *,
         FileSystemId: str,
         Name: str,
         ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...
-    ) -> CreateStorageVirtualMachineResponseOutputTypeDef:
+    ) -> CreateStorageVirtualMachineResponseTypeDef:
         """
         Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_storage_virtual_machine)
         """
+
     def create_volume(
         self,
         *,
         VolumeType: VolumeTypeType,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> CreateVolumeResponseOutputTypeDef:
+    ) -> CreateVolumeResponseTypeDef:
         """
         Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume)
         """
+
     def create_volume_from_backup(
         self,
         *,
         BackupId: str,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVolumeFromBackupResponseOutputTypeDef:
+    ) -> CreateVolumeFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
         volume backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume_from_backup)
         """
+
     def delete_backup(
         self, *, BackupId: str, ClientRequestToken: str = ...
-    ) -> DeleteBackupResponseOutputTypeDef:
+    ) -> DeleteBackupResponseTypeDef:
         """
         Deletes an Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_backup)
         """
+
     def delete_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         DeleteDataInFileSystem: bool = ...
-    ) -> DeleteDataRepositoryAssociationResponseOutputTypeDef:
+    ) -> DeleteDataRepositoryAssociationResponseTypeDef:
         """
         Deletes a data repository association on an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_data_repository_association)
         """
+
     def delete_file_cache(
         self, *, FileCacheId: str, ClientRequestToken: str = ...
-    ) -> DeleteFileCacheResponseOutputTypeDef:
+    ) -> DeleteFileCacheResponseTypeDef:
         """
         Deletes an Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_cache)
         """
+
     def delete_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteFileSystemResponseOutputTypeDef:
+    ) -> DeleteFileSystemResponseTypeDef:
         """
         Deletes a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_system)
         """
+
     def delete_snapshot(
         self, *, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> DeleteSnapshotResponseOutputTypeDef:
+    ) -> DeleteSnapshotResponseTypeDef:
         """
         Deletes an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_snapshot)
         """
+
     def delete_storage_virtual_machine(
         self, *, StorageVirtualMachineId: str, ClientRequestToken: str = ...
-    ) -> DeleteStorageVirtualMachineResponseOutputTypeDef:
+    ) -> DeleteStorageVirtualMachineResponseTypeDef:
         """
         Deletes an existing Amazon FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_storage_virtual_machine)
         """
+
     def delete_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteVolumeResponseOutputTypeDef:
+    ) -> DeleteVolumeResponseTypeDef:
         """
         Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_volume)
         """
+
     def describe_backups(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeBackupsResponseOutputTypeDef:
+    ) -> DescribeBackupsResponseTypeDef:
         """
         Returns the description of a specific Amazon FSx backup, if a `BackupIds` value
         is provided for that backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_backups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_backups)
         """
+
     def describe_data_repository_associations(
         self,
         *,
         AssociationIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryAssociationsResponseOutputTypeDef:
+    ) -> DescribeDataRepositoryAssociationsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository associations, if one or more `AssociationIds` values are
         provided in the request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_associations)
         """
+
     def describe_data_repository_tasks(
         self,
         *,
         TaskIds: Sequence[str] = ...,
         Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryTasksResponseOutputTypeDef:
+    ) -> DescribeDataRepositoryTasksResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository tasks, if one or more `TaskIds` values are provided in the
         request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_tasks)
         """
+
     def describe_file_caches(
         self, *, FileCacheIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileCachesResponseOutputTypeDef:
+    ) -> DescribeFileCachesResponseTypeDef:
         """
         Returns the description of a specific Amazon File Cache resource, if a
         `FileCacheIds` value is provided for that cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_caches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_caches)
         """
+
     def describe_file_system_aliases(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeFileSystemAliasesResponseOutputTypeDef:
+    ) -> DescribeFileSystemAliasesResponseTypeDef:
         """
         Returns the DNS aliases that are associated with the specified Amazon FSx for
         Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_system_aliases)
         """
+
     def describe_file_systems(
         self, *, FileSystemIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileSystemsResponseOutputTypeDef:
+    ) -> DescribeFileSystemsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx file systems, if a
         `FileSystemIds` value is provided for that file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_systems)
         """
+
     def describe_snapshots(
         self,
         *,
         SnapshotIds: Sequence[str] = ...,
         Filters: Sequence[SnapshotFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeSnapshotsResponseOutputTypeDef:
+    ) -> DescribeSnapshotsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
         `SnapshotIds` value is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_snapshots)
         """
+
     def describe_storage_virtual_machines(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageVirtualMachinesResponseOutputTypeDef:
+    ) -> DescribeStorageVirtualMachinesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
         (SVMs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_storage_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_storage_virtual_machines)
         """
+
     def describe_volumes(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeVolumesResponseOutputTypeDef:
+    ) -> DescribeVolumesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
         volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_volumes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_volumes)
         """
+
     def disassociate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> DisassociateFileSystemAliasesResponseOutputTypeDef:
+    ) -> DisassociateFileSystemAliasesResponseTypeDef:
         """
         Use this action to disassociate, or remove, one or more Domain Name Service
         (DNS) aliases from an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.disassociate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#disassociate_file_system_aliases)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#generate_presigned_url)
         """
+
     def list_tags_for_resource(
         self, *, ResourceARN: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists tags for Amazon FSx resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#list_tags_for_resource)
         """
+
     def release_file_system_nfs_v3_locks(
         self, *, FileSystemId: str, ClientRequestToken: str = ...
-    ) -> ReleaseFileSystemNfsV3LocksResponseOutputTypeDef:
+    ) -> ReleaseFileSystemNfsV3LocksResponseTypeDef:
         """
         Releases the file system lock from an Amazon FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.release_file_system_nfs_v3_locks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#release_file_system_nfs_v3_locks)
         """
+
     def restore_volume_from_snapshot(
         self,
         *,
         VolumeId: str,
         SnapshotId: str,
         ClientRequestToken: str = ...,
         Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...
-    ) -> RestoreVolumeFromSnapshotResponseOutputTypeDef:
+    ) -> RestoreVolumeFromSnapshotResponseTypeDef:
         """
         Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.restore_volume_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#restore_volume_from_snapshot)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags an Amazon FSx resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         This action removes a tag from an Amazon FSx resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#untag_resource)
         """
+
     def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...
-    ) -> UpdateDataRepositoryAssociationResponseOutputTypeDef:
+    ) -> UpdateDataRepositoryAssociationResponseTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_data_repository_association)
         """
+
     def update_file_cache(
         self,
         *,
         FileCacheId: str,
         ClientRequestToken: str = ...,
         LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...
-    ) -> UpdateFileCacheResponseOutputTypeDef:
+    ) -> UpdateFileCacheResponseTypeDef:
         """
         Updates the configuration of an existing Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_cache)
         """
+
     def update_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         StorageCapacity: int = ...,
         WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> UpdateFileSystemResponseOutputTypeDef:
+    ) -> UpdateFileSystemResponseTypeDef:
         """
         Use this operation to update the configuration of an existing Amazon FSx file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_system)
         """
+
     def update_snapshot(
         self, *, Name: str, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> UpdateSnapshotResponseOutputTypeDef:
+    ) -> UpdateSnapshotResponseTypeDef:
         """
         Updates the name of an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_snapshot)
         """
+
     def update_storage_virtual_machine(
         self,
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...
-    ) -> UpdateStorageVirtualMachineResponseOutputTypeDef:
+    ) -> UpdateStorageVirtualMachineResponseTypeDef:
         """
         Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_storage_virtual_machine)
         """
+
     def update_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,
         Name: str = ...,
         OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> UpdateVolumeResponseOutputTypeDef:
+    ) -> UpdateVolumeResponseTypeDef:
         """
         Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
         OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_volume)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_backups"]
     ) -> DescribeBackupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_file_systems"]
     ) -> DescribeFileSystemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_storage_virtual_machines"]
     ) -> DescribeStorageVirtualMachinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_volumes"]
     ) -> DescribeVolumesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#get_paginator)
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.py` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.pyi` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.py` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeBackupsResponseOutputTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
+    DescribeBackupsResponseTypeDef,
+    DescribeFileSystemsResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
 )
 
 __all__ = (
     "DescribeBackupsPaginator",
@@ -70,15 +70,15 @@
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeBackupsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describebackupspaginator)
         """
 
 
 class DescribeFileSystemsPaginator(Paginator):
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         FileSystemIds: Sequence[str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeFileSystemsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
         """
 
 
 class DescribeStorageVirtualMachinesPaginator(Paginator):
@@ -107,15 +107,15 @@
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
 
 class DescribeVolumesPaginator(Paginator):
@@ -126,27 +126,27 @@
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeVolumesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeVolumesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describevolumespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.pyi` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeBackupsResponseOutputTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
+    DescribeBackupsResponseTypeDef,
+    DescribeFileSystemsResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
 )
 
 __all__ = (
     "DescribeBackupsPaginator",
@@ -67,15 +67,15 @@
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeBackupsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describebackupspaginator)
         """
 
 class DescribeFileSystemsPaginator(Paginator):
     """
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         FileSystemIds: Sequence[str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeFileSystemsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
         """
 
 class DescribeStorageVirtualMachinesPaginator(Paginator):
     """
@@ -102,15 +102,15 @@
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
 class DescribeVolumesPaginator(Paginator):
     """
@@ -120,26 +120,26 @@
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeVolumesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeVolumesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describevolumespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.py` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for fsx service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesOutputTypeDef
+    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesTypeDef
 
-    data: ActiveDirectoryBackupAttributesOutputTypeDef = {...}
+    data: ActiveDirectoryBackupAttributesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
@@ -73,110 +73,110 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActiveDirectoryBackupAttributesOutputTypeDef",
-    "AdministrativeActionFailureDetailsOutputTypeDef",
-    "AliasOutputTypeDef",
+    "ActiveDirectoryBackupAttributesTypeDef",
+    "AdministrativeActionFailureDetailsTypeDef",
+    "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "AutoExportPolicyOutputTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyOutputTypeDef",
     "AutoImportPolicyTypeDef",
     "AutocommitPeriodOutputTypeDef",
     "AutocommitPeriodTypeDef",
-    "BackupFailureDetailsOutputTypeDef",
+    "BackupFailureDetailsTypeDef",
     "TagOutputTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
-    "CancelDataRepositoryTaskResponseOutputTypeDef",
+    "CancelDataRepositoryTaskResponseTypeDef",
     "CompletionReportOutputTypeDef",
     "CompletionReportTypeDef",
     "TagTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
-    "CreateFileSystemFromBackupResponseOutputTypeDef",
+    "CreateFileSystemFromBackupResponseTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
     "DiskIopsConfigurationTypeDef",
-    "CreateFileSystemResponseOutputTypeDef",
+    "CreateFileSystemResponseTypeDef",
     "SelfManagedActiveDirectoryConfigurationTypeDef",
     "WindowsAuditLogCreateConfigurationTypeDef",
     "TieringPolicyTypeDef",
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaTypeDef",
-    "DataRepositoryFailureDetailsOutputTypeDef",
-    "DataRepositoryTaskFailureDetailsOutputTypeDef",
+    "DataRepositoryFailureDetailsTypeDef",
+    "DataRepositoryTaskFailureDetailsTypeDef",
     "DataRepositoryTaskFilterTypeDef",
-    "DataRepositoryTaskStatusOutputTypeDef",
+    "DataRepositoryTaskStatusTypeDef",
     "DeleteBackupRequestRequestTypeDef",
-    "DeleteBackupResponseOutputTypeDef",
+    "DeleteBackupResponseTypeDef",
     "DeleteDataRepositoryAssociationRequestRequestTypeDef",
-    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
+    "DeleteDataRepositoryAssociationResponseTypeDef",
     "DeleteFileCacheRequestRequestTypeDef",
-    "DeleteFileCacheResponseOutputTypeDef",
+    "DeleteFileCacheResponseTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResponseOutputTypeDef",
+    "DeleteSnapshotResponseTypeDef",
     "DeleteStorageVirtualMachineRequestRequestTypeDef",
-    "DeleteStorageVirtualMachineResponseOutputTypeDef",
+    "DeleteStorageVirtualMachineResponseTypeDef",
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     "FilterTypeDef",
     "DescribeFileCachesRequestRequestTypeDef",
     "DescribeFileSystemAliasesRequestRequestTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
-    "DescribeFileSystemsResponseOutputTypeDef",
+    "DescribeFileSystemsResponseTypeDef",
     "SnapshotFilterTypeDef",
     "StorageVirtualMachineFilterTypeDef",
     "VolumeFilterTypeDef",
     "DisassociateFileSystemAliasesRequestRequestTypeDef",
     "DiskIopsConfigurationOutputTypeDef",
-    "FileCacheFailureDetailsOutputTypeDef",
+    "FileCacheFailureDetailsTypeDef",
     "FileCacheNFSConfigurationTypeDef",
     "FileCacheLustreMetadataConfigurationOutputTypeDef",
-    "LustreLogConfigurationOutputTypeDef",
-    "FileSystemEndpointOutputTypeDef",
-    "FileSystemFailureDetailsOutputTypeDef",
-    "LifecycleTransitionReasonOutputTypeDef",
+    "LustreLogConfigurationTypeDef",
+    "FileSystemEndpointTypeDef",
+    "FileSystemFailureDetailsTypeDef",
+    "LifecycleTransitionReasonTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LustreRootSquashConfigurationOutputTypeDef",
     "TieringPolicyOutputTypeDef",
     "OpenZFSClientConfigurationOutputTypeDef",
     "OpenZFSClientConfigurationTypeDef",
-    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
+    "OpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
-    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
-    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
+    "RestoreVolumeFromSnapshotResponseTypeDef",
     "RetentionPeriodOutputTypeDef",
     "RetentionPeriodTypeDef",
-    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
+    "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
-    "SvmEndpointOutputTypeDef",
+    "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
-    "UpdateFileSystemResponseOutputTypeDef",
+    "UpdateFileSystemResponseTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
-    "WindowsAuditLogConfigurationOutputTypeDef",
-    "AssociateFileSystemAliasesResponseOutputTypeDef",
-    "DescribeFileSystemAliasesResponseOutputTypeDef",
-    "DisassociateFileSystemAliasesResponseOutputTypeDef",
-    "NFSDataRepositoryConfigurationOutputTypeDef",
+    "WindowsAuditLogConfigurationTypeDef",
+    "AssociateFileSystemAliasesResponseTypeDef",
+    "DescribeFileSystemAliasesResponseTypeDef",
+    "DisassociateFileSystemAliasesResponseTypeDef",
+    "NFSDataRepositoryConfigurationTypeDef",
     "S3DataRepositoryConfigurationOutputTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
-    "DeleteFileSystemLustreResponseOutputTypeDef",
-    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
-    "DeleteFileSystemWindowsResponseOutputTypeDef",
-    "DeleteVolumeOntapResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "DeleteFileSystemLustreResponseTypeDef",
+    "DeleteFileSystemOpenZFSResponseTypeDef",
+    "DeleteFileSystemWindowsResponseTypeDef",
+    "DeleteVolumeOntapResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateDataRepositoryTaskRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
     "DeleteFileSystemWindowsConfigurationTypeDef",
@@ -186,117 +186,117 @@
     "CreateFileSystemLustreConfigurationTypeDef",
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "DataRepositoryConfigurationOutputTypeDef",
+    "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
-    "DataRepositoryTaskOutputTypeDef",
+    "DataRepositoryTaskTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
-    "OpenZFSFileSystemConfigurationOutputTypeDef",
+    "OpenZFSFileSystemConfigurationTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
-    "FileCacheLustreConfigurationOutputTypeDef",
-    "FileSystemEndpointsOutputTypeDef",
-    "SnapshotOutputTypeDef",
+    "FileCacheLustreConfigurationTypeDef",
+    "FileSystemEndpointsTypeDef",
+    "SnapshotTypeDef",
     "OpenZFSNfsExportOutputTypeDef",
     "OpenZFSNfsExportTypeDef",
     "SnaplockRetentionPeriodOutputTypeDef",
     "SnaplockRetentionPeriodTypeDef",
-    "SvmActiveDirectoryConfigurationOutputTypeDef",
+    "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
-    "SvmEndpointsOutputTypeDef",
+    "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
-    "WindowsFileSystemConfigurationOutputTypeDef",
-    "DataRepositoryAssociationOutputTypeDef",
+    "WindowsFileSystemConfigurationTypeDef",
+    "DataRepositoryAssociationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
-    "DeleteFileSystemResponseOutputTypeDef",
-    "DeleteVolumeResponseOutputTypeDef",
+    "DeleteFileSystemResponseTypeDef",
+    "DeleteVolumeResponseTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "LustreFileSystemConfigurationOutputTypeDef",
-    "CreateDataRepositoryTaskResponseOutputTypeDef",
-    "DescribeDataRepositoryTasksResponseOutputTypeDef",
+    "LustreFileSystemConfigurationTypeDef",
+    "CreateDataRepositoryTaskResponseTypeDef",
+    "DescribeDataRepositoryTasksResponseTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
-    "FileCacheCreatingOutputTypeDef",
-    "FileCacheOutputTypeDef",
-    "OntapFileSystemConfigurationOutputTypeDef",
-    "CreateSnapshotResponseOutputTypeDef",
-    "DescribeSnapshotsResponseOutputTypeDef",
-    "UpdateSnapshotResponseOutputTypeDef",
-    "OpenZFSVolumeConfigurationOutputTypeDef",
+    "FileCacheCreatingTypeDef",
+    "FileCacheTypeDef",
+    "OntapFileSystemConfigurationTypeDef",
+    "CreateSnapshotResponseTypeDef",
+    "DescribeSnapshotsResponseTypeDef",
+    "UpdateSnapshotResponseTypeDef",
+    "OpenZFSVolumeConfigurationTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
-    "SnaplockConfigurationOutputTypeDef",
+    "SnaplockConfigurationTypeDef",
     "CreateSnaplockConfigurationTypeDef",
     "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
-    "StorageVirtualMachineOutputTypeDef",
-    "CreateDataRepositoryAssociationResponseOutputTypeDef",
-    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
-    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
-    "CreateFileCacheResponseOutputTypeDef",
-    "DescribeFileCachesResponseOutputTypeDef",
-    "UpdateFileCacheResponseOutputTypeDef",
-    "FileSystemOutputTypeDef",
+    "StorageVirtualMachineTypeDef",
+    "CreateDataRepositoryAssociationResponseTypeDef",
+    "DescribeDataRepositoryAssociationsResponseTypeDef",
+    "UpdateDataRepositoryAssociationResponseTypeDef",
+    "CreateFileCacheResponseTypeDef",
+    "DescribeFileCachesResponseTypeDef",
+    "UpdateFileCacheResponseTypeDef",
+    "FileSystemTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
-    "OntapVolumeConfigurationOutputTypeDef",
+    "OntapVolumeConfigurationTypeDef",
     "CreateOntapVolumeConfigurationTypeDef",
     "UpdateOntapVolumeConfigurationTypeDef",
-    "CreateStorageVirtualMachineResponseOutputTypeDef",
-    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
-    "UpdateStorageVirtualMachineResponseOutputTypeDef",
+    "CreateStorageVirtualMachineResponseTypeDef",
+    "DescribeStorageVirtualMachinesResponseTypeDef",
+    "UpdateStorageVirtualMachineResponseTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
-    "VolumeOutputTypeDef",
+    "VolumeTypeDef",
     "CreateVolumeFromBackupRequestRequestTypeDef",
     "CreateVolumeRequestRequestTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
-    "AdministrativeActionOutputTypeDef",
-    "BackupOutputTypeDef",
-    "CreateVolumeFromBackupResponseOutputTypeDef",
-    "CreateVolumeResponseOutputTypeDef",
-    "DescribeVolumesResponseOutputTypeDef",
-    "UpdateVolumeResponseOutputTypeDef",
-    "CopyBackupResponseOutputTypeDef",
-    "CreateBackupResponseOutputTypeDef",
-    "DescribeBackupsResponseOutputTypeDef",
+    "AdministrativeActionTypeDef",
+    "BackupTypeDef",
+    "CreateVolumeFromBackupResponseTypeDef",
+    "CreateVolumeResponseTypeDef",
+    "DescribeVolumesResponseTypeDef",
+    "UpdateVolumeResponseTypeDef",
+    "CopyBackupResponseTypeDef",
+    "CreateBackupResponseTypeDef",
+    "DescribeBackupsResponseTypeDef",
 )
 
-ActiveDirectoryBackupAttributesOutputTypeDef = TypedDict(
-    "ActiveDirectoryBackupAttributesOutputTypeDef",
+ActiveDirectoryBackupAttributesTypeDef = TypedDict(
+    "ActiveDirectoryBackupAttributesTypeDef",
     {
         "DomainName": str,
         "ActiveDirectoryId": str,
         "ResourceARN": str,
     },
 )
 
-AdministrativeActionFailureDetailsOutputTypeDef = TypedDict(
-    "AdministrativeActionFailureDetailsOutputTypeDef",
+AdministrativeActionFailureDetailsTypeDef = TypedDict(
+    "AdministrativeActionFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
-AliasOutputTypeDef = TypedDict(
-    "AliasOutputTypeDef",
+AliasTypeDef = TypedDict(
+    "AliasTypeDef",
     {
         "Name": str,
         "Lifecycle": AliasLifecycleType,
     },
 )
 
 _RequiredAssociateFileSystemAliasesRequestRequestTypeDef = TypedDict(
@@ -375,16 +375,16 @@
 )
 
 
 class AutocommitPeriodTypeDef(_RequiredAutocommitPeriodTypeDef, _OptionalAutocommitPeriodTypeDef):
     pass
 
 
-BackupFailureDetailsOutputTypeDef = TypedDict(
-    "BackupFailureDetailsOutputTypeDef",
+BackupFailureDetailsTypeDef = TypedDict(
+    "BackupFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
@@ -397,16 +397,16 @@
 CancelDataRepositoryTaskRequestRequestTypeDef = TypedDict(
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
-CancelDataRepositoryTaskResponseOutputTypeDef = TypedDict(
-    "CancelDataRepositoryTaskResponseOutputTypeDef",
+CancelDataRepositoryTaskResponseTypeDef = TypedDict(
+    "CancelDataRepositoryTaskResponseTypeDef",
     {
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "TaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -452,18 +452,18 @@
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
-CreateFileSystemFromBackupResponseOutputTypeDef = TypedDict(
-    "CreateFileSystemFromBackupResponseOutputTypeDef",
+CreateFileSystemFromBackupResponseTypeDef = TypedDict(
+    "CreateFileSystemFromBackupResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLustreLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogCreateConfigurationTypeDef",
     {
@@ -499,18 +499,18 @@
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
     total=False,
 )
 
-CreateFileSystemResponseOutputTypeDef = TypedDict(
-    "CreateFileSystemResponseOutputTypeDef",
+CreateFileSystemResponseTypeDef = TypedDict(
+    "CreateFileSystemResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSelfManagedActiveDirectoryConfigurationTypeDef = TypedDict(
     "_RequiredSelfManagedActiveDirectoryConfigurationTypeDef",
     {
@@ -582,39 +582,39 @@
     {
         "Type": OpenZFSQuotaTypeType,
         "Id": int,
         "StorageCapacityQuotaGiB": int,
     },
 )
 
-DataRepositoryFailureDetailsOutputTypeDef = TypedDict(
-    "DataRepositoryFailureDetailsOutputTypeDef",
+DataRepositoryFailureDetailsTypeDef = TypedDict(
+    "DataRepositoryFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
-DataRepositoryTaskFailureDetailsOutputTypeDef = TypedDict(
-    "DataRepositoryTaskFailureDetailsOutputTypeDef",
+DataRepositoryTaskFailureDetailsTypeDef = TypedDict(
+    "DataRepositoryTaskFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
 DataRepositoryTaskFilterTypeDef = TypedDict(
     "DataRepositoryTaskFilterTypeDef",
     {
         "Name": DataRepositoryTaskFilterNameType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DataRepositoryTaskStatusOutputTypeDef = TypedDict(
-    "DataRepositoryTaskStatusOutputTypeDef",
+DataRepositoryTaskStatusTypeDef = TypedDict(
+    "DataRepositoryTaskStatusTypeDef",
     {
         "TotalCount": int,
         "SucceededCount": int,
         "FailedCount": int,
         "LastUpdatedTime": datetime,
         "ReleasedCapacity": int,
     },
@@ -637,16 +637,16 @@
 
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
 
-DeleteBackupResponseOutputTypeDef = TypedDict(
-    "DeleteBackupResponseOutputTypeDef",
+DeleteBackupResponseTypeDef = TypedDict(
+    "DeleteBackupResponseTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -669,16 +669,16 @@
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
-    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
+DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "DeleteDataRepositoryAssociationResponseTypeDef",
     {
         "AssociationId": str,
         "Lifecycle": DataRepositoryLifecycleType,
         "DeleteDataInFileSystem": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -700,16 +700,16 @@
 
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
 
-DeleteFileCacheResponseOutputTypeDef = TypedDict(
-    "DeleteFileCacheResponseOutputTypeDef",
+DeleteFileCacheResponseTypeDef = TypedDict(
+    "DeleteFileCacheResponseTypeDef",
     {
         "FileCacheId": str,
         "Lifecycle": FileCacheLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -730,16 +730,16 @@
 
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-DeleteSnapshotResponseOutputTypeDef = TypedDict(
-    "DeleteSnapshotResponseOutputTypeDef",
+DeleteSnapshotResponseTypeDef = TypedDict(
+    "DeleteSnapshotResponseTypeDef",
     {
         "SnapshotId": str,
         "Lifecycle": SnapshotLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -761,16 +761,16 @@
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteStorageVirtualMachineResponseOutputTypeDef = TypedDict(
-    "DeleteStorageVirtualMachineResponseOutputTypeDef",
+DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
+    "DeleteStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachineId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -840,18 +840,18 @@
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeFileSystemsResponseOutputTypeDef = TypedDict(
-    "DescribeFileSystemsResponseOutputTypeDef",
+DescribeFileSystemsResponseTypeDef = TypedDict(
+    "DescribeFileSystemsResponseTypeDef",
     {
-        "FileSystems": List["FileSystemOutputTypeDef"],
+        "FileSystems": List["FileSystemTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotFilterTypeDef = TypedDict(
     "SnapshotFilterTypeDef",
@@ -907,16 +907,16 @@
     "DiskIopsConfigurationOutputTypeDef",
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
 )
 
-FileCacheFailureDetailsOutputTypeDef = TypedDict(
-    "FileCacheFailureDetailsOutputTypeDef",
+FileCacheFailureDetailsTypeDef = TypedDict(
+    "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredFileCacheNFSConfigurationTypeDef = TypedDict(
     "_RequiredFileCacheNFSConfigurationTypeDef",
@@ -942,39 +942,39 @@
 FileCacheLustreMetadataConfigurationOutputTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationOutputTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
-LustreLogConfigurationOutputTypeDef = TypedDict(
-    "LustreLogConfigurationOutputTypeDef",
+LustreLogConfigurationTypeDef = TypedDict(
+    "LustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
         "Destination": str,
     },
 )
 
-FileSystemEndpointOutputTypeDef = TypedDict(
-    "FileSystemEndpointOutputTypeDef",
+FileSystemEndpointTypeDef = TypedDict(
+    "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
-FileSystemFailureDetailsOutputTypeDef = TypedDict(
-    "FileSystemFailureDetailsOutputTypeDef",
+FileSystemFailureDetailsTypeDef = TypedDict(
+    "FileSystemFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
-LifecycleTransitionReasonOutputTypeDef = TypedDict(
-    "LifecycleTransitionReasonOutputTypeDef",
+LifecycleTransitionReasonTypeDef = TypedDict(
+    "LifecycleTransitionReasonTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
@@ -1049,16 +1049,16 @@
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
         "Options": Sequence[str],
     },
 )
 
-OpenZFSOriginSnapshotConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
+OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
+    "OpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
     },
 )
 
 OpenZFSUserOrGroupQuotaOutputTypeDef = TypedDict(
@@ -1098,18 +1098,18 @@
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
 
-ReleaseFileSystemNfsV3LocksResponseOutputTypeDef = TypedDict(
-    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
+ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
@@ -1141,20 +1141,20 @@
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
 
-RestoreVolumeFromSnapshotResponseOutputTypeDef = TypedDict(
-    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
+RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
+    "RestoreVolumeFromSnapshotResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
-        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RetentionPeriodOutputTypeDef = TypedDict(
     "RetentionPeriodOutputTypeDef",
     {
@@ -1178,16 +1178,16 @@
 )
 
 
 class RetentionPeriodTypeDef(_RequiredRetentionPeriodTypeDef, _OptionalRetentionPeriodTypeDef):
     pass
 
 
-SelfManagedActiveDirectoryAttributesOutputTypeDef = TypedDict(
-    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
+SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
+    "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
         "DnsIps": List[str],
     },
@@ -1202,16 +1202,16 @@
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-SvmEndpointOutputTypeDef = TypedDict(
-    "SvmEndpointOutputTypeDef",
+SvmEndpointTypeDef = TypedDict(
+    "SvmEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -1226,18 +1226,18 @@
     "UpdateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-UpdateFileSystemResponseOutputTypeDef = TypedDict(
-    "UpdateFileSystemResponseOutputTypeDef",
+UpdateFileSystemResponseTypeDef = TypedDict(
+    "UpdateFileSystemResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
@@ -1256,50 +1256,50 @@
 
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-WindowsAuditLogConfigurationOutputTypeDef = TypedDict(
-    "WindowsAuditLogConfigurationOutputTypeDef",
+WindowsAuditLogConfigurationTypeDef = TypedDict(
+    "WindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "AuditLogDestination": str,
     },
 )
 
-AssociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
-    "AssociateFileSystemAliasesResponseOutputTypeDef",
+AssociateFileSystemAliasesResponseTypeDef = TypedDict(
+    "AssociateFileSystemAliasesResponseTypeDef",
     {
-        "Aliases": List[AliasOutputTypeDef],
+        "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileSystemAliasesResponseOutputTypeDef = TypedDict(
-    "DescribeFileSystemAliasesResponseOutputTypeDef",
+DescribeFileSystemAliasesResponseTypeDef = TypedDict(
+    "DescribeFileSystemAliasesResponseTypeDef",
     {
-        "Aliases": List[AliasOutputTypeDef],
+        "Aliases": List[AliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DisassociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
-    "DisassociateFileSystemAliasesResponseOutputTypeDef",
+DisassociateFileSystemAliasesResponseTypeDef = TypedDict(
+    "DisassociateFileSystemAliasesResponseTypeDef",
     {
-        "Aliases": List[AliasOutputTypeDef],
+        "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NFSDataRepositoryConfigurationOutputTypeDef = TypedDict(
-    "NFSDataRepositoryConfigurationOutputTypeDef",
+NFSDataRepositoryConfigurationTypeDef = TypedDict(
+    "NFSDataRepositoryConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
     },
 )
 
@@ -1316,48 +1316,48 @@
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
-DeleteFileSystemLustreResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemLustreResponseOutputTypeDef",
+DeleteFileSystemLustreResponseTypeDef = TypedDict(
+    "DeleteFileSystemLustreResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-DeleteFileSystemOpenZFSResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
+DeleteFileSystemOpenZFSResponseTypeDef = TypedDict(
+    "DeleteFileSystemOpenZFSResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-DeleteFileSystemWindowsResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemWindowsResponseOutputTypeDef",
+DeleteFileSystemWindowsResponseTypeDef = TypedDict(
+    "DeleteFileSystemWindowsResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-DeleteVolumeOntapResponseOutputTypeDef = TypedDict(
-    "DeleteVolumeOntapResponseOutputTypeDef",
+DeleteVolumeOntapResponseTypeDef = TypedDict(
+    "DeleteVolumeOntapResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1660,52 +1660,52 @@
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
 
-DataRepositoryConfigurationOutputTypeDef = TypedDict(
-    "DataRepositoryConfigurationOutputTypeDef",
+DataRepositoryConfigurationTypeDef = TypedDict(
+    "DataRepositoryConfigurationTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
         "AutoImportPolicy": AutoImportPolicyTypeType,
-        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
+        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
     },
 )
 
 DescribeDataRepositoryTasksRequestRequestTypeDef = TypedDict(
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     {
         "TaskIds": Sequence[str],
         "Filters": Sequence[DataRepositoryTaskFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DataRepositoryTaskOutputTypeDef = TypedDict(
-    "DataRepositoryTaskOutputTypeDef",
+DataRepositoryTaskTypeDef = TypedDict(
+    "DataRepositoryTaskTypeDef",
     {
         "TaskId": str,
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "Type": DataRepositoryTaskTypeType,
         "CreationTime": datetime,
         "StartTime": datetime,
         "EndTime": datetime,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
         "FileSystemId": str,
         "Paths": List[str],
-        "FailureDetails": DataRepositoryTaskFailureDetailsOutputTypeDef,
-        "Status": DataRepositoryTaskStatusOutputTypeDef,
+        "FailureDetails": DataRepositoryTaskFailureDetailsTypeDef,
+        "Status": DataRepositoryTaskStatusTypeDef,
         "Report": CompletionReportOutputTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
 )
 
 DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
@@ -1789,16 +1789,16 @@
         "Filters": Sequence[VolumeFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-OpenZFSFileSystemConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSFileSystemConfigurationOutputTypeDef",
+OpenZFSFileSystemConfigurationTypeDef = TypedDict(
+    "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
@@ -1828,46 +1828,46 @@
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
 
-FileCacheLustreConfigurationOutputTypeDef = TypedDict(
-    "FileCacheLustreConfigurationOutputTypeDef",
+FileCacheLustreConfigurationTypeDef = TypedDict(
+    "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationOutputTypeDef,
-        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
+        "LogConfiguration": LustreLogConfigurationTypeDef,
     },
 )
 
-FileSystemEndpointsOutputTypeDef = TypedDict(
-    "FileSystemEndpointsOutputTypeDef",
+FileSystemEndpointsTypeDef = TypedDict(
+    "FileSystemEndpointsTypeDef",
     {
-        "Intercluster": FileSystemEndpointOutputTypeDef,
-        "Management": FileSystemEndpointOutputTypeDef,
+        "Intercluster": FileSystemEndpointTypeDef,
+        "Management": FileSystemEndpointTypeDef,
     },
 )
 
-SnapshotOutputTypeDef = TypedDict(
-    "SnapshotOutputTypeDef",
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
     {
         "ResourceARN": str,
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
     },
 )
 
 OpenZFSNfsExportOutputTypeDef = TypedDict(
     "OpenZFSNfsExportOutputTypeDef",
     {
         "ClientConfigurations": List[OpenZFSClientConfigurationOutputTypeDef],
@@ -1895,21 +1895,19 @@
     {
         "DefaultRetention": RetentionPeriodTypeDef,
         "MinimumRetention": RetentionPeriodTypeDef,
         "MaximumRetention": RetentionPeriodTypeDef,
     },
 )
 
-SvmActiveDirectoryConfigurationOutputTypeDef = TypedDict(
-    "SvmActiveDirectoryConfigurationOutputTypeDef",
+SvmActiveDirectoryConfigurationTypeDef = TypedDict(
+    "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
-        "SelfManagedActiveDirectoryConfiguration": (
-            SelfManagedActiveDirectoryAttributesOutputTypeDef
-        ),
+        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
     },
 )
 
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
@@ -1931,21 +1929,21 @@
             SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
         ),
         "NetBiosName": str,
     },
     total=False,
 )
 
-SvmEndpointsOutputTypeDef = TypedDict(
-    "SvmEndpointsOutputTypeDef",
+SvmEndpointsTypeDef = TypedDict(
+    "SvmEndpointsTypeDef",
     {
-        "Iscsi": SvmEndpointOutputTypeDef,
-        "Management": SvmEndpointOutputTypeDef,
-        "Nfs": SvmEndpointOutputTypeDef,
-        "Smb": SvmEndpointOutputTypeDef,
+        "Iscsi": SvmEndpointTypeDef,
+        "Management": SvmEndpointTypeDef,
+        "Nfs": SvmEndpointTypeDef,
+        "Smb": SvmEndpointTypeDef,
     },
 )
 
 _RequiredUpdateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
@@ -1963,55 +1961,53 @@
 
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
 
-WindowsFileSystemConfigurationOutputTypeDef = TypedDict(
-    "WindowsFileSystemConfigurationOutputTypeDef",
+WindowsFileSystemConfigurationTypeDef = TypedDict(
+    "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
-        "SelfManagedActiveDirectoryConfiguration": (
-            SelfManagedActiveDirectoryAttributesOutputTypeDef
-        ),
+        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
         "PreferredSubnetId": str,
         "PreferredFileServerIp": str,
         "ThroughputCapacity": int,
         "MaintenanceOperationsInProgress": List[FileSystemMaintenanceOperationType],
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
-        "Aliases": List[AliasOutputTypeDef],
-        "AuditLogConfiguration": WindowsAuditLogConfigurationOutputTypeDef,
+        "Aliases": List[AliasTypeDef],
+        "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
     },
 )
 
-DataRepositoryAssociationOutputTypeDef = TypedDict(
-    "DataRepositoryAssociationOutputTypeDef",
+DataRepositoryAssociationTypeDef = TypedDict(
+    "DataRepositoryAssociationTypeDef",
     {
         "AssociationId": str,
         "ResourceARN": str,
         "FileSystemId": str,
         "Lifecycle": DataRepositoryLifecycleType,
-        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
+        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
         "FileSystemPath": str,
         "DataRepositoryPath": str,
         "BatchImportMetaDataOnCreate": bool,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationOutputTypeDef,
         "Tags": List[TagOutputTypeDef],
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCachePath": str,
         "DataRepositorySubdirectories": List[str],
-        "NFS": NFSDataRepositoryConfigurationOutputTypeDef,
+        "NFS": NFSDataRepositoryConfigurationTypeDef,
     },
 )
 
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -2059,32 +2055,32 @@
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteFileSystemResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemResponseOutputTypeDef",
+DeleteFileSystemResponseTypeDef = TypedDict(
+    "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
-        "WindowsResponse": DeleteFileSystemWindowsResponseOutputTypeDef,
-        "LustreResponse": DeleteFileSystemLustreResponseOutputTypeDef,
-        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseOutputTypeDef,
+        "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
+        "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
+        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteVolumeResponseOutputTypeDef = TypedDict(
-    "DeleteVolumeResponseOutputTypeDef",
+DeleteVolumeResponseTypeDef = TypedDict(
+    "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
-        "OntapResponse": DeleteVolumeOntapResponseOutputTypeDef,
+        "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
@@ -2155,44 +2151,44 @@
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-LustreFileSystemConfigurationOutputTypeDef = TypedDict(
-    "LustreFileSystemConfigurationOutputTypeDef",
+LustreFileSystemConfigurationTypeDef = TypedDict(
+    "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
-        "DataRepositoryConfiguration": DataRepositoryConfigurationOutputTypeDef,
+        "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
         "MountName": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
-        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
+        "LogConfiguration": LustreLogConfigurationTypeDef,
         "RootSquashConfiguration": LustreRootSquashConfigurationOutputTypeDef,
     },
 )
 
-CreateDataRepositoryTaskResponseOutputTypeDef = TypedDict(
-    "CreateDataRepositoryTaskResponseOutputTypeDef",
+CreateDataRepositoryTaskResponseTypeDef = TypedDict(
+    "CreateDataRepositoryTaskResponseTypeDef",
     {
-        "DataRepositoryTask": DataRepositoryTaskOutputTypeDef,
+        "DataRepositoryTask": DataRepositoryTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryTasksResponseOutputTypeDef = TypedDict(
-    "DescribeDataRepositoryTasksResponseOutputTypeDef",
+DescribeDataRepositoryTasksResponseTypeDef = TypedDict(
+    "DescribeDataRepositoryTasksResponseTypeDef",
     {
-        "DataRepositoryTasks": List[DataRepositoryTaskOutputTypeDef],
+        "DataRepositoryTasks": List[DataRepositoryTaskTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileCacheRequestRequestTypeDef",
@@ -2220,113 +2216,113 @@
 
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
 
-FileCacheCreatingOutputTypeDef = TypedDict(
-    "FileCacheCreatingOutputTypeDef",
+FileCacheCreatingTypeDef = TypedDict(
+    "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
+        "FailureDetails": FileCacheFailureDetailsTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
         "CopyTagsToDataRepositoryAssociations": bool,
-        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-FileCacheOutputTypeDef = TypedDict(
-    "FileCacheOutputTypeDef",
+FileCacheTypeDef = TypedDict(
+    "FileCacheTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
+        "FailureDetails": FileCacheFailureDetailsTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-OntapFileSystemConfigurationOutputTypeDef = TypedDict(
-    "OntapFileSystemConfigurationOutputTypeDef",
+OntapFileSystemConfigurationTypeDef = TypedDict(
+    "OntapFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OntapDeploymentTypeType,
         "EndpointIpAddressRange": str,
-        "Endpoints": FileSystemEndpointsOutputTypeDef,
+        "Endpoints": FileSystemEndpointsTypeDef,
         "DiskIopsConfiguration": DiskIopsConfigurationOutputTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "FsxAdminPassword": str,
     },
 )
 
-CreateSnapshotResponseOutputTypeDef = TypedDict(
-    "CreateSnapshotResponseOutputTypeDef",
+CreateSnapshotResponseTypeDef = TypedDict(
+    "CreateSnapshotResponseTypeDef",
     {
-        "Snapshot": SnapshotOutputTypeDef,
+        "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSnapshotsResponseOutputTypeDef = TypedDict(
-    "DescribeSnapshotsResponseOutputTypeDef",
+DescribeSnapshotsResponseTypeDef = TypedDict(
+    "DescribeSnapshotsResponseTypeDef",
     {
-        "Snapshots": List[SnapshotOutputTypeDef],
+        "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSnapshotResponseOutputTypeDef = TypedDict(
-    "UpdateSnapshotResponseOutputTypeDef",
+UpdateSnapshotResponseTypeDef = TypedDict(
+    "UpdateSnapshotResponseTypeDef",
     {
-        "Snapshot": SnapshotOutputTypeDef,
+        "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-OpenZFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSVolumeConfigurationOutputTypeDef",
+OpenZFSVolumeConfigurationTypeDef = TypedDict(
+    "OpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
         "VolumePath": str,
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "CopyTagsToSnapshots": bool,
-        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
         "ReadOnly": bool,
         "NfsExports": List[OpenZFSNfsExportOutputTypeDef],
         "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaOutputTypeDef],
         "RestoreToSnapshot": str,
         "DeleteIntermediateSnaphots": bool,
         "DeleteClonedVolumes": bool,
     },
@@ -2385,16 +2381,16 @@
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
-SnaplockConfigurationOutputTypeDef = TypedDict(
-    "SnaplockConfigurationOutputTypeDef",
+SnaplockConfigurationTypeDef = TypedDict(
+    "SnaplockConfigurationTypeDef",
     {
         "AuditLogVolume": bool,
         "AutocommitPeriod": AutocommitPeriodOutputTypeDef,
         "PrivilegedDelete": PrivilegedDeleteType,
         "RetentionPeriod": SnaplockRetentionPeriodOutputTypeDef,
         "SnaplockType": SnaplockTypeType,
         "VolumeAppendModeEnabled": bool,
@@ -2484,107 +2480,107 @@
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-StorageVirtualMachineOutputTypeDef = TypedDict(
-    "StorageVirtualMachineOutputTypeDef",
+StorageVirtualMachineTypeDef = TypedDict(
+    "StorageVirtualMachineTypeDef",
     {
-        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationOutputTypeDef,
+        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
-        "Endpoints": SvmEndpointsOutputTypeDef,
+        "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "Name": str,
         "ResourceARN": str,
         "StorageVirtualMachineId": str,
         "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
         "Tags": List[TagOutputTypeDef],
-        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
 )
 
-CreateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
-    "CreateDataRepositoryAssociationResponseOutputTypeDef",
+CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "CreateDataRepositoryAssociationResponseTypeDef",
     {
-        "Association": DataRepositoryAssociationOutputTypeDef,
+        "Association": DataRepositoryAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryAssociationsResponseOutputTypeDef = TypedDict(
-    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
+DescribeDataRepositoryAssociationsResponseTypeDef = TypedDict(
+    "DescribeDataRepositoryAssociationsResponseTypeDef",
     {
-        "Associations": List[DataRepositoryAssociationOutputTypeDef],
+        "Associations": List[DataRepositoryAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
-    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
+UpdateDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "UpdateDataRepositoryAssociationResponseTypeDef",
     {
-        "Association": DataRepositoryAssociationOutputTypeDef,
+        "Association": DataRepositoryAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFileCacheResponseOutputTypeDef = TypedDict(
-    "CreateFileCacheResponseOutputTypeDef",
+CreateFileCacheResponseTypeDef = TypedDict(
+    "CreateFileCacheResponseTypeDef",
     {
-        "FileCache": FileCacheCreatingOutputTypeDef,
+        "FileCache": FileCacheCreatingTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileCachesResponseOutputTypeDef = TypedDict(
-    "DescribeFileCachesResponseOutputTypeDef",
+DescribeFileCachesResponseTypeDef = TypedDict(
+    "DescribeFileCachesResponseTypeDef",
     {
-        "FileCaches": List[FileCacheOutputTypeDef],
+        "FileCaches": List[FileCacheTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateFileCacheResponseOutputTypeDef = TypedDict(
-    "UpdateFileCacheResponseOutputTypeDef",
+UpdateFileCacheResponseTypeDef = TypedDict(
+    "UpdateFileCacheResponseTypeDef",
     {
-        "FileCache": FileCacheOutputTypeDef,
+        "FileCache": FileCacheTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FileSystemOutputTypeDef = TypedDict(
-    "FileSystemOutputTypeDef",
+FileSystemTypeDef = TypedDict(
+    "FileSystemTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileSystemId": str,
         "FileSystemType": FileSystemTypeType,
         "Lifecycle": FileSystemLifecycleType,
-        "FailureDetails": FileSystemFailureDetailsOutputTypeDef,
+        "FailureDetails": FileSystemFailureDetailsTypeDef,
         "StorageCapacity": int,
         "StorageType": StorageTypeType,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
-        "WindowsConfiguration": WindowsFileSystemConfigurationOutputTypeDef,
-        "LustreConfiguration": LustreFileSystemConfigurationOutputTypeDef,
-        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
-        "OntapConfiguration": OntapFileSystemConfigurationOutputTypeDef,
+        "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
+        "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationOutputTypeDef,
+        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
 )
 
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
@@ -2609,30 +2605,30 @@
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
 
-OntapVolumeConfigurationOutputTypeDef = TypedDict(
-    "OntapVolumeConfigurationOutputTypeDef",
+OntapVolumeConfigurationTypeDef = TypedDict(
+    "OntapVolumeConfigurationTypeDef",
     {
         "FlexCacheEndpointType": FlexCacheEndpointTypeType,
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
         "StorageEfficiencyEnabled": bool,
         "StorageVirtualMachineId": str,
         "StorageVirtualMachineRoot": bool,
         "TieringPolicy": TieringPolicyOutputTypeDef,
         "UUID": str,
         "OntapVolumeType": OntapVolumeTypeType,
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
-        "SnaplockConfiguration": SnaplockConfigurationOutputTypeDef,
+        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
     },
 )
 
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
@@ -2672,35 +2668,35 @@
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
         "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-CreateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
-    "CreateStorageVirtualMachineResponseOutputTypeDef",
+CreateStorageVirtualMachineResponseTypeDef = TypedDict(
+    "CreateStorageVirtualMachineResponseTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageVirtualMachinesResponseOutputTypeDef = TypedDict(
-    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
+DescribeStorageVirtualMachinesResponseTypeDef = TypedDict(
+    "DescribeStorageVirtualMachinesResponseTypeDef",
     {
-        "StorageVirtualMachines": List[StorageVirtualMachineOutputTypeDef],
+        "StorageVirtualMachines": List[StorageVirtualMachineTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
-    "UpdateStorageVirtualMachineResponseOutputTypeDef",
+UpdateStorageVirtualMachineResponseTypeDef = TypedDict(
+    "UpdateStorageVirtualMachineResponseTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
     {
@@ -2761,29 +2757,29 @@
 
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
 
-VolumeOutputTypeDef = TypedDict(
-    "VolumeOutputTypeDef",
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
     {
         "CreationTime": datetime,
         "FileSystemId": str,
         "Lifecycle": VolumeLifecycleType,
         "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationOutputTypeDef,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
         "VolumeId": str,
         "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationOutputTypeDef,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
     },
 )
 
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
@@ -2853,100 +2849,100 @@
 
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
 
-AdministrativeActionOutputTypeDef = TypedDict(
-    "AdministrativeActionOutputTypeDef",
+AdministrativeActionTypeDef = TypedDict(
+    "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
         "TargetFileSystemValues": Dict[str, Any],
-        "FailureDetails": AdministrativeActionFailureDetailsOutputTypeDef,
+        "FailureDetails": AdministrativeActionFailureDetailsTypeDef,
         "TargetVolumeValues": Dict[str, Any],
         "TargetSnapshotValues": Dict[str, Any],
     },
 )
 
-BackupOutputTypeDef = TypedDict(
-    "BackupOutputTypeDef",
+BackupTypeDef = TypedDict(
+    "BackupTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
-        "FailureDetails": BackupFailureDetailsOutputTypeDef,
+        "FailureDetails": BackupFailureDetailsTypeDef,
         "Type": BackupTypeType,
         "ProgressPercent": int,
         "CreationTime": datetime,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
-        "FileSystem": "FileSystemOutputTypeDef",
-        "DirectoryInformation": ActiveDirectoryBackupAttributesOutputTypeDef,
+        "FileSystem": "FileSystemTypeDef",
+        "DirectoryInformation": ActiveDirectoryBackupAttributesTypeDef,
         "OwnerId": str,
         "SourceBackupId": str,
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
     },
 )
 
-CreateVolumeFromBackupResponseOutputTypeDef = TypedDict(
-    "CreateVolumeFromBackupResponseOutputTypeDef",
+CreateVolumeFromBackupResponseTypeDef = TypedDict(
+    "CreateVolumeFromBackupResponseTypeDef",
     {
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVolumeResponseOutputTypeDef = TypedDict(
-    "CreateVolumeResponseOutputTypeDef",
+CreateVolumeResponseTypeDef = TypedDict(
+    "CreateVolumeResponseTypeDef",
     {
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVolumesResponseOutputTypeDef = TypedDict(
-    "DescribeVolumesResponseOutputTypeDef",
+DescribeVolumesResponseTypeDef = TypedDict(
+    "DescribeVolumesResponseTypeDef",
     {
-        "Volumes": List[VolumeOutputTypeDef],
+        "Volumes": List[VolumeTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVolumeResponseOutputTypeDef = TypedDict(
-    "UpdateVolumeResponseOutputTypeDef",
+UpdateVolumeResponseTypeDef = TypedDict(
+    "UpdateVolumeResponseTypeDef",
     {
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CopyBackupResponseOutputTypeDef = TypedDict(
-    "CopyBackupResponseOutputTypeDef",
+CopyBackupResponseTypeDef = TypedDict(
+    "CopyBackupResponseTypeDef",
     {
-        "Backup": BackupOutputTypeDef,
+        "Backup": BackupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBackupResponseOutputTypeDef = TypedDict(
-    "CreateBackupResponseOutputTypeDef",
+CreateBackupResponseTypeDef = TypedDict(
+    "CreateBackupResponseTypeDef",
     {
-        "Backup": BackupOutputTypeDef,
+        "Backup": BackupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeBackupsResponseOutputTypeDef = TypedDict(
-    "DescribeBackupsResponseOutputTypeDef",
+DescribeBackupsResponseTypeDef = TypedDict(
+    "DescribeBackupsResponseTypeDef",
     {
-        "Backups": List[BackupOutputTypeDef],
+        "Backups": List[BackupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.pyi` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for fsx service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesOutputTypeDef
+    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesTypeDef
 
-    data: ActiveDirectoryBackupAttributesOutputTypeDef = {...}
+    data: ActiveDirectoryBackupAttributesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
@@ -72,110 +72,110 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActiveDirectoryBackupAttributesOutputTypeDef",
-    "AdministrativeActionFailureDetailsOutputTypeDef",
-    "AliasOutputTypeDef",
+    "ActiveDirectoryBackupAttributesTypeDef",
+    "AdministrativeActionFailureDetailsTypeDef",
+    "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "AutoExportPolicyOutputTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyOutputTypeDef",
     "AutoImportPolicyTypeDef",
     "AutocommitPeriodOutputTypeDef",
     "AutocommitPeriodTypeDef",
-    "BackupFailureDetailsOutputTypeDef",
+    "BackupFailureDetailsTypeDef",
     "TagOutputTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
-    "CancelDataRepositoryTaskResponseOutputTypeDef",
+    "CancelDataRepositoryTaskResponseTypeDef",
     "CompletionReportOutputTypeDef",
     "CompletionReportTypeDef",
     "TagTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
-    "CreateFileSystemFromBackupResponseOutputTypeDef",
+    "CreateFileSystemFromBackupResponseTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
     "DiskIopsConfigurationTypeDef",
-    "CreateFileSystemResponseOutputTypeDef",
+    "CreateFileSystemResponseTypeDef",
     "SelfManagedActiveDirectoryConfigurationTypeDef",
     "WindowsAuditLogCreateConfigurationTypeDef",
     "TieringPolicyTypeDef",
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaTypeDef",
-    "DataRepositoryFailureDetailsOutputTypeDef",
-    "DataRepositoryTaskFailureDetailsOutputTypeDef",
+    "DataRepositoryFailureDetailsTypeDef",
+    "DataRepositoryTaskFailureDetailsTypeDef",
     "DataRepositoryTaskFilterTypeDef",
-    "DataRepositoryTaskStatusOutputTypeDef",
+    "DataRepositoryTaskStatusTypeDef",
     "DeleteBackupRequestRequestTypeDef",
-    "DeleteBackupResponseOutputTypeDef",
+    "DeleteBackupResponseTypeDef",
     "DeleteDataRepositoryAssociationRequestRequestTypeDef",
-    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
+    "DeleteDataRepositoryAssociationResponseTypeDef",
     "DeleteFileCacheRequestRequestTypeDef",
-    "DeleteFileCacheResponseOutputTypeDef",
+    "DeleteFileCacheResponseTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResponseOutputTypeDef",
+    "DeleteSnapshotResponseTypeDef",
     "DeleteStorageVirtualMachineRequestRequestTypeDef",
-    "DeleteStorageVirtualMachineResponseOutputTypeDef",
+    "DeleteStorageVirtualMachineResponseTypeDef",
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     "FilterTypeDef",
     "DescribeFileCachesRequestRequestTypeDef",
     "DescribeFileSystemAliasesRequestRequestTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
-    "DescribeFileSystemsResponseOutputTypeDef",
+    "DescribeFileSystemsResponseTypeDef",
     "SnapshotFilterTypeDef",
     "StorageVirtualMachineFilterTypeDef",
     "VolumeFilterTypeDef",
     "DisassociateFileSystemAliasesRequestRequestTypeDef",
     "DiskIopsConfigurationOutputTypeDef",
-    "FileCacheFailureDetailsOutputTypeDef",
+    "FileCacheFailureDetailsTypeDef",
     "FileCacheNFSConfigurationTypeDef",
     "FileCacheLustreMetadataConfigurationOutputTypeDef",
-    "LustreLogConfigurationOutputTypeDef",
-    "FileSystemEndpointOutputTypeDef",
-    "FileSystemFailureDetailsOutputTypeDef",
-    "LifecycleTransitionReasonOutputTypeDef",
+    "LustreLogConfigurationTypeDef",
+    "FileSystemEndpointTypeDef",
+    "FileSystemFailureDetailsTypeDef",
+    "LifecycleTransitionReasonTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LustreRootSquashConfigurationOutputTypeDef",
     "TieringPolicyOutputTypeDef",
     "OpenZFSClientConfigurationOutputTypeDef",
     "OpenZFSClientConfigurationTypeDef",
-    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
+    "OpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
-    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
-    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
+    "RestoreVolumeFromSnapshotResponseTypeDef",
     "RetentionPeriodOutputTypeDef",
     "RetentionPeriodTypeDef",
-    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
+    "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
-    "SvmEndpointOutputTypeDef",
+    "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
-    "UpdateFileSystemResponseOutputTypeDef",
+    "UpdateFileSystemResponseTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
-    "WindowsAuditLogConfigurationOutputTypeDef",
-    "AssociateFileSystemAliasesResponseOutputTypeDef",
-    "DescribeFileSystemAliasesResponseOutputTypeDef",
-    "DisassociateFileSystemAliasesResponseOutputTypeDef",
-    "NFSDataRepositoryConfigurationOutputTypeDef",
+    "WindowsAuditLogConfigurationTypeDef",
+    "AssociateFileSystemAliasesResponseTypeDef",
+    "DescribeFileSystemAliasesResponseTypeDef",
+    "DisassociateFileSystemAliasesResponseTypeDef",
+    "NFSDataRepositoryConfigurationTypeDef",
     "S3DataRepositoryConfigurationOutputTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
-    "DeleteFileSystemLustreResponseOutputTypeDef",
-    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
-    "DeleteFileSystemWindowsResponseOutputTypeDef",
-    "DeleteVolumeOntapResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "DeleteFileSystemLustreResponseTypeDef",
+    "DeleteFileSystemOpenZFSResponseTypeDef",
+    "DeleteFileSystemWindowsResponseTypeDef",
+    "DeleteVolumeOntapResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateDataRepositoryTaskRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
     "DeleteFileSystemWindowsConfigurationTypeDef",
@@ -185,117 +185,117 @@
     "CreateFileSystemLustreConfigurationTypeDef",
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "DataRepositoryConfigurationOutputTypeDef",
+    "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
-    "DataRepositoryTaskOutputTypeDef",
+    "DataRepositoryTaskTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
-    "OpenZFSFileSystemConfigurationOutputTypeDef",
+    "OpenZFSFileSystemConfigurationTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
-    "FileCacheLustreConfigurationOutputTypeDef",
-    "FileSystemEndpointsOutputTypeDef",
-    "SnapshotOutputTypeDef",
+    "FileCacheLustreConfigurationTypeDef",
+    "FileSystemEndpointsTypeDef",
+    "SnapshotTypeDef",
     "OpenZFSNfsExportOutputTypeDef",
     "OpenZFSNfsExportTypeDef",
     "SnaplockRetentionPeriodOutputTypeDef",
     "SnaplockRetentionPeriodTypeDef",
-    "SvmActiveDirectoryConfigurationOutputTypeDef",
+    "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
-    "SvmEndpointsOutputTypeDef",
+    "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
-    "WindowsFileSystemConfigurationOutputTypeDef",
-    "DataRepositoryAssociationOutputTypeDef",
+    "WindowsFileSystemConfigurationTypeDef",
+    "DataRepositoryAssociationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
-    "DeleteFileSystemResponseOutputTypeDef",
-    "DeleteVolumeResponseOutputTypeDef",
+    "DeleteFileSystemResponseTypeDef",
+    "DeleteVolumeResponseTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "LustreFileSystemConfigurationOutputTypeDef",
-    "CreateDataRepositoryTaskResponseOutputTypeDef",
-    "DescribeDataRepositoryTasksResponseOutputTypeDef",
+    "LustreFileSystemConfigurationTypeDef",
+    "CreateDataRepositoryTaskResponseTypeDef",
+    "DescribeDataRepositoryTasksResponseTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
-    "FileCacheCreatingOutputTypeDef",
-    "FileCacheOutputTypeDef",
-    "OntapFileSystemConfigurationOutputTypeDef",
-    "CreateSnapshotResponseOutputTypeDef",
-    "DescribeSnapshotsResponseOutputTypeDef",
-    "UpdateSnapshotResponseOutputTypeDef",
-    "OpenZFSVolumeConfigurationOutputTypeDef",
+    "FileCacheCreatingTypeDef",
+    "FileCacheTypeDef",
+    "OntapFileSystemConfigurationTypeDef",
+    "CreateSnapshotResponseTypeDef",
+    "DescribeSnapshotsResponseTypeDef",
+    "UpdateSnapshotResponseTypeDef",
+    "OpenZFSVolumeConfigurationTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
-    "SnaplockConfigurationOutputTypeDef",
+    "SnaplockConfigurationTypeDef",
     "CreateSnaplockConfigurationTypeDef",
     "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
-    "StorageVirtualMachineOutputTypeDef",
-    "CreateDataRepositoryAssociationResponseOutputTypeDef",
-    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
-    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
-    "CreateFileCacheResponseOutputTypeDef",
-    "DescribeFileCachesResponseOutputTypeDef",
-    "UpdateFileCacheResponseOutputTypeDef",
-    "FileSystemOutputTypeDef",
+    "StorageVirtualMachineTypeDef",
+    "CreateDataRepositoryAssociationResponseTypeDef",
+    "DescribeDataRepositoryAssociationsResponseTypeDef",
+    "UpdateDataRepositoryAssociationResponseTypeDef",
+    "CreateFileCacheResponseTypeDef",
+    "DescribeFileCachesResponseTypeDef",
+    "UpdateFileCacheResponseTypeDef",
+    "FileSystemTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
-    "OntapVolumeConfigurationOutputTypeDef",
+    "OntapVolumeConfigurationTypeDef",
     "CreateOntapVolumeConfigurationTypeDef",
     "UpdateOntapVolumeConfigurationTypeDef",
-    "CreateStorageVirtualMachineResponseOutputTypeDef",
-    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
-    "UpdateStorageVirtualMachineResponseOutputTypeDef",
+    "CreateStorageVirtualMachineResponseTypeDef",
+    "DescribeStorageVirtualMachinesResponseTypeDef",
+    "UpdateStorageVirtualMachineResponseTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
-    "VolumeOutputTypeDef",
+    "VolumeTypeDef",
     "CreateVolumeFromBackupRequestRequestTypeDef",
     "CreateVolumeRequestRequestTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
-    "AdministrativeActionOutputTypeDef",
-    "BackupOutputTypeDef",
-    "CreateVolumeFromBackupResponseOutputTypeDef",
-    "CreateVolumeResponseOutputTypeDef",
-    "DescribeVolumesResponseOutputTypeDef",
-    "UpdateVolumeResponseOutputTypeDef",
-    "CopyBackupResponseOutputTypeDef",
-    "CreateBackupResponseOutputTypeDef",
-    "DescribeBackupsResponseOutputTypeDef",
+    "AdministrativeActionTypeDef",
+    "BackupTypeDef",
+    "CreateVolumeFromBackupResponseTypeDef",
+    "CreateVolumeResponseTypeDef",
+    "DescribeVolumesResponseTypeDef",
+    "UpdateVolumeResponseTypeDef",
+    "CopyBackupResponseTypeDef",
+    "CreateBackupResponseTypeDef",
+    "DescribeBackupsResponseTypeDef",
 )
 
-ActiveDirectoryBackupAttributesOutputTypeDef = TypedDict(
-    "ActiveDirectoryBackupAttributesOutputTypeDef",
+ActiveDirectoryBackupAttributesTypeDef = TypedDict(
+    "ActiveDirectoryBackupAttributesTypeDef",
     {
         "DomainName": str,
         "ActiveDirectoryId": str,
         "ResourceARN": str,
     },
 )
 
-AdministrativeActionFailureDetailsOutputTypeDef = TypedDict(
-    "AdministrativeActionFailureDetailsOutputTypeDef",
+AdministrativeActionFailureDetailsTypeDef = TypedDict(
+    "AdministrativeActionFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
-AliasOutputTypeDef = TypedDict(
-    "AliasOutputTypeDef",
+AliasTypeDef = TypedDict(
+    "AliasTypeDef",
     {
         "Name": str,
         "Lifecycle": AliasLifecycleType,
     },
 )
 
 _RequiredAssociateFileSystemAliasesRequestRequestTypeDef = TypedDict(
@@ -370,16 +370,16 @@
     },
     total=False,
 )
 
 class AutocommitPeriodTypeDef(_RequiredAutocommitPeriodTypeDef, _OptionalAutocommitPeriodTypeDef):
     pass
 
-BackupFailureDetailsOutputTypeDef = TypedDict(
-    "BackupFailureDetailsOutputTypeDef",
+BackupFailureDetailsTypeDef = TypedDict(
+    "BackupFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
@@ -392,16 +392,16 @@
 CancelDataRepositoryTaskRequestRequestTypeDef = TypedDict(
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
-CancelDataRepositoryTaskResponseOutputTypeDef = TypedDict(
-    "CancelDataRepositoryTaskResponseOutputTypeDef",
+CancelDataRepositoryTaskResponseTypeDef = TypedDict(
+    "CancelDataRepositoryTaskResponseTypeDef",
     {
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "TaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -445,18 +445,18 @@
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
-CreateFileSystemFromBackupResponseOutputTypeDef = TypedDict(
-    "CreateFileSystemFromBackupResponseOutputTypeDef",
+CreateFileSystemFromBackupResponseTypeDef = TypedDict(
+    "CreateFileSystemFromBackupResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLustreLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogCreateConfigurationTypeDef",
     {
@@ -490,18 +490,18 @@
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
     total=False,
 )
 
-CreateFileSystemResponseOutputTypeDef = TypedDict(
-    "CreateFileSystemResponseOutputTypeDef",
+CreateFileSystemResponseTypeDef = TypedDict(
+    "CreateFileSystemResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSelfManagedActiveDirectoryConfigurationTypeDef = TypedDict(
     "_RequiredSelfManagedActiveDirectoryConfigurationTypeDef",
     {
@@ -569,39 +569,39 @@
     {
         "Type": OpenZFSQuotaTypeType,
         "Id": int,
         "StorageCapacityQuotaGiB": int,
     },
 )
 
-DataRepositoryFailureDetailsOutputTypeDef = TypedDict(
-    "DataRepositoryFailureDetailsOutputTypeDef",
+DataRepositoryFailureDetailsTypeDef = TypedDict(
+    "DataRepositoryFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
-DataRepositoryTaskFailureDetailsOutputTypeDef = TypedDict(
-    "DataRepositoryTaskFailureDetailsOutputTypeDef",
+DataRepositoryTaskFailureDetailsTypeDef = TypedDict(
+    "DataRepositoryTaskFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
 DataRepositoryTaskFilterTypeDef = TypedDict(
     "DataRepositoryTaskFilterTypeDef",
     {
         "Name": DataRepositoryTaskFilterNameType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DataRepositoryTaskStatusOutputTypeDef = TypedDict(
-    "DataRepositoryTaskStatusOutputTypeDef",
+DataRepositoryTaskStatusTypeDef = TypedDict(
+    "DataRepositoryTaskStatusTypeDef",
     {
         "TotalCount": int,
         "SucceededCount": int,
         "FailedCount": int,
         "LastUpdatedTime": datetime,
         "ReleasedCapacity": int,
     },
@@ -622,16 +622,16 @@
 )
 
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
-DeleteBackupResponseOutputTypeDef = TypedDict(
-    "DeleteBackupResponseOutputTypeDef",
+DeleteBackupResponseTypeDef = TypedDict(
+    "DeleteBackupResponseTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -652,16 +652,16 @@
 
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-DeleteDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
-    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
+DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "DeleteDataRepositoryAssociationResponseTypeDef",
     {
         "AssociationId": str,
         "Lifecycle": DataRepositoryLifecycleType,
         "DeleteDataInFileSystem": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -681,16 +681,16 @@
 )
 
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
-DeleteFileCacheResponseOutputTypeDef = TypedDict(
-    "DeleteFileCacheResponseOutputTypeDef",
+DeleteFileCacheResponseTypeDef = TypedDict(
+    "DeleteFileCacheResponseTypeDef",
     {
         "FileCacheId": str,
         "Lifecycle": FileCacheLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -709,16 +709,16 @@
 )
 
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-DeleteSnapshotResponseOutputTypeDef = TypedDict(
-    "DeleteSnapshotResponseOutputTypeDef",
+DeleteSnapshotResponseTypeDef = TypedDict(
+    "DeleteSnapshotResponseTypeDef",
     {
         "SnapshotId": str,
         "Lifecycle": SnapshotLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -738,16 +738,16 @@
 
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-DeleteStorageVirtualMachineResponseOutputTypeDef = TypedDict(
-    "DeleteStorageVirtualMachineResponseOutputTypeDef",
+DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
+    "DeleteStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachineId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -815,18 +815,18 @@
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeFileSystemsResponseOutputTypeDef = TypedDict(
-    "DescribeFileSystemsResponseOutputTypeDef",
+DescribeFileSystemsResponseTypeDef = TypedDict(
+    "DescribeFileSystemsResponseTypeDef",
     {
-        "FileSystems": List["FileSystemOutputTypeDef"],
+        "FileSystems": List["FileSystemTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotFilterTypeDef = TypedDict(
     "SnapshotFilterTypeDef",
@@ -880,16 +880,16 @@
     "DiskIopsConfigurationOutputTypeDef",
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
 )
 
-FileCacheFailureDetailsOutputTypeDef = TypedDict(
-    "FileCacheFailureDetailsOutputTypeDef",
+FileCacheFailureDetailsTypeDef = TypedDict(
+    "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredFileCacheNFSConfigurationTypeDef = TypedDict(
     "_RequiredFileCacheNFSConfigurationTypeDef",
@@ -913,39 +913,39 @@
 FileCacheLustreMetadataConfigurationOutputTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationOutputTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
-LustreLogConfigurationOutputTypeDef = TypedDict(
-    "LustreLogConfigurationOutputTypeDef",
+LustreLogConfigurationTypeDef = TypedDict(
+    "LustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
         "Destination": str,
     },
 )
 
-FileSystemEndpointOutputTypeDef = TypedDict(
-    "FileSystemEndpointOutputTypeDef",
+FileSystemEndpointTypeDef = TypedDict(
+    "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
-FileSystemFailureDetailsOutputTypeDef = TypedDict(
-    "FileSystemFailureDetailsOutputTypeDef",
+FileSystemFailureDetailsTypeDef = TypedDict(
+    "FileSystemFailureDetailsTypeDef",
     {
         "Message": str,
     },
 )
 
-LifecycleTransitionReasonOutputTypeDef = TypedDict(
-    "LifecycleTransitionReasonOutputTypeDef",
+LifecycleTransitionReasonTypeDef = TypedDict(
+    "LifecycleTransitionReasonTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
@@ -1016,16 +1016,16 @@
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
         "Options": Sequence[str],
     },
 )
 
-OpenZFSOriginSnapshotConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
+OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
+    "OpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
     },
 )
 
 OpenZFSUserOrGroupQuotaOutputTypeDef = TypedDict(
@@ -1063,18 +1063,18 @@
 
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
-ReleaseFileSystemNfsV3LocksResponseOutputTypeDef = TypedDict(
-    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
+ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
@@ -1104,20 +1104,20 @@
 
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-RestoreVolumeFromSnapshotResponseOutputTypeDef = TypedDict(
-    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
+RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
+    "RestoreVolumeFromSnapshotResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
-        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RetentionPeriodOutputTypeDef = TypedDict(
     "RetentionPeriodOutputTypeDef",
     {
@@ -1139,16 +1139,16 @@
     },
     total=False,
 )
 
 class RetentionPeriodTypeDef(_RequiredRetentionPeriodTypeDef, _OptionalRetentionPeriodTypeDef):
     pass
 
-SelfManagedActiveDirectoryAttributesOutputTypeDef = TypedDict(
-    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
+SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
+    "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
         "DnsIps": List[str],
     },
@@ -1163,16 +1163,16 @@
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-SvmEndpointOutputTypeDef = TypedDict(
-    "SvmEndpointOutputTypeDef",
+SvmEndpointTypeDef = TypedDict(
+    "SvmEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -1187,18 +1187,18 @@
     "UpdateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-UpdateFileSystemResponseOutputTypeDef = TypedDict(
-    "UpdateFileSystemResponseOutputTypeDef",
+UpdateFileSystemResponseTypeDef = TypedDict(
+    "UpdateFileSystemResponseTypeDef",
     {
-        "FileSystem": "FileSystemOutputTypeDef",
+        "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
@@ -1215,50 +1215,50 @@
 )
 
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-WindowsAuditLogConfigurationOutputTypeDef = TypedDict(
-    "WindowsAuditLogConfigurationOutputTypeDef",
+WindowsAuditLogConfigurationTypeDef = TypedDict(
+    "WindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "AuditLogDestination": str,
     },
 )
 
-AssociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
-    "AssociateFileSystemAliasesResponseOutputTypeDef",
+AssociateFileSystemAliasesResponseTypeDef = TypedDict(
+    "AssociateFileSystemAliasesResponseTypeDef",
     {
-        "Aliases": List[AliasOutputTypeDef],
+        "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileSystemAliasesResponseOutputTypeDef = TypedDict(
-    "DescribeFileSystemAliasesResponseOutputTypeDef",
+DescribeFileSystemAliasesResponseTypeDef = TypedDict(
+    "DescribeFileSystemAliasesResponseTypeDef",
     {
-        "Aliases": List[AliasOutputTypeDef],
+        "Aliases": List[AliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DisassociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
-    "DisassociateFileSystemAliasesResponseOutputTypeDef",
+DisassociateFileSystemAliasesResponseTypeDef = TypedDict(
+    "DisassociateFileSystemAliasesResponseTypeDef",
     {
-        "Aliases": List[AliasOutputTypeDef],
+        "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NFSDataRepositoryConfigurationOutputTypeDef = TypedDict(
-    "NFSDataRepositoryConfigurationOutputTypeDef",
+NFSDataRepositoryConfigurationTypeDef = TypedDict(
+    "NFSDataRepositoryConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
     },
 )
 
@@ -1275,48 +1275,48 @@
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
-DeleteFileSystemLustreResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemLustreResponseOutputTypeDef",
+DeleteFileSystemLustreResponseTypeDef = TypedDict(
+    "DeleteFileSystemLustreResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-DeleteFileSystemOpenZFSResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
+DeleteFileSystemOpenZFSResponseTypeDef = TypedDict(
+    "DeleteFileSystemOpenZFSResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-DeleteFileSystemWindowsResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemWindowsResponseOutputTypeDef",
+DeleteFileSystemWindowsResponseTypeDef = TypedDict(
+    "DeleteFileSystemWindowsResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-DeleteVolumeOntapResponseOutputTypeDef = TypedDict(
-    "DeleteVolumeOntapResponseOutputTypeDef",
+DeleteVolumeOntapResponseTypeDef = TypedDict(
+    "DeleteVolumeOntapResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagOutputTypeDef],
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1605,52 +1605,52 @@
 
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-DataRepositoryConfigurationOutputTypeDef = TypedDict(
-    "DataRepositoryConfigurationOutputTypeDef",
+DataRepositoryConfigurationTypeDef = TypedDict(
+    "DataRepositoryConfigurationTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
         "AutoImportPolicy": AutoImportPolicyTypeType,
-        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
+        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
     },
 )
 
 DescribeDataRepositoryTasksRequestRequestTypeDef = TypedDict(
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     {
         "TaskIds": Sequence[str],
         "Filters": Sequence[DataRepositoryTaskFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DataRepositoryTaskOutputTypeDef = TypedDict(
-    "DataRepositoryTaskOutputTypeDef",
+DataRepositoryTaskTypeDef = TypedDict(
+    "DataRepositoryTaskTypeDef",
     {
         "TaskId": str,
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "Type": DataRepositoryTaskTypeType,
         "CreationTime": datetime,
         "StartTime": datetime,
         "EndTime": datetime,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
         "FileSystemId": str,
         "Paths": List[str],
-        "FailureDetails": DataRepositoryTaskFailureDetailsOutputTypeDef,
-        "Status": DataRepositoryTaskStatusOutputTypeDef,
+        "FailureDetails": DataRepositoryTaskFailureDetailsTypeDef,
+        "Status": DataRepositoryTaskStatusTypeDef,
         "Report": CompletionReportOutputTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
 )
 
 DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
@@ -1734,16 +1734,16 @@
         "Filters": Sequence[VolumeFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-OpenZFSFileSystemConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSFileSystemConfigurationOutputTypeDef",
+OpenZFSFileSystemConfigurationTypeDef = TypedDict(
+    "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
@@ -1771,46 +1771,46 @@
 
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
-FileCacheLustreConfigurationOutputTypeDef = TypedDict(
-    "FileCacheLustreConfigurationOutputTypeDef",
+FileCacheLustreConfigurationTypeDef = TypedDict(
+    "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationOutputTypeDef,
-        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
+        "LogConfiguration": LustreLogConfigurationTypeDef,
     },
 )
 
-FileSystemEndpointsOutputTypeDef = TypedDict(
-    "FileSystemEndpointsOutputTypeDef",
+FileSystemEndpointsTypeDef = TypedDict(
+    "FileSystemEndpointsTypeDef",
     {
-        "Intercluster": FileSystemEndpointOutputTypeDef,
-        "Management": FileSystemEndpointOutputTypeDef,
+        "Intercluster": FileSystemEndpointTypeDef,
+        "Management": FileSystemEndpointTypeDef,
     },
 )
 
-SnapshotOutputTypeDef = TypedDict(
-    "SnapshotOutputTypeDef",
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
     {
         "ResourceARN": str,
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
     },
 )
 
 OpenZFSNfsExportOutputTypeDef = TypedDict(
     "OpenZFSNfsExportOutputTypeDef",
     {
         "ClientConfigurations": List[OpenZFSClientConfigurationOutputTypeDef],
@@ -1838,21 +1838,19 @@
     {
         "DefaultRetention": RetentionPeriodTypeDef,
         "MinimumRetention": RetentionPeriodTypeDef,
         "MaximumRetention": RetentionPeriodTypeDef,
     },
 )
 
-SvmActiveDirectoryConfigurationOutputTypeDef = TypedDict(
-    "SvmActiveDirectoryConfigurationOutputTypeDef",
+SvmActiveDirectoryConfigurationTypeDef = TypedDict(
+    "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
-        "SelfManagedActiveDirectoryConfiguration": (
-            SelfManagedActiveDirectoryAttributesOutputTypeDef
-        ),
+        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
     },
 )
 
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
@@ -1874,21 +1872,21 @@
             SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
         ),
         "NetBiosName": str,
     },
     total=False,
 )
 
-SvmEndpointsOutputTypeDef = TypedDict(
-    "SvmEndpointsOutputTypeDef",
+SvmEndpointsTypeDef = TypedDict(
+    "SvmEndpointsTypeDef",
     {
-        "Iscsi": SvmEndpointOutputTypeDef,
-        "Management": SvmEndpointOutputTypeDef,
-        "Nfs": SvmEndpointOutputTypeDef,
-        "Smb": SvmEndpointOutputTypeDef,
+        "Iscsi": SvmEndpointTypeDef,
+        "Management": SvmEndpointTypeDef,
+        "Nfs": SvmEndpointTypeDef,
+        "Smb": SvmEndpointTypeDef,
     },
 )
 
 _RequiredUpdateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
@@ -1904,55 +1902,53 @@
 )
 
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
-WindowsFileSystemConfigurationOutputTypeDef = TypedDict(
-    "WindowsFileSystemConfigurationOutputTypeDef",
+WindowsFileSystemConfigurationTypeDef = TypedDict(
+    "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
-        "SelfManagedActiveDirectoryConfiguration": (
-            SelfManagedActiveDirectoryAttributesOutputTypeDef
-        ),
+        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
         "PreferredSubnetId": str,
         "PreferredFileServerIp": str,
         "ThroughputCapacity": int,
         "MaintenanceOperationsInProgress": List[FileSystemMaintenanceOperationType],
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
-        "Aliases": List[AliasOutputTypeDef],
-        "AuditLogConfiguration": WindowsAuditLogConfigurationOutputTypeDef,
+        "Aliases": List[AliasTypeDef],
+        "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
     },
 )
 
-DataRepositoryAssociationOutputTypeDef = TypedDict(
-    "DataRepositoryAssociationOutputTypeDef",
+DataRepositoryAssociationTypeDef = TypedDict(
+    "DataRepositoryAssociationTypeDef",
     {
         "AssociationId": str,
         "ResourceARN": str,
         "FileSystemId": str,
         "Lifecycle": DataRepositoryLifecycleType,
-        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
+        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
         "FileSystemPath": str,
         "DataRepositoryPath": str,
         "BatchImportMetaDataOnCreate": bool,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationOutputTypeDef,
         "Tags": List[TagOutputTypeDef],
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCachePath": str,
         "DataRepositorySubdirectories": List[str],
-        "NFS": NFSDataRepositoryConfigurationOutputTypeDef,
+        "NFS": NFSDataRepositoryConfigurationTypeDef,
     },
 )
 
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -1996,32 +1992,32 @@
 
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-DeleteFileSystemResponseOutputTypeDef = TypedDict(
-    "DeleteFileSystemResponseOutputTypeDef",
+DeleteFileSystemResponseTypeDef = TypedDict(
+    "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
-        "WindowsResponse": DeleteFileSystemWindowsResponseOutputTypeDef,
-        "LustreResponse": DeleteFileSystemLustreResponseOutputTypeDef,
-        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseOutputTypeDef,
+        "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
+        "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
+        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteVolumeResponseOutputTypeDef = TypedDict(
-    "DeleteVolumeResponseOutputTypeDef",
+DeleteVolumeResponseTypeDef = TypedDict(
+    "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
-        "OntapResponse": DeleteVolumeOntapResponseOutputTypeDef,
+        "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
@@ -2086,44 +2082,44 @@
 
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-LustreFileSystemConfigurationOutputTypeDef = TypedDict(
-    "LustreFileSystemConfigurationOutputTypeDef",
+LustreFileSystemConfigurationTypeDef = TypedDict(
+    "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
-        "DataRepositoryConfiguration": DataRepositoryConfigurationOutputTypeDef,
+        "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
         "MountName": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
-        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
+        "LogConfiguration": LustreLogConfigurationTypeDef,
         "RootSquashConfiguration": LustreRootSquashConfigurationOutputTypeDef,
     },
 )
 
-CreateDataRepositoryTaskResponseOutputTypeDef = TypedDict(
-    "CreateDataRepositoryTaskResponseOutputTypeDef",
+CreateDataRepositoryTaskResponseTypeDef = TypedDict(
+    "CreateDataRepositoryTaskResponseTypeDef",
     {
-        "DataRepositoryTask": DataRepositoryTaskOutputTypeDef,
+        "DataRepositoryTask": DataRepositoryTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryTasksResponseOutputTypeDef = TypedDict(
-    "DescribeDataRepositoryTasksResponseOutputTypeDef",
+DescribeDataRepositoryTasksResponseTypeDef = TypedDict(
+    "DescribeDataRepositoryTasksResponseTypeDef",
     {
-        "DataRepositoryTasks": List[DataRepositoryTaskOutputTypeDef],
+        "DataRepositoryTasks": List[DataRepositoryTaskTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileCacheRequestRequestTypeDef",
@@ -2149,113 +2145,113 @@
 )
 
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
-FileCacheCreatingOutputTypeDef = TypedDict(
-    "FileCacheCreatingOutputTypeDef",
+FileCacheCreatingTypeDef = TypedDict(
+    "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
+        "FailureDetails": FileCacheFailureDetailsTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
         "CopyTagsToDataRepositoryAssociations": bool,
-        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-FileCacheOutputTypeDef = TypedDict(
-    "FileCacheOutputTypeDef",
+FileCacheTypeDef = TypedDict(
+    "FileCacheTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
+        "FailureDetails": FileCacheFailureDetailsTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-OntapFileSystemConfigurationOutputTypeDef = TypedDict(
-    "OntapFileSystemConfigurationOutputTypeDef",
+OntapFileSystemConfigurationTypeDef = TypedDict(
+    "OntapFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OntapDeploymentTypeType,
         "EndpointIpAddressRange": str,
-        "Endpoints": FileSystemEndpointsOutputTypeDef,
+        "Endpoints": FileSystemEndpointsTypeDef,
         "DiskIopsConfiguration": DiskIopsConfigurationOutputTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "FsxAdminPassword": str,
     },
 )
 
-CreateSnapshotResponseOutputTypeDef = TypedDict(
-    "CreateSnapshotResponseOutputTypeDef",
+CreateSnapshotResponseTypeDef = TypedDict(
+    "CreateSnapshotResponseTypeDef",
     {
-        "Snapshot": SnapshotOutputTypeDef,
+        "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSnapshotsResponseOutputTypeDef = TypedDict(
-    "DescribeSnapshotsResponseOutputTypeDef",
+DescribeSnapshotsResponseTypeDef = TypedDict(
+    "DescribeSnapshotsResponseTypeDef",
     {
-        "Snapshots": List[SnapshotOutputTypeDef],
+        "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSnapshotResponseOutputTypeDef = TypedDict(
-    "UpdateSnapshotResponseOutputTypeDef",
+UpdateSnapshotResponseTypeDef = TypedDict(
+    "UpdateSnapshotResponseTypeDef",
     {
-        "Snapshot": SnapshotOutputTypeDef,
+        "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-OpenZFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSVolumeConfigurationOutputTypeDef",
+OpenZFSVolumeConfigurationTypeDef = TypedDict(
+    "OpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
         "VolumePath": str,
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "CopyTagsToSnapshots": bool,
-        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
         "ReadOnly": bool,
         "NfsExports": List[OpenZFSNfsExportOutputTypeDef],
         "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaOutputTypeDef],
         "RestoreToSnapshot": str,
         "DeleteIntermediateSnaphots": bool,
         "DeleteClonedVolumes": bool,
     },
@@ -2312,16 +2308,16 @@
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
-SnaplockConfigurationOutputTypeDef = TypedDict(
-    "SnaplockConfigurationOutputTypeDef",
+SnaplockConfigurationTypeDef = TypedDict(
+    "SnaplockConfigurationTypeDef",
     {
         "AuditLogVolume": bool,
         "AutocommitPeriod": AutocommitPeriodOutputTypeDef,
         "PrivilegedDelete": PrivilegedDeleteType,
         "RetentionPeriod": SnaplockRetentionPeriodOutputTypeDef,
         "SnaplockType": SnaplockTypeType,
         "VolumeAppendModeEnabled": bool,
@@ -2405,107 +2401,107 @@
 
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-StorageVirtualMachineOutputTypeDef = TypedDict(
-    "StorageVirtualMachineOutputTypeDef",
+StorageVirtualMachineTypeDef = TypedDict(
+    "StorageVirtualMachineTypeDef",
     {
-        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationOutputTypeDef,
+        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
-        "Endpoints": SvmEndpointsOutputTypeDef,
+        "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "Name": str,
         "ResourceARN": str,
         "StorageVirtualMachineId": str,
         "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
         "Tags": List[TagOutputTypeDef],
-        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
 )
 
-CreateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
-    "CreateDataRepositoryAssociationResponseOutputTypeDef",
+CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "CreateDataRepositoryAssociationResponseTypeDef",
     {
-        "Association": DataRepositoryAssociationOutputTypeDef,
+        "Association": DataRepositoryAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryAssociationsResponseOutputTypeDef = TypedDict(
-    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
+DescribeDataRepositoryAssociationsResponseTypeDef = TypedDict(
+    "DescribeDataRepositoryAssociationsResponseTypeDef",
     {
-        "Associations": List[DataRepositoryAssociationOutputTypeDef],
+        "Associations": List[DataRepositoryAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
-    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
+UpdateDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "UpdateDataRepositoryAssociationResponseTypeDef",
     {
-        "Association": DataRepositoryAssociationOutputTypeDef,
+        "Association": DataRepositoryAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFileCacheResponseOutputTypeDef = TypedDict(
-    "CreateFileCacheResponseOutputTypeDef",
+CreateFileCacheResponseTypeDef = TypedDict(
+    "CreateFileCacheResponseTypeDef",
     {
-        "FileCache": FileCacheCreatingOutputTypeDef,
+        "FileCache": FileCacheCreatingTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileCachesResponseOutputTypeDef = TypedDict(
-    "DescribeFileCachesResponseOutputTypeDef",
+DescribeFileCachesResponseTypeDef = TypedDict(
+    "DescribeFileCachesResponseTypeDef",
     {
-        "FileCaches": List[FileCacheOutputTypeDef],
+        "FileCaches": List[FileCacheTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateFileCacheResponseOutputTypeDef = TypedDict(
-    "UpdateFileCacheResponseOutputTypeDef",
+UpdateFileCacheResponseTypeDef = TypedDict(
+    "UpdateFileCacheResponseTypeDef",
     {
-        "FileCache": FileCacheOutputTypeDef,
+        "FileCache": FileCacheTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FileSystemOutputTypeDef = TypedDict(
-    "FileSystemOutputTypeDef",
+FileSystemTypeDef = TypedDict(
+    "FileSystemTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileSystemId": str,
         "FileSystemType": FileSystemTypeType,
         "Lifecycle": FileSystemLifecycleType,
-        "FailureDetails": FileSystemFailureDetailsOutputTypeDef,
+        "FailureDetails": FileSystemFailureDetailsTypeDef,
         "StorageCapacity": int,
         "StorageType": StorageTypeType,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
-        "WindowsConfiguration": WindowsFileSystemConfigurationOutputTypeDef,
-        "LustreConfiguration": LustreFileSystemConfigurationOutputTypeDef,
-        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
-        "OntapConfiguration": OntapFileSystemConfigurationOutputTypeDef,
+        "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
+        "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationOutputTypeDef,
+        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
 )
 
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
@@ -2528,30 +2524,30 @@
 
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
-OntapVolumeConfigurationOutputTypeDef = TypedDict(
-    "OntapVolumeConfigurationOutputTypeDef",
+OntapVolumeConfigurationTypeDef = TypedDict(
+    "OntapVolumeConfigurationTypeDef",
     {
         "FlexCacheEndpointType": FlexCacheEndpointTypeType,
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
         "StorageEfficiencyEnabled": bool,
         "StorageVirtualMachineId": str,
         "StorageVirtualMachineRoot": bool,
         "TieringPolicy": TieringPolicyOutputTypeDef,
         "UUID": str,
         "OntapVolumeType": OntapVolumeTypeType,
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
-        "SnaplockConfiguration": SnaplockConfigurationOutputTypeDef,
+        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
     },
 )
 
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
@@ -2589,35 +2585,35 @@
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
         "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-CreateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
-    "CreateStorageVirtualMachineResponseOutputTypeDef",
+CreateStorageVirtualMachineResponseTypeDef = TypedDict(
+    "CreateStorageVirtualMachineResponseTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageVirtualMachinesResponseOutputTypeDef = TypedDict(
-    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
+DescribeStorageVirtualMachinesResponseTypeDef = TypedDict(
+    "DescribeStorageVirtualMachinesResponseTypeDef",
     {
-        "StorageVirtualMachines": List[StorageVirtualMachineOutputTypeDef],
+        "StorageVirtualMachines": List[StorageVirtualMachineTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
-    "UpdateStorageVirtualMachineResponseOutputTypeDef",
+UpdateStorageVirtualMachineResponseTypeDef = TypedDict(
+    "UpdateStorageVirtualMachineResponseTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
     {
@@ -2674,29 +2670,29 @@
 )
 
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
-VolumeOutputTypeDef = TypedDict(
-    "VolumeOutputTypeDef",
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
     {
         "CreationTime": datetime,
         "FileSystemId": str,
         "Lifecycle": VolumeLifecycleType,
         "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationOutputTypeDef,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
         "VolumeId": str,
         "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationOutputTypeDef,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
     },
 )
 
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
@@ -2760,100 +2756,100 @@
 )
 
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
-AdministrativeActionOutputTypeDef = TypedDict(
-    "AdministrativeActionOutputTypeDef",
+AdministrativeActionTypeDef = TypedDict(
+    "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
         "TargetFileSystemValues": Dict[str, Any],
-        "FailureDetails": AdministrativeActionFailureDetailsOutputTypeDef,
+        "FailureDetails": AdministrativeActionFailureDetailsTypeDef,
         "TargetVolumeValues": Dict[str, Any],
         "TargetSnapshotValues": Dict[str, Any],
     },
 )
 
-BackupOutputTypeDef = TypedDict(
-    "BackupOutputTypeDef",
+BackupTypeDef = TypedDict(
+    "BackupTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
-        "FailureDetails": BackupFailureDetailsOutputTypeDef,
+        "FailureDetails": BackupFailureDetailsTypeDef,
         "Type": BackupTypeType,
         "ProgressPercent": int,
         "CreationTime": datetime,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagOutputTypeDef],
-        "FileSystem": "FileSystemOutputTypeDef",
-        "DirectoryInformation": ActiveDirectoryBackupAttributesOutputTypeDef,
+        "FileSystem": "FileSystemTypeDef",
+        "DirectoryInformation": ActiveDirectoryBackupAttributesTypeDef,
         "OwnerId": str,
         "SourceBackupId": str,
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
     },
 )
 
-CreateVolumeFromBackupResponseOutputTypeDef = TypedDict(
-    "CreateVolumeFromBackupResponseOutputTypeDef",
+CreateVolumeFromBackupResponseTypeDef = TypedDict(
+    "CreateVolumeFromBackupResponseTypeDef",
     {
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVolumeResponseOutputTypeDef = TypedDict(
-    "CreateVolumeResponseOutputTypeDef",
+CreateVolumeResponseTypeDef = TypedDict(
+    "CreateVolumeResponseTypeDef",
     {
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVolumesResponseOutputTypeDef = TypedDict(
-    "DescribeVolumesResponseOutputTypeDef",
+DescribeVolumesResponseTypeDef = TypedDict(
+    "DescribeVolumesResponseTypeDef",
     {
-        "Volumes": List[VolumeOutputTypeDef],
+        "Volumes": List[VolumeTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVolumeResponseOutputTypeDef = TypedDict(
-    "UpdateVolumeResponseOutputTypeDef",
+UpdateVolumeResponseTypeDef = TypedDict(
+    "UpdateVolumeResponseTypeDef",
     {
-        "Volume": VolumeOutputTypeDef,
+        "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CopyBackupResponseOutputTypeDef = TypedDict(
-    "CopyBackupResponseOutputTypeDef",
+CopyBackupResponseTypeDef = TypedDict(
+    "CopyBackupResponseTypeDef",
     {
-        "Backup": BackupOutputTypeDef,
+        "Backup": BackupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBackupResponseOutputTypeDef = TypedDict(
-    "CreateBackupResponseOutputTypeDef",
+CreateBackupResponseTypeDef = TypedDict(
+    "CreateBackupResponseTypeDef",
     {
-        "Backup": BackupOutputTypeDef,
+        "Backup": BackupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeBackupsResponseOutputTypeDef = TypedDict(
-    "DescribeBackupsResponseOutputTypeDef",
+DescribeBackupsResponseTypeDef = TypedDict(
+    "DescribeBackupsResponseTypeDef",
     {
-        "Backups": List[BackupOutputTypeDef],
+        "Backups": List[BackupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/PKG-INFO` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,110 +393,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_fsx.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fsx.type_defs import (
-    ActiveDirectoryBackupAttributesOutputTypeDef,
-    AdministrativeActionFailureDetailsOutputTypeDef,
-    AliasOutputTypeDef,
+    ActiveDirectoryBackupAttributesTypeDef,
+    AdministrativeActionFailureDetailsTypeDef,
+    AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
     AutoExportPolicyOutputTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyOutputTypeDef,
     AutoImportPolicyTypeDef,
     AutocommitPeriodOutputTypeDef,
     AutocommitPeriodTypeDef,
-    BackupFailureDetailsOutputTypeDef,
+    BackupFailureDetailsTypeDef,
     TagOutputTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
-    CancelDataRepositoryTaskResponseOutputTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportOutputTypeDef,
     CompletionReportTypeDef,
     TagTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
-    CreateFileSystemFromBackupResponseOutputTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
-    CreateFileSystemResponseOutputTypeDef,
+    CreateFileSystemResponseTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
-    DataRepositoryFailureDetailsOutputTypeDef,
-    DataRepositoryTaskFailureDetailsOutputTypeDef,
+    DataRepositoryFailureDetailsTypeDef,
+    DataRepositoryTaskFailureDetailsTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DataRepositoryTaskStatusOutputTypeDef,
+    DataRepositoryTaskStatusTypeDef,
     DeleteBackupRequestRequestTypeDef,
-    DeleteBackupResponseOutputTypeDef,
+    DeleteBackupResponseTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteDataRepositoryAssociationResponseOutputTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
-    DeleteFileCacheResponseOutputTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResponseOutputTypeDef,
+    DeleteSnapshotResponseTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
-    DeleteStorageVirtualMachineResponseOutputTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
-    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeFileSystemsResponseTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
     DiskIopsConfigurationOutputTypeDef,
-    FileCacheFailureDetailsOutputTypeDef,
+    FileCacheFailureDetailsTypeDef,
     FileCacheNFSConfigurationTypeDef,
     FileCacheLustreMetadataConfigurationOutputTypeDef,
-    LustreLogConfigurationOutputTypeDef,
-    FileSystemEndpointOutputTypeDef,
-    FileSystemFailureDetailsOutputTypeDef,
-    LifecycleTransitionReasonOutputTypeDef,
+    LustreLogConfigurationTypeDef,
+    FileSystemEndpointTypeDef,
+    FileSystemFailureDetailsTypeDef,
+    LifecycleTransitionReasonTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LustreRootSquashConfigurationOutputTypeDef,
     TieringPolicyOutputTypeDef,
     OpenZFSClientConfigurationOutputTypeDef,
     OpenZFSClientConfigurationTypeDef,
-    OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+    OpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaOutputTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
-    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     RetentionPeriodOutputTypeDef,
     RetentionPeriodTypeDef,
-    SelfManagedActiveDirectoryAttributesOutputTypeDef,
+    SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
-    SvmEndpointOutputTypeDef,
+    SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileSystemResponseOutputTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
-    WindowsAuditLogConfigurationOutputTypeDef,
-    AssociateFileSystemAliasesResponseOutputTypeDef,
-    DescribeFileSystemAliasesResponseOutputTypeDef,
-    DisassociateFileSystemAliasesResponseOutputTypeDef,
-    NFSDataRepositoryConfigurationOutputTypeDef,
+    WindowsAuditLogConfigurationTypeDef,
+    AssociateFileSystemAliasesResponseTypeDef,
+    DescribeFileSystemAliasesResponseTypeDef,
+    DisassociateFileSystemAliasesResponseTypeDef,
+    NFSDataRepositoryConfigurationTypeDef,
     S3DataRepositoryConfigurationOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
-    DeleteFileSystemLustreResponseOutputTypeDef,
-    DeleteFileSystemOpenZFSResponseOutputTypeDef,
-    DeleteFileSystemWindowsResponseOutputTypeDef,
-    DeleteVolumeOntapResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    DeleteFileSystemLustreResponseTypeDef,
+    DeleteFileSystemOpenZFSResponseTypeDef,
+    DeleteFileSystemWindowsResponseTypeDef,
+    DeleteVolumeOntapResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
@@ -506,101 +506,101 @@
     CreateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    DataRepositoryConfigurationOutputTypeDef,
+    DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
-    DataRepositoryTaskOutputTypeDef,
+    DataRepositoryTaskTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
-    OpenZFSFileSystemConfigurationOutputTypeDef,
+    OpenZFSFileSystemConfigurationTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
-    FileCacheLustreConfigurationOutputTypeDef,
-    FileSystemEndpointsOutputTypeDef,
-    SnapshotOutputTypeDef,
+    FileCacheLustreConfigurationTypeDef,
+    FileSystemEndpointsTypeDef,
+    SnapshotTypeDef,
     OpenZFSNfsExportOutputTypeDef,
     OpenZFSNfsExportTypeDef,
     SnaplockRetentionPeriodOutputTypeDef,
     SnaplockRetentionPeriodTypeDef,
-    SvmActiveDirectoryConfigurationOutputTypeDef,
+    SvmActiveDirectoryConfigurationTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    SvmEndpointsOutputTypeDef,
+    SvmEndpointsTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
-    WindowsFileSystemConfigurationOutputTypeDef,
-    DataRepositoryAssociationOutputTypeDef,
+    WindowsFileSystemConfigurationTypeDef,
+    DataRepositoryAssociationTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteFileSystemResponseOutputTypeDef,
-    DeleteVolumeResponseOutputTypeDef,
+    DeleteFileSystemResponseTypeDef,
+    DeleteVolumeResponseTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteVolumeRequestRequestTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    LustreFileSystemConfigurationOutputTypeDef,
-    CreateDataRepositoryTaskResponseOutputTypeDef,
-    DescribeDataRepositoryTasksResponseOutputTypeDef,
+    LustreFileSystemConfigurationTypeDef,
+    CreateDataRepositoryTaskResponseTypeDef,
+    DescribeDataRepositoryTasksResponseTypeDef,
     CreateFileCacheRequestRequestTypeDef,
-    FileCacheCreatingOutputTypeDef,
-    FileCacheOutputTypeDef,
-    OntapFileSystemConfigurationOutputTypeDef,
-    CreateSnapshotResponseOutputTypeDef,
-    DescribeSnapshotsResponseOutputTypeDef,
-    UpdateSnapshotResponseOutputTypeDef,
-    OpenZFSVolumeConfigurationOutputTypeDef,
+    FileCacheCreatingTypeDef,
+    FileCacheTypeDef,
+    OntapFileSystemConfigurationTypeDef,
+    CreateSnapshotResponseTypeDef,
+    DescribeSnapshotsResponseTypeDef,
+    UpdateSnapshotResponseTypeDef,
+    OpenZFSVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    SnaplockConfigurationOutputTypeDef,
+    SnaplockConfigurationTypeDef,
     CreateSnaplockConfigurationTypeDef,
     UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
-    StorageVirtualMachineOutputTypeDef,
-    CreateDataRepositoryAssociationResponseOutputTypeDef,
-    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
-    UpdateDataRepositoryAssociationResponseOutputTypeDef,
-    CreateFileCacheResponseOutputTypeDef,
-    DescribeFileCachesResponseOutputTypeDef,
-    UpdateFileCacheResponseOutputTypeDef,
-    FileSystemOutputTypeDef,
+    StorageVirtualMachineTypeDef,
+    CreateDataRepositoryAssociationResponseTypeDef,
+    DescribeDataRepositoryAssociationsResponseTypeDef,
+    UpdateDataRepositoryAssociationResponseTypeDef,
+    CreateFileCacheResponseTypeDef,
+    DescribeFileCachesResponseTypeDef,
+    UpdateFileCacheResponseTypeDef,
+    FileSystemTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    OntapVolumeConfigurationOutputTypeDef,
+    OntapVolumeConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
-    CreateStorageVirtualMachineResponseOutputTypeDef,
-    DescribeStorageVirtualMachinesResponseOutputTypeDef,
-    UpdateStorageVirtualMachineResponseOutputTypeDef,
+    CreateStorageVirtualMachineResponseTypeDef,
+    DescribeStorageVirtualMachinesResponseTypeDef,
+    UpdateStorageVirtualMachineResponseTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
-    VolumeOutputTypeDef,
+    VolumeTypeDef,
     CreateVolumeFromBackupRequestRequestTypeDef,
     CreateVolumeRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
-    AdministrativeActionOutputTypeDef,
-    BackupOutputTypeDef,
-    CreateVolumeFromBackupResponseOutputTypeDef,
-    CreateVolumeResponseOutputTypeDef,
-    DescribeVolumesResponseOutputTypeDef,
-    UpdateVolumeResponseOutputTypeDef,
-    CopyBackupResponseOutputTypeDef,
-    CreateBackupResponseOutputTypeDef,
-    DescribeBackupsResponseOutputTypeDef,
+    AdministrativeActionTypeDef,
+    BackupTypeDef,
+    CreateVolumeFromBackupResponseTypeDef,
+    CreateVolumeResponseTypeDef,
+    DescribeVolumesResponseTypeDef,
+    UpdateVolumeResponseTypeDef,
+    CopyBackupResponseTypeDef,
+    CreateBackupResponseTypeDef,
+    DescribeBackupsResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryBackupAttributesOutputTypeDef:
+def get_structure() -> ActiveDirectoryBackupAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/SOURCES.txt` & `mypy-boto3-fsx-1.28.3.post2/mypy_boto3_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3.post1/setup.py` & `mypy-boto3-fsx-1.28.3.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fsx",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.7"
+        "Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

