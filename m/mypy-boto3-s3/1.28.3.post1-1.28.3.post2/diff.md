# Comparing `tmp/mypy-boto3-s3-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-s3-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
+gzip compressed data, was "mypy-boto3-s3-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:35 2023, max compression
```

## Comparing `mypy-boto3-s3-1.28.3.post1.tar` & `mypy-boto3-s3-1.28.3.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37496 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36025 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.003731 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84515 2023-07-14 16:17:05.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    84396 2023-07-14 16:17:05.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-07-14 16:17:08.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-14 16:17:08.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   118063 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   117847 2023-07-14 16:17:06.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   206191 2023-07-14 16:17:13.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   205879 2023-07-14 16:17:11.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37496 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37030 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.242399 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83859 2023-07-15 06:37:38.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83740 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   117865 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117649 2023-07-15 06:37:38.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   204619 2023-07-15 06:37:47.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204307 2023-07-15 06:37:44.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37030 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-s3-1.28.3.post1/LICENSE` & `mypy-boto3-s3-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/PKG-INFO` & `mypy-boto3-s3-1.28.3.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -553,55 +553,55 @@
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
     TagOutputTypeDef,
     TagTypeDef,
     AnalyticsS3BucketDestinationOutputTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
     CopySourceTypeDef,
     BucketDownloadFileRequestTypeDef,
     BucketDownloadFileobjRequestTypeDef,
-    BucketOutputTypeDef,
+    BucketTypeDef,
     BucketUploadFileRequestTypeDef,
     BucketUploadFileobjRequestTypeDef,
     CORSRuleTypeDef,
     CORSRuleOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
-    ChecksumOutputTypeDef,
+    ChecksumTypeDef,
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
-    CommonPrefixOutputTypeDef,
-    CompleteMultipartUploadOutputOutputTypeDef,
+    CommonPrefixTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionOutputTypeDef,
     ConditionTypeDef,
-    CopyObjectResultOutputTypeDef,
+    CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
-    CopyPartResultOutputTypeDef,
+    CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    CreateMultipartUploadOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
@@ -622,95 +622,95 @@
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     OwnerOutputTypeDef,
     DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
-    DeletedObjectOutputTypeDef,
-    ErrorOutputTypeDef,
+    DeletedObjectTypeDef,
+    ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     ErrorDocumentOutputTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    PolicyStatusOutputTypeDef,
+    PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentOutputTypeDef,
     RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
-    ObjectPartOutputTypeDef,
+    ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputOutputTypeDef,
+    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     IndexDocumentTypeDef,
-    InitiatorOutputTypeDef,
     InitiatorResponseMetadataTypeDef,
+    InitiatorTypeDef,
     JSONInputTypeDef,
     TieringOutputTypeDef,
     TieringTypeDef,
     InventoryFilterOutputTypeDef,
     InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
@@ -733,78 +733,78 @@
     ListMultipartUploadsRequestRequestTypeDef,
     ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
     ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
     ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
-    PartOutputTypeDef,
+    PartTypeDef,
     ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedOutputTypeDef,
     TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
-    RestoreStatusOutputTypeDef,
+    RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
     OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
     PaginatorConfigTypeDef,
-    ProgressOutputTypeDef,
+    ProgressTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectLegalHoldOutputOutputTypeDef,
-    PutObjectLockConfigurationOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputOutputTypeDef,
-    PutObjectTaggingOutputOutputTypeDef,
-    RecordsEventOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RecordsEventTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectAllRequestsToTypeDef,
     RedirectOutputTypeDef,
     RedirectTypeDef,
     ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
     ResponseMetadataTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StatsOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    StatsTypeDef,
+    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     AnalyticsAndOperatorOutputTypeDef,
-    GetBucketTaggingOutputOutputTypeDef,
-    GetObjectTaggingOutputOutputTypeDef,
+    GetBucketTaggingOutputTypeDef,
+    GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorOutputTypeDef,
     MetricsAndOperatorOutputTypeDef,
     ReplicationRuleAndOperatorOutputTypeDef,
     AnalyticsAndOperatorTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
@@ -816,75 +816,75 @@
     BucketCopyRequestTypeDef,
     ClientCopyRequestTypeDef,
     CopyObjectRequestRequestTypeDef,
     ObjectCopyRequestTypeDef,
     UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     UploadPartCopyRequestRequestTypeDef,
     CORSConfigurationTypeDef,
-    GetBucketCorsOutputOutputTypeDef,
+    GetBucketCorsOutputTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputOutputTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
+    CopyObjectOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
     CreateBucketRequestBucketCreateTypeDef,
     CreateBucketRequestRequestTypeDef,
     CreateBucketRequestServiceResourceCreateBucketTypeDef,
     ObjectLockRuleOutputTypeDef,
     ObjectLockRuleTypeDef,
-    DeleteMarkerEntryOutputTypeDef,
-    ListBucketsOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
+    DeleteMarkerEntryTypeDef,
+    ListBucketsOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     S3KeyFilterOutputTypeDef,
     S3KeyFilterTypeDef,
-    GetBucketPolicyStatusOutputOutputTypeDef,
-    GetObjectAttributesPartsOutputTypeDef,
-    GetObjectLegalHoldOutputOutputTypeDef,
-    GetObjectRetentionOutputOutputTypeDef,
-    GetPublicAccessBlockOutputOutputTypeDef,
+    GetBucketPolicyStatusOutputTypeDef,
+    GetObjectAttributesPartsTypeDef,
+    GetObjectLegalHoldOutputTypeDef,
+    GetObjectRetentionOutputTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
     GrantOutputTypeDef,
     TargetGrantOutputTypeDef,
     GrantTypeDef,
     TargetGrantTypeDef,
     HeadBucketRequestBucketExistsWaitTypeDef,
     HeadBucketRequestBucketNotExistsWaitTypeDef,
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
-    MultipartUploadOutputTypeDef,
+    MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListPartsOutputTypeDef,
     MetricsOutputTypeDef,
     ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
-    NotificationConfigurationDeprecatedOutputTypeDef,
+    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     PutObjectLegalHoldRequestRequestTypeDef,
     PutObjectRetentionRequestRequestTypeDef,
-    ObjectOutputTypeDef,
-    ObjectVersionOutputTypeDef,
+    ObjectTypeDef,
+    ObjectVersionTypeDef,
     OwnershipControlsOutputTypeDef,
     OwnershipControlsTypeDef,
-    ProgressEventOutputTypeDef,
+    ProgressEventTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
     PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     PutBucketRequestPaymentRequestRequestTypeDef,
     PutBucketVersioningRequestBucketVersioningPutTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
     RoutingRuleOutputTypeDef,
     RoutingRuleTypeDef,
     ServerSideEncryptionRuleOutputTypeDef,
     ServerSideEncryptionRuleTypeDef,
     SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
-    StatsEventOutputTypeDef,
+    StatsEventTypeDef,
     AnalyticsFilterOutputTypeDef,
     IntelligentTieringFilterOutputTypeDef,
     LifecycleRuleFilterOutputTypeDef,
     MetricsFilterOutputTypeDef,
     ReplicationRuleFilterOutputTypeDef,
     AnalyticsFilterTypeDef,
     IntelligentTieringFilterTypeDef,
@@ -902,109 +902,109 @@
     CompleteMultipartUploadRequestRequestTypeDef,
     ObjectLockConfigurationOutputTypeDef,
     ObjectLockConfigurationTypeDef,
     DeleteObjectsRequestBucketDeleteObjectsTypeDef,
     DeleteObjectsRequestRequestTypeDef,
     NotificationConfigurationFilterOutputTypeDef,
     NotificationConfigurationFilterTypeDef,
-    GetObjectAttributesOutputOutputTypeDef,
-    GetBucketAclOutputOutputTypeDef,
-    GetObjectAclOutputOutputTypeDef,
+    GetObjectAttributesOutputTypeDef,
+    GetBucketAclOutputTypeDef,
+    GetObjectAclOutputTypeDef,
     LoggingEnabledOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     AccessControlPolicyTypeDef,
     S3LocationTypeDef,
     LoggingEnabledTypeDef,
-    ListMultipartUploadsOutputOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
     InventoryS3BucketDestinationOutputTypeDef,
     InventoryS3BucketDestinationTypeDef,
     SelectObjectContentRequestRequestTypeDef,
     SelectParametersTypeDef,
-    GetBucketLifecycleOutputOutputTypeDef,
+    GetBucketLifecycleOutputTypeDef,
     LifecycleConfigurationTypeDef,
     DestinationOutputTypeDef,
     DestinationTypeDef,
     PutBucketNotificationRequestRequestTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    GetBucketOwnershipControlsOutputOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    GetBucketOwnershipControlsOutputTypeDef,
     PutBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketWebsiteOutputOutputTypeDef,
+    GetBucketWebsiteOutputTypeDef,
     WebsiteConfigurationTypeDef,
     ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SelectObjectContentEventStreamOutputTypeDef,
+    SelectObjectContentEventStreamTypeDef,
     IntelligentTieringConfigurationOutputTypeDef,
     LifecycleRuleOutputTypeDef,
     MetricsConfigurationOutputTypeDef,
     IntelligentTieringConfigurationTypeDef,
     LifecycleRuleTypeDef,
     MetricsConfigurationTypeDef,
     StorageClassAnalysisOutputTypeDef,
     StorageClassAnalysisTypeDef,
-    GetObjectLockConfigurationOutputOutputTypeDef,
+    GetObjectLockConfigurationOutputTypeDef,
     PutObjectLockConfigurationRequestRequestTypeDef,
     LambdaFunctionConfigurationOutputTypeDef,
     QueueConfigurationOutputTypeDef,
     TopicConfigurationOutputTypeDef,
     LambdaFunctionConfigurationTypeDef,
     QueueConfigurationTypeDef,
     TopicConfigurationTypeDef,
-    GetBucketLoggingOutputOutputTypeDef,
+    GetBucketLoggingOutputTypeDef,
     PutBucketAclRequestBucketAclPutTypeDef,
     PutBucketAclRequestRequestTypeDef,
     PutObjectAclRequestObjectAclPutTypeDef,
     PutObjectAclRequestRequestTypeDef,
     OutputLocationTypeDef,
     BucketLoggingStatusTypeDef,
     InventoryDestinationOutputTypeDef,
     InventoryDestinationTypeDef,
     PutBucketLifecycleRequestBucketLifecyclePutTypeDef,
     PutBucketLifecycleRequestRequestTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     PutBucketWebsiteRequestBucketWebsitePutTypeDef,
     PutBucketWebsiteRequestRequestTypeDef,
-    GetBucketEncryptionOutputOutputTypeDef,
+    GetBucketEncryptionOutputTypeDef,
     PutBucketEncryptionRequestRequestTypeDef,
-    SelectObjectContentOutputOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputOutputTypeDef,
-    GetBucketMetricsConfigurationOutputOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputOutputTypeDef,
+    SelectObjectContentOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputTypeDef,
+    GetBucketMetricsConfigurationOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputTypeDef,
     PutBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     BucketLifecycleConfigurationTypeDef,
     PutBucketMetricsConfigurationRequestRequestTypeDef,
     AnalyticsConfigurationOutputTypeDef,
     AnalyticsConfigurationTypeDef,
-    NotificationConfigurationOutputTypeDef,
+    NotificationConfigurationResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     RestoreRequestTypeDef,
     PutBucketLoggingRequestBucketLoggingPutTypeDef,
     PutBucketLoggingRequestRequestTypeDef,
     InventoryConfigurationOutputTypeDef,
     InventoryConfigurationTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
-    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
-    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputTypeDef,
     PutBucketAnalyticsConfigurationRequestRequestTypeDef,
     PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     PutBucketNotificationConfigurationRequestRequestTypeDef,
     RestoreObjectRequestObjectRestoreObjectTypeDef,
     RestoreObjectRequestObjectSummaryRestoreObjectTypeDef,
     RestoreObjectRequestRequestTypeDef,
-    GetBucketInventoryConfigurationOutputOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputOutputTypeDef,
+    GetBucketInventoryConfigurationOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputTypeDef,
     PutBucketInventoryConfigurationRequestRequestTypeDef,
