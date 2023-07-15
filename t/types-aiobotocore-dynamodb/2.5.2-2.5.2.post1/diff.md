# Comparing `tmp/types-aiobotocore-dynamodb-2.5.2.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.tar", last modified: Sat Jul  8 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post1.tar", last modified: Sat Jul 15 06:45:02 2023, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.5.2.tar` & `types-aiobotocore-dynamodb-2.5.2.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26764 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.070045 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56380 2023-07-08 01:29:09.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56311 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-07-08 01:29:09.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   152204 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   152051 2023-07-08 01:29:12.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-15 06:32:45.000000 types-aiobotocore-dynamodb-2.5.2.post1/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29459 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27884 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-07-15 06:44:52.000000 types-aiobotocore-dynamodb-2.5.2.post1/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1813 2023-07-15 06:32:46.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1812 2023-07-15 06:32:46.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    56380 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    56311 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12866 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12864 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8705 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8698 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:32:46.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28868 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28840 2023-07-15 06:44:54.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   151413 2023-07-15 06:44:58.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   151276 2023-07-15 06:44:56.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-07-15 06:44:53.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2442 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2440 2023-07-15 06:32:48.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-15 06:45:02.797319 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29459 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1002 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-07-15 06:45:02.000000 types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/LICENSE` & `types-aiobotocore-dynamodb-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -48,15 +48,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -457,31 +457,35 @@
 ### Typed dictionaries
 
 `types_aiobotocore_dynamodb.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodb.type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
+    AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
+    AttributeValueServiceResourceTypeDef,
+    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
+    KeysAndAttributesServiceResourceOutputTypeDef,
     BatchStatementErrorTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -501,173 +505,197 @@
     StreamSpecificationTypeDef,
     TagTypeDef,
     KeySchemaElementServiceResourceTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     SSESpecificationServiceResourceTypeDef,
     StreamSpecificationServiceResourceTypeDef,
     TagServiceResourceTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
     DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
     ExpectedAttributeValueTableTypeDef,
     ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
     DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
+    DeleteRequestServiceResourceOutputTypeDef,
     DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
+    KeySchemaElementTableOutputTypeDef,
+    ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
+    KeySchemaElementOutputTypeDef,
+    ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
+    ReplicaOutputTypeDef,
+    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputOverrideOutputTypeDef,
+    ProvisionedThroughputOverrideTableOutputTypeDef,
+    PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
+    SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
+    StreamSpecificationOutputTypeDef,
+    StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
-    TableBatchWriterRequestTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
+    DeleteRequestOutputTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
     GetItemInputRequestTypeDef,
     GetTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
+    KeysAndAttributesOutputTypeDef,
     KeysAndAttributesTypeDef,
     ParameterizedStatementTypeDef,
+    PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     BatchStatementResponseTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
-    LocalSecondaryIndexInfoTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexTypeDef,
-    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    GlobalTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     ReplicaGlobalSecondaryIndexTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
     DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputTablePutItemTypeDef,
     UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
+    SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
+    GlobalTableTypeDef,
     ImportSummaryTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
+    WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    UpdateTimeToLiveInputRequestTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
     ExecuteTransactionInputRequestTypeDef,
+    WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
@@ -686,81 +714,82 @@
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     CreateTableInputRequestTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    ListGlobalTablesOutputTypeDef,
-    ReplicaDescriptionTableTypeDef,
     CreateReplicationGroupMemberActionTableTypeDef,
     UpdateReplicationGroupMemberActionTableTypeDef,
-    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
+    SourceTableFeatureDetailsTypeDef,
+    TableCreationParametersOutputTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicaDescriptionTableTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     ImportTableInputRequestTypeDef,
-    TableDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    BackupDescriptionTypeDef,
+    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    ReplicationGroupUpdateTypeDef,
+    TableDescriptionTableTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    UpdateTableInputRequestTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    UpdateTableInputRequestTypeDef,
+    DeleteTableOutputTableTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/README.md` & `types-aiobotocore-dynamodb-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -424,31 +424,35 @@
 ### Typed dictionaries
 
 `types_aiobotocore_dynamodb.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodb.type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
+    AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
+    AttributeValueServiceResourceTypeDef,
+    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
+    KeysAndAttributesServiceResourceOutputTypeDef,
     BatchStatementErrorTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -468,173 +472,197 @@
     StreamSpecificationTypeDef,
     TagTypeDef,
     KeySchemaElementServiceResourceTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     SSESpecificationServiceResourceTypeDef,
     StreamSpecificationServiceResourceTypeDef,
     TagServiceResourceTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
     DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
     ExpectedAttributeValueTableTypeDef,
     ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
     DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
+    DeleteRequestServiceResourceOutputTypeDef,
     DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
+    KeySchemaElementTableOutputTypeDef,
+    ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
+    KeySchemaElementOutputTypeDef,
+    ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
+    ReplicaOutputTypeDef,
+    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputOverrideOutputTypeDef,
+    ProvisionedThroughputOverrideTableOutputTypeDef,
+    PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
+    SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
+    StreamSpecificationOutputTypeDef,
+    StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
-    TableBatchWriterRequestTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
+    DeleteRequestOutputTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
     GetItemInputRequestTypeDef,
     GetTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
+    KeysAndAttributesOutputTypeDef,
     KeysAndAttributesTypeDef,
     ParameterizedStatementTypeDef,
+    PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     BatchStatementResponseTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
-    LocalSecondaryIndexInfoTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexTypeDef,
-    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    GlobalTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     ReplicaGlobalSecondaryIndexTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
     DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputTablePutItemTypeDef,
     UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
+    SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
+    GlobalTableTypeDef,
     ImportSummaryTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
+    WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    UpdateTimeToLiveInputRequestTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
     ExecuteTransactionInputRequestTypeDef,
+    WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
@@ -653,81 +681,82 @@
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     CreateTableInputRequestTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    ListGlobalTablesOutputTypeDef,
-    ReplicaDescriptionTableTypeDef,
     CreateReplicationGroupMemberActionTableTypeDef,
     UpdateReplicationGroupMemberActionTableTypeDef,
-    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
+    SourceTableFeatureDetailsTypeDef,
+    TableCreationParametersOutputTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicaDescriptionTableTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     ImportTableInputRequestTypeDef,
-    TableDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    BackupDescriptionTypeDef,
+    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    ReplicationGroupUpdateTypeDef,
+    TableDescriptionTableTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    UpdateTableInputRequestTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    UpdateTableInputRequestTypeDef,
+    DeleteTableOutputTableTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/setup.py` & `types-aiobotocore-dynamodb-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        " 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2")
+    print("2.5.2.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,45 +79,45 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
         """
 
 
 class ListTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
         """
 
 
 class ListTagsOfResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 
@@ -159,15 +159,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 
@@ -208,13 +208,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,43 +76,43 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
         """
 
 class ListTagsOfResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 class QueryPaginator(AioPaginator):
@@ -153,15 +153,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(AioPaginator):
@@ -201,13 +201,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,72 +30,73 @@
     ReturnItemCollectionMetricsType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeValueUpdateTableTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     ConditionTableTypeDef,
     DeleteItemOutputTableTypeDef,
     DeleteTableOutputTableTypeDef,
     ExpectedAttributeValueTableTypeDef,
     GetItemOutputTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableTypeDef,
+    KeySchemaElementTableOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     ProvisionedThroughputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ReplicaDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     ScanOutputTableTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSESpecificationServiceResourceTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationServiceResourceTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TagServiceResourceTypeDef,
     UpdateItemOutputTableTypeDef,
     WriteRequestServiceResourceTypeDef,
 )
 
 try:
+    from aioboto3.dynamodb.table import CustomTableResource
+except (ModuleNotFoundError, ImportError):
+    from builtins import object as CustomTableResource
+try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
     from aioboto3.resources.collection import AIOResourceCollection
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOResourceCollection
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 try:
-    from boto3.dynamodb.table import BatchWriter
-except (ModuleNotFoundError, ImportError):
-    from builtins import object as BatchWriter
-try:
     from boto3.resources.base import ResourceMeta
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ResourceMeta
 
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
@@ -161,53 +162,45 @@
         A generator which yields Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#serviceresourcetablescollection)
         """
 
 
-class Table(AIOBoto3ServiceResource):
+class Table(AIOBoto3ServiceResource, CustomTableResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: Awaitable[List[AttributeDefinitionTableTypeDef]]
+    attribute_definitions: Awaitable[List[AttributeDefinitionTableOutputTypeDef]]
     table_name: Awaitable[str]
-    key_schema: Awaitable[List[KeySchemaElementTableTypeDef]]
+    key_schema: Awaitable[List[KeySchemaElementTableOutputTypeDef]]
     table_status: Awaitable[TableStatusType]
     creation_date_time: Awaitable[datetime]
-    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionResponseMetadataTypeDef]
+    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionTableResponseMetadataTypeDef]
     table_size_bytes: Awaitable[int]
     item_count: Awaitable[int]
     table_arn: Awaitable[str]
     table_id: Awaitable[str]
-    billing_mode_summary: Awaitable[BillingModeSummaryResponseMetadataTypeDef]
+    billing_mode_summary: Awaitable[BillingModeSummaryTableResponseMetadataTypeDef]
     local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTableTypeDef]]
     global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTableTypeDef]]
-    stream_specification: Awaitable[StreamSpecificationResponseMetadataTypeDef]
+    stream_specification: Awaitable[StreamSpecificationTableResponseMetadataTypeDef]
     latest_stream_label: Awaitable[str]
     latest_stream_arn: Awaitable[str]
     global_table_version: Awaitable[str]
     replicas: Awaitable[List[ReplicaDescriptionTableTypeDef]]
-    restore_summary: Awaitable[RestoreSummaryResponseMetadataTypeDef]
-    sse_description: Awaitable[SSEDescriptionResponseMetadataTypeDef]
-    archival_summary: Awaitable[ArchivalSummaryResponseMetadataTypeDef]
-    table_class_summary: Awaitable[TableClassSummaryResponseMetadataTypeDef]
+    restore_summary: Awaitable[RestoreSummaryTableResponseMetadataTypeDef]
+    sse_description: Awaitable[SSEDescriptionTableResponseMetadataTypeDef]
+    archival_summary: Awaitable[ArchivalSummaryTableResponseMetadataTypeDef]
+    table_class_summary: Awaitable[TableClassSummaryTableResponseMetadataTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
 
-    async def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
-        """
-        Create a batch writer object.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
-        """
-
     async def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,72 +30,73 @@
     ReturnItemCollectionMetricsType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeValueUpdateTableTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
     ConditionTableTypeDef,
     DeleteItemOutputTableTypeDef,
     DeleteTableOutputTableTypeDef,
     ExpectedAttributeValueTableTypeDef,
     GetItemOutputTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
     KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableTypeDef,
+    KeySchemaElementTableOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     ProvisionedThroughputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ReplicaDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
     ScanOutputTableTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
     SSESpecificationServiceResourceTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationServiceResourceTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     TagServiceResourceTypeDef,
     UpdateItemOutputTableTypeDef,
     WriteRequestServiceResourceTypeDef,
 )
 
 try:
+    from aioboto3.dynamodb.table import CustomTableResource
+except (ModuleNotFoundError, ImportError):
+    from builtins import object as CustomTableResource
+try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
     from aioboto3.resources.collection import AIOResourceCollection
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOResourceCollection
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 try:
-    from boto3.dynamodb.table import BatchWriter
-except (ModuleNotFoundError, ImportError):
-    from builtins import object as BatchWriter
-try:
     from boto3.resources.base import ResourceMeta
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ResourceMeta
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
 class ServiceResourceTablesCollection(AIOResourceCollection):
@@ -152,52 +153,45 @@
         """
         A generator which yields Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#serviceresourcetablescollection)
         """
 
-class Table(AIOBoto3ServiceResource):
+class Table(AIOBoto3ServiceResource, CustomTableResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: Awaitable[List[AttributeDefinitionTableTypeDef]]
+    attribute_definitions: Awaitable[List[AttributeDefinitionTableOutputTypeDef]]
     table_name: Awaitable[str]
-    key_schema: Awaitable[List[KeySchemaElementTableTypeDef]]
+    key_schema: Awaitable[List[KeySchemaElementTableOutputTypeDef]]
     table_status: Awaitable[TableStatusType]
     creation_date_time: Awaitable[datetime]
-    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionResponseMetadataTypeDef]
+    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionTableResponseMetadataTypeDef]
     table_size_bytes: Awaitable[int]
     item_count: Awaitable[int]
     table_arn: Awaitable[str]
     table_id: Awaitable[str]
-    billing_mode_summary: Awaitable[BillingModeSummaryResponseMetadataTypeDef]
+    billing_mode_summary: Awaitable[BillingModeSummaryTableResponseMetadataTypeDef]
     local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTableTypeDef]]
     global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTableTypeDef]]
-    stream_specification: Awaitable[StreamSpecificationResponseMetadataTypeDef]
+    stream_specification: Awaitable[StreamSpecificationTableResponseMetadataTypeDef]
     latest_stream_label: Awaitable[str]
     latest_stream_arn: Awaitable[str]
     global_table_version: Awaitable[str]
     replicas: Awaitable[List[ReplicaDescriptionTableTypeDef]]
-    restore_summary: Awaitable[RestoreSummaryResponseMetadataTypeDef]
-    sse_description: Awaitable[SSEDescriptionResponseMetadataTypeDef]
-    archival_summary: Awaitable[ArchivalSummaryResponseMetadataTypeDef]
-    table_class_summary: Awaitable[TableClassSummaryResponseMetadataTypeDef]
+    restore_summary: Awaitable[RestoreSummaryTableResponseMetadataTypeDef]
+    sse_description: Awaitable[SSEDescriptionTableResponseMetadataTypeDef]
+    archival_summary: Awaitable[ArchivalSummaryTableResponseMetadataTypeDef]
+    table_class_summary: Awaitable[TableClassSummaryTableResponseMetadataTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
 
-    async def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
-        """
-        Create a batch writer object.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
-        """
     async def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef
+    from types_aiobotocore_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ArchivalSummaryResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -60,33 +60,36 @@
 else:
     from typing_extensions import TypedDict
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 
-
 __all__ = (
-    "ArchivalSummaryResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
+    "AttributeDefinitionOutputTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
+    "AttributeDefinitionTableOutputTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
+    "AttributeValueServiceResourceTypeDef",
+    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
+    "KeysAndAttributesServiceResourceOutputTypeDef",
     "BatchStatementErrorTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -106,173 +109,197 @@
     "StreamSpecificationTypeDef",
     "TagTypeDef",
     "KeySchemaElementServiceResourceTypeDef",
     "ProvisionedThroughputServiceResourceTypeDef",
     "SSESpecificationServiceResourceTypeDef",
     "StreamSpecificationServiceResourceTypeDef",
     "TagServiceResourceTypeDef",
+    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
     "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
     "ExpectedAttributeValueTableTypeDef",
     "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
     "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
+    "DeleteRequestServiceResourceOutputTypeDef",
     "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
+    "KeySchemaElementTableOutputTypeDef",
+    "ProjectionTableOutputTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
+    "KeySchemaElementOutputTypeDef",
+    "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
+    "ProvisionedThroughputOutputTypeDef",
     "ProjectionServiceResourceTypeDef",
+    "ReplicaOutputTypeDef",
+    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+    "ProvisionedThroughputOverrideOutputTypeDef",
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
+    "PutRequestServiceResourceOutputTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreSummaryResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
+    "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
-    "StreamSpecificationResponseMetadataTypeDef",
+    "StreamSpecificationOutputTypeDef",
+    "StreamSpecificationTableOutputTypeDef",
     "StreamSpecificationTableTypeDef",
-    "TableBatchWriterRequestTypeDef",
-    "TableClassSummaryResponseMetadataTypeDef",
+    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    "DescribeLimitsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    "TableClassSummaryTableResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
+    "DeleteRequestOutputTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "ExpectedAttributeValueTypeDef",
     "GetItemInputRequestTypeDef",
     "GetTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
+    "KeysAndAttributesOutputTypeDef",
     "KeysAndAttributesTypeDef",
     "ParameterizedStatementTypeDef",
+    "PutRequestOutputTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "BatchStatementResponseTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
-    "LocalSecondaryIndexDescriptionTypeDef",
-    "LocalSecondaryIndexInfoTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexTypeDef",
-    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "GlobalTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     "ReplicaGlobalSecondaryIndexTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
     "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "LocalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "LocalSecondaryIndexDescriptionTypeDef",
+    "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
+    "SourceTableDetailsTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
+    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    "WriteRequestServiceResourceOutputTypeDef",
     "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "UpdateTimeToLiveInputRequestTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
     "BatchGetItemInputRequestTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestOutputTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "GetItemOutputTableTypeDef",
@@ -291,117 +318,133 @@
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
     "GlobalSecondaryIndexUpdateTableTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "CreateTableInputRequestTypeDef",
     "RestoreTableFromBackupInputRequestTypeDef",
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "ListGlobalTablesOutputTypeDef",
-    "ReplicaDescriptionTableTypeDef",
     "CreateReplicationGroupMemberActionTableTypeDef",
     "UpdateReplicationGroupMemberActionTableTypeDef",
-    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
+    "TableCreationParametersOutputTypeDef",
     "CreateTableInputServiceResourceCreateTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
     "ListImportsOutputTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    "ReplicaDescriptionTypeDef",
+    "ReplicaDescriptionTableTypeDef",
     "BatchWriteItemOutputServiceResourceTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "ImportTableInputRequestTypeDef",
-    "TableDescriptionTableTypeDef",
     "ReplicationGroupUpdateTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "BackupDescriptionTypeDef",
+    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "ReplicationGroupUpdateTypeDef",
+    "TableDescriptionTableTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "UpdateTableInputRequestTypeDef",
     "DeleteBackupOutputTypeDef",
     "DescribeBackupOutputTypeDef",
     "DescribeImportOutputTypeDef",
     "ImportTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "UpdateTableInputRequestTypeDef",
+    "DeleteTableOutputTableTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ArchivalSummaryResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
+)
+
+AttributeDefinitionOutputTypeDef = TypedDict(
+    "AttributeDefinitionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
 )
 
 AttributeDefinitionServiceResourceTypeDef = TypedDict(
     "AttributeDefinitionServiceResourceTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeDefinitionTableOutputTypeDef = TypedDict(
+    "AttributeDefinitionTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
+)
+
 AttributeDefinitionTableTypeDef = TypedDict(
     "AttributeDefinitionTableTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
@@ -410,14 +453,46 @@
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeValueServiceResourceTypeDef = TypedDict(
+    "AttributeValueServiceResourceTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
+AttributeValueTableTypeDef = TypedDict(
+    "AttributeValueTableTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -451,38 +526,24 @@
             None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
+        "TargetValue": float,
     },
-    total=False,
 )
 
-
-class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
-    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-):
-    pass
-
-
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -491,61 +552,47 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
-
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-
-_RequiredBackupDetailsTypeDef = TypedDict(
-    "_RequiredBackupDetailsTypeDef",
+BackupDetailsTypeDef = TypedDict(
+    "BackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
+        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
-    },
-)
-_OptionalBackupDetailsTypeDef = TypedDict(
-    "_OptionalBackupDetailsTypeDef",
-    {
-        "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
-    total=False,
 )
 
-
-class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
-    pass
-
-
 BackupSummaryTableTypeDef = TypedDict(
     "BackupSummaryTableTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
@@ -554,15 +601,14 @@
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 _RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
     "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -594,113 +640,88 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
+KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "KeysAndAttributesServiceResourceOutputTypeDef",
+    {
+        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
+    },
+)
 
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
     },
-    total=False,
 )
 
 ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
     "ItemCollectionMetricsServiceResourceTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