-    GetBucketReplicationOutputOutputTypeDef,
+    GetBucketReplicationOutputTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-s3-1.28.3.post1/README.md` & `mypy-boto3-s3-1.28.3.post2/README.md`

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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -521,55 +521,55 @@
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
     TagOutputTypeDef,
     TagTypeDef,
     AnalyticsS3BucketDestinationOutputTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
     CopySourceTypeDef,
     BucketDownloadFileRequestTypeDef,
     BucketDownloadFileobjRequestTypeDef,
-    BucketOutputTypeDef,
+    BucketTypeDef,
     BucketUploadFileRequestTypeDef,
     BucketUploadFileobjRequestTypeDef,
     CORSRuleTypeDef,
     CORSRuleOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
-    ChecksumOutputTypeDef,
+    ChecksumTypeDef,
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
-    CommonPrefixOutputTypeDef,
-    CompleteMultipartUploadOutputOutputTypeDef,
+    CommonPrefixTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionOutputTypeDef,
     ConditionTypeDef,
-    CopyObjectResultOutputTypeDef,
+    CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
-    CopyPartResultOutputTypeDef,
+    CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    CreateMultipartUploadOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
@@ -590,95 +590,95 @@
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     OwnerOutputTypeDef,
     DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
-    DeletedObjectOutputTypeDef,
-    ErrorOutputTypeDef,
+    DeletedObjectTypeDef,
+    ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     ErrorDocumentOutputTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    PolicyStatusOutputTypeDef,
+    PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentOutputTypeDef,
     RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
-    ObjectPartOutputTypeDef,
+    ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputOutputTypeDef,
+    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     IndexDocumentTypeDef,
-    InitiatorOutputTypeDef,
     InitiatorResponseMetadataTypeDef,
+    InitiatorTypeDef,
     JSONInputTypeDef,
     TieringOutputTypeDef,
     TieringTypeDef,
     InventoryFilterOutputTypeDef,
     InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
@@ -701,78 +701,78 @@
     ListMultipartUploadsRequestRequestTypeDef,
     ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
     ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
     ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
-    PartOutputTypeDef,
+    PartTypeDef,
     ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedOutputTypeDef,
     TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
-    RestoreStatusOutputTypeDef,
+    RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
     OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
     PaginatorConfigTypeDef,
-    ProgressOutputTypeDef,
+    ProgressTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectLegalHoldOutputOutputTypeDef,
-    PutObjectLockConfigurationOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputOutputTypeDef,
-    PutObjectTaggingOutputOutputTypeDef,
-    RecordsEventOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RecordsEventTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectAllRequestsToTypeDef,
     RedirectOutputTypeDef,
     RedirectTypeDef,
     ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
     ResponseMetadataTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StatsOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    StatsTypeDef,
+    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     AnalyticsAndOperatorOutputTypeDef,
-    GetBucketTaggingOutputOutputTypeDef,
-    GetObjectTaggingOutputOutputTypeDef,
+    GetBucketTaggingOutputTypeDef,
+    GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorOutputTypeDef,
     MetricsAndOperatorOutputTypeDef,
     ReplicationRuleAndOperatorOutputTypeDef,
     AnalyticsAndOperatorTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
@@ -784,75 +784,75 @@
     BucketCopyRequestTypeDef,
     ClientCopyRequestTypeDef,
     CopyObjectRequestRequestTypeDef,
     ObjectCopyRequestTypeDef,
     UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     UploadPartCopyRequestRequestTypeDef,
     CORSConfigurationTypeDef,
-    GetBucketCorsOutputOutputTypeDef,
+    GetBucketCorsOutputTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputOutputTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
+    CopyObjectOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
     CreateBucketRequestBucketCreateTypeDef,
     CreateBucketRequestRequestTypeDef,
     CreateBucketRequestServiceResourceCreateBucketTypeDef,
     ObjectLockRuleOutputTypeDef,
     ObjectLockRuleTypeDef,
-    DeleteMarkerEntryOutputTypeDef,
-    ListBucketsOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
+    DeleteMarkerEntryTypeDef,
+    ListBucketsOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     S3KeyFilterOutputTypeDef,
     S3KeyFilterTypeDef,
-    GetBucketPolicyStatusOutputOutputTypeDef,
-    GetObjectAttributesPartsOutputTypeDef,
-    GetObjectLegalHoldOutputOutputTypeDef,
-    GetObjectRetentionOutputOutputTypeDef,
-    GetPublicAccessBlockOutputOutputTypeDef,
+    GetBucketPolicyStatusOutputTypeDef,
+    GetObjectAttributesPartsTypeDef,
+    GetObjectLegalHoldOutputTypeDef,
+    GetObjectRetentionOutputTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
     GrantOutputTypeDef,
     TargetGrantOutputTypeDef,
     GrantTypeDef,
     TargetGrantTypeDef,
     HeadBucketRequestBucketExistsWaitTypeDef,
     HeadBucketRequestBucketNotExistsWaitTypeDef,
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
-    MultipartUploadOutputTypeDef,
+    MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListPartsOutputTypeDef,
     MetricsOutputTypeDef,
     ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
-    NotificationConfigurationDeprecatedOutputTypeDef,
+    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     PutObjectLegalHoldRequestRequestTypeDef,
     PutObjectRetentionRequestRequestTypeDef,
-    ObjectOutputTypeDef,
-    ObjectVersionOutputTypeDef,
+    ObjectTypeDef,
+    ObjectVersionTypeDef,
     OwnershipControlsOutputTypeDef,
     OwnershipControlsTypeDef,
-    ProgressEventOutputTypeDef,
+    ProgressEventTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
     PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     PutBucketRequestPaymentRequestRequestTypeDef,
     PutBucketVersioningRequestBucketVersioningPutTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
     RoutingRuleOutputTypeDef,
     RoutingRuleTypeDef,
     ServerSideEncryptionRuleOutputTypeDef,
     ServerSideEncryptionRuleTypeDef,
     SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
-    StatsEventOutputTypeDef,
+    StatsEventTypeDef,
     AnalyticsFilterOutputTypeDef,
     IntelligentTieringFilterOutputTypeDef,
     LifecycleRuleFilterOutputTypeDef,
     MetricsFilterOutputTypeDef,
     ReplicationRuleFilterOutputTypeDef,
     AnalyticsFilterTypeDef,
     IntelligentTieringFilterTypeDef,
@@ -870,109 +870,109 @@
     CompleteMultipartUploadRequestRequestTypeDef,
     ObjectLockConfigurationOutputTypeDef,
     ObjectLockConfigurationTypeDef,
     DeleteObjectsRequestBucketDeleteObjectsTypeDef,
     DeleteObjectsRequestRequestTypeDef,
     NotificationConfigurationFilterOutputTypeDef,
     NotificationConfigurationFilterTypeDef,
-    GetObjectAttributesOutputOutputTypeDef,
-    GetBucketAclOutputOutputTypeDef,
-    GetObjectAclOutputOutputTypeDef,
+    GetObjectAttributesOutputTypeDef,
+    GetBucketAclOutputTypeDef,
+    GetObjectAclOutputTypeDef,
     LoggingEnabledOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     AccessControlPolicyTypeDef,
     S3LocationTypeDef,
     LoggingEnabledTypeDef,
-    ListMultipartUploadsOutputOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
     InventoryS3BucketDestinationOutputTypeDef,
     InventoryS3BucketDestinationTypeDef,
     SelectObjectContentRequestRequestTypeDef,
     SelectParametersTypeDef,
-    GetBucketLifecycleOutputOutputTypeDef,
+    GetBucketLifecycleOutputTypeDef,
     LifecycleConfigurationTypeDef,
     DestinationOutputTypeDef,
     DestinationTypeDef,
     PutBucketNotificationRequestRequestTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    GetBucketOwnershipControlsOutputOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    GetBucketOwnershipControlsOutputTypeDef,
     PutBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketWebsiteOutputOutputTypeDef,
+    GetBucketWebsiteOutputTypeDef,
     WebsiteConfigurationTypeDef,
     ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SelectObjectContentEventStreamOutputTypeDef,
+    SelectObjectContentEventStreamTypeDef,
     IntelligentTieringConfigurationOutputTypeDef,
     LifecycleRuleOutputTypeDef,
     MetricsConfigurationOutputTypeDef,
     IntelligentTieringConfigurationTypeDef,
     LifecycleRuleTypeDef,
     MetricsConfigurationTypeDef,
     StorageClassAnalysisOutputTypeDef,
     StorageClassAnalysisTypeDef,
-    GetObjectLockConfigurationOutputOutputTypeDef,
+    GetObjectLockConfigurationOutputTypeDef,
     PutObjectLockConfigurationRequestRequestTypeDef,
     LambdaFunctionConfigurationOutputTypeDef,
     QueueConfigurationOutputTypeDef,
     TopicConfigurationOutputTypeDef,
     LambdaFunctionConfigurationTypeDef,
     QueueConfigurationTypeDef,
     TopicConfigurationTypeDef,
-    GetBucketLoggingOutputOutputTypeDef,
+    GetBucketLoggingOutputTypeDef,
     PutBucketAclRequestBucketAclPutTypeDef,
     PutBucketAclRequestRequestTypeDef,
     PutObjectAclRequestObjectAclPutTypeDef,
     PutObjectAclRequestRequestTypeDef,
     OutputLocationTypeDef,
     BucketLoggingStatusTypeDef,
     InventoryDestinationOutputTypeDef,
     InventoryDestinationTypeDef,
     PutBucketLifecycleRequestBucketLifecyclePutTypeDef,
     PutBucketLifecycleRequestRequestTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     PutBucketWebsiteRequestBucketWebsitePutTypeDef,
     PutBucketWebsiteRequestRequestTypeDef,
-    GetBucketEncryptionOutputOutputTypeDef,
+    GetBucketEncryptionOutputTypeDef,
     PutBucketEncryptionRequestRequestTypeDef,
-    SelectObjectContentOutputOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputOutputTypeDef,
-    GetBucketMetricsConfigurationOutputOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputOutputTypeDef,
+    SelectObjectContentOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputTypeDef,
+    GetBucketMetricsConfigurationOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputTypeDef,
     PutBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     BucketLifecycleConfigurationTypeDef,
     PutBucketMetricsConfigurationRequestRequestTypeDef,
     AnalyticsConfigurationOutputTypeDef,
     AnalyticsConfigurationTypeDef,
-    NotificationConfigurationOutputTypeDef,
+    NotificationConfigurationResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     RestoreRequestTypeDef,
     PutBucketLoggingRequestBucketLoggingPutTypeDef,
     PutBucketLoggingRequestRequestTypeDef,
     InventoryConfigurationOutputTypeDef,
     InventoryConfigurationTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
-    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
-    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputTypeDef,
     PutBucketAnalyticsConfigurationRequestRequestTypeDef,
     PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     PutBucketNotificationConfigurationRequestRequestTypeDef,
     RestoreObjectRequestObjectRestoreObjectTypeDef,
     RestoreObjectRequestObjectSummaryRestoreObjectTypeDef,
     RestoreObjectRequestRequestTypeDef,
-    GetBucketInventoryConfigurationOutputOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputOutputTypeDef,
+    GetBucketInventoryConfigurationOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputTypeDef,
     PutBucketInventoryConfigurationRequestRequestTypeDef,
-    GetBucketReplicationOutputOutputTypeDef,
+    GetBucketReplicationOutputTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__main__.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
-        " 7.14.7\nDocs:           "
+        "Type annotations for boto3.S3 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
+        " 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
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

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,105 +39,105 @@
     ListMultipartUploadsPaginator,
     ListObjectsPaginator,
     ListObjectsV2Paginator,
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
     AnalyticsConfigurationTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CompleteMultipartUploadOutputOutputTypeDef,
-    CopyObjectOutputOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CopyObjectOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    CreateMultipartUploadOutputOutputTypeDef,
-    DeleteObjectOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
-    DeleteObjectTaggingOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
     DeleteTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetBucketAccelerateConfigurationOutputOutputTypeDef,
-    GetBucketAclOutputOutputTypeDef,
-    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
-    GetBucketCorsOutputOutputTypeDef,
-    GetBucketEncryptionOutputOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
-    GetBucketInventoryConfigurationOutputOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputOutputTypeDef,
-    GetBucketLifecycleOutputOutputTypeDef,
-    GetBucketLocationOutputOutputTypeDef,
-    GetBucketLoggingOutputOutputTypeDef,
-    GetBucketMetricsConfigurationOutputOutputTypeDef,
-    GetBucketOwnershipControlsOutputOutputTypeDef,
-    GetBucketPolicyOutputOutputTypeDef,
-    GetBucketPolicyStatusOutputOutputTypeDef,
-    GetBucketReplicationOutputOutputTypeDef,
-    GetBucketRequestPaymentOutputOutputTypeDef,
-    GetBucketTaggingOutputOutputTypeDef,
-    GetBucketVersioningOutputOutputTypeDef,
-    GetBucketWebsiteOutputOutputTypeDef,
-    GetObjectAclOutputOutputTypeDef,
-    GetObjectAttributesOutputOutputTypeDef,
-    GetObjectLegalHoldOutputOutputTypeDef,
-    GetObjectLockConfigurationOutputOutputTypeDef,
-    GetObjectOutputOutputTypeDef,
-    GetObjectRetentionOutputOutputTypeDef,
-    GetObjectTaggingOutputOutputTypeDef,
-    GetObjectTorrentOutputOutputTypeDef,
-    GetPublicAccessBlockOutputOutputTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketAclOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputTypeDef,
+    GetBucketCorsOutputTypeDef,
+    GetBucketEncryptionOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputTypeDef,
+    GetBucketInventoryConfigurationOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputTypeDef,
+    GetBucketLifecycleOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketLoggingOutputTypeDef,
+    GetBucketMetricsConfigurationOutputTypeDef,
+    GetBucketOwnershipControlsOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketPolicyStatusOutputTypeDef,
+    GetBucketReplicationOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketTaggingOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetBucketWebsiteOutputTypeDef,
+    GetObjectAclOutputTypeDef,
+    GetObjectAttributesOutputTypeDef,
+    GetObjectLegalHoldOutputTypeDef,
+    GetObjectLockConfigurationOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectRetentionOutputTypeDef,
+    GetObjectTaggingOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    HeadObjectOutputTypeDef,
     InputSerializationTypeDef,
     IntelligentTieringConfigurationTypeDef,
     InventoryConfigurationTypeDef,
     LifecycleConfigurationTypeDef,
-    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputOutputTypeDef,
-    ListBucketsOutputOutputTypeDef,
-    ListMultipartUploadsOutputOutputTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputTypeDef,
+    ListBucketsOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    ListPartsOutputTypeDef,
     MetricsConfigurationTypeDef,
-    NotificationConfigurationDeprecatedOutputTypeDef,
+    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    NotificationConfigurationOutputTypeDef,
+    NotificationConfigurationResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     OutputSerializationTypeDef,
     OwnershipControlsTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectLegalHoldOutputOutputTypeDef,
-    PutObjectLockConfigurationOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
-    PutObjectRetentionOutputOutputTypeDef,
-    PutObjectTaggingOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
     ReplicationConfigurationTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
-    SelectObjectContentOutputOutputTypeDef,
+    SelectObjectContentOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TaggingTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
+    UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 from .waiter import (
     BucketExistsWaiter,
     BucketNotExistsWaiter,
     ObjectExistsWaiter,
@@ -194,15 +194,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputOutputTypeDef:
+    ) -> AbortMultipartUploadOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.abort_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#abort_multipart_upload)
         """
 
@@ -234,15 +234,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> CompleteMultipartUploadOutputOutputTypeDef:
+    ) -> CompleteMultipartUploadOutputTypeDef:
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.complete_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#complete_multipart_upload)
         """
 
@@ -303,15 +303,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputOutputTypeDef:
+    ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#copy_object)
         """
 
@@ -324,15 +324,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputOutputTypeDef:
+    ) -> CreateBucketOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_bucket)
         """
 
@@ -365,15 +365,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> CreateMultipartUploadOutputOutputTypeDef:
+    ) -> CreateMultipartUploadOutputTypeDef:
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_multipart_upload)
         """
 
@@ -518,26 +518,26 @@
         Bucket: str,
         Key: str,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object)
         """
 
     def delete_object_tagging(
         self, *, Bucket: str, Key: str, VersionId: str = ..., ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectTaggingOutputOutputTypeDef:
+    ) -> DeleteObjectTaggingOutputTypeDef:
         """
         Removes the entire tag set from the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object_tagging)
         """
 
@@ -547,15 +547,15 @@
         Bucket: str,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputOutputTypeDef:
+    ) -> DeleteObjectsOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_objects)
         """
@@ -633,235 +633,235 @@
 
     def get_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetBucketAccelerateConfigurationOutputOutputTypeDef:
+    ) -> GetBucketAccelerateConfigurationOutputTypeDef:
         """
         This implementation of the GET action uses the `accelerate` subresource to
         return the Transfer Acceleration state of a bucket, which is either `Enabled` or
         `Suspended`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_accelerate_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_accelerate_configuration)
         """
 
     def get_bucket_acl(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAclOutputOutputTypeDef:
+    ) -> GetBucketAclOutputTypeDef:
         """
         This implementation of the `GET` action uses the `acl` subresource to return the
         access control list (ACL) of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_acl)
         """
 
     def get_bucket_analytics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAnalyticsConfigurationOutputOutputTypeDef:
+    ) -> GetBucketAnalyticsConfigurationOutputTypeDef:
         """
         This implementation of the GET action returns an analytics configuration
         (identified by the analytics configuration ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_analytics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_analytics_configuration)
         """
 
     def get_bucket_cors(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketCorsOutputOutputTypeDef:
+    ) -> GetBucketCorsOutputTypeDef:
         """
         Returns the Cross-Origin Resource Sharing (CORS) configuration information set
         for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_cors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_cors)
         """
 
     def get_bucket_encryption(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketEncryptionOutputOutputTypeDef:
+    ) -> GetBucketEncryptionOutputTypeDef:
         """
         Returns the default encryption configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_encryption)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_encryption)
         """
 
     def get_bucket_intelligent_tiering_configuration(
         self, *, Bucket: str, Id: str
-    ) -> GetBucketIntelligentTieringConfigurationOutputOutputTypeDef:
+    ) -> GetBucketIntelligentTieringConfigurationOutputTypeDef:
         """
         Gets the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_intelligent_tiering_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_intelligent_tiering_configuration)
         """
 
     def get_bucket_inventory_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketInventoryConfigurationOutputOutputTypeDef:
+    ) -> GetBucketInventoryConfigurationOutputTypeDef:
         """
         Returns an inventory configuration (identified by the inventory configuration
         ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_inventory_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_inventory_configuration)
         """
 
     def get_bucket_lifecycle(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleOutputOutputTypeDef:
+    ) -> GetBucketLifecycleOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle)
         """
 
     def get_bucket_lifecycle_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleConfigurationOutputOutputTypeDef:
+    ) -> GetBucketLifecycleConfigurationOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle_configuration)
         """
 
     def get_bucket_location(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLocationOutputOutputTypeDef:
+    ) -> GetBucketLocationOutputTypeDef:
         """
         Returns the Region the bucket resides in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_location)
         """
 
     def get_bucket_logging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLoggingOutputOutputTypeDef:
+    ) -> GetBucketLoggingOutputTypeDef:
         """
         Returns the logging status of a bucket and the permissions users have to view
         and modify that status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_logging)
         """
 
     def get_bucket_metrics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketMetricsConfigurationOutputOutputTypeDef:
+    ) -> GetBucketMetricsConfigurationOutputTypeDef:
         """
         Gets a metrics configuration (specified by the metrics configuration ID) from
         the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_metrics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_metrics_configuration)
         """
 
     def get_bucket_notification(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationDeprecatedOutputTypeDef:
+    ) -> NotificationConfigurationDeprecatedResponseMetadataTypeDef:
         """
         No longer used, see
         [GetBucketNotificationConfiguration](https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetBucketNotificationConfiguration.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification)
         """
 
     def get_bucket_notification_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationOutputTypeDef:
+    ) -> NotificationConfigurationResponseMetadataTypeDef:
         """
         Returns the notification configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification_configuration)
         """
 
     def get_bucket_ownership_controls(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketOwnershipControlsOutputOutputTypeDef:
+    ) -> GetBucketOwnershipControlsOutputTypeDef:
         """
         Retrieves `OwnershipControls` for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_ownership_controls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_ownership_controls)
         """
 
     def get_bucket_policy(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyOutputOutputTypeDef:
+    ) -> GetBucketPolicyOutputTypeDef:
         """
         Returns the policy of a specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy)
         """
 
     def get_bucket_policy_status(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyStatusOutputOutputTypeDef:
+    ) -> GetBucketPolicyStatusOutputTypeDef:
         """
         Retrieves the policy status for an Amazon S3 bucket, indicating whether the
         bucket is public.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy_status)
         """
 
     def get_bucket_replication(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketReplicationOutputOutputTypeDef:
+    ) -> GetBucketReplicationOutputTypeDef:
         """
         Returns the replication configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_replication)
         """
 
     def get_bucket_request_payment(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketRequestPaymentOutputOutputTypeDef:
+    ) -> GetBucketRequestPaymentOutputTypeDef:
         """
         Returns the request payment configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_request_payment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_request_payment)
         """
 
     def get_bucket_tagging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketTaggingOutputOutputTypeDef:
+    ) -> GetBucketTaggingOutputTypeDef:
         """
         Returns the tag set associated with the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_tagging)
         """
 
     def get_bucket_versioning(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketVersioningOutputOutputTypeDef:
+    ) -> GetBucketVersioningOutputTypeDef:
         """
         Returns the versioning state of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_versioning)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_versioning)
         """
 
     def get_bucket_website(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketWebsiteOutputOutputTypeDef:
+    ) -> GetBucketWebsiteOutputTypeDef:
         """
         Returns the website configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_website)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_website)
         """
 
@@ -885,15 +885,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object)
         """
 
@@ -901,15 +901,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAclOutputOutputTypeDef:
+    ) -> GetObjectAclOutputTypeDef:
         """
         Returns the access control list (ACL) of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_acl)
         """
 
@@ -923,15 +923,15 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAttributesOutputOutputTypeDef:
+    ) -> GetObjectAttributesOutputTypeDef:
         """
         Retrieves all the metadata from an object without returning the object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_attributes)
         """
 
@@ -939,25 +939,25 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectLegalHoldOutputOutputTypeDef:
+    ) -> GetObjectLegalHoldOutputTypeDef:
         """
         Gets an object's current legal hold status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_legal_hold)
         """
 
     def get_object_lock_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetObjectLockConfigurationOutputOutputTypeDef:
+    ) -> GetObjectLockConfigurationOutputTypeDef:
         """
         Gets the Object Lock configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_lock_configuration)
         """
 
@@ -965,15 +965,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectRetentionOutputOutputTypeDef:
+    ) -> GetObjectRetentionOutputTypeDef:
         """
         Retrieves an object's retention settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_retention)
         """
 
@@ -981,40 +981,40 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetObjectTaggingOutputOutputTypeDef:
+    ) -> GetObjectTaggingOutputTypeDef:
         """
         Returns the tag-set of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_tagging)
         """
 
     def get_object_torrent(
         self,
         *,
         Bucket: str,
         Key: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectTorrentOutputOutputTypeDef:
+    ) -> GetObjectTorrentOutputTypeDef:
         """
         Returns torrent files from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_torrent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_torrent)
         """
 
     def get_public_access_block(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetPublicAccessBlockOutputOutputTypeDef:
+    ) -> GetPublicAccessBlockOutputTypeDef:
         """
         Retrieves the `PublicAccessBlock` configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_public_access_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_public_access_block)
         """
 
@@ -1043,64 +1043,64 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputOutputTypeDef:
+    ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.head_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#head_object)
         """
 
     def list_bucket_analytics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketAnalyticsConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketAnalyticsConfigurationsOutputTypeDef:
         """
         Lists the analytics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_analytics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_analytics_configurations)
         """
 
     def list_bucket_intelligent_tiering_configurations(
         self, *, Bucket: str, ContinuationToken: str = ...
-    ) -> ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketIntelligentTieringConfigurationsOutputTypeDef:
         """
         Lists the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_intelligent_tiering_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_intelligent_tiering_configurations)
         """
 
     def list_bucket_inventory_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketInventoryConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketInventoryConfigurationsOutputTypeDef:
         """
         Returns a list of inventory configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_inventory_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_inventory_configurations)
         """
 
     def list_bucket_metrics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketMetricsConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketMetricsConfigurationsOutputTypeDef:
         """
         Lists the metrics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_metrics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_metrics_configurations)
         """
 
-    def list_buckets(self) -> ListBucketsOutputOutputTypeDef:
+    def list_buckets(self) -> ListBucketsOutputTypeDef:
         """
         Returns a list of all buckets owned by the authenticated sender of the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_buckets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_buckets)
         """
 
@@ -1112,15 +1112,15 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> ListMultipartUploadsOutputOutputTypeDef:
+    ) -> ListMultipartUploadsOutputTypeDef:
         """
         This action lists in-progress multipart uploads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_multipart_uploads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_multipart_uploads)
         """
 
@@ -1133,15 +1133,15 @@
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectVersionsOutputOutputTypeDef:
+    ) -> ListObjectVersionsOutputTypeDef:
         """
         Returns metadata about all versions of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_object_versions)
         """
 
@@ -1153,15 +1153,15 @@
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsOutputOutputTypeDef:
+    ) -> ListObjectsOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects)
         """
 
@@ -1175,15 +1175,15 @@
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsV2OutputOutputTypeDef:
+    ) -> ListObjectsV2OutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects_v2)
         """
 
@@ -1196,15 +1196,15 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> ListPartsOutputOutputTypeDef:
+    ) -> ListPartsOutputTypeDef:
         """
         Lists the parts that have been uploaded for a specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_parts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_parts)
         """
 
@@ -1562,15 +1562,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputOutputTypeDef:
+    ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object)
         """
 
@@ -1586,15 +1586,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputOutputTypeDef:
+    ) -> PutObjectAclOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_acl)
         """
@@ -1606,15 +1606,15 @@
         Key: str,
         LegalHold: ObjectLockLegalHoldTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLegalHoldOutputOutputTypeDef:
+    ) -> PutObjectLegalHoldOutputTypeDef:
         """
         Applies a legal hold configuration to the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_legal_hold)
         """
 
@@ -1624,15 +1624,15 @@
         Bucket: str,
         ObjectLockConfiguration: ObjectLockConfigurationTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         Token: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLockConfigurationOutputOutputTypeDef:
+    ) -> PutObjectLockConfigurationOutputTypeDef:
         """
         Places an Object Lock configuration on the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_lock_configuration)
         """
 
@@ -1644,15 +1644,15 @@
         Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectRetentionOutputOutputTypeDef:
+    ) -> PutObjectRetentionOutputTypeDef:
         """
         Places an Object Retention configuration on an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_retention)
         """
 
@@ -1663,15 +1663,15 @@
         Key: str,
         Tagging: TaggingTypeDef,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> PutObjectTaggingOutputOutputTypeDef:
+    ) -> PutObjectTaggingOutputTypeDef:
         """
         Sets the supplied tag-set to an object that already exists in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_tagging)
         """
 
@@ -1698,15 +1698,15 @@
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputOutputTypeDef:
+    ) -> RestoreObjectOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#restore_object)
         """
@@ -1722,15 +1722,15 @@
         OutputSerialization: OutputSerializationTypeDef,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestProgress: RequestProgressTypeDef = ...,
         ScanRange: ScanRangeTypeDef = ...,
         ExpectedBucketOwner: str = ...
-    ) -> SelectObjectContentOutputOutputTypeDef:
+    ) -> SelectObjectContentOutputTypeDef:
         """
         This action filters the contents of an Amazon S3 object based on a simple
         structured query language (SQL) statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.select_object_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#select_object_content)
         """
@@ -1783,15 +1783,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputOutputTypeDef:
+    ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part)
         """
 
@@ -1813,15 +1813,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputOutputTypeDef:
+    ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part_copy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part_copy)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -39,105 +39,105 @@
     ListMultipartUploadsPaginator,
     ListObjectsPaginator,
     ListObjectsV2Paginator,
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
     AnalyticsConfigurationTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CompleteMultipartUploadOutputOutputTypeDef,
-    CopyObjectOutputOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CopyObjectOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    CreateMultipartUploadOutputOutputTypeDef,
-    DeleteObjectOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
-    DeleteObjectTaggingOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
     DeleteTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetBucketAccelerateConfigurationOutputOutputTypeDef,
-    GetBucketAclOutputOutputTypeDef,
-    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
-    GetBucketCorsOutputOutputTypeDef,
-    GetBucketEncryptionOutputOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
-    GetBucketInventoryConfigurationOutputOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputOutputTypeDef,
-    GetBucketLifecycleOutputOutputTypeDef,
-    GetBucketLocationOutputOutputTypeDef,
-    GetBucketLoggingOutputOutputTypeDef,
-    GetBucketMetricsConfigurationOutputOutputTypeDef,
-    GetBucketOwnershipControlsOutputOutputTypeDef,
-    GetBucketPolicyOutputOutputTypeDef,
-    GetBucketPolicyStatusOutputOutputTypeDef,
-    GetBucketReplicationOutputOutputTypeDef,
-    GetBucketRequestPaymentOutputOutputTypeDef,
-    GetBucketTaggingOutputOutputTypeDef,
-    GetBucketVersioningOutputOutputTypeDef,
-    GetBucketWebsiteOutputOutputTypeDef,
-    GetObjectAclOutputOutputTypeDef,
-    GetObjectAttributesOutputOutputTypeDef,
-    GetObjectLegalHoldOutputOutputTypeDef,
-    GetObjectLockConfigurationOutputOutputTypeDef,
-    GetObjectOutputOutputTypeDef,
-    GetObjectRetentionOutputOutputTypeDef,
-    GetObjectTaggingOutputOutputTypeDef,
-    GetObjectTorrentOutputOutputTypeDef,
-    GetPublicAccessBlockOutputOutputTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketAclOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputTypeDef,
+    GetBucketCorsOutputTypeDef,
+    GetBucketEncryptionOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputTypeDef,
+    GetBucketInventoryConfigurationOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputTypeDef,
+    GetBucketLifecycleOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketLoggingOutputTypeDef,
+    GetBucketMetricsConfigurationOutputTypeDef,
+    GetBucketOwnershipControlsOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketPolicyStatusOutputTypeDef,
+    GetBucketReplicationOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketTaggingOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetBucketWebsiteOutputTypeDef,
+    GetObjectAclOutputTypeDef,
+    GetObjectAttributesOutputTypeDef,
+    GetObjectLegalHoldOutputTypeDef,
+    GetObjectLockConfigurationOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectRetentionOutputTypeDef,
+    GetObjectTaggingOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    HeadObjectOutputTypeDef,
     InputSerializationTypeDef,
     IntelligentTieringConfigurationTypeDef,
     InventoryConfigurationTypeDef,
     LifecycleConfigurationTypeDef,
-    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputOutputTypeDef,
-    ListBucketsOutputOutputTypeDef,
-    ListMultipartUploadsOutputOutputTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputTypeDef,
+    ListBucketsOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    ListPartsOutputTypeDef,
     MetricsConfigurationTypeDef,
-    NotificationConfigurationDeprecatedOutputTypeDef,
+    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    NotificationConfigurationOutputTypeDef,
+    NotificationConfigurationResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     OutputSerializationTypeDef,
     OwnershipControlsTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectLegalHoldOutputOutputTypeDef,
-    PutObjectLockConfigurationOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
-    PutObjectRetentionOutputOutputTypeDef,
-    PutObjectTaggingOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
     ReplicationConfigurationTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
-    SelectObjectContentOutputOutputTypeDef,
+    SelectObjectContentOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TaggingTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
+    UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 from .waiter import (
     BucketExistsWaiter,
     BucketNotExistsWaiter,
     ObjectExistsWaiter,
@@ -189,15 +189,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputOutputTypeDef:
+    ) -> AbortMultipartUploadOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.abort_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#abort_multipart_upload)
         """
     def can_paginate(self, operation_name: str) -> bool:
@@ -226,15 +226,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> CompleteMultipartUploadOutputOutputTypeDef:
+    ) -> CompleteMultipartUploadOutputTypeDef:
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.complete_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#complete_multipart_upload)
         """
     def copy(
@@ -293,15 +293,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputOutputTypeDef:
+    ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#copy_object)
         """
     def create_bucket(
@@ -313,15 +313,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputOutputTypeDef:
+    ) -> CreateBucketOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_bucket)
         """
     def create_multipart_upload(
@@ -353,15 +353,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> CreateMultipartUploadOutputOutputTypeDef:
+    ) -> CreateMultipartUploadOutputTypeDef:
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_multipart_upload)
         """
     def delete_bucket(
@@ -492,25 +492,25 @@
         Bucket: str,
         Key: str,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object)
         """
     def delete_object_tagging(
         self, *, Bucket: str, Key: str, VersionId: str = ..., ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectTaggingOutputOutputTypeDef:
+    ) -> DeleteObjectTaggingOutputTypeDef:
         """
         Removes the entire tag set from the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object_tagging)
         """
     def delete_objects(
@@ -519,15 +519,15 @@
         Bucket: str,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputOutputTypeDef:
+    ) -> DeleteObjectsOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_objects)
         """
@@ -599,214 +599,214 @@
         """
     def get_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetBucketAccelerateConfigurationOutputOutputTypeDef:
+    ) -> GetBucketAccelerateConfigurationOutputTypeDef:
         """
         This implementation of the GET action uses the `accelerate` subresource to
         return the Transfer Acceleration state of a bucket, which is either `Enabled` or
         `Suspended`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_accelerate_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_accelerate_configuration)
         """
     def get_bucket_acl(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAclOutputOutputTypeDef:
+    ) -> GetBucketAclOutputTypeDef:
         """
         This implementation of the `GET` action uses the `acl` subresource to return the
         access control list (ACL) of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_acl)
         """
     def get_bucket_analytics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAnalyticsConfigurationOutputOutputTypeDef:
+    ) -> GetBucketAnalyticsConfigurationOutputTypeDef:
         """
         This implementation of the GET action returns an analytics configuration
         (identified by the analytics configuration ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_analytics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_analytics_configuration)
         """
     def get_bucket_cors(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketCorsOutputOutputTypeDef:
+    ) -> GetBucketCorsOutputTypeDef:
         """
         Returns the Cross-Origin Resource Sharing (CORS) configuration information set
         for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_cors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_cors)
         """
     def get_bucket_encryption(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketEncryptionOutputOutputTypeDef:
+    ) -> GetBucketEncryptionOutputTypeDef:
         """
         Returns the default encryption configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_encryption)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_encryption)
         """
     def get_bucket_intelligent_tiering_configuration(
         self, *, Bucket: str, Id: str
-    ) -> GetBucketIntelligentTieringConfigurationOutputOutputTypeDef:
+    ) -> GetBucketIntelligentTieringConfigurationOutputTypeDef:
         """
         Gets the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_intelligent_tiering_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_intelligent_tiering_configuration)
         """
     def get_bucket_inventory_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketInventoryConfigurationOutputOutputTypeDef:
+    ) -> GetBucketInventoryConfigurationOutputTypeDef:
         """
         Returns an inventory configuration (identified by the inventory configuration
         ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_inventory_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_inventory_configuration)
         """
     def get_bucket_lifecycle(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleOutputOutputTypeDef:
+    ) -> GetBucketLifecycleOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle)
         """
     def get_bucket_lifecycle_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleConfigurationOutputOutputTypeDef:
+    ) -> GetBucketLifecycleConfigurationOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle_configuration)
         """
     def get_bucket_location(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLocationOutputOutputTypeDef:
+    ) -> GetBucketLocationOutputTypeDef:
         """
         Returns the Region the bucket resides in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_location)
         """
     def get_bucket_logging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLoggingOutputOutputTypeDef:
+    ) -> GetBucketLoggingOutputTypeDef:
         """
         Returns the logging status of a bucket and the permissions users have to view
         and modify that status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_logging)
         """
     def get_bucket_metrics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketMetricsConfigurationOutputOutputTypeDef:
+    ) -> GetBucketMetricsConfigurationOutputTypeDef:
         """
         Gets a metrics configuration (specified by the metrics configuration ID) from
         the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_metrics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_metrics_configuration)
         """
     def get_bucket_notification(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationDeprecatedOutputTypeDef:
+    ) -> NotificationConfigurationDeprecatedResponseMetadataTypeDef:
         """
         No longer used, see
         [GetBucketNotificationConfiguration](https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetBucketNotificationConfiguration.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification)
         """
     def get_bucket_notification_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationOutputTypeDef:
+    ) -> NotificationConfigurationResponseMetadataTypeDef:
         """
         Returns the notification configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification_configuration)
         """
     def get_bucket_ownership_controls(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketOwnershipControlsOutputOutputTypeDef:
+    ) -> GetBucketOwnershipControlsOutputTypeDef:
         """
         Retrieves `OwnershipControls` for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_ownership_controls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_ownership_controls)
         """
     def get_bucket_policy(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyOutputOutputTypeDef:
+    ) -> GetBucketPolicyOutputTypeDef:
         """
         Returns the policy of a specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy)
         """
     def get_bucket_policy_status(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyStatusOutputOutputTypeDef:
+    ) -> GetBucketPolicyStatusOutputTypeDef:
         """
         Retrieves the policy status for an Amazon S3 bucket, indicating whether the
         bucket is public.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy_status)
         """
     def get_bucket_replication(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketReplicationOutputOutputTypeDef:
+    ) -> GetBucketReplicationOutputTypeDef:
         """
         Returns the replication configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_replication)
         """
     def get_bucket_request_payment(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketRequestPaymentOutputOutputTypeDef:
+    ) -> GetBucketRequestPaymentOutputTypeDef:
         """
         Returns the request payment configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_request_payment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_request_payment)
         """
     def get_bucket_tagging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketTaggingOutputOutputTypeDef:
+    ) -> GetBucketTaggingOutputTypeDef:
         """
         Returns the tag set associated with the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_tagging)
         """
     def get_bucket_versioning(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketVersioningOutputOutputTypeDef:
+    ) -> GetBucketVersioningOutputTypeDef:
         """
         Returns the versioning state of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_versioning)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_versioning)
         """
     def get_bucket_website(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketWebsiteOutputOutputTypeDef:
+    ) -> GetBucketWebsiteOutputTypeDef:
         """
         Returns the website configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_website)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_website)
         """
     def get_object(
@@ -829,30 +829,30 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object)
         """
     def get_object_acl(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAclOutputOutputTypeDef:
+    ) -> GetObjectAclOutputTypeDef:
         """
         Returns the access control list (ACL) of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_acl)
         """
     def get_object_attributes(
@@ -865,92 +865,92 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAttributesOutputOutputTypeDef:
+    ) -> GetObjectAttributesOutputTypeDef:
         """
         Retrieves all the metadata from an object without returning the object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_attributes)
         """
     def get_object_legal_hold(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectLegalHoldOutputOutputTypeDef:
+    ) -> GetObjectLegalHoldOutputTypeDef:
         """
         Gets an object's current legal hold status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_legal_hold)
         """
     def get_object_lock_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetObjectLockConfigurationOutputOutputTypeDef:
+    ) -> GetObjectLockConfigurationOutputTypeDef:
         """
         Gets the Object Lock configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_lock_configuration)
         """
     def get_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectRetentionOutputOutputTypeDef:
+    ) -> GetObjectRetentionOutputTypeDef:
         """
         Retrieves an object's retention settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_retention)
         """
     def get_object_tagging(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetObjectTaggingOutputOutputTypeDef:
+    ) -> GetObjectTaggingOutputTypeDef:
         """
         Returns the tag-set of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_tagging)
         """
     def get_object_torrent(
         self,
         *,
         Bucket: str,
         Key: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectTorrentOutputOutputTypeDef:
+    ) -> GetObjectTorrentOutputTypeDef:
         """
         Returns torrent files from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_torrent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_torrent)
         """
     def get_public_access_block(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetPublicAccessBlockOutputOutputTypeDef:
+    ) -> GetPublicAccessBlockOutputTypeDef:
         """
         Retrieves the `PublicAccessBlock` configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_public_access_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_public_access_block)
         """
     def head_bucket(
@@ -977,59 +977,59 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputOutputTypeDef:
+    ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.head_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#head_object)
         """
     def list_bucket_analytics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketAnalyticsConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketAnalyticsConfigurationsOutputTypeDef:
         """
         Lists the analytics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_analytics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_analytics_configurations)
         """
     def list_bucket_intelligent_tiering_configurations(
         self, *, Bucket: str, ContinuationToken: str = ...
-    ) -> ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketIntelligentTieringConfigurationsOutputTypeDef:
         """
         Lists the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_intelligent_tiering_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_intelligent_tiering_configurations)
         """
     def list_bucket_inventory_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketInventoryConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketInventoryConfigurationsOutputTypeDef:
         """
         Returns a list of inventory configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_inventory_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_inventory_configurations)
         """
     def list_bucket_metrics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketMetricsConfigurationsOutputOutputTypeDef:
+    ) -> ListBucketMetricsConfigurationsOutputTypeDef:
         """
         Lists the metrics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_metrics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_metrics_configurations)
         """
-    def list_buckets(self) -> ListBucketsOutputOutputTypeDef:
+    def list_buckets(self) -> ListBucketsOutputTypeDef:
         """
         Returns a list of all buckets owned by the authenticated sender of the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_buckets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_buckets)
         """
     def list_multipart_uploads(
@@ -1040,15 +1040,15 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> ListMultipartUploadsOutputOutputTypeDef:
+    ) -> ListMultipartUploadsOutputTypeDef:
         """
         This action lists in-progress multipart uploads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_multipart_uploads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_multipart_uploads)
         """
     def list_object_versions(
@@ -1060,15 +1060,15 @@
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectVersionsOutputOutputTypeDef:
+    ) -> ListObjectVersionsOutputTypeDef:
         """
         Returns metadata about all versions of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_object_versions)
         """
     def list_objects(
@@ -1079,15 +1079,15 @@
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsOutputOutputTypeDef:
+    ) -> ListObjectsOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects)
         """
     def list_objects_v2(
@@ -1100,15 +1100,15 @@
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsV2OutputOutputTypeDef:
+    ) -> ListObjectsV2OutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects_v2)
         """
     def list_parts(
@@ -1120,15 +1120,15 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> ListPartsOutputOutputTypeDef:
+    ) -> ListPartsOutputTypeDef:
         """
         Lists the parts that have been uploaded for a specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_parts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_parts)
         """
     def put_bucket_accelerate_configuration(
@@ -1465,15 +1465,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputOutputTypeDef:
+    ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object)
         """
     def put_object_acl(
@@ -1488,15 +1488,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputOutputTypeDef:
+    ) -> PutObjectAclOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_acl)
         """
@@ -1507,15 +1507,15 @@
         Key: str,
         LegalHold: ObjectLockLegalHoldTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLegalHoldOutputOutputTypeDef:
+    ) -> PutObjectLegalHoldOutputTypeDef:
         """
         Applies a legal hold configuration to the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_legal_hold)
         """
     def put_object_lock_configuration(
@@ -1524,15 +1524,15 @@
         Bucket: str,
         ObjectLockConfiguration: ObjectLockConfigurationTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         Token: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLockConfigurationOutputOutputTypeDef:
+    ) -> PutObjectLockConfigurationOutputTypeDef:
         """
         Places an Object Lock configuration on the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_lock_configuration)
         """
     def put_object_retention(
@@ -1543,15 +1543,15 @@
         Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectRetentionOutputOutputTypeDef:
+    ) -> PutObjectRetentionOutputTypeDef:
         """
         Places an Object Retention configuration on an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_retention)
         """
     def put_object_tagging(
@@ -1561,15 +1561,15 @@
         Key: str,
         Tagging: TaggingTypeDef,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> PutObjectTaggingOutputOutputTypeDef:
+    ) -> PutObjectTaggingOutputTypeDef:
         """
         Sets the supplied tag-set to an object that already exists in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_tagging)
         """
     def put_public_access_block(
@@ -1594,15 +1594,15 @@
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputOutputTypeDef:
+    ) -> RestoreObjectOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#restore_object)
         """
@@ -1617,15 +1617,15 @@
         OutputSerialization: OutputSerializationTypeDef,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestProgress: RequestProgressTypeDef = ...,
         ScanRange: ScanRangeTypeDef = ...,
         ExpectedBucketOwner: str = ...
-    ) -> SelectObjectContentOutputOutputTypeDef:
+    ) -> SelectObjectContentOutputTypeDef:
         """
         This action filters the contents of an Amazon S3 object based on a simple
         structured query language (SQL) statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.select_object_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#select_object_content)
         """
@@ -1675,15 +1675,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputOutputTypeDef:
+    ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part)
         """
     def upload_part_copy(
@@ -1704,15 +1704,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputOutputTypeDef:
+    ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part_copy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part_copy)
         """
     def write_get_object_response(
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 """
 import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListMultipartUploadsOutputOutputTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    ListPartsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -78,15 +78,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMultipartUploadsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 
 class ListObjectVersionsPaginator(Paginator):
@@ -102,15 +102,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectVersionsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 
 class ListObjectsPaginator(Paginator):
@@ -126,15 +126,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 
 class ListObjectsV2Paginator(Paginator):
@@ -152,15 +152,15 @@
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsV2OutputOutputTypeDef]:
+    ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 
 class ListPartsPaginator(Paginator):
@@ -177,12 +177,12 @@
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPartsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 """
 import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListMultipartUploadsOutputOutputTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    ListPartsOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -74,15 +74,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMultipartUploadsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 class ListObjectVersionsPaginator(Paginator):
     """
@@ -97,15 +97,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectVersionsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 class ListObjectsPaginator(Paginator):
     """
@@ -120,15 +120,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 class ListObjectsV2Paginator(Paginator):
     """
@@ -145,15 +145,15 @@
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsV2OutputOutputTypeDef]:
+    ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 class ListPartsPaginator(Paginator):
     """
@@ -169,12 +169,12 @@
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPartsOutputOutputTypeDef]:
+    ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,55 +60,55 @@
     PayerType,
     ReplicationStatusType,
     ServerSideEncryptionType,
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AccessControlPolicyTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputOutputTypeDef,
+    CopyObjectOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
     CORSRuleOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    DeleteObjectOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
-    GetObjectOutputOutputTypeDef,
+    GetObjectOutputTypeDef,
     GrantOutputTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    HeadObjectOutputTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     InitiatorResponseMetadataTypeDef,
     LambdaFunctionConfigurationOutputTypeDef,
     LifecycleConfigurationTypeDef,
     LifecycleRuleOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     OwnerResponseMetadataTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectOutputTypeDef,
     QueueConfigurationOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RequestPaymentConfigurationTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     RoutingRuleOutputTypeDef,
     RuleOutputTypeDef,
     TaggingTypeDef,
     TagOutputTypeDef,
     TopicConfigurationOutputTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
+    UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -268,15 +268,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectVersionsCollection":
         """
         Return at most this many ObjectVersions.
@@ -324,15 +324,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectsCollection":
         """
         Return at most this many ObjectSummarys.
@@ -1203,15 +1203,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputOutputTypeDef:
+    ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartcopy_from-method)
         """
 
@@ -1235,15 +1235,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputOutputTypeDef:
+    ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartupload-method)
         """
 
@@ -1298,15 +1298,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputOutputTypeDef:
+    ) -> PutObjectAclOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectaclput-method)
         """
@@ -1355,15 +1355,15 @@
     def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversiondelete-method)
         """
@@ -1385,15 +1385,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionget-method)
         """
 
@@ -1416,15 +1416,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputOutputTypeDef:
+    ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.head)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionhead-method)
         """
@@ -1465,15 +1465,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpart-method)
         """
 
     def abort(
         self, *, RequestPayer: Literal["requester"] = ..., ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputOutputTypeDef:
+    ) -> AbortMultipartUploadOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.abort)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadabort-method)
         """
 
@@ -1638,15 +1638,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputOutputTypeDef:
+    ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectcopy_from-method)
         """
 
@@ -1654,15 +1654,15 @@
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectdelete-method)
         """
@@ -1713,15 +1713,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectget-method)
         """
 
@@ -1815,15 +1815,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputOutputTypeDef:
+    ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectput-method)
         """
 
@@ -1840,15 +1840,15 @@
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputOutputTypeDef:
+    ) -> RestoreObjectOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectrestore_object-method)
         """
@@ -1995,15 +1995,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputOutputTypeDef:
+    ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarycopy_from-method)
         """
 
@@ -2011,15 +2011,15 @@
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarydelete-method)
         """
@@ -2042,15 +2042,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryget-method)
         """
 
@@ -2144,15 +2144,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputOutputTypeDef:
+    ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryput-method)
         """
 
@@ -2160,15 +2160,15 @@
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputOutputTypeDef:
+    ) -> RestoreObjectOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryrestore_object-method)
         """
@@ -2325,15 +2325,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputOutputTypeDef:
+    ) -> CreateBucketOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.create)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcreate-method)
         """
 
@@ -2350,15 +2350,15 @@
         *,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputOutputTypeDef:
+    ) -> DeleteObjectsOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketdelete_objects-method)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,55 +60,55 @@
     PayerType,
     ReplicationStatusType,
     ServerSideEncryptionType,
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AccessControlPolicyTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputOutputTypeDef,
+    CopyObjectOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
     CORSRuleOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    DeleteObjectOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
-    GetObjectOutputOutputTypeDef,
+    GetObjectOutputTypeDef,
     GrantOutputTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    HeadObjectOutputTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     InitiatorResponseMetadataTypeDef,
     LambdaFunctionConfigurationOutputTypeDef,
     LifecycleConfigurationTypeDef,
     LifecycleRuleOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     OwnerResponseMetadataTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectOutputTypeDef,
     QueueConfigurationOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RequestPaymentConfigurationTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     RoutingRuleOutputTypeDef,
     RuleOutputTypeDef,
     TaggingTypeDef,
     TagOutputTypeDef,
     TopicConfigurationOutputTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
+    UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -252,15 +252,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
     def limit(self, count: int) -> "BucketObjectVersionsCollection":
         """
         Return at most this many ObjectVersions.
         """
@@ -301,15 +301,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
     def limit(self, count: int) -> "BucketObjectsCollection":
         """
         Return at most this many ObjectSummarys.
         """
@@ -1094,15 +1094,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputOutputTypeDef:
+    ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartcopy_from-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1124,15 +1124,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputOutputTypeDef:
+    ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartupload-method)
         """
 
@@ -1182,15 +1182,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputOutputTypeDef:
+    ) -> PutObjectAclOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectaclput-method)
         """
@@ -1235,15 +1235,15 @@
     def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversiondelete-method)
         """
@@ -1264,15 +1264,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionget-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1293,15 +1293,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputOutputTypeDef:
+    ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.head)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionhead-method)
         """
@@ -1338,15 +1338,15 @@
         Creates a MultipartUploadPart resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpart-method)
         """
     def abort(
         self, *, RequestPayer: Literal["requester"] = ..., ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputOutputTypeDef:
+    ) -> AbortMultipartUploadOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.abort)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadabort-method)
         """
     def complete(
@@ -1502,30 +1502,30 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputOutputTypeDef:
+    ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectcopy_from-method)
         """
     def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectdelete-method)
         """
@@ -1573,15 +1573,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectget-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1671,15 +1671,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputOutputTypeDef:
+    ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectput-method)
         """
     def reload(self) -> None:
@@ -1694,15 +1694,15 @@
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputOutputTypeDef:
+    ) -> RestoreObjectOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectrestore_object-method)
         """
@@ -1838,30 +1838,30 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputOutputTypeDef:
+    ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarycopy_from-method)
         """
     def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputOutputTypeDef:
+    ) -> DeleteObjectOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarydelete-method)
         """
@@ -1883,15 +1883,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputOutputTypeDef:
+    ) -> GetObjectOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryget-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1981,30 +1981,30 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputOutputTypeDef:
+    ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryput-method)
         """
     def restore_object(
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputOutputTypeDef:
+    ) -> RestoreObjectOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryrestore_object-method)
         """
@@ -2144,15 +2144,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputOutputTypeDef:
+    ) -> CreateBucketOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.create)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcreate-method)
         """
     def delete(self, *, ExpectedBucketOwner: str = ...) -> None:
@@ -2167,15 +2167,15 @@
         *,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputOutputTypeDef:
+    ) -> DeleteObjectsOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketdelete_objects-method)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,55 +79,55 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputOutputTypeDef",
+    "AbortMultipartUploadOutputTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
     "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
     "TagOutputTypeDef",
     "TagTypeDef",
     "AnalyticsS3BucketDestinationOutputTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "BucketDownloadFileobjRequestTypeDef",
-    "BucketOutputTypeDef",
+    "BucketTypeDef",
     "BucketUploadFileRequestTypeDef",
     "BucketUploadFileobjRequestTypeDef",
     "CORSRuleTypeDef",
     "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
-    "ChecksumOutputTypeDef",
+    "ChecksumTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
-    "CommonPrefixOutputTypeDef",
-    "CompleteMultipartUploadOutputOutputTypeDef",
+    "CommonPrefixTypeDef",
+    "CompleteMultipartUploadOutputTypeDef",
     "CompletedPartTypeDef",
     "ConditionOutputTypeDef",
     "ConditionTypeDef",
-    "CopyObjectResultOutputTypeDef",
+    "CopyObjectResultTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
-    "CopyPartResultOutputTypeDef",
+    "CopyPartResultTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputOutputTypeDef",
-    "CreateMultipartUploadOutputOutputTypeDef",
+    "CreateBucketOutputTypeDef",
+    "CreateMultipartUploadOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
     "DefaultRetentionOutputTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
@@ -148,95 +148,95 @@
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
     "OwnerOutputTypeDef",
     "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputOutputTypeDef",
+    "DeleteObjectOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputOutputTypeDef",
+    "DeleteObjectTaggingOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
-    "DeletedObjectOutputTypeDef",
-    "ErrorOutputTypeDef",
+    "DeletedObjectTypeDef",
+    "ErrorTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
     "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
     "ErrorDocumentOutputTypeDef",
     "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
     "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
     "FilterRuleOutputTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
+    "GetBucketAccelerateConfigurationOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputOutputTypeDef",
+    "GetBucketLocationOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputOutputTypeDef",
+    "GetBucketPolicyOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
-    "PolicyStatusOutputTypeDef",
+    "PolicyStatusTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputOutputTypeDef",
+    "GetBucketRequestPaymentOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputOutputTypeDef",
+    "GetBucketVersioningOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "IndexDocumentOutputTypeDef",
     "RedirectAllRequestsToOutputTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
-    "ObjectPartOutputTypeDef",
+    "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldOutputTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputOutputTypeDef",
+    "GetObjectOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputOutputTypeDef",
+    "GetObjectTorrentOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputOutputTypeDef",
+    "HeadObjectOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
     "IndexDocumentResponseMetadataTypeDef",
     "IndexDocumentTypeDef",
-    "InitiatorOutputTypeDef",
     "InitiatorResponseMetadataTypeDef",
+    "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringOutputTypeDef",
     "TieringTypeDef",
     "InventoryFilterOutputTypeDef",
     "InventoryScheduleOutputTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
@@ -259,78 +259,78 @@
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
-    "PartOutputTypeDef",
+    "PartTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "QueueConfigurationDeprecatedOutputTypeDef",
     "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "ObjectLockRetentionTypeDef",
-    "RestoreStatusOutputTypeDef",
+    "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
     "OwnerResponseMetadataTypeDef",
     "OwnershipControlsRuleOutputTypeDef",
     "OwnershipControlsRuleTypeDef",
     "PaginatorConfigTypeDef",
-    "ProgressOutputTypeDef",
+    "ProgressTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputOutputTypeDef",
-    "PutObjectLegalHoldOutputOutputTypeDef",
-    "PutObjectLockConfigurationOutputOutputTypeDef",
-    "PutObjectOutputOutputTypeDef",
+    "PutObjectAclOutputTypeDef",
+    "PutObjectLegalHoldOutputTypeDef",
+    "PutObjectLockConfigurationOutputTypeDef",
+    "PutObjectOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputOutputTypeDef",
-    "PutObjectTaggingOutputOutputTypeDef",
-    "RecordsEventOutputTypeDef",
+    "PutObjectRetentionOutputTypeDef",
+    "PutObjectTaggingOutputTypeDef",
+    "RecordsEventTypeDef",
     "RedirectAllRequestsToResponseMetadataTypeDef",
     "RedirectAllRequestsToTypeDef",
     "RedirectOutputTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
     "ResponseMetadataTypeDef",
-    "RestoreObjectOutputOutputTypeDef",
+    "RestoreObjectOutputTypeDef",
     "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultOutputTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
-    "StatsOutputTypeDef",
-    "UploadPartOutputOutputTypeDef",
+    "StatsTypeDef",
+    "UploadPartOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "AnalyticsAndOperatorOutputTypeDef",
-    "GetBucketTaggingOutputOutputTypeDef",
-    "GetObjectTaggingOutputOutputTypeDef",
+    "GetBucketTaggingOutputTypeDef",
+    "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorOutputTypeDef",
     "MetricsAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
@@ -342,75 +342,75 @@
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "ObjectCopyRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
     "CORSConfigurationTypeDef",
-    "GetBucketCorsOutputOutputTypeDef",
+    "GetBucketCorsOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
-    "CopyObjectOutputOutputTypeDef",
-    "UploadPartCopyOutputOutputTypeDef",
+    "CopyObjectOutputTypeDef",
+    "UploadPartCopyOutputTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
     "ObjectLockRuleOutputTypeDef",
     "ObjectLockRuleTypeDef",
-    "DeleteMarkerEntryOutputTypeDef",
-    "ListBucketsOutputOutputTypeDef",
-    "DeleteObjectsOutputOutputTypeDef",
+    "DeleteMarkerEntryTypeDef",
+    "ListBucketsOutputTypeDef",
+    "DeleteObjectsOutputTypeDef",
     "DeleteTypeDef",
     "S3KeyFilterOutputTypeDef",
     "S3KeyFilterTypeDef",
-    "GetBucketPolicyStatusOutputOutputTypeDef",
-    "GetObjectAttributesPartsOutputTypeDef",
-    "GetObjectLegalHoldOutputOutputTypeDef",
-    "GetObjectRetentionOutputOutputTypeDef",
-    "GetPublicAccessBlockOutputOutputTypeDef",
+    "GetBucketPolicyStatusOutputTypeDef",
+    "GetObjectAttributesPartsTypeDef",
+    "GetObjectLegalHoldOutputTypeDef",
+    "GetObjectRetentionOutputTypeDef",
+    "GetPublicAccessBlockOutputTypeDef",
     "GrantOutputTypeDef",
     "TargetGrantOutputTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
-    "MultipartUploadOutputTypeDef",
+    "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
     "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
-    "ListPartsOutputOutputTypeDef",
+    "ListPartsOutputTypeDef",
     "MetricsOutputTypeDef",
     "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
-    "NotificationConfigurationDeprecatedOutputTypeDef",
+    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
     "PutObjectLegalHoldRequestRequestTypeDef",
     "PutObjectRetentionRequestRequestTypeDef",
-    "ObjectOutputTypeDef",
-    "ObjectVersionOutputTypeDef",
+    "ObjectTypeDef",
+    "ObjectVersionTypeDef",
     "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
-    "ProgressEventOutputTypeDef",
+    "ProgressEventTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "RoutingRuleOutputTypeDef",
     "RoutingRuleTypeDef",
     "ServerSideEncryptionRuleOutputTypeDef",
     "ServerSideEncryptionRuleTypeDef",
     "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
-    "StatsEventOutputTypeDef",
+    "StatsEventTypeDef",
     "AnalyticsFilterOutputTypeDef",
     "IntelligentTieringFilterOutputTypeDef",
     "LifecycleRuleFilterOutputTypeDef",
     "MetricsFilterOutputTypeDef",
     "ReplicationRuleFilterOutputTypeDef",
     "AnalyticsFilterTypeDef",
     "IntelligentTieringFilterTypeDef",
@@ -428,109 +428,109 @@
     "CompleteMultipartUploadRequestRequestTypeDef",
     "ObjectLockConfigurationOutputTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
     "NotificationConfigurationFilterOutputTypeDef",
     "NotificationConfigurationFilterTypeDef",
-    "GetObjectAttributesOutputOutputTypeDef",
-    "GetBucketAclOutputOutputTypeDef",
-    "GetObjectAclOutputOutputTypeDef",
+    "GetObjectAttributesOutputTypeDef",
+    "GetBucketAclOutputTypeDef",
+    "GetObjectAclOutputTypeDef",
     "LoggingEnabledOutputTypeDef",
     "LoggingEnabledResponseMetadataTypeDef",
     "AccessControlPolicyTypeDef",
     "S3LocationTypeDef",
     "LoggingEnabledTypeDef",
-    "ListMultipartUploadsOutputOutputTypeDef",
+    "ListMultipartUploadsOutputTypeDef",
     "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
-    "GetBucketLifecycleOutputOutputTypeDef",
+    "GetBucketLifecycleOutputTypeDef",
     "LifecycleConfigurationTypeDef",
     "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
-    "ListObjectsOutputOutputTypeDef",
-    "ListObjectsV2OutputOutputTypeDef",
-    "ListObjectVersionsOutputOutputTypeDef",
-    "GetBucketOwnershipControlsOutputOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "ListObjectsV2OutputTypeDef",
+    "ListObjectVersionsOutputTypeDef",
+    "GetBucketOwnershipControlsOutputTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketWebsiteOutputOutputTypeDef",
+    "GetBucketWebsiteOutputTypeDef",
     "WebsiteConfigurationTypeDef",
     "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
-    "SelectObjectContentEventStreamOutputTypeDef",
+    "SelectObjectContentEventStreamTypeDef",
     "IntelligentTieringConfigurationOutputTypeDef",
     "LifecycleRuleOutputTypeDef",
     "MetricsConfigurationOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
     "LifecycleRuleTypeDef",
     "MetricsConfigurationTypeDef",
     "StorageClassAnalysisOutputTypeDef",
     "StorageClassAnalysisTypeDef",
-    "GetObjectLockConfigurationOutputOutputTypeDef",
+    "GetObjectLockConfigurationOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
     "LambdaFunctionConfigurationOutputTypeDef",
     "QueueConfigurationOutputTypeDef",
     "TopicConfigurationOutputTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
-    "GetBucketLoggingOutputOutputTypeDef",
+    "GetBucketLoggingOutputTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
     "BucketLoggingStatusTypeDef",
     "InventoryDestinationOutputTypeDef",
     "InventoryDestinationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     "PutBucketLifecycleRequestRequestTypeDef",
     "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
-    "GetBucketEncryptionOutputOutputTypeDef",
+    "GetBucketEncryptionOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
-    "SelectObjectContentOutputOutputTypeDef",
-    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
-    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
-    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
-    "GetBucketMetricsConfigurationOutputOutputTypeDef",
-    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
+    "SelectObjectContentOutputTypeDef",
+    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
+    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+    "GetBucketLifecycleConfigurationOutputTypeDef",
+    "GetBucketMetricsConfigurationOutputTypeDef",
+    "ListBucketMetricsConfigurationsOutputTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "BucketLifecycleConfigurationTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
     "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
-    "NotificationConfigurationOutputTypeDef",
+    "NotificationConfigurationResponseMetadataTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
     "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
-    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
-    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
+    "GetBucketAnalyticsConfigurationOutputTypeDef",
+    "ListBucketAnalyticsConfigurationsOutputTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
-    "GetBucketInventoryConfigurationOutputOutputTypeDef",
-    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
+    "GetBucketInventoryConfigurationOutputTypeDef",
+    "ListBucketInventoryConfigurationsOutputTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
-    "GetBucketReplicationOutputOutputTypeDef",
+    "GetBucketReplicationOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
 )
 
 AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadOutputTypeDef",
     {
         "DaysAfterInitiation": int,
@@ -541,16 +541,16 @@
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
-AbortMultipartUploadOutputOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputOutputTypeDef",
+AbortMultipartUploadOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
@@ -731,16 +731,16 @@
 
 class BucketDownloadFileobjRequestTypeDef(
     _RequiredBucketDownloadFileobjRequestTypeDef, _OptionalBucketDownloadFileobjRequestTypeDef
 ):
     pass
 
 
-BucketOutputTypeDef = TypedDict(
-    "BucketOutputTypeDef",
+BucketTypeDef = TypedDict(
+    "BucketTypeDef",
     {
         "Name": str,
         "CreationDate": datetime,
     },
 )
 
 _RequiredBucketUploadFileRequestTypeDef = TypedDict(
@@ -848,16 +848,16 @@
         "RecordDelimiter": str,
         "FieldDelimiter": str,
         "QuoteCharacter": str,
     },
     total=False,
 )
 
-ChecksumOutputTypeDef = TypedDict(
-    "ChecksumOutputTypeDef",
+ChecksumTypeDef = TypedDict(
+    "ChecksumTypeDef",
     {
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
 )
@@ -1006,23 +1006,23 @@
         "Events": Sequence[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
     total=False,
 )
 
-CommonPrefixOutputTypeDef = TypedDict(
-    "CommonPrefixOutputTypeDef",
+CommonPrefixTypeDef = TypedDict(
+    "CommonPrefixTypeDef",
     {
         "Prefix": str,
     },
 )
 
-CompleteMultipartUploadOutputOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputOutputTypeDef",
+CompleteMultipartUploadOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputTypeDef",
     {
         "Location": str,
         "Bucket": str,
         "Key": str,
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
@@ -1064,16 +1064,16 @@
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
     total=False,
 )
 
-CopyObjectResultOutputTypeDef = TypedDict(
-    "CopyObjectResultOutputTypeDef",
+CopyObjectResultTypeDef = TypedDict(
+    "CopyObjectResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1193,16 +1193,16 @@
 class CopyObjectRequestObjectSummaryCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef,
     _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef,
 ):
     pass
 
 
-CopyPartResultOutputTypeDef = TypedDict(
-    "CopyPartResultOutputTypeDef",
+CopyPartResultTypeDef = TypedDict(
+    "CopyPartResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1213,24 +1213,24 @@
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputOutputTypeDef = TypedDict(
-    "CreateBucketOutputOutputTypeDef",
+CreateBucketOutputTypeDef = TypedDict(
+    "CreateBucketOutputTypeDef",
     {
         "Location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateMultipartUploadOutputOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputOutputTypeDef",
+CreateMultipartUploadOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
@@ -1732,16 +1732,16 @@
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
     total=False,
 )
 
-DeleteObjectOutputOutputTypeDef = TypedDict(
-    "DeleteObjectOutputOutputTypeDef",
+DeleteObjectOutputTypeDef = TypedDict(
+    "DeleteObjectOutputTypeDef",
     {
         "DeleteMarker": bool,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1803,16 +1803,16 @@
 
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
 
-DeleteObjectTaggingOutputOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputOutputTypeDef",
+DeleteObjectTaggingOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
@@ -1835,26 +1835,26 @@
 class DeleteObjectTaggingRequestRequestTypeDef(
     _RequiredDeleteObjectTaggingRequestRequestTypeDef,
     _OptionalDeleteObjectTaggingRequestRequestTypeDef,
 ):
     pass
 
 
-DeletedObjectOutputTypeDef = TypedDict(
-    "DeletedObjectOutputTypeDef",
+DeletedObjectTypeDef = TypedDict(
+    "DeletedObjectTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "DeleteMarker": bool,
         "DeleteMarkerVersionId": str,
     },
 )
 
-ErrorOutputTypeDef = TypedDict(
-    "ErrorOutputTypeDef",
+ErrorTypeDef = TypedDict(
+    "ErrorTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "Code": str,
         "Message": str,
     },
 )
@@ -1991,16 +1991,16 @@
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
-GetBucketAccelerateConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
+GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputTypeDef",
     {
         "Status": BucketAccelerateStatusType,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2185,16 +2185,16 @@
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketLocationOutputOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputOutputTypeDef",
+GetBucketLocationOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
@@ -2302,16 +2302,16 @@
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketPolicyOutputOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputOutputTypeDef",
+GetBucketPolicyOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
@@ -2331,16 +2331,16 @@
 
 class GetBucketPolicyRequestRequestTypeDef(
     _RequiredGetBucketPolicyRequestRequestTypeDef, _OptionalGetBucketPolicyRequestRequestTypeDef
 ):
     pass
 
 
-PolicyStatusOutputTypeDef = TypedDict(
-    "PolicyStatusOutputTypeDef",
+PolicyStatusTypeDef = TypedDict(
+    "PolicyStatusTypeDef",
     {
         "IsPublic": bool,
     },
 )
 
 _RequiredGetBucketPolicyStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyStatusRequestRequestTypeDef",
@@ -2382,16 +2382,16 @@
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketRequestPaymentOutputOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputOutputTypeDef",
+GetBucketRequestPaymentOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputTypeDef",
     {
         "Payer": PayerType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
@@ -2433,16 +2433,16 @@
 
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketVersioningOutputOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputOutputTypeDef",
+GetBucketVersioningOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputTypeDef",
     {
         "Status": BucketVersioningStatusType,
         "MFADelete": MFADeleteStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2524,16 +2524,16 @@
 
 class GetObjectAclRequestRequestTypeDef(
     _RequiredGetObjectAclRequestRequestTypeDef, _OptionalGetObjectAclRequestRequestTypeDef
 ):
     pass
 
 
-ObjectPartOutputTypeDef = TypedDict(
-    "ObjectPartOutputTypeDef",
+ObjectPartTypeDef = TypedDict(
+    "ObjectPartTypeDef",
     {
         "PartNumber": int,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -2621,16 +2621,16 @@
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetObjectOutputOutputTypeDef = TypedDict(
-    "GetObjectOutputOutputTypeDef",
+GetObjectOutputTypeDef = TypedDict(
+    "GetObjectOutputTypeDef",
     {
         "Body": StreamingBody,
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "LastModified": datetime,
@@ -2838,16 +2838,16 @@
 
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
 
-GetObjectTorrentOutputOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputOutputTypeDef",
+GetObjectTorrentOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputTypeDef",
     {
         "Body": StreamingBody,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2972,16 +2972,16 @@
 
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
 
-HeadObjectOutputOutputTypeDef = TypedDict(
-    "HeadObjectOutputOutputTypeDef",
+HeadObjectOutputTypeDef = TypedDict(
+    "HeadObjectOutputTypeDef",
     {
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "ArchiveStatus": ArchiveStatusType,
         "LastModified": datetime,
@@ -3081,28 +3081,28 @@
 IndexDocumentTypeDef = TypedDict(
     "IndexDocumentTypeDef",
     {
         "Suffix": str,
     },
 )
 
-InitiatorOutputTypeDef = TypedDict(
-    "InitiatorOutputTypeDef",
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
     {
         "ID": str,
         "DisplayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
+InitiatorTypeDef = TypedDict(
+    "InitiatorTypeDef",
     {
         "ID": str,
         "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JSONInputTypeDef = TypedDict(
     "JSONInputTypeDef",
     {
         "Type": JSONTypeType,
@@ -3567,16 +3567,16 @@
 
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
     pass
 
 
-PartOutputTypeDef = TypedDict(
-    "PartOutputTypeDef",
+PartTypeDef = TypedDict(
+    "PartTypeDef",
     {
         "PartNumber": int,
         "LastModified": datetime,
         "ETag": str,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
@@ -3768,16 +3768,16 @@
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": Union[datetime, str],
     },
     total=False,
 )
 
-RestoreStatusOutputTypeDef = TypedDict(
-    "RestoreStatusOutputTypeDef",
+RestoreStatusTypeDef = TypedDict(
+    "RestoreStatusTypeDef",
     {
         "IsRestoreInProgress": bool,
         "RestoreExpiryDate": datetime,
     },
 )
 
 _RequiredObjectUploadFileRequestTypeDef = TypedDict(
@@ -3855,16 +3855,16 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ProgressOutputTypeDef = TypedDict(
-    "ProgressOutputTypeDef",
+ProgressTypeDef = TypedDict(
+    "ProgressTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
@@ -3959,40 +3959,40 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputOutputTypeDef = TypedDict(
-    "PutObjectAclOutputOutputTypeDef",
+PutObjectAclOutputTypeDef = TypedDict(
+    "PutObjectAclOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLegalHoldOutputOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputOutputTypeDef",
+PutObjectLegalHoldOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLockConfigurationOutputOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputOutputTypeDef",
+PutObjectLockConfigurationOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectOutputOutputTypeDef = TypedDict(
-    "PutObjectOutputOutputTypeDef",
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
     {
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -4199,32 +4199,32 @@
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
 
-PutObjectRetentionOutputOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputOutputTypeDef",
+PutObjectRetentionOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectTaggingOutputOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputOutputTypeDef",
+PutObjectTaggingOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecordsEventOutputTypeDef = TypedDict(
-    "RecordsEventOutputTypeDef",
+RecordsEventTypeDef = TypedDict(
+    "RecordsEventTypeDef",
     {
         "Payload": bytes,
     },
 )
 
 RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
     "RedirectAllRequestsToResponseMetadataTypeDef",
@@ -4308,16 +4308,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RestoreObjectOutputOutputTypeDef = TypedDict(
-    "RestoreObjectOutputOutputTypeDef",
+RestoreObjectOutputTypeDef = TypedDict(
+    "RestoreObjectOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "RestoreOutputPath": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4378,25 +4378,25 @@
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
-StatsOutputTypeDef = TypedDict(
-    "StatsOutputTypeDef",
+StatsTypeDef = TypedDict(
+    "StatsTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
-UploadPartOutputOutputTypeDef = TypedDict(
-    "UploadPartOutputOutputTypeDef",
+UploadPartOutputTypeDef = TypedDict(
+    "UploadPartOutputTypeDef",
     {
         "ServerSideEncryption": ServerSideEncryptionType,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -4553,24 +4553,24 @@
     "AnalyticsAndOperatorOutputTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetBucketTaggingOutputOutputTypeDef = TypedDict(
-    "GetBucketTaggingOutputOutputTypeDef",
+GetBucketTaggingOutputTypeDef = TypedDict(
+    "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectTaggingOutputOutputTypeDef = TypedDict(
-    "GetObjectTaggingOutputOutputTypeDef",
+GetObjectTaggingOutputTypeDef = TypedDict(
+    "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4889,53 +4889,53 @@
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
-GetBucketCorsOutputOutputTypeDef = TypedDict(
-    "GetBucketCorsOutputOutputTypeDef",
+GetBucketCorsOutputTypeDef = TypedDict(
+    "GetBucketCorsOutputTypeDef",
     {
         "CORSRules": List[CORSRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
     },
     total=False,
 )
 
-CopyObjectOutputOutputTypeDef = TypedDict(
-    "CopyObjectOutputOutputTypeDef",
+CopyObjectOutputTypeDef = TypedDict(
+    "CopyObjectOutputTypeDef",
     {
-        "CopyObjectResult": CopyObjectResultOutputTypeDef,
+        "CopyObjectResult": CopyObjectResultTypeDef,
         "Expiration": str,
         "CopySourceVersionId": str,
         "VersionId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadPartCopyOutputOutputTypeDef = TypedDict(
-    "UploadPartCopyOutputOutputTypeDef",
+UploadPartCopyOutputTypeDef = TypedDict(
+    "UploadPartCopyOutputTypeDef",
     {
         "CopySourceVersionId": str,
-        "CopyPartResult": CopyPartResultOutputTypeDef,
+        "CopyPartResult": CopyPartResultTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -5028,40 +5028,40 @@
     "ObjectLockRuleTypeDef",
     {
         "DefaultRetention": DefaultRetentionTypeDef,
     },
     total=False,
 )
 
-DeleteMarkerEntryOutputTypeDef = TypedDict(
-    "DeleteMarkerEntryOutputTypeDef",
+DeleteMarkerEntryTypeDef = TypedDict(
+    "DeleteMarkerEntryTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
     },
 )
 
-ListBucketsOutputOutputTypeDef = TypedDict(
-    "ListBucketsOutputOutputTypeDef",
+ListBucketsOutputTypeDef = TypedDict(
+    "ListBucketsOutputTypeDef",
     {
-        "Buckets": List[BucketOutputTypeDef],
+        "Buckets": List[BucketTypeDef],
         "Owner": OwnerOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteObjectsOutputOutputTypeDef = TypedDict(
-    "DeleteObjectsOutputOutputTypeDef",
+DeleteObjectsOutputTypeDef = TypedDict(
+    "DeleteObjectsOutputTypeDef",
     {
-        "Deleted": List[DeletedObjectOutputTypeDef],
+        "Deleted": List[DeletedObjectTypeDef],
         "RequestCharged": Literal["requester"],
-        "Errors": List[ErrorOutputTypeDef],
+        "Errors": List[ErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
@@ -5092,52 +5092,52 @@
     "S3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
-GetBucketPolicyStatusOutputOutputTypeDef = TypedDict(
-    "GetBucketPolicyStatusOutputOutputTypeDef",
+GetBucketPolicyStatusOutputTypeDef = TypedDict(
+    "GetBucketPolicyStatusOutputTypeDef",
     {
-        "PolicyStatus": PolicyStatusOutputTypeDef,
+        "PolicyStatus": PolicyStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAttributesPartsOutputTypeDef = TypedDict(
-    "GetObjectAttributesPartsOutputTypeDef",
+GetObjectAttributesPartsTypeDef = TypedDict(
+    "GetObjectAttributesPartsTypeDef",
     {
         "TotalPartsCount": int,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[ObjectPartOutputTypeDef],
+        "Parts": List[ObjectPartTypeDef],
     },
 )
 
-GetObjectLegalHoldOutputOutputTypeDef = TypedDict(
-    "GetObjectLegalHoldOutputOutputTypeDef",
+GetObjectLegalHoldOutputTypeDef = TypedDict(
+    "GetObjectLegalHoldOutputTypeDef",
     {
         "LegalHold": ObjectLockLegalHoldOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectRetentionOutputOutputTypeDef = TypedDict(
-    "GetObjectRetentionOutputOutputTypeDef",
+GetObjectRetentionOutputTypeDef = TypedDict(
+    "GetObjectRetentionOutputTypeDef",
     {
         "Retention": ObjectLockRetentionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPublicAccessBlockOutputOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputOutputTypeDef",
+GetPublicAccessBlockOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GrantOutputTypeDef = TypedDict(
@@ -5288,23 +5288,23 @@
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
 
-MultipartUploadOutputTypeDef = TypedDict(
-    "MultipartUploadOutputTypeDef",
+MultipartUploadTypeDef = TypedDict(
+    "MultipartUploadTypeDef",
     {
         "UploadId": str,
         "Key": str,
         "Initiated": datetime,
         "StorageClass": StorageClassType,
         "Owner": OwnerOutputTypeDef,
-        "Initiator": InitiatorOutputTypeDef,
+        "Initiator": InitiatorTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
@@ -5377,28 +5377,28 @@
 )
 
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 
-ListPartsOutputOutputTypeDef = TypedDict(
-    "ListPartsOutputOutputTypeDef",
+ListPartsOutputTypeDef = TypedDict(
+    "ListPartsOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[PartOutputTypeDef],
-        "Initiator": InitiatorOutputTypeDef,
+        "Parts": List[PartTypeDef],
+        "Initiator": InitiatorTypeDef,
         "Owner": OwnerOutputTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5442,16 +5442,16 @@
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
-NotificationConfigurationDeprecatedOutputTypeDef = TypedDict(
-    "NotificationConfigurationDeprecatedOutputTypeDef",
+NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
+    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5519,41 +5519,41 @@
 class PutObjectRetentionRequestRequestTypeDef(
     _RequiredPutObjectRetentionRequestRequestTypeDef,
     _OptionalPutObjectRetentionRequestRequestTypeDef,
 ):
     pass
 
 
-ObjectOutputTypeDef = TypedDict(
-    "ObjectOutputTypeDef",
+ObjectTypeDef = TypedDict(
+    "ObjectTypeDef",
     {
         "Key": str,
         "LastModified": datetime,
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": ObjectStorageClassType,
         "Owner": OwnerOutputTypeDef,
-        "RestoreStatus": RestoreStatusOutputTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
     },
 )
 
-ObjectVersionOutputTypeDef = TypedDict(
-    "ObjectVersionOutputTypeDef",
+ObjectVersionTypeDef = TypedDict(
+    "ObjectVersionTypeDef",
     {
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": Literal["STANDARD"],
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
         "Owner": OwnerOutputTypeDef,
-        "RestoreStatus": RestoreStatusOutputTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
     },
 )
 
 OwnershipControlsOutputTypeDef = TypedDict(
     "OwnershipControlsOutputTypeDef",
     {
         "Rules": List[OwnershipControlsRuleOutputTypeDef],
@@ -5563,18 +5563,18 @@
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
         "Rules": Sequence[OwnershipControlsRuleTypeDef],
     },
 )
 
-ProgressEventOutputTypeDef = TypedDict(
-    "ProgressEventOutputTypeDef",
+ProgressEventTypeDef = TypedDict(
+    "ProgressEventTypeDef",
     {
-        "Details": ProgressOutputTypeDef,
+        "Details": ProgressTypeDef,
     },
 )
 
 _RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -5752,18 +5752,18 @@
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
     total=False,
 )
 
-StatsEventOutputTypeDef = TypedDict(
-    "StatsEventOutputTypeDef",
+StatsEventTypeDef = TypedDict(
+    "StatsEventTypeDef",
     {
-        "Details": StatsOutputTypeDef,
+        "Details": StatsTypeDef,
     },
 )
 
 AnalyticsFilterOutputTypeDef = TypedDict(
     "AnalyticsFilterOutputTypeDef",
     {
         "Prefix": str,
@@ -6129,41 +6129,41 @@
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": S3KeyFilterTypeDef,
     },
     total=False,
 )
 
-GetObjectAttributesOutputOutputTypeDef = TypedDict(
-    "GetObjectAttributesOutputOutputTypeDef",
+GetObjectAttributesOutputTypeDef = TypedDict(
+    "GetObjectAttributesOutputTypeDef",
     {
         "DeleteMarker": bool,
         "LastModified": datetime,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
-        "Checksum": ChecksumOutputTypeDef,
-        "ObjectParts": GetObjectAttributesPartsOutputTypeDef,
+        "Checksum": ChecksumTypeDef,
+        "ObjectParts": GetObjectAttributesPartsTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketAclOutputOutputTypeDef = TypedDict(
-    "GetBucketAclOutputOutputTypeDef",
+GetBucketAclOutputTypeDef = TypedDict(
+    "GetBucketAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAclOutputOutputTypeDef = TypedDict(
-    "GetObjectAclOutputOutputTypeDef",
+GetObjectAclOutputTypeDef = TypedDict(
+    "GetObjectAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -6237,28 +6237,28 @@
 )
 
 
 class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
     pass
 
 
-ListMultipartUploadsOutputOutputTypeDef = TypedDict(
-    "ListMultipartUploadsOutputOutputTypeDef",
+ListMultipartUploadsOutputTypeDef = TypedDict(
+    "ListMultipartUploadsOutputTypeDef",
     {
         "Bucket": str,
         "KeyMarker": str,
         "UploadIdMarker": str,
         "NextKeyMarker": str,
         "Prefix": str,
         "Delimiter": str,
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
-        "Uploads": List[MultipartUploadOutputTypeDef],
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "Uploads": List[MultipartUploadTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InventoryS3BucketDestinationOutputTypeDef = TypedDict(
@@ -6334,16 +6334,16 @@
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
-GetBucketLifecycleOutputOutputTypeDef = TypedDict(
-    "GetBucketLifecycleOutputOutputTypeDef",
+GetBucketLifecycleOutputTypeDef = TypedDict(
+    "GetBucketLifecycleOutputTypeDef",
     {
         "Rules": List[RuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
@@ -6410,75 +6410,75 @@
 class PutBucketNotificationRequestRequestTypeDef(
     _RequiredPutBucketNotificationRequestRequestTypeDef,
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
 
-ListObjectsOutputOutputTypeDef = TypedDict(
-    "ListObjectsOutputOutputTypeDef",
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
-        "Contents": List[ObjectOutputTypeDef],
+        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectsV2OutputOutputTypeDef = TypedDict(
-    "ListObjectsV2OutputOutputTypeDef",
+ListObjectsV2OutputTypeDef = TypedDict(
+    "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
-        "Contents": List[ObjectOutputTypeDef],
+        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectVersionsOutputOutputTypeDef = TypedDict(
-    "ListObjectVersionsOutputOutputTypeDef",
+ListObjectVersionsOutputTypeDef = TypedDict(
+    "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
         "KeyMarker": str,
         "VersionIdMarker": str,
         "NextKeyMarker": str,
         "NextVersionIdMarker": str,
-        "Versions": List[ObjectVersionOutputTypeDef],
-        "DeleteMarkers": List[DeleteMarkerEntryOutputTypeDef],
+        "Versions": List[ObjectVersionTypeDef],
+        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketOwnershipControlsOutputOutputTypeDef = TypedDict(
-    "GetBucketOwnershipControlsOutputOutputTypeDef",
+GetBucketOwnershipControlsOutputTypeDef = TypedDict(
+    "GetBucketOwnershipControlsOutputTypeDef",
     {
         "OwnershipControls": OwnershipControlsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
@@ -6501,16 +6501,16 @@
 class PutBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredPutBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalPutBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketWebsiteOutputOutputTypeDef = TypedDict(
-    "GetBucketWebsiteOutputOutputTypeDef",
+GetBucketWebsiteOutputTypeDef = TypedDict(
+    "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToOutputTypeDef,
         "IndexDocument": IndexDocumentOutputTypeDef,
         "ErrorDocument": ErrorDocumentOutputTypeDef,
         "RoutingRules": List[RoutingRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6537,20 +6537,20 @@
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
     },
 )
 
-SelectObjectContentEventStreamOutputTypeDef = TypedDict(
-    "SelectObjectContentEventStreamOutputTypeDef",
+SelectObjectContentEventStreamTypeDef = TypedDict(
+    "SelectObjectContentEventStreamTypeDef",
     {
-        "Records": RecordsEventOutputTypeDef,
-        "Stats": StatsEventOutputTypeDef,
-        "Progress": ProgressEventOutputTypeDef,
+        "Records": RecordsEventTypeDef,
+        "Stats": StatsEventTypeDef,
+        "Progress": ProgressEventTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
 )
 
 IntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "IntelligentTieringConfigurationOutputTypeDef",
@@ -6666,16 +6666,16 @@
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
     total=False,
 )
 
-GetObjectLockConfigurationOutputOutputTypeDef = TypedDict(
-    "GetObjectLockConfigurationOutputOutputTypeDef",
+GetObjectLockConfigurationOutputTypeDef = TypedDict(
+    "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
@@ -6800,16 +6800,16 @@
 
 class TopicConfigurationTypeDef(
     _RequiredTopicConfigurationTypeDef, _OptionalTopicConfigurationTypeDef
 ):
     pass
 
 
-GetBucketLoggingOutputOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputOutputTypeDef",
+GetBucketLoggingOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputTypeDef",
     {
         "LoggingEnabled": LoggingEnabledOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
@@ -7054,16 +7054,16 @@
 
 class PutBucketWebsiteRequestRequestTypeDef(
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketEncryptionOutputOutputTypeDef = TypedDict(
-    "GetBucketEncryptionOutputOutputTypeDef",
+GetBucketEncryptionOutputTypeDef = TypedDict(
+    "GetBucketEncryptionOutputTypeDef",
     {
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
@@ -7087,59 +7087,59 @@
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
 
-SelectObjectContentOutputOutputTypeDef = TypedDict(
-    "SelectObjectContentOutputOutputTypeDef",
+SelectObjectContentOutputTypeDef = TypedDict(
+    "SelectObjectContentOutputTypeDef",
     {
-        "Payload": "EventStream[SelectObjectContentEventStreamOutputTypeDef]",
+        "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketIntelligentTieringConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
+GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
+    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
+ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketLifecycleConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
+GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputTypeDef",
     {
         "Rules": List[LifecycleRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketMetricsConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketMetricsConfigurationOutputOutputTypeDef",
+GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
+    "GetBucketMetricsConfigurationOutputTypeDef",
     {
         "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketMetricsConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
+ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7212,16 +7212,16 @@
 
 class AnalyticsConfigurationTypeDef(
     _RequiredAnalyticsConfigurationTypeDef, _OptionalAnalyticsConfigurationTypeDef
 ):
     pass
 
 
-NotificationConfigurationOutputTypeDef = TypedDict(
-    "NotificationConfigurationOutputTypeDef",
+NotificationConfigurationResponseMetadataTypeDef = TypedDict(
+    "NotificationConfigurationResponseMetadataTypeDef",
     {
         "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
         "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
         "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7383,24 +7383,24 @@
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketAnalyticsConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
+GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
         "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketAnalyticsConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
+ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7523,24 +7523,24 @@
 
 class RestoreObjectRequestRequestTypeDef(
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketInventoryConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketInventoryConfigurationOutputOutputTypeDef",
+GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
+    "GetBucketInventoryConfigurationOutputTypeDef",
     {
         "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketInventoryConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
+ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
         "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7566,16 +7566,16 @@
 class PutBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketReplicationOutputOutputTypeDef = TypedDict(
-    "GetBucketReplicationOutputOutputTypeDef",
+GetBucketReplicationOutputTypeDef = TypedDict(
+    "GetBucketReplicationOutputTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,55 +78,55 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputOutputTypeDef",
+    "AbortMultipartUploadOutputTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
     "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
     "TagOutputTypeDef",
     "TagTypeDef",
     "AnalyticsS3BucketDestinationOutputTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "BucketDownloadFileobjRequestTypeDef",
-    "BucketOutputTypeDef",
+    "BucketTypeDef",
     "BucketUploadFileRequestTypeDef",
     "BucketUploadFileobjRequestTypeDef",
     "CORSRuleTypeDef",
     "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
-    "ChecksumOutputTypeDef",
+    "ChecksumTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
-    "CommonPrefixOutputTypeDef",
-    "CompleteMultipartUploadOutputOutputTypeDef",
+    "CommonPrefixTypeDef",
+    "CompleteMultipartUploadOutputTypeDef",
     "CompletedPartTypeDef",
     "ConditionOutputTypeDef",
     "ConditionTypeDef",
-    "CopyObjectResultOutputTypeDef",
+    "CopyObjectResultTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
-    "CopyPartResultOutputTypeDef",
+    "CopyPartResultTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputOutputTypeDef",
-    "CreateMultipartUploadOutputOutputTypeDef",
+    "CreateBucketOutputTypeDef",
+    "CreateMultipartUploadOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
     "DefaultRetentionOutputTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
@@ -147,95 +147,95 @@
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
     "OwnerOutputTypeDef",
     "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputOutputTypeDef",
+    "DeleteObjectOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputOutputTypeDef",
+    "DeleteObjectTaggingOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
-    "DeletedObjectOutputTypeDef",
-    "ErrorOutputTypeDef",
+    "DeletedObjectTypeDef",
+    "ErrorTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
     "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
     "ErrorDocumentOutputTypeDef",
     "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
     "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
     "FilterRuleOutputTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
+    "GetBucketAccelerateConfigurationOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputOutputTypeDef",
+    "GetBucketLocationOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputOutputTypeDef",
+    "GetBucketPolicyOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
-    "PolicyStatusOutputTypeDef",
+    "PolicyStatusTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputOutputTypeDef",
+    "GetBucketRequestPaymentOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputOutputTypeDef",
+    "GetBucketVersioningOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "IndexDocumentOutputTypeDef",
     "RedirectAllRequestsToOutputTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
-    "ObjectPartOutputTypeDef",
+    "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldOutputTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputOutputTypeDef",
+    "GetObjectOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputOutputTypeDef",
+    "GetObjectTorrentOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputOutputTypeDef",
+    "HeadObjectOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
     "IndexDocumentResponseMetadataTypeDef",
     "IndexDocumentTypeDef",
-    "InitiatorOutputTypeDef",
     "InitiatorResponseMetadataTypeDef",
+    "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringOutputTypeDef",
     "TieringTypeDef",
     "InventoryFilterOutputTypeDef",
     "InventoryScheduleOutputTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
@@ -258,78 +258,78 @@
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
-    "PartOutputTypeDef",
+    "PartTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "QueueConfigurationDeprecatedOutputTypeDef",
     "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "ObjectLockRetentionTypeDef",
-    "RestoreStatusOutputTypeDef",
+    "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
     "OwnerResponseMetadataTypeDef",
     "OwnershipControlsRuleOutputTypeDef",
     "OwnershipControlsRuleTypeDef",
     "PaginatorConfigTypeDef",
-    "ProgressOutputTypeDef",
+    "ProgressTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputOutputTypeDef",
-    "PutObjectLegalHoldOutputOutputTypeDef",
-    "PutObjectLockConfigurationOutputOutputTypeDef",
-    "PutObjectOutputOutputTypeDef",
+    "PutObjectAclOutputTypeDef",
+    "PutObjectLegalHoldOutputTypeDef",
+    "PutObjectLockConfigurationOutputTypeDef",
+    "PutObjectOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputOutputTypeDef",
-    "PutObjectTaggingOutputOutputTypeDef",
-    "RecordsEventOutputTypeDef",
+    "PutObjectRetentionOutputTypeDef",
+    "PutObjectTaggingOutputTypeDef",
+    "RecordsEventTypeDef",
     "RedirectAllRequestsToResponseMetadataTypeDef",
     "RedirectAllRequestsToTypeDef",
     "RedirectOutputTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
     "ResponseMetadataTypeDef",
-    "RestoreObjectOutputOutputTypeDef",
+    "RestoreObjectOutputTypeDef",
     "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultOutputTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
-    "StatsOutputTypeDef",
-    "UploadPartOutputOutputTypeDef",
+    "StatsTypeDef",
+    "UploadPartOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "AnalyticsAndOperatorOutputTypeDef",
-    "GetBucketTaggingOutputOutputTypeDef",
-    "GetObjectTaggingOutputOutputTypeDef",
+    "GetBucketTaggingOutputTypeDef",
+    "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorOutputTypeDef",
     "MetricsAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
@@ -341,75 +341,75 @@
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "ObjectCopyRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
     "CORSConfigurationTypeDef",
-    "GetBucketCorsOutputOutputTypeDef",
+    "GetBucketCorsOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
-    "CopyObjectOutputOutputTypeDef",
-    "UploadPartCopyOutputOutputTypeDef",
+    "CopyObjectOutputTypeDef",
+    "UploadPartCopyOutputTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
     "ObjectLockRuleOutputTypeDef",
     "ObjectLockRuleTypeDef",
-    "DeleteMarkerEntryOutputTypeDef",
-    "ListBucketsOutputOutputTypeDef",
-    "DeleteObjectsOutputOutputTypeDef",
+    "DeleteMarkerEntryTypeDef",
+    "ListBucketsOutputTypeDef",
+    "DeleteObjectsOutputTypeDef",
     "DeleteTypeDef",
     "S3KeyFilterOutputTypeDef",
     "S3KeyFilterTypeDef",
-    "GetBucketPolicyStatusOutputOutputTypeDef",
-    "GetObjectAttributesPartsOutputTypeDef",
-    "GetObjectLegalHoldOutputOutputTypeDef",
-    "GetObjectRetentionOutputOutputTypeDef",
-    "GetPublicAccessBlockOutputOutputTypeDef",
+    "GetBucketPolicyStatusOutputTypeDef",
+    "GetObjectAttributesPartsTypeDef",
+    "GetObjectLegalHoldOutputTypeDef",
+    "GetObjectRetentionOutputTypeDef",
+    "GetPublicAccessBlockOutputTypeDef",
     "GrantOutputTypeDef",
     "TargetGrantOutputTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
-    "MultipartUploadOutputTypeDef",
+    "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
     "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
-    "ListPartsOutputOutputTypeDef",
+    "ListPartsOutputTypeDef",
     "MetricsOutputTypeDef",
     "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
-    "NotificationConfigurationDeprecatedOutputTypeDef",
+    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
     "PutObjectLegalHoldRequestRequestTypeDef",
     "PutObjectRetentionRequestRequestTypeDef",
-    "ObjectOutputTypeDef",
-    "ObjectVersionOutputTypeDef",
+    "ObjectTypeDef",
+    "ObjectVersionTypeDef",
     "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
-    "ProgressEventOutputTypeDef",
+    "ProgressEventTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "RoutingRuleOutputTypeDef",
     "RoutingRuleTypeDef",
     "ServerSideEncryptionRuleOutputTypeDef",
     "ServerSideEncryptionRuleTypeDef",
     "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
-    "StatsEventOutputTypeDef",
+    "StatsEventTypeDef",
     "AnalyticsFilterOutputTypeDef",
     "IntelligentTieringFilterOutputTypeDef",
     "LifecycleRuleFilterOutputTypeDef",
     "MetricsFilterOutputTypeDef",
     "ReplicationRuleFilterOutputTypeDef",
     "AnalyticsFilterTypeDef",
     "IntelligentTieringFilterTypeDef",
@@ -427,109 +427,109 @@
     "CompleteMultipartUploadRequestRequestTypeDef",
     "ObjectLockConfigurationOutputTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
     "NotificationConfigurationFilterOutputTypeDef",
     "NotificationConfigurationFilterTypeDef",
-    "GetObjectAttributesOutputOutputTypeDef",
-    "GetBucketAclOutputOutputTypeDef",
-    "GetObjectAclOutputOutputTypeDef",
+    "GetObjectAttributesOutputTypeDef",
+    "GetBucketAclOutputTypeDef",
+    "GetObjectAclOutputTypeDef",
     "LoggingEnabledOutputTypeDef",
     "LoggingEnabledResponseMetadataTypeDef",
     "AccessControlPolicyTypeDef",
     "S3LocationTypeDef",
     "LoggingEnabledTypeDef",
-    "ListMultipartUploadsOutputOutputTypeDef",
+    "ListMultipartUploadsOutputTypeDef",
     "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
-    "GetBucketLifecycleOutputOutputTypeDef",
+    "GetBucketLifecycleOutputTypeDef",
     "LifecycleConfigurationTypeDef",
     "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
-    "ListObjectsOutputOutputTypeDef",
-    "ListObjectsV2OutputOutputTypeDef",
-    "ListObjectVersionsOutputOutputTypeDef",
-    "GetBucketOwnershipControlsOutputOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "ListObjectsV2OutputTypeDef",
+    "ListObjectVersionsOutputTypeDef",
+    "GetBucketOwnershipControlsOutputTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketWebsiteOutputOutputTypeDef",
+    "GetBucketWebsiteOutputTypeDef",
     "WebsiteConfigurationTypeDef",
     "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
-    "SelectObjectContentEventStreamOutputTypeDef",
+    "SelectObjectContentEventStreamTypeDef",
     "IntelligentTieringConfigurationOutputTypeDef",
     "LifecycleRuleOutputTypeDef",
     "MetricsConfigurationOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
     "LifecycleRuleTypeDef",
     "MetricsConfigurationTypeDef",
     "StorageClassAnalysisOutputTypeDef",
     "StorageClassAnalysisTypeDef",
-    "GetObjectLockConfigurationOutputOutputTypeDef",
+    "GetObjectLockConfigurationOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
     "LambdaFunctionConfigurationOutputTypeDef",
     "QueueConfigurationOutputTypeDef",
     "TopicConfigurationOutputTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
-    "GetBucketLoggingOutputOutputTypeDef",
+    "GetBucketLoggingOutputTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
     "BucketLoggingStatusTypeDef",
     "InventoryDestinationOutputTypeDef",
     "InventoryDestinationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     "PutBucketLifecycleRequestRequestTypeDef",
     "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
-    "GetBucketEncryptionOutputOutputTypeDef",
+    "GetBucketEncryptionOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
-    "SelectObjectContentOutputOutputTypeDef",
-    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
-    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
-    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
-    "GetBucketMetricsConfigurationOutputOutputTypeDef",
-    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
+    "SelectObjectContentOutputTypeDef",
+    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
+    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+    "GetBucketLifecycleConfigurationOutputTypeDef",
+    "GetBucketMetricsConfigurationOutputTypeDef",
+    "ListBucketMetricsConfigurationsOutputTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "BucketLifecycleConfigurationTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
     "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
-    "NotificationConfigurationOutputTypeDef",
+    "NotificationConfigurationResponseMetadataTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
     "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
-    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
-    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
+    "GetBucketAnalyticsConfigurationOutputTypeDef",
+    "ListBucketAnalyticsConfigurationsOutputTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
-    "GetBucketInventoryConfigurationOutputOutputTypeDef",
-    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
+    "GetBucketInventoryConfigurationOutputTypeDef",
+    "ListBucketInventoryConfigurationsOutputTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
-    "GetBucketReplicationOutputOutputTypeDef",
+    "GetBucketReplicationOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
 )
 
 AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadOutputTypeDef",
     {
         "DaysAfterInitiation": int,
@@ -540,16 +540,16 @@
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
-AbortMultipartUploadOutputOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputOutputTypeDef",
+AbortMultipartUploadOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
@@ -720,16 +720,16 @@
 )
 
 class BucketDownloadFileobjRequestTypeDef(
     _RequiredBucketDownloadFileobjRequestTypeDef, _OptionalBucketDownloadFileobjRequestTypeDef
 ):
     pass
 
-BucketOutputTypeDef = TypedDict(
-    "BucketOutputTypeDef",
+BucketTypeDef = TypedDict(
+    "BucketTypeDef",
     {
         "Name": str,
         "CreationDate": datetime,
     },
 )
 
 _RequiredBucketUploadFileRequestTypeDef = TypedDict(
@@ -831,16 +831,16 @@
         "RecordDelimiter": str,
         "FieldDelimiter": str,
         "QuoteCharacter": str,
     },
     total=False,
 )
 
-ChecksumOutputTypeDef = TypedDict(
-    "ChecksumOutputTypeDef",
+ChecksumTypeDef = TypedDict(
+    "ChecksumTypeDef",
     {
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
 )
@@ -979,23 +979,23 @@
         "Events": Sequence[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
     total=False,
 )
 
-CommonPrefixOutputTypeDef = TypedDict(
-    "CommonPrefixOutputTypeDef",
+CommonPrefixTypeDef = TypedDict(
+    "CommonPrefixTypeDef",
     {
         "Prefix": str,
     },
 )
 
-CompleteMultipartUploadOutputOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputOutputTypeDef",
+CompleteMultipartUploadOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputTypeDef",
     {
         "Location": str,
         "Bucket": str,
         "Key": str,
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
@@ -1037,16 +1037,16 @@
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
     total=False,
 )
 
-CopyObjectResultOutputTypeDef = TypedDict(
-    "CopyObjectResultOutputTypeDef",
+CopyObjectResultTypeDef = TypedDict(
+    "CopyObjectResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1162,16 +1162,16 @@
 
 class CopyObjectRequestObjectSummaryCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef,
     _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef,
 ):
     pass
 
-CopyPartResultOutputTypeDef = TypedDict(
-    "CopyPartResultOutputTypeDef",
+CopyPartResultTypeDef = TypedDict(
+    "CopyPartResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1182,24 +1182,24 @@
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputOutputTypeDef = TypedDict(
-    "CreateBucketOutputOutputTypeDef",
+CreateBucketOutputTypeDef = TypedDict(
+    "CreateBucketOutputTypeDef",
     {
         "Location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateMultipartUploadOutputOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputOutputTypeDef",
+CreateMultipartUploadOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
@@ -1675,16 +1675,16 @@
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
     total=False,
 )
 
-DeleteObjectOutputOutputTypeDef = TypedDict(
-    "DeleteObjectOutputOutputTypeDef",
+DeleteObjectOutputTypeDef = TypedDict(
+    "DeleteObjectOutputTypeDef",
     {
         "DeleteMarker": bool,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1744,16 +1744,16 @@
 )
 
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
-DeleteObjectTaggingOutputOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputOutputTypeDef",
+DeleteObjectTaggingOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
@@ -1774,26 +1774,26 @@
 
 class DeleteObjectTaggingRequestRequestTypeDef(
     _RequiredDeleteObjectTaggingRequestRequestTypeDef,
     _OptionalDeleteObjectTaggingRequestRequestTypeDef,
 ):
     pass
 
-DeletedObjectOutputTypeDef = TypedDict(
-    "DeletedObjectOutputTypeDef",
+DeletedObjectTypeDef = TypedDict(
+    "DeletedObjectTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "DeleteMarker": bool,
         "DeleteMarkerVersionId": str,
     },
 )
 
-ErrorOutputTypeDef = TypedDict(
-    "ErrorOutputTypeDef",
+ErrorTypeDef = TypedDict(
+    "ErrorTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "Code": str,
         "Message": str,
     },
 )
@@ -1924,16 +1924,16 @@
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
-GetBucketAccelerateConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
+GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputTypeDef",
     {
         "Status": BucketAccelerateStatusType,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2102,16 +2102,16 @@
 
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-GetBucketLocationOutputOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputOutputTypeDef",
+GetBucketLocationOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
@@ -2209,16 +2209,16 @@
 
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-GetBucketPolicyOutputOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputOutputTypeDef",
+GetBucketPolicyOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
@@ -2236,16 +2236,16 @@
 )
 
 class GetBucketPolicyRequestRequestTypeDef(
     _RequiredGetBucketPolicyRequestRequestTypeDef, _OptionalGetBucketPolicyRequestRequestTypeDef
 ):
     pass
 
-PolicyStatusOutputTypeDef = TypedDict(
-    "PolicyStatusOutputTypeDef",
+PolicyStatusTypeDef = TypedDict(
+    "PolicyStatusTypeDef",
     {
         "IsPublic": bool,
     },
 )
 
 _RequiredGetBucketPolicyStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyStatusRequestRequestTypeDef",
@@ -2283,16 +2283,16 @@
 
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketRequestPaymentOutputOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputOutputTypeDef",
+GetBucketRequestPaymentOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputTypeDef",
     {
         "Payer": PayerType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
@@ -2330,16 +2330,16 @@
 )
 
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
-GetBucketVersioningOutputOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputOutputTypeDef",
+GetBucketVersioningOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputTypeDef",
     {
         "Status": BucketVersioningStatusType,
         "MFADelete": MFADeleteStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2415,16 +2415,16 @@
 )
 
 class GetObjectAclRequestRequestTypeDef(
     _RequiredGetObjectAclRequestRequestTypeDef, _OptionalGetObjectAclRequestRequestTypeDef
 ):
     pass
 
-ObjectPartOutputTypeDef = TypedDict(
-    "ObjectPartOutputTypeDef",
+ObjectPartTypeDef = TypedDict(
+    "ObjectPartTypeDef",
     {
         "PartNumber": int,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -2506,16 +2506,16 @@
 
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetObjectOutputOutputTypeDef = TypedDict(
-    "GetObjectOutputOutputTypeDef",
+GetObjectOutputTypeDef = TypedDict(
+    "GetObjectOutputTypeDef",
     {
         "Body": StreamingBody,
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "LastModified": datetime,
@@ -2717,16 +2717,16 @@
 )
 
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
-GetObjectTorrentOutputOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputOutputTypeDef",
+GetObjectTorrentOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputTypeDef",
     {
         "Body": StreamingBody,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2843,16 +2843,16 @@
 )
 
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
-HeadObjectOutputOutputTypeDef = TypedDict(
-    "HeadObjectOutputOutputTypeDef",
+HeadObjectOutputTypeDef = TypedDict(
+    "HeadObjectOutputTypeDef",
     {
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "ArchiveStatus": ArchiveStatusType,
         "LastModified": datetime,
@@ -2950,28 +2950,28 @@
 IndexDocumentTypeDef = TypedDict(
     "IndexDocumentTypeDef",
     {
         "Suffix": str,
     },
 )
 
-InitiatorOutputTypeDef = TypedDict(
-    "InitiatorOutputTypeDef",
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
     {
         "ID": str,
         "DisplayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
+InitiatorTypeDef = TypedDict(
+    "InitiatorTypeDef",
     {
         "ID": str,
         "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JSONInputTypeDef = TypedDict(
     "JSONInputTypeDef",
     {
         "Type": JSONTypeType,
@@ -3412,16 +3412,16 @@
 )
 
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
     pass
 
-PartOutputTypeDef = TypedDict(
-    "PartOutputTypeDef",
+PartTypeDef = TypedDict(
+    "PartTypeDef",
     {
         "PartNumber": int,
         "LastModified": datetime,
         "ETag": str,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
@@ -3605,16 +3605,16 @@
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": Union[datetime, str],
     },
     total=False,
 )
 
-RestoreStatusOutputTypeDef = TypedDict(
-    "RestoreStatusOutputTypeDef",
+RestoreStatusTypeDef = TypedDict(
+    "RestoreStatusTypeDef",
     {
         "IsRestoreInProgress": bool,
         "RestoreExpiryDate": datetime,
     },
 )
 
 _RequiredObjectUploadFileRequestTypeDef = TypedDict(
@@ -3688,16 +3688,16 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ProgressOutputTypeDef = TypedDict(
-    "ProgressOutputTypeDef",
+ProgressTypeDef = TypedDict(
+    "ProgressTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
@@ -3788,40 +3788,40 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputOutputTypeDef = TypedDict(
-    "PutObjectAclOutputOutputTypeDef",
+PutObjectAclOutputTypeDef = TypedDict(
+    "PutObjectAclOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLegalHoldOutputOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputOutputTypeDef",
+PutObjectLegalHoldOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLockConfigurationOutputOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputOutputTypeDef",
+PutObjectLockConfigurationOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectOutputOutputTypeDef = TypedDict(
-    "PutObjectOutputOutputTypeDef",
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
     {
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -4024,32 +4024,32 @@
 )
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-PutObjectRetentionOutputOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputOutputTypeDef",
+PutObjectRetentionOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectTaggingOutputOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputOutputTypeDef",
+PutObjectTaggingOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecordsEventOutputTypeDef = TypedDict(
-    "RecordsEventOutputTypeDef",
+RecordsEventTypeDef = TypedDict(
+    "RecordsEventTypeDef",
     {
         "Payload": bytes,
     },
 )
 
 RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
     "RedirectAllRequestsToResponseMetadataTypeDef",
@@ -4131,16 +4131,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RestoreObjectOutputOutputTypeDef = TypedDict(
-    "RestoreObjectOutputOutputTypeDef",
+RestoreObjectOutputTypeDef = TypedDict(
+    "RestoreObjectOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "RestoreOutputPath": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4199,25 +4199,25 @@
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
-StatsOutputTypeDef = TypedDict(
-    "StatsOutputTypeDef",
+StatsTypeDef = TypedDict(
+    "StatsTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
-UploadPartOutputOutputTypeDef = TypedDict(
-    "UploadPartOutputOutputTypeDef",
+UploadPartOutputTypeDef = TypedDict(
+    "UploadPartOutputTypeDef",
     {
         "ServerSideEncryption": ServerSideEncryptionType,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -4368,24 +4368,24 @@
     "AnalyticsAndOperatorOutputTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetBucketTaggingOutputOutputTypeDef = TypedDict(
-    "GetBucketTaggingOutputOutputTypeDef",
+GetBucketTaggingOutputTypeDef = TypedDict(
+    "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectTaggingOutputOutputTypeDef = TypedDict(
-    "GetObjectTaggingOutputOutputTypeDef",
+GetObjectTaggingOutputTypeDef = TypedDict(
+    "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -4692,53 +4692,53 @@
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
-GetBucketCorsOutputOutputTypeDef = TypedDict(
-    "GetBucketCorsOutputOutputTypeDef",
+GetBucketCorsOutputTypeDef = TypedDict(
+    "GetBucketCorsOutputTypeDef",
     {
         "CORSRules": List[CORSRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
     },
     total=False,
 )
 
-CopyObjectOutputOutputTypeDef = TypedDict(
-    "CopyObjectOutputOutputTypeDef",
+CopyObjectOutputTypeDef = TypedDict(
+    "CopyObjectOutputTypeDef",
     {
-        "CopyObjectResult": CopyObjectResultOutputTypeDef,
+        "CopyObjectResult": CopyObjectResultTypeDef,
         "Expiration": str,
         "CopySourceVersionId": str,
         "VersionId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadPartCopyOutputOutputTypeDef = TypedDict(
-    "UploadPartCopyOutputOutputTypeDef",
+UploadPartCopyOutputTypeDef = TypedDict(
+    "UploadPartCopyOutputTypeDef",
     {
         "CopySourceVersionId": str,
-        "CopyPartResult": CopyPartResultOutputTypeDef,
+        "CopyPartResult": CopyPartResultTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4827,40 +4827,40 @@
     "ObjectLockRuleTypeDef",
     {
         "DefaultRetention": DefaultRetentionTypeDef,
     },
     total=False,
 )
 
-DeleteMarkerEntryOutputTypeDef = TypedDict(
-    "DeleteMarkerEntryOutputTypeDef",
+DeleteMarkerEntryTypeDef = TypedDict(
+    "DeleteMarkerEntryTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
     },
 )
 
-ListBucketsOutputOutputTypeDef = TypedDict(
-    "ListBucketsOutputOutputTypeDef",
+ListBucketsOutputTypeDef = TypedDict(
+    "ListBucketsOutputTypeDef",
     {
-        "Buckets": List[BucketOutputTypeDef],
+        "Buckets": List[BucketTypeDef],
         "Owner": OwnerOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteObjectsOutputOutputTypeDef = TypedDict(
-    "DeleteObjectsOutputOutputTypeDef",
+DeleteObjectsOutputTypeDef = TypedDict(
+    "DeleteObjectsOutputTypeDef",
     {
-        "Deleted": List[DeletedObjectOutputTypeDef],
+        "Deleted": List[DeletedObjectTypeDef],
         "RequestCharged": Literal["requester"],
-        "Errors": List[ErrorOutputTypeDef],
+        "Errors": List[ErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
@@ -4889,52 +4889,52 @@
     "S3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
-GetBucketPolicyStatusOutputOutputTypeDef = TypedDict(
-    "GetBucketPolicyStatusOutputOutputTypeDef",
+GetBucketPolicyStatusOutputTypeDef = TypedDict(
+    "GetBucketPolicyStatusOutputTypeDef",
     {
-        "PolicyStatus": PolicyStatusOutputTypeDef,
+        "PolicyStatus": PolicyStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAttributesPartsOutputTypeDef = TypedDict(
-    "GetObjectAttributesPartsOutputTypeDef",
+GetObjectAttributesPartsTypeDef = TypedDict(
+    "GetObjectAttributesPartsTypeDef",
     {
         "TotalPartsCount": int,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[ObjectPartOutputTypeDef],
+        "Parts": List[ObjectPartTypeDef],
     },
 )
 
-GetObjectLegalHoldOutputOutputTypeDef = TypedDict(
-    "GetObjectLegalHoldOutputOutputTypeDef",
+GetObjectLegalHoldOutputTypeDef = TypedDict(
+    "GetObjectLegalHoldOutputTypeDef",
     {
         "LegalHold": ObjectLockLegalHoldOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectRetentionOutputOutputTypeDef = TypedDict(
-    "GetObjectRetentionOutputOutputTypeDef",
+GetObjectRetentionOutputTypeDef = TypedDict(
+    "GetObjectRetentionOutputTypeDef",
     {
         "Retention": ObjectLockRetentionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPublicAccessBlockOutputOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputOutputTypeDef",
+GetPublicAccessBlockOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GrantOutputTypeDef = TypedDict(
@@ -5077,23 +5077,23 @@
 
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
-MultipartUploadOutputTypeDef = TypedDict(
-    "MultipartUploadOutputTypeDef",
+MultipartUploadTypeDef = TypedDict(
+    "MultipartUploadTypeDef",
     {
         "UploadId": str,
         "Key": str,
         "Initiated": datetime,
         "StorageClass": StorageClassType,
         "Owner": OwnerOutputTypeDef,
-        "Initiator": InitiatorOutputTypeDef,
+        "Initiator": InitiatorTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
@@ -5164,28 +5164,28 @@
     },
     total=False,
 )
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-ListPartsOutputOutputTypeDef = TypedDict(
-    "ListPartsOutputOutputTypeDef",
+ListPartsOutputTypeDef = TypedDict(
+    "ListPartsOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[PartOutputTypeDef],
-        "Initiator": InitiatorOutputTypeDef,
+        "Parts": List[PartTypeDef],
+        "Initiator": InitiatorTypeDef,
         "Owner": OwnerOutputTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5227,16 +5227,16 @@
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
-NotificationConfigurationDeprecatedOutputTypeDef = TypedDict(
-    "NotificationConfigurationDeprecatedOutputTypeDef",
+NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
+    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5300,41 +5300,41 @@
 
 class PutObjectRetentionRequestRequestTypeDef(
     _RequiredPutObjectRetentionRequestRequestTypeDef,
     _OptionalPutObjectRetentionRequestRequestTypeDef,
 ):
     pass
 
-ObjectOutputTypeDef = TypedDict(
-    "ObjectOutputTypeDef",
+ObjectTypeDef = TypedDict(
+    "ObjectTypeDef",
     {
         "Key": str,
         "LastModified": datetime,
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": ObjectStorageClassType,
         "Owner": OwnerOutputTypeDef,
-        "RestoreStatus": RestoreStatusOutputTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
     },
 )
 
-ObjectVersionOutputTypeDef = TypedDict(
-    "ObjectVersionOutputTypeDef",
+ObjectVersionTypeDef = TypedDict(
+    "ObjectVersionTypeDef",
     {
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": Literal["STANDARD"],
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
         "Owner": OwnerOutputTypeDef,
-        "RestoreStatus": RestoreStatusOutputTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
     },
 )
 
 OwnershipControlsOutputTypeDef = TypedDict(
     "OwnershipControlsOutputTypeDef",
     {
         "Rules": List[OwnershipControlsRuleOutputTypeDef],
@@ -5344,18 +5344,18 @@
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
         "Rules": Sequence[OwnershipControlsRuleTypeDef],
     },
 )
 
-ProgressEventOutputTypeDef = TypedDict(
-    "ProgressEventOutputTypeDef",
+ProgressEventTypeDef = TypedDict(
+    "ProgressEventTypeDef",
     {
-        "Details": ProgressOutputTypeDef,
+        "Details": ProgressTypeDef,
     },
 )
 
 _RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -5521,18 +5521,18 @@
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
     total=False,
 )
 
-StatsEventOutputTypeDef = TypedDict(
-    "StatsEventOutputTypeDef",
+StatsEventTypeDef = TypedDict(
+    "StatsEventTypeDef",
     {
-        "Details": StatsOutputTypeDef,
+        "Details": StatsTypeDef,
     },
 )
 
 AnalyticsFilterOutputTypeDef = TypedDict(
     "AnalyticsFilterOutputTypeDef",
     {
         "Prefix": str,
@@ -5882,41 +5882,41 @@
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": S3KeyFilterTypeDef,
     },
     total=False,
 )
 
-GetObjectAttributesOutputOutputTypeDef = TypedDict(
-    "GetObjectAttributesOutputOutputTypeDef",
+GetObjectAttributesOutputTypeDef = TypedDict(
+    "GetObjectAttributesOutputTypeDef",
     {
         "DeleteMarker": bool,
         "LastModified": datetime,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
-        "Checksum": ChecksumOutputTypeDef,
-        "ObjectParts": GetObjectAttributesPartsOutputTypeDef,
+        "Checksum": ChecksumTypeDef,
+        "ObjectParts": GetObjectAttributesPartsTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketAclOutputOutputTypeDef = TypedDict(
-    "GetBucketAclOutputOutputTypeDef",
+GetBucketAclOutputTypeDef = TypedDict(
+    "GetBucketAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAclOutputOutputTypeDef = TypedDict(
-    "GetObjectAclOutputOutputTypeDef",
+GetObjectAclOutputTypeDef = TypedDict(
+    "GetObjectAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5986,28 +5986,28 @@
     },
     total=False,
 )
 
 class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
     pass
 
-ListMultipartUploadsOutputOutputTypeDef = TypedDict(
-    "ListMultipartUploadsOutputOutputTypeDef",
+ListMultipartUploadsOutputTypeDef = TypedDict(
+    "ListMultipartUploadsOutputTypeDef",
     {
         "Bucket": str,
         "KeyMarker": str,
         "UploadIdMarker": str,
         "NextKeyMarker": str,
         "Prefix": str,
         "Delimiter": str,
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
-        "Uploads": List[MultipartUploadOutputTypeDef],
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "Uploads": List[MultipartUploadTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InventoryS3BucketDestinationOutputTypeDef = TypedDict(
@@ -6079,16 +6079,16 @@
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
-GetBucketLifecycleOutputOutputTypeDef = TypedDict(
-    "GetBucketLifecycleOutputOutputTypeDef",
+GetBucketLifecycleOutputTypeDef = TypedDict(
+    "GetBucketLifecycleOutputTypeDef",
     {
         "Rules": List[RuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
@@ -6151,75 +6151,75 @@
 
 class PutBucketNotificationRequestRequestTypeDef(
     _RequiredPutBucketNotificationRequestRequestTypeDef,
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
-ListObjectsOutputOutputTypeDef = TypedDict(
-    "ListObjectsOutputOutputTypeDef",
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
-        "Contents": List[ObjectOutputTypeDef],
+        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectsV2OutputOutputTypeDef = TypedDict(
-    "ListObjectsV2OutputOutputTypeDef",
+ListObjectsV2OutputTypeDef = TypedDict(
+    "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
-        "Contents": List[ObjectOutputTypeDef],
+        "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectVersionsOutputOutputTypeDef = TypedDict(
-    "ListObjectVersionsOutputOutputTypeDef",
+ListObjectVersionsOutputTypeDef = TypedDict(
+    "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
         "KeyMarker": str,
         "VersionIdMarker": str,
         "NextKeyMarker": str,
         "NextVersionIdMarker": str,
-        "Versions": List[ObjectVersionOutputTypeDef],
-        "DeleteMarkers": List[DeleteMarkerEntryOutputTypeDef],
+        "Versions": List[ObjectVersionTypeDef],
+        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketOwnershipControlsOutputOutputTypeDef = TypedDict(
-    "GetBucketOwnershipControlsOutputOutputTypeDef",
+GetBucketOwnershipControlsOutputTypeDef = TypedDict(
+    "GetBucketOwnershipControlsOutputTypeDef",
     {
         "OwnershipControls": OwnershipControlsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
@@ -6240,16 +6240,16 @@
 
 class PutBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredPutBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalPutBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-GetBucketWebsiteOutputOutputTypeDef = TypedDict(
-    "GetBucketWebsiteOutputOutputTypeDef",
+GetBucketWebsiteOutputTypeDef = TypedDict(
+    "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToOutputTypeDef,
         "IndexDocument": IndexDocumentOutputTypeDef,
         "ErrorDocument": ErrorDocumentOutputTypeDef,
         "RoutingRules": List[RoutingRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6276,20 +6276,20 @@
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
     },
 )
 
-SelectObjectContentEventStreamOutputTypeDef = TypedDict(
-    "SelectObjectContentEventStreamOutputTypeDef",
+SelectObjectContentEventStreamTypeDef = TypedDict(
+    "SelectObjectContentEventStreamTypeDef",
     {
-        "Records": RecordsEventOutputTypeDef,
-        "Stats": StatsEventOutputTypeDef,
-        "Progress": ProgressEventOutputTypeDef,
+        "Records": RecordsEventTypeDef,
+        "Stats": StatsEventTypeDef,
+        "Progress": ProgressEventTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
 )
 
 IntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "IntelligentTieringConfigurationOutputTypeDef",
@@ -6399,16 +6399,16 @@
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
     total=False,
 )
 
-GetObjectLockConfigurationOutputOutputTypeDef = TypedDict(
-    "GetObjectLockConfigurationOutputOutputTypeDef",
+GetObjectLockConfigurationOutputTypeDef = TypedDict(
+    "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
@@ -6525,16 +6525,16 @@
 )
 
 class TopicConfigurationTypeDef(
     _RequiredTopicConfigurationTypeDef, _OptionalTopicConfigurationTypeDef
 ):
     pass
 
-GetBucketLoggingOutputOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputOutputTypeDef",
+GetBucketLoggingOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputTypeDef",
     {
         "LoggingEnabled": LoggingEnabledOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
@@ -6767,16 +6767,16 @@
 )
 
 class PutBucketWebsiteRequestRequestTypeDef(
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
-GetBucketEncryptionOutputOutputTypeDef = TypedDict(
-    "GetBucketEncryptionOutputOutputTypeDef",
+GetBucketEncryptionOutputTypeDef = TypedDict(
+    "GetBucketEncryptionOutputTypeDef",
     {
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
@@ -6798,59 +6798,59 @@
 
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
-SelectObjectContentOutputOutputTypeDef = TypedDict(
-    "SelectObjectContentOutputOutputTypeDef",
+SelectObjectContentOutputTypeDef = TypedDict(
+    "SelectObjectContentOutputTypeDef",
     {
-        "Payload": "EventStream[SelectObjectContentEventStreamOutputTypeDef]",
+        "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketIntelligentTieringConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
+GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
+    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
+ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketLifecycleConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
+GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputTypeDef",
     {
         "Rules": List[LifecycleRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketMetricsConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketMetricsConfigurationOutputOutputTypeDef",
+GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
+    "GetBucketMetricsConfigurationOutputTypeDef",
     {
         "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketMetricsConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
+ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6919,16 +6919,16 @@
 )
 
 class AnalyticsConfigurationTypeDef(
     _RequiredAnalyticsConfigurationTypeDef, _OptionalAnalyticsConfigurationTypeDef
 ):
     pass
 
-NotificationConfigurationOutputTypeDef = TypedDict(
-    "NotificationConfigurationOutputTypeDef",
+NotificationConfigurationResponseMetadataTypeDef = TypedDict(
+    "NotificationConfigurationResponseMetadataTypeDef",
     {
         "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
         "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
         "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7082,24 +7082,24 @@
 
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketAnalyticsConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
+GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
         "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketAnalyticsConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
+ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7214,24 +7214,24 @@
 )
 
 class RestoreObjectRequestRequestTypeDef(
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
-GetBucketInventoryConfigurationOutputOutputTypeDef = TypedDict(
-    "GetBucketInventoryConfigurationOutputOutputTypeDef",
+GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
+    "GetBucketInventoryConfigurationOutputTypeDef",
     {
         "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketInventoryConfigurationsOutputOutputTypeDef = TypedDict(
-    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
+ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
+    "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
         "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7255,16 +7255,16 @@
 
 class PutBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketReplicationOutputOutputTypeDef = TypedDict(
-    "GetBucketReplicationOutputOutputTypeDef",
+GetBucketReplicationOutputTypeDef = TypedDict(
+    "GetBucketReplicationOutputTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.py` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.pyi` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/PKG-INFO` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -553,55 +553,55 @@
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputOutputTypeDef,
+    AbortMultipartUploadOutputTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
     TagOutputTypeDef,
     TagTypeDef,
     AnalyticsS3BucketDestinationOutputTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
     CopySourceTypeDef,
     BucketDownloadFileRequestTypeDef,
     BucketDownloadFileobjRequestTypeDef,
-    BucketOutputTypeDef,
+    BucketTypeDef,
     BucketUploadFileRequestTypeDef,
     BucketUploadFileobjRequestTypeDef,
     CORSRuleTypeDef,
     CORSRuleOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
-    ChecksumOutputTypeDef,
+    ChecksumTypeDef,
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
-    CommonPrefixOutputTypeDef,
-    CompleteMultipartUploadOutputOutputTypeDef,
+    CommonPrefixTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionOutputTypeDef,
     ConditionTypeDef,
-    CopyObjectResultOutputTypeDef,
+    CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
-    CopyPartResultOutputTypeDef,
+    CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputOutputTypeDef,
-    CreateMultipartUploadOutputOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
@@ -622,95 +622,95 @@
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     OwnerOutputTypeDef,
     DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
-    DeletedObjectOutputTypeDef,
-    ErrorOutputTypeDef,
+    DeletedObjectTypeDef,
+    ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     ErrorDocumentOutputTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    PolicyStatusOutputTypeDef,
+    PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentOutputTypeDef,
     RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
-    ObjectPartOutputTypeDef,
+    ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputOutputTypeDef,
+    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputOutputTypeDef,
+    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     IndexDocumentTypeDef,
-    InitiatorOutputTypeDef,
     InitiatorResponseMetadataTypeDef,