-)
-
-BillingModeSummaryResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 CapacityServiceResourceTypeDef = TypedDict(
     "CapacityServiceResourceTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTableTypeDef = TypedDict(
     "CapacityTableTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 _RequiredConditionTableTypeDef = TypedDict(
     "_RequiredConditionTableTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -726,37 +747,33 @@
                 None,
             ]
         ],
     },
     total=False,
 )
 
-
 class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
-
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
-    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
-    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
@@ -771,15 +788,15 @@
     },
 )
 
 ProjectionTableTypeDef = TypedDict(
     "ProjectionTableTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
+        "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
 ProvisionedThroughputTableTypeDef = TypedDict(
     "ProvisionedThroughputTableTypeDef",
     {
@@ -864,21 +881,19 @@
     "_OptionalStreamSpecificationTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationTypeDef(
     _RequiredStreamSpecificationTypeDef, _OptionalStreamSpecificationTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -919,35 +934,41 @@
     "_OptionalStreamSpecificationServiceResourceTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationServiceResourceTypeDef(
     _RequiredStreamSpecificationServiceResourceTypeDef,
     _OptionalStreamSpecificationServiceResourceTypeDef,
 ):
     pass
 
-
 TagServiceResourceTypeDef = TypedDict(
     "TagServiceResourceTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CsvOptionsOutputTypeDef = TypedDict(
+    "CsvOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+        "HeaderList": List[str],
+    },
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
-        "HeaderList": List[str],
+        "HeaderList": Sequence[str],
     },
     total=False,
 )
 
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
@@ -1011,36 +1032,17 @@
     },
     total=False,
 )
 
 ItemCollectionMetricsTableTypeDef = TypedDict(
     "ItemCollectionMetricsTableTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
@@ -1056,14 +1058,21 @@
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
+DeleteRequestServiceResourceOutputTypeDef = TypedDict(
+    "DeleteRequestServiceResourceOutputTypeDef",
+    {
+        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
+    },
+)
+
 DeleteRequestServiceResourceTypeDef = TypedDict(
     "DeleteRequestServiceResourceTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1116,29 +1125,26 @@
     "_OptionalDescribeContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
-
 class DescribeContributorInsightsInputRequestTypeDef(
     _RequiredDescribeContributorInsightsInputRequestTypeDef,
     _OptionalDescribeContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1171,15 +1177,14 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
-    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1209,26 +1214,14 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
-    total=False,
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1259,31 +1252,22 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
-    total=False,
 )
 
 _RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
         "TableArn": str,
         "S3Bucket": str,
@@ -1299,22 +1283,20 @@
         "S3SseAlgorithm": S3SseAlgorithmType,
         "S3SseKmsKeyId": str,
         "ExportFormat": ExportFormatType,
     },
     total=False,
 )
 
-
 class ExportTableToPointInTimeInputRequestTypeDef(
     _RequiredExportTableToPointInTimeInputRequestTypeDef,
     _OptionalExportTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1343,54 +1325,106 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
+KeySchemaElementTableOutputTypeDef = TypedDict(
+    "KeySchemaElementTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionTableOutputTypeDef = TypedDict(
+    "ProjectionTableOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
+)
 
 ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTableTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+KeySchemaElementOutputTypeDef = TypedDict(
+    "KeySchemaElementOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionOutputTypeDef = TypedDict(
+    "ProjectionOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+ProvisionedThroughputOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+    },
 )
 
 ProjectionServiceResourceTypeDef = TypedDict(
     "ProjectionServiceResourceTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
+ReplicaOutputTypeDef = TypedDict(
+    "ReplicaOutputTypeDef",
+    {
+        "RegionName": str,
+    },
+)
+
+S3BucketSourceOutputTypeDef = TypedDict(
+    "S3BucketSourceOutputTypeDef",
+    {
+        "S3BucketOwner": str,
+        "S3Bucket": str,
+        "S3KeyPrefix": str,
+    },
+)
+
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1398,45 +1432,31 @@
     {
         "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
-
 KinesisStreamingDestinationInputRequestTypeDef = TypedDict(
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1486,126 +1506,83 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsOfResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
-
 TagTableTypeDef = TypedDict(
     "TagTableTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+    },
+)
+
+ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
     {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutRequestServiceResourceOutputTypeDef = TypedDict(
+    "PutRequestServiceResourceOutputTypeDef",
+    {
+        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
     },
 )
 
 PutRequestServiceResourceTypeDef = TypedDict(
     "PutRequestServiceResourceTypeDef",
     {
         "Item": Mapping[
@@ -1632,141 +1609,96 @@
 
 TableClassSummaryTableTypeDef = TypedDict(
     "TableClassSummaryTableTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
 )
 
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
-RestoreSummaryResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryResponseMetadataTypeDef",
+RestoreSummaryTableTypeDef = TypedDict(
+    "RestoreSummaryTableTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRestoreSummaryTableTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTableTypeDef",
-    {
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-    },
-)
-_OptionalRestoreSummaryTableTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTableTypeDef",
+RestoreSummaryTypeDef = TypedDict(
+    "RestoreSummaryTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
-    },
-    total=False,
-)
-
-
-class RestoreSummaryTableTypeDef(
-    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
-):
-    pass
-
-
-_RequiredRestoreSummaryTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTypeDef",
-    {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
-_OptionalRestoreSummaryTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-    },
-    total=False,
-)
-
-
-class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
-    pass
-
 
-SSEDescriptionResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionResponseMetadataTypeDef",
+SSEDescriptionTableTypeDef = TypedDict(
+    "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
+SSEDescriptionTypeDef = TypedDict(
+    "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
-    total=False,
 )
 
-SSEDescriptionTypeDef = TypedDict(
-    "SSEDescriptionTypeDef",
+SSESpecificationOutputTypeDef = TypedDict(
+    "SSESpecificationOutputTypeDef",
     {
-        "Status": SSEStatusType,
+        "Enabled": bool,
         "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
+        "KMSMasterKeyId": str,
     },
-    total=False,
 )
 
 SSESpecificationTableTypeDef = TypedDict(
     "SSESpecificationTableTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
-StreamSpecificationResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationResponseMetadataTypeDef",
+StreamSpecificationOutputTypeDef = TypedDict(
+    "StreamSpecificationOutputTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+    },
+)
+
+StreamSpecificationTableOutputTypeDef = TypedDict(
+    "StreamSpecificationTableOutputTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
@@ -1776,35 +1708,24 @@
     "_OptionalStreamSpecificationTableTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationTableTypeDef(
     _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
 ):
     pass
 
-
-TableBatchWriterRequestTypeDef = TypedDict(
-    "TableBatchWriterRequestTypeDef",
-    {
-        "overwrite_by_pkeys": List[str],
-    },
-    total=False,
-)
-
-TableClassSummaryResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryResponseMetadataTypeDef",
+TimeToLiveSpecificationOutputTypeDef = TypedDict(
+    "TimeToLiveSpecificationOutputTypeDef",
     {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Enabled": bool,
+        "AttributeName": str,
     },
 )
 
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
@@ -1831,29 +1752,144 @@
     "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
-
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    {
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
+    {
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryTableResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1911,21 +1947,19 @@
             ]
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
-
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -1978,19 +2012,17 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
-
 _RequiredConditionTypeDef = TypedDict(
     "_RequiredConditionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
 )
 _OptionalConditionTypeDef = TypedDict(
@@ -2017,18 +2049,23 @@
                 ],
             ]
         ],
     },
     total=False,
 )
 
-
 class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
+DeleteRequestOutputTypeDef = TypedDict(
+    "DeleteRequestOutputTypeDef",
+    {
+        "Key": Dict[str, AttributeValueTypeDef],
+    },
+)
 
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
@@ -2110,19 +2147,17 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
-
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2153,21 +2188,19 @@
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
-
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": Union[
             AttributeValueTypeDef,
             Union[
                 bytes,
@@ -2249,21 +2282,19 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetItemInputRequestTypeDef(
     _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2293,34 +2324,41 @@
     {
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
-
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
+)
+
+KeysAndAttributesOutputTypeDef = TypedDict(
+    "KeysAndAttributesOutputTypeDef",
+    {
+        "Keys": List[Dict[str, AttributeValueTypeDef]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
+    },
 )
 
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -2355,21 +2393,19 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class KeysAndAttributesTypeDef(
     _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
-
 _RequiredParameterizedStatementTypeDef = TypedDict(
     "_RequiredParameterizedStatementTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
@@ -2396,20 +2432,25 @@
                 ],
             ]
         ],
     },
     total=False,
 )
 
-
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
+PutRequestOutputTypeDef = TypedDict(
+    "PutRequestOutputTypeDef",
+    {
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+)
 
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
@@ -2491,19 +2532,17 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
-
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2557,28 +2596,25 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
-
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
         ),
     },
-    total=False,
 )
 
 _RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
@@ -2589,44 +2625,42 @@
     "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-
 class AutoScalingPolicyUpdateTypeDef(
     _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
-
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2636,127 +2670,68 @@
     "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
     _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
     _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
 ):
     pass
 
-
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityServiceResourceTypeDef = TypedDict(
     "ConsumedCapacityServiceResourceTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityServiceResourceTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTableTypeDef = TypedDict(
     "ConsumedCapacityTableTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTableTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
-    total=False,
 )
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2808,66 +2783,14 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2918,55 +2841,29 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_RequiredContinuousBackupsDescriptionTypeDef",
+ContinuousBackupsDescriptionTypeDef = TypedDict(
+    "ContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
-    },
-)
-_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_OptionalContinuousBackupsDescriptionTypeDef",
-    {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
-    total=False,
 )
 
-
-class ContinuousBackupsDescriptionTypeDef(
-    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
-):
-    pass
-
-
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTableTypeDef],
@@ -2977,53 +2874,28 @@
     "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
     total=False,
 )
 
-
 class CreateGlobalSecondaryIndexActionTableTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
 ):
     pass
 