+    InitiatorTypeDef,
     JSONInputTypeDef,
     TieringOutputTypeDef,
     TieringTypeDef,
     InventoryFilterOutputTypeDef,
     InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
@@ -733,78 +733,78 @@
     ListMultipartUploadsRequestRequestTypeDef,
     ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
     ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
     ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
-    PartOutputTypeDef,
+    PartTypeDef,
     ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedOutputTypeDef,
     TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
-    RestoreStatusOutputTypeDef,
+    RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
     OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
     PaginatorConfigTypeDef,
-    ProgressOutputTypeDef,
+    ProgressTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputOutputTypeDef,
-    PutObjectLegalHoldOutputOutputTypeDef,
-    PutObjectLockConfigurationOutputOutputTypeDef,
-    PutObjectOutputOutputTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputOutputTypeDef,
-    PutObjectTaggingOutputOutputTypeDef,
-    RecordsEventOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RecordsEventTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectAllRequestsToTypeDef,
     RedirectOutputTypeDef,
     RedirectTypeDef,
     ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
     ResponseMetadataTypeDef,
-    RestoreObjectOutputOutputTypeDef,
+    RestoreObjectOutputTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StatsOutputTypeDef,
-    UploadPartOutputOutputTypeDef,
+    StatsTypeDef,
+    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     AnalyticsAndOperatorOutputTypeDef,
-    GetBucketTaggingOutputOutputTypeDef,
-    GetObjectTaggingOutputOutputTypeDef,
+    GetBucketTaggingOutputTypeDef,
+    GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorOutputTypeDef,
     MetricsAndOperatorOutputTypeDef,
     ReplicationRuleAndOperatorOutputTypeDef,
     AnalyticsAndOperatorTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
@@ -816,75 +816,75 @@
     BucketCopyRequestTypeDef,
     ClientCopyRequestTypeDef,
     CopyObjectRequestRequestTypeDef,
     ObjectCopyRequestTypeDef,
     UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     UploadPartCopyRequestRequestTypeDef,
     CORSConfigurationTypeDef,
-    GetBucketCorsOutputOutputTypeDef,
+    GetBucketCorsOutputTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputOutputTypeDef,
-    UploadPartCopyOutputOutputTypeDef,
+    CopyObjectOutputTypeDef,
+    UploadPartCopyOutputTypeDef,
     CreateBucketRequestBucketCreateTypeDef,
     CreateBucketRequestRequestTypeDef,
     CreateBucketRequestServiceResourceCreateBucketTypeDef,
     ObjectLockRuleOutputTypeDef,
     ObjectLockRuleTypeDef,
-    DeleteMarkerEntryOutputTypeDef,
-    ListBucketsOutputOutputTypeDef,
-    DeleteObjectsOutputOutputTypeDef,
+    DeleteMarkerEntryTypeDef,
+    ListBucketsOutputTypeDef,
+    DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     S3KeyFilterOutputTypeDef,
     S3KeyFilterTypeDef,
-    GetBucketPolicyStatusOutputOutputTypeDef,
-    GetObjectAttributesPartsOutputTypeDef,
-    GetObjectLegalHoldOutputOutputTypeDef,
-    GetObjectRetentionOutputOutputTypeDef,
-    GetPublicAccessBlockOutputOutputTypeDef,
+    GetBucketPolicyStatusOutputTypeDef,
+    GetObjectAttributesPartsTypeDef,
+    GetObjectLegalHoldOutputTypeDef,
+    GetObjectRetentionOutputTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
     GrantOutputTypeDef,
     TargetGrantOutputTypeDef,
     GrantTypeDef,
     TargetGrantTypeDef,
     HeadBucketRequestBucketExistsWaitTypeDef,
     HeadBucketRequestBucketNotExistsWaitTypeDef,
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
-    MultipartUploadOutputTypeDef,
+    MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
-    ListPartsOutputOutputTypeDef,
+    ListPartsOutputTypeDef,
     MetricsOutputTypeDef,
     ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