-
 UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-    total=False,
-)
-
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-    },
-    total=False,
-)
-
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -3041,33 +2913,20 @@
     "_OptionalCreateGlobalSecondaryIndexActionTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-
 class CreateGlobalSecondaryIndexActionTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTypeDef,
 ):
     pass
 
-
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -3076,49 +2935,19 @@
     "_OptionalGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
-
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-)
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
-    {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
-    },
-    total=False,
-)
-
-
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
-
-
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
@@ -3127,101 +2956,68 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
-    {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaTypeDef],
-    },
-    total=False,
-)
-
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexTableTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
     _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
 ):
     pass
 
-
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-    },
-    total=False,
-)
-
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_OptionalReplicaGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
-
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+InputFormatOptionsOutputTypeDef = TypedDict(
+    "InputFormatOptionsOutputTypeDef",
+    {
+        "Csv": CsvOptionsOutputTypeDef,
+    },
+)
+
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
@@ -3279,21 +3075,19 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
-
 _RequiredPutItemInputTablePutItemTypeDef = TypedDict(
     "_RequiredPutItemInputTablePutItemTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 bytes,
@@ -3343,21 +3137,19 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
     pass
 
-
 _RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
     "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -3409,21 +3201,19 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
 ):
     pass
 
-
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3434,48 +3224,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3485,91 +3275,153 @@
     "_OptionalDescribeTableInputTableExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTableInputTableExistsWaitTypeDef(
     _RequiredDescribeTableInputTableExistsWaitTypeDef,
     _OptionalDescribeTableInputTableExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTableInputTableNotExistsWaitTypeDef(
     _RequiredDescribeTableInputTableNotExistsWaitTypeDef,
     _OptionalDescribeTableInputTableNotExistsWaitTypeDef,
 ):
     pass
 
-
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+)
+
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+    },
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+GlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "GlobalSecondaryIndexOutputTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+SourceTableDetailsTypeDef = TypedDict(
+    "SourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
 )
 
 _RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
@@ -3580,85 +3432,264 @@
     "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
     },
     total=False,
 )
 
-
 class GlobalSecondaryIndexServiceResourceTypeDef(
     _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
     _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
 ):
     pass
 
-
 LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "LocalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
         "Projection": ProjectionServiceResourceTypeDef,
     },
 )
 
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
+    {
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaOutputTypeDef],
+    },
+)
+
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
 
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+    },
+)
+
+ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+    },
+)
+
+WriteRequestServiceResourceOutputTypeDef = TypedDict(
+    "WriteRequestServiceResourceOutputTypeDef",
+    {
+        "PutRequest": PutRequestServiceResourceOutputTypeDef,
+        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
+    },
+)
+
 WriteRequestServiceResourceTypeDef = TypedDict(
     "WriteRequestServiceResourceTypeDef",
     {
         "PutRequest": PutRequestServiceResourceTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceTypeDef,
     },
     total=False,
 )
 
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
+UpdateTimeToLiveOutputTypeDef = TypedDict(
+    "UpdateTimeToLiveOutputTypeDef",
     {
-        "TableName": str,
-        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateTimeToLiveOutputTypeDef = TypedDict(
-    "UpdateTimeToLiveOutputTypeDef",
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
+        "TableName": str,
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
@@ -3668,22 +3699,20 @@
     "_OptionalBatchExecuteStatementInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -3747,21 +3776,19 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
-
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
-
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -3824,19 +3851,17 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
-
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -3893,21 +3918,19 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
-
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[
             str,
             Union[
@@ -3964,21 +3987,19 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
-
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -4037,21 +4058,19 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
-
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
-
 TransactGetItemTypeDef = TypedDict(
     "TransactGetItemTypeDef",
     {
         "Get": GetTypeDef,
     },
 )
 
@@ -4065,21 +4084,19 @@
     "_OptionalBatchGetItemInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchGetItemInputRequestTypeDef(
     _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -4087,20 +4104,26 @@
     {
         "ClientRequestToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class ExecuteTransactionInputRequestTypeDef(
     _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
+    {
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
+    },
+)
 
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
     },
@@ -4123,15 +4146,14 @@
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
-    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
@@ -4141,413 +4163,230 @@
     },
     total=False,
 )
 
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
-        "Responses": Dict[
-            str,
-            List[
-                Dict[
-                    str,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
-                ]
-            ],
-        ],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
+        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
-        "Item": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Item": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
     },
     total=False,
 )
 
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateTableInputRequestTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4564,21 +4403,19 @@
         "Tags": Sequence[TagTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-
 class CreateTableInputRequestTypeDef(
     _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
 ):
     pass
 
-
 _RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
     },
 )
@@ -4590,22 +4427,20 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
-
 class RestoreTableFromBackupInputRequestTypeDef(
     _RequiredRestoreTableFromBackupInputRequestTypeDef,
     _OptionalRestoreTableFromBackupInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
     {
         "TargetTableName": str,
     },
 )
 _OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
@@ -4620,83 +4455,54 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
-
 class RestoreTableToPointInTimeInputRequestTypeDef(
     _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
     _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersTypeDef = TypedDict(
     "_OptionalTableCreationParametersTypeDef",
     {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
     },
     total=False,
 )
 
-
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
-
 GlobalSecondaryIndexUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
-    {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4706,22 +4512,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMemberActionTableTypeDef(
     _RequiredCreateReplicationGroupMemberActionTableTypeDef,
     _OptionalCreateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
-
 _RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4731,38 +4535,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class UpdateReplicationGroupMemberActionTableTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
-
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4772,22 +4558,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMemberActionTypeDef(
     _RequiredCreateReplicationGroupMemberActionTypeDef,
     _OptionalCreateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-
 _RequiredUpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4797,30 +4581,52 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
+    {
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationOutputTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+    },
+)
+
+TableCreationParametersOutputTypeDef = TypedDict(
+    "TableCreationParametersOutputTypeDef",
+    {
+        "TableName": str,
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "SSESpecification": SSESpecificationOutputTypeDef,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+    },
+)
+
 _RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
@@ -4837,28 +4643,75 @@
         "Tags": Sequence[TagServiceResourceTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-
 class CreateTableInputServiceResourceCreateTableTypeDef(
     _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
     _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
 ):
     pass
 
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
+    {
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
+    },
+)
+
+ReplicaDescriptionTableTypeDef = TypedDict(
+    "ReplicaDescriptionTableTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
+    },
+)
+
+BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchWriteItemOutputServiceResourceTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4869,52 +4722,48 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
-
 class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
     _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
 ):
     pass
 
-
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
     },
 )
 _OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
     "_OptionalTransactGetItemsInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
     },
 )
@@ -4923,31 +4772,19 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
-
 class BatchWriteItemInputRequestTypeDef(
     _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
-
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
 _OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
@@ -4956,58 +4793,41 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class TransactWriteItemsInputRequestTypeDef(
     _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
 ):
     pass
 
-
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
-    },
-)
-_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
-    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-
-class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-):
-    pass
-
-
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -5024,22 +4844,20 @@
     {
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-
 ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -5056,58 +4874,20 @@
     {
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
-
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
     },
@@ -5118,155 +4898,170 @@
         "ClientToken": str,
         "InputFormatOptions": InputFormatOptionsTypeDef,
         "InputCompressionType": InputCompressionTypeType,
     },
     total=False,
 )
 