-    NotificationConfigurationDeprecatedOutputTypeDef,
+    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     PutObjectLegalHoldRequestRequestTypeDef,
     PutObjectRetentionRequestRequestTypeDef,
-    ObjectOutputTypeDef,
-    ObjectVersionOutputTypeDef,
+    ObjectTypeDef,
+    ObjectVersionTypeDef,
     OwnershipControlsOutputTypeDef,
     OwnershipControlsTypeDef,
-    ProgressEventOutputTypeDef,
+    ProgressEventTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
     PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     PutBucketRequestPaymentRequestRequestTypeDef,
     PutBucketVersioningRequestBucketVersioningPutTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
     RoutingRuleOutputTypeDef,
     RoutingRuleTypeDef,
     ServerSideEncryptionRuleOutputTypeDef,
     ServerSideEncryptionRuleTypeDef,
     SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
-    StatsEventOutputTypeDef,
+    StatsEventTypeDef,
     AnalyticsFilterOutputTypeDef,
     IntelligentTieringFilterOutputTypeDef,
     LifecycleRuleFilterOutputTypeDef,
     MetricsFilterOutputTypeDef,
     ReplicationRuleFilterOutputTypeDef,
     AnalyticsFilterTypeDef,
     IntelligentTieringFilterTypeDef,