-
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
-
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
-    {
-        "AttributeDefinitions": List[AttributeDefinitionTableTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
 ReplicationGroupUpdateTableTypeDef = TypedDict(
     "ReplicationGroupUpdateTableTypeDef",
     {
         "Create": CreateReplicationGroupMemberActionTableTypeDef,
         "Update": UpdateReplicationGroupMemberActionTableTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
     },
     total=False,
 )
 
+ReplicationGroupUpdateTypeDef = TypedDict(
+    "ReplicationGroupUpdateTypeDef",
+    {
+        "Create": CreateReplicationGroupMemberActionTypeDef,
+        "Update": UpdateReplicationGroupMemberActionTypeDef,
+        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+    },
+    total=False,
+)
+
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+    },
+)
+
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
+    {
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "TableId": str,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersOutputTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
+    },
+)
+
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
-    total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "TableName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
         "TableStatus": TableStatusType,
         "CreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "TableSizeBytes": int,
         "ItemCount": int,
         "TableArn": str,
         "TableId": str,
         "BillingModeSummary": BillingModeSummaryTypeDef,
         "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
+        "StreamSpecification": StreamSpecificationOutputTypeDef,
         "LatestStreamLabel": str,
         "LatestStreamArn": str,
         "GlobalTableVersion": str,
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
-ReplicationGroupUpdateTypeDef = TypedDict(
-    "ReplicationGroupUpdateTypeDef",
+TableDescriptionTableTypeDef = TypedDict(
+    "TableDescriptionTableTypeDef",
     {
-        "Create": CreateReplicationGroupMemberActionTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTableTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTableTypeDef],
+        "RestoreSummary": RestoreSummaryTableTypeDef,
+        "SSEDescription": SSEDescriptionTableTypeDef,
+        "ArchivalSummary": ArchivalSummaryTableTypeDef,
+        "TableClassSummary": TableClassSummaryTableTypeDef,
+        "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
-    total=False,
 )
 
-_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaSettingsDescriptionTypeDef",
+ReplicaSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaSettingsDescriptionTypeDef",
-    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
-    total=False,
 )
 
-
-class ReplicaSettingsDescriptionTypeDef(
-    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
-):
-    pass
-
-
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5276,21 +5071,19 @@
             ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef
         ],
         "ReplicaProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaAutoScalingUpdateTypeDef(
     _RequiredReplicaAutoScalingUpdateTypeDef, _OptionalReplicaAutoScalingUpdateTypeDef
 ):
     pass
 
-
 _RequiredReplicaSettingsUpdateTypeDef = TypedDict(
     "_RequiredReplicaSettingsUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaSettingsUpdateTypeDef = TypedDict(
@@ -5302,203 +5095,198 @@
             ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaTableClass": TableClassType,
     },
     total=False,
 )
 
-
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableTypeDef,
+        "SSESpecification": SSESpecificationTableTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+_RequiredUpdateTableInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateTableInputRequestTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalUpdateTableInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class UpdateTableInputRequestTypeDef(
+    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
+):
+    pass
 
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
-    {
-        "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateTableInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateTableInputRequestTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalUpdateTableInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateTableInputRequestTypeDef",
+DeleteTableOutputTableTypeDef = TypedDict(
+    "DeleteTableOutputTableTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "TableDescription": TableDescriptionTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateTableInputRequestTypeDef(
-    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
-):
-    pass
-
-
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
-    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5510,22 +5298,20 @@
         "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef],
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
         "ReplicaUpdates": Sequence[ReplicaAutoScalingUpdateTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTableReplicaAutoScalingInputRequestTypeDef(
     _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef,
     _OptionalUpdateTableReplicaAutoScalingInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalTableSettingsInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
 )
 _OptionalUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
@@ -5540,30 +5326,28 @@
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaSettingsUpdate": Sequence[ReplicaSettingsUpdateTypeDef],
     },
     total=False,
 )
 
-
 class UpdateGlobalTableSettingsInputRequestTypeDef(
     _RequiredUpdateGlobalTableSettingsInputRequestTypeDef,
     _OptionalUpdateGlobalTableSettingsInputRequestTypeDef,
 ):
     pass
 
-
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef
+    from types_aiobotocore_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ArchivalSummaryResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -60,32 +60,37 @@
 else:
     from typing_extensions import TypedDict
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 
+
 __all__ = (
-    "ArchivalSummaryResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
+    "AttributeDefinitionOutputTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
+    "AttributeDefinitionTableOutputTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
+    "AttributeValueServiceResourceTypeDef",
+    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
+    "KeysAndAttributesServiceResourceOutputTypeDef",
     "BatchStatementErrorTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -105,173 +110,197 @@
     "StreamSpecificationTypeDef",
     "TagTypeDef",
     "KeySchemaElementServiceResourceTypeDef",
     "ProvisionedThroughputServiceResourceTypeDef",
     "SSESpecificationServiceResourceTypeDef",
     "StreamSpecificationServiceResourceTypeDef",
     "TagServiceResourceTypeDef",
+    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
     "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
     "ExpectedAttributeValueTableTypeDef",
     "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
     "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
+    "DeleteRequestServiceResourceOutputTypeDef",
     "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
+    "KeySchemaElementTableOutputTypeDef",
+    "ProjectionTableOutputTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
+    "KeySchemaElementOutputTypeDef",
+    "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
+    "ProvisionedThroughputOutputTypeDef",
     "ProjectionServiceResourceTypeDef",
+    "ReplicaOutputTypeDef",
+    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+    "ProvisionedThroughputOverrideOutputTypeDef",
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
+    "PutRequestServiceResourceOutputTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreSummaryResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
+    "SSESpecificationOutputTypeDef",
     "SSESpecificationTableTypeDef",
-    "StreamSpecificationResponseMetadataTypeDef",
+    "StreamSpecificationOutputTypeDef",
+    "StreamSpecificationTableOutputTypeDef",
     "StreamSpecificationTableTypeDef",
-    "TableBatchWriterRequestTypeDef",
-    "TableClassSummaryResponseMetadataTypeDef",
+    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    "DescribeLimitsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    "TableClassSummaryTableResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
+    "DeleteRequestOutputTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "ExpectedAttributeValueTypeDef",
     "GetItemInputRequestTypeDef",
     "GetTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
+    "KeysAndAttributesOutputTypeDef",
     "KeysAndAttributesTypeDef",
     "ParameterizedStatementTypeDef",
+    "PutRequestOutputTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "BatchStatementResponseTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
-    "LocalSecondaryIndexDescriptionTypeDef",
-    "LocalSecondaryIndexInfoTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexTypeDef",
-    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "GlobalTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
     "ReplicaGlobalSecondaryIndexTableTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
     "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "LocalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "LocalSecondaryIndexDescriptionTypeDef",
+    "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
+    "SourceTableDetailsTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
+    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    "WriteRequestServiceResourceOutputTypeDef",
     "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "UpdateTimeToLiveInputRequestTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
     "BatchGetItemInputRequestTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestOutputTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "GetItemOutputTableTypeDef",
@@ -290,117 +319,133 @@
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
     "GlobalSecondaryIndexUpdateTableTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "CreateTableInputRequestTypeDef",
     "RestoreTableFromBackupInputRequestTypeDef",
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "ListGlobalTablesOutputTypeDef",
-    "ReplicaDescriptionTableTypeDef",
     "CreateReplicationGroupMemberActionTableTypeDef",
     "UpdateReplicationGroupMemberActionTableTypeDef",
-    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
+    "TableCreationParametersOutputTypeDef",
     "CreateTableInputServiceResourceCreateTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
     "ListImportsOutputTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    "ReplicaDescriptionTypeDef",
+    "ReplicaDescriptionTableTypeDef",
     "BatchWriteItemOutputServiceResourceTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "ImportTableInputRequestTypeDef",
-    "TableDescriptionTableTypeDef",
     "ReplicationGroupUpdateTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "BackupDescriptionTypeDef",
+    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "ReplicationGroupUpdateTypeDef",
+    "TableDescriptionTableTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "UpdateTableInputRequestTypeDef",
     "DeleteBackupOutputTypeDef",
     "DescribeBackupOutputTypeDef",
     "DescribeImportOutputTypeDef",
     "ImportTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "UpdateTableInputRequestTypeDef",
+    "DeleteTableOutputTableTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ArchivalSummaryResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-    total=False,
+)
+
+AttributeDefinitionOutputTypeDef = TypedDict(
+    "AttributeDefinitionOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
 )
 
 AttributeDefinitionServiceResourceTypeDef = TypedDict(
     "AttributeDefinitionServiceResourceTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeDefinitionTableOutputTypeDef = TypedDict(
+    "AttributeDefinitionTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "AttributeType": ScalarAttributeTypeType,
+    },
+)
+
 AttributeDefinitionTableTypeDef = TypedDict(
     "AttributeDefinitionTableTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
@@ -409,14 +454,46 @@
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
+AttributeValueServiceResourceTypeDef = TypedDict(
+    "AttributeValueServiceResourceTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
+AttributeValueTableTypeDef = TypedDict(
+    "AttributeValueTableTypeDef",
+    {
+        "S": str,
+        "N": str,
+        "B": bytes,
+        "SS": List[str],
+        "NS": List[str],
+        "BS": List[bytes],
+        "M": Dict[str, Dict[str, Any]],
+        "L": List[Dict[str, Any]],
+        "NULL": bool,
+        "BOOL": bool,
+    },
+)
+
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -450,36 +527,24 @@
             None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
+        "TargetValue": float,
     },
-    total=False,
 )
 
-class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
-    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
-):
-    pass
-
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -488,57 +553,49 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
+
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-_RequiredBackupDetailsTypeDef = TypedDict(
-    "_RequiredBackupDetailsTypeDef",
+
+BackupDetailsTypeDef = TypedDict(
+    "BackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
+        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
-    },
-)
-_OptionalBackupDetailsTypeDef = TypedDict(
-    "_OptionalBackupDetailsTypeDef",
-    {
-        "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
-    total=False,
 )
 
-class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
-    pass
-
 BackupSummaryTableTypeDef = TypedDict(
     "BackupSummaryTableTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
@@ -547,15 +604,14 @@
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-    total=False,
 )
 
 _RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
     "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -587,111 +643,90 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
+
+KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
+    "KeysAndAttributesServiceResourceOutputTypeDef",
+    {
+        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
+    },
+)
+
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
     },
-    total=False,
 )
 
 ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
     "ItemCollectionMetricsServiceResourceTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
-)
-
-BillingModeSummaryResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-    total=False,
 )
 
 CapacityServiceResourceTypeDef = TypedDict(
     "CapacityServiceResourceTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTableTypeDef = TypedDict(
     "CapacityTableTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-    total=False,
 )
 
 _RequiredConditionTableTypeDef = TypedDict(
     "_RequiredConditionTableTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -717,35 +752,35 @@
                 None,
             ]
         ],
     },
     total=False,
 )
 
+
 class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
+
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
-    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
-    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
@@ -760,15 +795,15 @@
     },
 )
 
 ProjectionTableTypeDef = TypedDict(
     "ProjectionTableTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
+        "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
 ProvisionedThroughputTableTypeDef = TypedDict(
     "ProvisionedThroughputTableTypeDef",
     {
@@ -853,19 +888,21 @@
     "_OptionalStreamSpecificationTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationTypeDef(
     _RequiredStreamSpecificationTypeDef, _OptionalStreamSpecificationTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -906,33 +943,43 @@
     "_OptionalStreamSpecificationServiceResourceTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationServiceResourceTypeDef(
     _RequiredStreamSpecificationServiceResourceTypeDef,
     _OptionalStreamSpecificationServiceResourceTypeDef,
 ):
     pass
 
+
 TagServiceResourceTypeDef = TypedDict(
     "TagServiceResourceTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CsvOptionsOutputTypeDef = TypedDict(
+    "CsvOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+        "HeaderList": List[str],
+    },
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
-        "HeaderList": List[str],
+        "HeaderList": Sequence[str],
     },
     total=False,
 )
 
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
@@ -996,36 +1043,17 @@
     },
     total=False,
 )
 
 ItemCollectionMetricsTableTypeDef = TypedDict(
     "ItemCollectionMetricsTableTypeDef",
     {
-        "ItemCollectionKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
@@ -1041,14 +1069,21 @@
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
+DeleteRequestServiceResourceOutputTypeDef = TypedDict(
+    "DeleteRequestServiceResourceOutputTypeDef",
+    {
+        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
+    },
+)
+
 DeleteRequestServiceResourceTypeDef = TypedDict(
     "DeleteRequestServiceResourceTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1101,27 +1136,28 @@
     "_OptionalDescribeContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
+
 class DescribeContributorInsightsInputRequestTypeDef(
     _RequiredDescribeContributorInsightsInputRequestTypeDef,
     _OptionalDescribeContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1154,15 +1190,14 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
-    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1192,26 +1227,14 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
-    total=False,
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1242,31 +1265,22 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
-    total=False,
 )
 
 _RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
         "TableArn": str,
         "S3Bucket": str,
@@ -1282,20 +1296,22 @@
         "S3SseAlgorithm": S3SseAlgorithmType,
         "S3SseKmsKeyId": str,
         "ExportFormat": ExportFormatType,
     },
     total=False,
 )
 
+
 class ExportTableToPointInTimeInputRequestTypeDef(
     _RequiredExportTableToPointInTimeInputRequestTypeDef,
     _OptionalExportTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -1324,52 +1340,108 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
+
+KeySchemaElementTableOutputTypeDef = TypedDict(
+    "KeySchemaElementTableOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionTableOutputTypeDef = TypedDict(
+    "ProjectionTableOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
+)
+
 ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTableTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+KeySchemaElementOutputTypeDef = TypedDict(
+    "KeySchemaElementOutputTypeDef",
+    {
+        "AttributeName": str,
+        "KeyType": KeyTypeType,
+    },
+)
+
+ProjectionOutputTypeDef = TypedDict(
+    "ProjectionOutputTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": List[str],
+    },
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-    total=False,
+)
+
+ProvisionedThroughputOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+    },
 )
 
 ProjectionServiceResourceTypeDef = TypedDict(
     "ProjectionServiceResourceTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": Sequence[str],
     },
     total=False,
 )
 
+ReplicaOutputTypeDef = TypedDict(
+    "ReplicaOutputTypeDef",
+    {
+        "RegionName": str,
+    },
+)
+
+S3BucketSourceOutputTypeDef = TypedDict(
+    "S3BucketSourceOutputTypeDef",
+    {
+        "S3BucketOwner": str,
+        "S3Bucket": str,
+        "S3KeyPrefix": str,
+    },
+)
+
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1377,43 +1449,33 @@
     {
         "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
+
 KinesisStreamingDestinationInputRequestTypeDef = TypedDict(
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1463,122 +1525,85 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsOfResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
+
 TagTableTypeDef = TypedDict(
     "TagTableTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideOutputTypeDef",
     {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOverrideTableOutputTypeDef",
+    {
+        "ReadCapacityUnits": int,
+    },
+)
+
+PutRequestServiceResourceOutputTypeDef = TypedDict(
+    "PutRequestServiceResourceOutputTypeDef",
+    {
+        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
     },
 )
 
 PutRequestServiceResourceTypeDef = TypedDict(
     "PutRequestServiceResourceTypeDef",
     {
         "Item": Mapping[
@@ -1605,137 +1630,96 @@
 
 TableClassSummaryTableTypeDef = TypedDict(
     "TableClassSummaryTableTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
 )
 
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
-RestoreSummaryResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryResponseMetadataTypeDef",
+RestoreSummaryTableTypeDef = TypedDict(
+    "RestoreSummaryTableTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRestoreSummaryTableTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTableTypeDef",
-    {
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-    },
-)
-_OptionalRestoreSummaryTableTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTableTypeDef",
+RestoreSummaryTypeDef = TypedDict(
+    "RestoreSummaryTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
-    },
-    total=False,
-)
-
-class RestoreSummaryTableTypeDef(
-    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
-):
-    pass
-
-_RequiredRestoreSummaryTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTypeDef",
-    {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
-_OptionalRestoreSummaryTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-    },
-    total=False,
-)
-
-class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
-    pass
 
-SSEDescriptionResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionResponseMetadataTypeDef",
+SSEDescriptionTableTypeDef = TypedDict(
+    "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
+SSEDescriptionTypeDef = TypedDict(
+    "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
-    total=False,
 )
 
-SSEDescriptionTypeDef = TypedDict(
-    "SSEDescriptionTypeDef",
+SSESpecificationOutputTypeDef = TypedDict(
+    "SSESpecificationOutputTypeDef",
     {
-        "Status": SSEStatusType,
+        "Enabled": bool,
         "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
+        "KMSMasterKeyId": str,
     },
-    total=False,
 )
 
 SSESpecificationTableTypeDef = TypedDict(
     "SSESpecificationTableTypeDef",
     {
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
-StreamSpecificationResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationResponseMetadataTypeDef",
+StreamSpecificationOutputTypeDef = TypedDict(
+    "StreamSpecificationOutputTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+    },
+)
+
+StreamSpecificationTableOutputTypeDef = TypedDict(
+    "StreamSpecificationTableOutputTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
@@ -1745,33 +1729,26 @@
     "_OptionalStreamSpecificationTableTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationTableTypeDef(
     _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
 ):
     pass
 
-TableBatchWriterRequestTypeDef = TypedDict(
-    "TableBatchWriterRequestTypeDef",
-    {
-        "overwrite_by_pkeys": List[str],
-    },
-    total=False,
-)
 
-TableClassSummaryResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryResponseMetadataTypeDef",
+TimeToLiveSpecificationOutputTypeDef = TypedDict(
+    "TimeToLiveSpecificationOutputTypeDef",
     {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Enabled": bool,
+        "AttributeName": str,
     },
 )
 
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
@@ -1798,27 +1775,146 @@
     "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
+
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+
+ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryTableResponseMetadataTypeDef",
+    {
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryTableResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
+    {
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryTableResponseMetadataTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionTableResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationTableResponseMetadataTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryTableResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1876,19 +1972,21 @@
             ]
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
+
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
+
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -1941,17 +2039,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
+
 _RequiredConditionTypeDef = TypedDict(
     "_RequiredConditionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
 )
 _OptionalConditionTypeDef = TypedDict(
@@ -1978,17 +2078,26 @@
                 ],
             ]
         ],
     },
     total=False,
 )
 
+
 class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
+
+DeleteRequestOutputTypeDef = TypedDict(
+    "DeleteRequestOutputTypeDef",
+    {
+        "Key": Dict[str, AttributeValueTypeDef],
+    },
+)
+
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2069,17 +2178,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
+
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2110,19 +2221,21 @@
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
+
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": Union[
             AttributeValueTypeDef,
             Union[
                 bytes,
@@ -2204,19 +2317,21 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetItemInputRequestTypeDef(
     _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2246,32 +2361,43 @@
     {
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
+
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
-    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
+)
+
+KeysAndAttributesOutputTypeDef = TypedDict(
+    "KeysAndAttributesOutputTypeDef",
+    {
+        "Keys": List[Dict[str, AttributeValueTypeDef]],
+        "AttributesToGet": List[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
+        "ExpressionAttributeNames": Dict[str, str],
+    },
 )
 
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
@@ -2306,19 +2432,21 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class KeysAndAttributesTypeDef(
     _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
+
 _RequiredParameterizedStatementTypeDef = TypedDict(
     "_RequiredParameterizedStatementTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
@@ -2345,19 +2473,28 @@
                 ],
             ]
         ],
     },
     total=False,
 )
 
+
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
+
+PutRequestOutputTypeDef = TypedDict(
+    "PutRequestOutputTypeDef",
+    {
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+)
+
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2438,17 +2575,19 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
+
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
@@ -2502,26 +2641,27 @@
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
+
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
         ),
     },
-    total=False,
 )
 
 _RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
         "TargetTrackingScalingPolicyConfiguration": (
             AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
@@ -2532,42 +2672,44 @@
     "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
+
 class AutoScalingPolicyUpdateTypeDef(
     _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
+
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2577,123 +2719,70 @@
     "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
     _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
     _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
 ):
     pass
 
+
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
         "Item": Dict[str, AttributeValueTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityServiceResourceTypeDef = TypedDict(
     "ConsumedCapacityServiceResourceTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityServiceResourceTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTableTypeDef = TypedDict(
     "ConsumedCapacityTableTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTableTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
     },
-    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
-    total=False,
 )
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2745,64 +2834,14 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2853,55 +2892,31 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_RequiredContinuousBackupsDescriptionTypeDef",
+ContinuousBackupsDescriptionTypeDef = TypedDict(
+    "ContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
-    },
-)
-_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
-    "_OptionalContinuousBackupsDescriptionTypeDef",
-    {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
-    total=False,
 )
 
-class ContinuousBackupsDescriptionTypeDef(
-    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
-):
-    pass
-
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTableTypeDef],
         "Projection": ProjectionTableTypeDef,
     },
@@ -2910,51 +2925,30 @@
     "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
     total=False,
 )
 