@@ -902,109 +902,109 @@
     CompleteMultipartUploadRequestRequestTypeDef,
     ObjectLockConfigurationOutputTypeDef,
     ObjectLockConfigurationTypeDef,
     DeleteObjectsRequestBucketDeleteObjectsTypeDef,
     DeleteObjectsRequestRequestTypeDef,
     NotificationConfigurationFilterOutputTypeDef,
     NotificationConfigurationFilterTypeDef,
-    GetObjectAttributesOutputOutputTypeDef,
-    GetBucketAclOutputOutputTypeDef,
-    GetObjectAclOutputOutputTypeDef,
+    GetObjectAttributesOutputTypeDef,
+    GetBucketAclOutputTypeDef,
+    GetObjectAclOutputTypeDef,
     LoggingEnabledOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     AccessControlPolicyTypeDef,
     S3LocationTypeDef,
     LoggingEnabledTypeDef,
-    ListMultipartUploadsOutputOutputTypeDef,
+    ListMultipartUploadsOutputTypeDef,
     InventoryS3BucketDestinationOutputTypeDef,
     InventoryS3BucketDestinationTypeDef,
     SelectObjectContentRequestRequestTypeDef,
     SelectParametersTypeDef,
-    GetBucketLifecycleOutputOutputTypeDef,
+    GetBucketLifecycleOutputTypeDef,
     LifecycleConfigurationTypeDef,
     DestinationOutputTypeDef,
     DestinationTypeDef,
     PutBucketNotificationRequestRequestTypeDef,
-    ListObjectsOutputOutputTypeDef,
-    ListObjectsV2OutputOutputTypeDef,
-    ListObjectVersionsOutputOutputTypeDef,
-    GetBucketOwnershipControlsOutputOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListObjectsV2OutputTypeDef,
+    ListObjectVersionsOutputTypeDef,
+    GetBucketOwnershipControlsOutputTypeDef,
     PutBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketWebsiteOutputOutputTypeDef,
+    GetBucketWebsiteOutputTypeDef,
     WebsiteConfigurationTypeDef,
     ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SelectObjectContentEventStreamOutputTypeDef,
+    SelectObjectContentEventStreamTypeDef,
     IntelligentTieringConfigurationOutputTypeDef,
     LifecycleRuleOutputTypeDef,
     MetricsConfigurationOutputTypeDef,
     IntelligentTieringConfigurationTypeDef,
     LifecycleRuleTypeDef,
     MetricsConfigurationTypeDef,
     StorageClassAnalysisOutputTypeDef,
     StorageClassAnalysisTypeDef,
-    GetObjectLockConfigurationOutputOutputTypeDef,
+    GetObjectLockConfigurationOutputTypeDef,
     PutObjectLockConfigurationRequestRequestTypeDef,
     LambdaFunctionConfigurationOutputTypeDef,
     QueueConfigurationOutputTypeDef,
     TopicConfigurationOutputTypeDef,
     LambdaFunctionConfigurationTypeDef,
     QueueConfigurationTypeDef,
     TopicConfigurationTypeDef,
-    GetBucketLoggingOutputOutputTypeDef,
+    GetBucketLoggingOutputTypeDef,
     PutBucketAclRequestBucketAclPutTypeDef,
     PutBucketAclRequestRequestTypeDef,
     PutObjectAclRequestObjectAclPutTypeDef,
     PutObjectAclRequestRequestTypeDef,
     OutputLocationTypeDef,
     BucketLoggingStatusTypeDef,
     InventoryDestinationOutputTypeDef,
     InventoryDestinationTypeDef,
     PutBucketLifecycleRequestBucketLifecyclePutTypeDef,
     PutBucketLifecycleRequestRequestTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     PutBucketWebsiteRequestBucketWebsitePutTypeDef,
     PutBucketWebsiteRequestRequestTypeDef,
-    GetBucketEncryptionOutputOutputTypeDef,
+    GetBucketEncryptionOutputTypeDef,
     PutBucketEncryptionRequestRequestTypeDef,
-    SelectObjectContentOutputOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputOutputTypeDef,
-    GetBucketMetricsConfigurationOutputOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputOutputTypeDef,
+    SelectObjectContentOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputTypeDef,
+    GetBucketMetricsConfigurationOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputTypeDef,
     PutBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     BucketLifecycleConfigurationTypeDef,
     PutBucketMetricsConfigurationRequestRequestTypeDef,
     AnalyticsConfigurationOutputTypeDef,
     AnalyticsConfigurationTypeDef,
-    NotificationConfigurationOutputTypeDef,
+    NotificationConfigurationResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     RestoreRequestTypeDef,
     PutBucketLoggingRequestBucketLoggingPutTypeDef,
     PutBucketLoggingRequestRequestTypeDef,
     InventoryConfigurationOutputTypeDef,
     InventoryConfigurationTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
-    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
-    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputTypeDef,
     PutBucketAnalyticsConfigurationRequestRequestTypeDef,
     PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     PutBucketNotificationConfigurationRequestRequestTypeDef,
     RestoreObjectRequestObjectRestoreObjectTypeDef,
     RestoreObjectRequestObjectSummaryRestoreObjectTypeDef,
     RestoreObjectRequestRequestTypeDef,
-    GetBucketInventoryConfigurationOutputOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputOutputTypeDef,
+    GetBucketInventoryConfigurationOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputTypeDef,
     PutBucketInventoryConfigurationRequestRequestTypeDef,
-    GetBucketReplicationOutputOutputTypeDef,
+    GetBucketReplicationOutputTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/SOURCES.txt` & `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post1/setup.py` & `mypy-boto3-s3-1.28.3.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.7"
+        "Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