+
 class CreateGlobalSecondaryIndexActionTableTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
 ):
     pass
 
+
 UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-    total=False,
-)
-
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-    },
-    total=False,
-)
-
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -2972,30 +2966,21 @@
     "_OptionalCreateGlobalSecondaryIndexActionTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
 class CreateGlobalSecondaryIndexActionTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTypeDef,
 ):
     pass
 
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
 
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
@@ -3005,44 +2990,20 @@
     "_OptionalGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-)
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
-    {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
-    },
-    total=False,
-)
-
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
 
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
@@ -3052,60 +3013,35 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
-    {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaTypeDef],
-    },
-    total=False,
-)
-
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
     "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexTableTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
     _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
 ):
     pass
 
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-    },
-    total=False,
-)
 
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
@@ -3113,36 +3049,36 @@
     "_OptionalReplicaGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+InputFormatOptionsOutputTypeDef = TypedDict(
+    "InputFormatOptionsOutputTypeDef",
+    {
+        "Csv": CsvOptionsOutputTypeDef,
+    },
+)
+
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
@@ -3200,19 +3136,21 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
+
 _RequiredPutItemInputTablePutItemTypeDef = TypedDict(
     "_RequiredPutItemInputTablePutItemTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 bytes,
@@ -3262,19 +3200,21 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
     pass
 
+
 _RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
     "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 bytes,
@@ -3326,19 +3266,21 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
 ):
     pass
 
+
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3349,48 +3291,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3400,87 +3342,157 @@
     "_OptionalDescribeTableInputTableExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTableInputTableExistsWaitTypeDef(
     _RequiredDescribeTableInputTableExistsWaitTypeDef,
     _OptionalDescribeTableInputTableExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTableInputTableNotExistsWaitTypeDef(
     _RequiredDescribeTableInputTableNotExistsWaitTypeDef,
     _OptionalDescribeTableInputTableNotExistsWaitTypeDef,
 ):
     pass
 
+
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "Projection": ProjectionTableOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+)
+
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+    },
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
-    total=False,
+)
+
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+GlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "GlobalSecondaryIndexOutputTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+    },
+)
+
+SourceTableDetailsTypeDef = TypedDict(
+    "SourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
 )
 
 _RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
@@ -3491,83 +3503,272 @@
     "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
     },
     total=False,
 )
 
+
 class GlobalSecondaryIndexServiceResourceTypeDef(
     _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
     _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
 ):
     pass
 
+
 LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
     "LocalSecondaryIndexServiceResourceTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
         "Projection": ProjectionServiceResourceTypeDef,
     },
 )
 
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
+    {
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaOutputTypeDef],
+    },
+)
+
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
 
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+    },
+)
+
+ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+    },
+)
+
+WriteRequestServiceResourceOutputTypeDef = TypedDict(
+    "WriteRequestServiceResourceOutputTypeDef",
+    {
+        "PutRequest": PutRequestServiceResourceOutputTypeDef,
+        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
+    },
+)
+
 WriteRequestServiceResourceTypeDef = TypedDict(
     "WriteRequestServiceResourceTypeDef",
     {
         "PutRequest": PutRequestServiceResourceTypeDef,
         "DeleteRequest": DeleteRequestServiceResourceTypeDef,
     },
     total=False,
 )
 
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
+UpdateTimeToLiveOutputTypeDef = TypedDict(
+    "UpdateTimeToLiveOutputTypeDef",
     {
-        "TableName": str,
-        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateTimeToLiveOutputTypeDef = TypedDict(
-    "UpdateTimeToLiveOutputTypeDef",
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
+        "TableName": str,
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
@@ -3577,20 +3778,22 @@
     "_OptionalBatchExecuteStatementInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -3654,19 +3857,21 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
+
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
+
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -3729,17 +3934,19 @@
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
+
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
+
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -3796,19 +4003,21 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
+
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[
             str,
             Union[
@@ -3865,19 +4074,21 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
+
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
@@ -3936,19 +4147,21 @@
                 ],
             ],
         ],
     },
     total=False,
 )
 
+
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
+
 TransactGetItemTypeDef = TypedDict(
     "TransactGetItemTypeDef",
     {
         "Get": GetTypeDef,
     },
 )
 
@@ -3962,19 +4175,21 @@
     "_OptionalBatchGetItemInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchGetItemInputRequestTypeDef(
     _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -3982,19 +4197,29 @@
     {
         "ClientRequestToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class ExecuteTransactionInputRequestTypeDef(
     _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
+
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
+    {
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
+    },
+)
+
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
     },
     total=False,
@@ -4016,15 +4241,14 @@
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
-    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
@@ -4034,413 +4258,230 @@
     },
     total=False,
 )
 
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
-        "Responses": Dict[
-            str,
-            List[
-                Dict[
-                    str,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
-                ]
-            ],
-        ],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
+        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
-        "Item": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Item": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
-        "Items": List[
-            Dict[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
-        "Attributes": Dict[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
     },
     total=False,
 )
 
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateTableInputRequestTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4457,19 +4498,21 @@
         "Tags": Sequence[TagTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
+
 class CreateTableInputRequestTypeDef(
     _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
 ):
     pass
 
+
 _RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
     },
 )
@@ -4481,20 +4524,22 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
+
 class RestoreTableFromBackupInputRequestTypeDef(
     _RequiredRestoreTableFromBackupInputRequestTypeDef,
     _OptionalRestoreTableFromBackupInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
     {
         "TargetTableName": str,
     },
 )
 _OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
@@ -4509,79 +4554,58 @@
         "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
         "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
         "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
+
 class RestoreTableToPointInTimeInputRequestTypeDef(
     _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
     _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersTypeDef = TypedDict(
     "_OptionalTableCreationParametersTypeDef",
     {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
     },
     total=False,
 )
 
+
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
+
 GlobalSecondaryIndexUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
-    {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4591,20 +4615,22 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMemberActionTableTypeDef(
     _RequiredCreateReplicationGroupMemberActionTableTypeDef,
     _OptionalCreateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
+
 _RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
@@ -4614,35 +4640,21 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class UpdateReplicationGroupMemberActionTableTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
 ):
     pass
 
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
@@ -4653,20 +4665,22 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMemberActionTypeDef(
     _RequiredCreateReplicationGroupMemberActionTypeDef,
     _OptionalCreateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
+
 _RequiredUpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4676,28 +4690,54 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
+
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
+    {
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationOutputTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+    },
+)
+
+TableCreationParametersOutputTypeDef = TypedDict(
+    "TableCreationParametersOutputTypeDef",
+    {
+        "TableName": str,
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "SSESpecification": SSESpecificationOutputTypeDef,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+    },
+)
+
 _RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
@@ -4714,26 +4754,77 @@
         "Tags": Sequence[TagServiceResourceTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
+
 class CreateTableInputServiceResourceCreateTableTypeDef(
     _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
     _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
 ):
     pass
 
+
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
+    {
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
+    },
+)
+
+ReplicaDescriptionTableTypeDef = TypedDict(
+    "ReplicaDescriptionTableTypeDef",
+    {
+        "RegionName": str,
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
+        "KMSMasterKeyId": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
+    },
+)
+
+BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchWriteItemOutputServiceResourceTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4744,29 +4835,21 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
+
 class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
     _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
 ):
     pass
 
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
     },
 )
@@ -4774,19 +4857,31 @@
     "_OptionalTransactGetItemsInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
+
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
     },
 )
 _OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
@@ -4794,28 +4889,20 @@
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
+
 class BatchWriteItemInputRequestTypeDef(
     _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
@@ -4825,54 +4912,43 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class TransactWriteItemsInputRequestTypeDef(
     _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
 ):
     pass
 
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
-    },
-)
-_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
-    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
-    total=False,
 )
 
-class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
-):
-    pass
-
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -4889,20 +4965,22 @@
     {
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
+
 ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -4919,55 +4997,21 @@
     {
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
 
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
@@ -4979,151 +5023,172 @@
         "ClientToken": str,
         "InputFormatOptions": InputFormatOptionsTypeDef,
         "InputCompressionType": InputCompressionTypeType,
     },
     total=False,
 )
 
+
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
-    {
-        "AttributeDefinitions": List[AttributeDefinitionTableTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
 
 ReplicationGroupUpdateTableTypeDef = TypedDict(
     "ReplicationGroupUpdateTableTypeDef",
     {
         "Create": CreateReplicationGroupMemberActionTableTypeDef,
         "Update": UpdateReplicationGroupMemberActionTableTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
     },
     total=False,
 )
 
+ReplicationGroupUpdateTypeDef = TypedDict(
+    "ReplicationGroupUpdateTypeDef",
+    {
+        "Create": CreateReplicationGroupMemberActionTypeDef,
+        "Update": UpdateReplicationGroupMemberActionTypeDef,
+        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+    },
+    total=False,
+)
+
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+    },
+)
+
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
+    {
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "TableId": str,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersOutputTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
+    },
+)
+
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
-    total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
         "TableName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
+        "KeySchema": List[KeySchemaElementOutputTypeDef],
         "TableStatus": TableStatusType,
         "CreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "TableSizeBytes": int,
         "ItemCount": int,
         "TableArn": str,
         "TableId": str,
         "BillingModeSummary": BillingModeSummaryTypeDef,
         "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
+        "StreamSpecification": StreamSpecificationOutputTypeDef,
         "LatestStreamLabel": str,
         "LatestStreamArn": str,
         "GlobalTableVersion": str,
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
-ReplicationGroupUpdateTypeDef = TypedDict(
-    "ReplicationGroupUpdateTypeDef",
+TableDescriptionTableTypeDef = TypedDict(
+    "TableDescriptionTableTypeDef",
     {
-        "Create": CreateReplicationGroupMemberActionTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTableTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTableTypeDef],
+        "RestoreSummary": RestoreSummaryTableTypeDef,
+        "SSEDescription": SSEDescriptionTableTypeDef,
+        "ArchivalSummary": ArchivalSummaryTableTypeDef,
+        "TableClassSummary": TableClassSummaryTableTypeDef,
+        "DeletionProtectionEnabled": bool,
     },
-    total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
-    total=False,
 )
 
-_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_RequiredReplicaSettingsDescriptionTypeDef",
+ReplicaSettingsDescriptionTypeDef = TypedDict(
+    "ReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
-    "_OptionalReplicaSettingsDescriptionTypeDef",
-    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
-    total=False,
 )
 
-class ReplicaSettingsDescriptionTypeDef(
-    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
-):
-    pass
-
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5133,19 +5198,21 @@
             ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef
         ],
         "ReplicaProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaAutoScalingUpdateTypeDef(
     _RequiredReplicaAutoScalingUpdateTypeDef, _OptionalReplicaAutoScalingUpdateTypeDef
 ):
     pass
 
+
 _RequiredReplicaSettingsUpdateTypeDef = TypedDict(
     "_RequiredReplicaSettingsUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaSettingsUpdateTypeDef = TypedDict(
@@ -5157,199 +5224,202 @@
             ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaTableClass": TableClassType,
     },
     total=False,
 )
 
+
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
+
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
+        "StreamSpecification": StreamSpecificationTableTypeDef,
+        "SSESpecification": SSESpecificationTableTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+_RequiredUpdateTableInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateTableInputRequestTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalUpdateTableInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class UpdateTableInputRequestTypeDef(
+    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
+):
+    pass
+
+
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
-    {
-        "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateTableInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateTableInputRequestTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalUpdateTableInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateTableInputRequestTypeDef",
+DeleteTableOutputTableTypeDef = TypedDict(
+    "DeleteTableOutputTableTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "TableDescription": TableDescriptionTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateTableInputRequestTypeDef(
-    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
-):
-    pass
-
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
-    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5361,20 +5431,22 @@
         "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef],
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
         "ReplicaUpdates": Sequence[ReplicaAutoScalingUpdateTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTableReplicaAutoScalingInputRequestTypeDef(
     _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef,
     _OptionalUpdateTableReplicaAutoScalingInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalTableSettingsInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
 )
 _OptionalUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
@@ -5389,28 +5461,30 @@
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaSettingsUpdate": Sequence[ReplicaSettingsUpdateTypeDef],
     },
     total=False,
 )
 
+
 class UpdateGlobalTableSettingsInputRequestTypeDef(
     _RequiredUpdateGlobalTableSettingsInputRequestTypeDef,
     _OptionalUpdateGlobalTableSettingsInputRequestTypeDef,
 ):
     pass
 
+
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -48,15 +48,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -457,31 +457,35 @@
 ### Typed dictionaries
 
 `types_aiobotocore_dynamodb.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodb.type_defs import (
-    ArchivalSummaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
+    AttributeDefinitionOutputTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
+    AttributeDefinitionTableOutputTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
+    AttributeValueServiceResourceTypeDef,
+    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
+    KeysAndAttributesServiceResourceOutputTypeDef,
     BatchStatementErrorTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -501,173 +505,197 @@
     StreamSpecificationTypeDef,
     TagTypeDef,
     KeySchemaElementServiceResourceTypeDef,
     ProvisionedThroughputServiceResourceTypeDef,
     SSESpecificationServiceResourceTypeDef,
     StreamSpecificationServiceResourceTypeDef,
     TagServiceResourceTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
     DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
     ExpectedAttributeValueTableTypeDef,
     ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
     DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
+    DeleteRequestServiceResourceOutputTypeDef,
     DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
+    KeySchemaElementTableOutputTypeDef,
+    ProjectionTableOutputTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
+    KeySchemaElementOutputTypeDef,
+    ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProjectionServiceResourceTypeDef,
+    ReplicaOutputTypeDef,
+    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
+    ProvisionedThroughputOverrideOutputTypeDef,
+    ProvisionedThroughputOverrideTableOutputTypeDef,
+    PutRequestServiceResourceOutputTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
+    SSESpecificationOutputTypeDef,
     SSESpecificationTableTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
+    StreamSpecificationOutputTypeDef,
+    StreamSpecificationTableOutputTypeDef,
     StreamSpecificationTableTypeDef,
-    TableBatchWriterRequestTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
+    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryTableResponseMetadataTypeDef,
+    BillingModeSummaryTableResponseMetadataTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
+    RestoreSummaryTableResponseMetadataTypeDef,
+    SSEDescriptionTableResponseMetadataTypeDef,
+    StreamSpecificationTableResponseMetadataTypeDef,
+    TableClassSummaryTableResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
+    DeleteRequestOutputTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
     GetItemInputRequestTypeDef,
     GetTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
+    KeysAndAttributesOutputTypeDef,
     KeysAndAttributesTypeDef,
     ParameterizedStatementTypeDef,
+    PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     BatchStatementResponseTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
-    LocalSecondaryIndexInfoTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexTypeDef,
-    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    GlobalTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
     ReplicaGlobalSecondaryIndexTableTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
     DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputTablePutItemTypeDef,
     UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
+    SourceTableDetailsTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
+    GlobalTableTypeDef,
     ImportSummaryTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
+    WriteRequestServiceResourceOutputTypeDef,
     WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    UpdateTimeToLiveInputRequestTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
     ExecuteTransactionInputRequestTypeDef,
+    WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
@@ -686,81 +714,82 @@
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     GlobalSecondaryIndexUpdateTableTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     CreateTableInputRequestTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    ListGlobalTablesOutputTypeDef,
-    ReplicaDescriptionTableTypeDef,
     CreateReplicationGroupMemberActionTableTypeDef,
     UpdateReplicationGroupMemberActionTableTypeDef,
-    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
+    SourceTableFeatureDetailsTypeDef,
+    TableCreationParametersOutputTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicaDescriptionTableTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     ImportTableInputRequestTypeDef,
-    TableDescriptionTableTypeDef,
     ReplicationGroupUpdateTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    BackupDescriptionTypeDef,
+    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    ReplicationGroupUpdateTypeDef,
+    TableDescriptionTableTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    UpdateTableInputRequestTypeDef,
     DeleteBackupOutputTypeDef,
     DescribeBackupOutputTypeDef,
     DescribeImportOutputTypeDef,
     ImportTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    UpdateTableInputRequestTypeDef,
+    DeleteTableOutputTableTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.5.2.post1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

