# Comparing `tmp/mypy-boto3-dms-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-dms-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dms-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+gzip compressed data, was "mypy-boto3-dms-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
```

## Comparing `mypy-boto3-dms-1.28.3.post1.tar` & `mypy-boto3-dms-1.28.3.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.899361 mypy-boto3-dms-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30941 2023-07-14 16:17:59.895360 mypy-boto3-dms-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29445 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74110 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    74004 2023-07-14 16:15:37.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17287 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   119853 2023-07-14 16:15:41.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   119790 2023-07-14 16:15:39.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-14 16:15:38.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30941 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 16:17:59.000000 mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.899361 mypy-boto3-dms-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-14 16:15:36.000000 mypy-boto3-dms-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.334244 mypy-boto3-dms-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30197 2023-07-15 06:38:32.322243 mypy-boto3-dms-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28701 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.314243 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73220 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73114 2023-07-15 06:36:05.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   117089 2023-07-15 06:36:10.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117026 2023-07-15 06:36:08.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-15 06:36:06.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.322243 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30197 2023-07-15 06:38:32.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-15 06:38:32.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 06:38:32.000000 mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.334244 mypy-boto3-dms-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-15 06:36:04.000000 mypy-boto3-dms-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-dms-1.28.3.post1/LICENSE` & `mypy-boto3-dms-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/PKG-INFO` & `mypy-boto3-dms-1.28.3.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,27 +472,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_dms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
-    AccountQuotaOutputTypeDef,
+    AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    AvailabilityZoneOutputTypeDef,
-    BatchStartRecommendationsErrorEntryOutputTypeDef,
+    AvailabilityZoneTypeDef,
+    BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
-    CertificateOutputTypeDef,
-    CollectorHealthCheckOutputTypeDef,
-    InventoryDataOutputTypeDef,
-    CollectorShortInfoResponseOutputTypeDef,
+    CertificateTypeDef,
+    CollectorHealthCheckTypeDef,
+    InventoryDataTypeDef,
+    CollectorShortInfoResponseTypeDef,
     ComputeConfigOutputTypeDef,
     ComputeConfigTypeDef,
-    ConnectionOutputTypeDef,
+    ConnectionTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
     KafkaSettingsTypeDef,
@@ -504,60 +504,60 @@
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
-    EventSubscriptionOutputTypeDef,
+    EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseOutputTypeDef,
-    DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
-    ServerShortInfoResponseOutputTypeDef,
-    DatabaseShortInfoResponseOutputTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    DatabaseInstanceSoftwareDetailsResponseTypeDef,
+    ServerShortInfoResponseTypeDef,
+    DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
-    EndpointSettingOutputTypeDef,
-    SupportedEndpointTypeOutputTypeDef,
-    EventCategoryGroupOutputTypeDef,
-    EventOutputTypeDef,
+    EndpointSettingTypeDef,
+    SupportedEndpointTypeTypeDef,
+    EventCategoryGroupTypeDef,
+    EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
-    FleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    FleetAdvisorSchemaObjectResponseOutputTypeDef,
+    FleetAdvisorLsaAnalysisResponseTypeDef,
+    FleetAdvisorSchemaObjectResponseTypeDef,
     DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
-    OrderableReplicationInstanceOutputTypeDef,
-    LimitationOutputTypeDef,
+    OrderableReplicationInstanceTypeDef,
+    LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
-    RefreshSchemasStatusOutputTypeDef,
+    RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
-    ReplicationInstanceTaskLogOutputTypeDef,
-    TableStatisticsOutputTypeDef,
+    ReplicationInstanceTaskLogTypeDef,
+    TableStatisticsTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
-    ReplicationTaskAssessmentResultOutputTypeDef,
-    ReplicationTaskIndividualAssessmentOutputTypeDef,
+    ReplicationTaskAssessmentResultTypeDef,
+    ReplicationTaskIndividualAssessmentTypeDef,
     DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
+    DescribeSchemasResponseTypeDef,
     DmsTransferSettingsOutputTypeDef,
     DocDbSettingsOutputTypeDef,
     DynamoDbSettingsOutputTypeDef,
     ElasticsearchSettingsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GcpMySQLSettingsOutputTypeDef,
     IBMDb2SettingsOutputTypeDef,
@@ -578,69 +578,69 @@
     TagOutputTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
     PaginatorConfigTypeDef,
-    PendingMaintenanceActionOutputTypeDef,
-    ProvisionDataOutputTypeDef,
-    RdsConfigurationOutputTypeDef,
-    RdsRequirementsOutputTypeDef,
+    PendingMaintenanceActionTypeDef,
+    ProvisionDataTypeDef,
+    RdsConfigurationTypeDef,
+    RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsOutputTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadReplicationTablesResponseOutputTypeDef,
-    ReloadTablesResponseOutputTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ReplicationPendingModifiedValuesOutputTypeDef,
-    VpcSecurityGroupMembershipOutputTypeDef,
-    ReplicationStatsOutputTypeDef,
-    ReplicationTaskAssessmentRunProgressOutputTypeDef,
-    ReplicationTaskStatsOutputTypeDef,
+    ReplicationPendingModifiedValuesTypeDef,
+    VpcSecurityGroupMembershipTypeDef,
+    ReplicationStatsTypeDef,
+    ReplicationTaskAssessmentRunProgressTypeDef,
+    ReplicationTaskStatsTypeDef,
     ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    SchemaShortInfoResponseOutputTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    SchemaShortInfoResponseTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
-    DescribeAccountAttributesResponseOutputTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    SubnetOutputTypeDef,
-    BatchStartRecommendationsResponseOutputTypeDef,
-    DeleteCertificateResponseOutputTypeDef,
-    DescribeCertificatesResponseOutputTypeDef,
-    ImportCertificateResponseOutputTypeDef,
-    CollectorResponseOutputTypeDef,
-    ReplicationConfigOutputTypeDef,
+    SubnetTypeDef,
+    BatchStartRecommendationsResponseTypeDef,
+    DeleteCertificateResponseTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    ImportCertificateResponseTypeDef,
+    CollectorResponseTypeDef,
+    ReplicationConfigTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
     ModifyReplicationConfigMessageRequestTypeDef,
-    DeleteConnectionResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    TestConnectionResponseOutputTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    TestConnectionResponseTypeDef,
     CreateEndpointMessageRequestTypeDef,
     ModifyEndpointMessageRequestTypeDef,
-    CreateEventSubscriptionResponseOutputTypeDef,
-    DeleteEventSubscriptionResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    ModifyEventSubscriptionResponseOutputTypeDef,
-    DatabaseResponseOutputTypeDef,
+    CreateEventSubscriptionResponseTypeDef,
+    DeleteEventSubscriptionResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    ModifyEventSubscriptionResponseTypeDef,
+    DatabaseResponseTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
     DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
     DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
@@ -674,87 +674,87 @@
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef,
-    DescribeEndpointSettingsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventCategoriesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribeRecommendationLimitationsResponseOutputTypeDef,
-    DescribeRefreshSchemasStatusResponseOutputTypeDef,
-    RefreshSchemasResponseOutputTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
-    DescribeReplicationTableStatisticsResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
-    EndpointOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ResourcePendingMaintenanceActionsOutputTypeDef,
-    RdsRecommendationOutputTypeDef,
+    DescribeEndpointSettingsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventCategoriesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribeRecommendationLimitationsResponseTypeDef,
+    DescribeRefreshSchemasStatusResponseTypeDef,
+    RefreshSchemasResponseTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
+    EndpointTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResourcePendingMaintenanceActionsTypeDef,
+    RdsRecommendationTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadReplicationTablesMessageRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
-    ReplicationOutputTypeDef,
-    ReplicationTaskAssessmentRunOutputTypeDef,
-    ReplicationTaskOutputTypeDef,
-    SchemaResponseOutputTypeDef,
-    ReplicationSubnetGroupOutputTypeDef,
-    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
-    CreateReplicationConfigResponseOutputTypeDef,
-    DeleteReplicationConfigResponseOutputTypeDef,
-    DescribeReplicationConfigsResponseOutputTypeDef,
-    ModifyReplicationConfigResponseOutputTypeDef,
-    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
-    CreateEndpointResponseOutputTypeDef,
-    DeleteEndpointResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    ModifyEndpointResponseOutputTypeDef,
-    ApplyPendingMaintenanceActionResponseOutputTypeDef,
-    DescribePendingMaintenanceActionsResponseOutputTypeDef,
-    RecommendationDataOutputTypeDef,
+    ReplicationTypeDef,
+    ReplicationTaskAssessmentRunTypeDef,
+    ReplicationTaskTypeDef,
+    SchemaResponseTypeDef,
+    ReplicationSubnetGroupTypeDef,
+    DescribeFleetAdvisorCollectorsResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    DeleteEndpointResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    ModifyEndpointResponseTypeDef,
+    ApplyPendingMaintenanceActionResponseTypeDef,
+    DescribePendingMaintenanceActionsResponseTypeDef,
+    RecommendationDataTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
-    DescribeReplicationsResponseOutputTypeDef,
-    StartReplicationResponseOutputTypeDef,
-    StopReplicationResponseOutputTypeDef,
-    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
-    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
-    CreateReplicationTaskResponseOutputTypeDef,
-    DeleteReplicationTaskResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    ModifyReplicationTaskResponseOutputTypeDef,
-    MoveReplicationTaskResponseOutputTypeDef,
-    StartReplicationTaskAssessmentResponseOutputTypeDef,
-    StartReplicationTaskResponseOutputTypeDef,
-    StopReplicationTaskResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
-    CreateReplicationSubnetGroupResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    ModifyReplicationSubnetGroupResponseOutputTypeDef,
-    ReplicationInstanceOutputTypeDef,
-    RecommendationOutputTypeDef,
-    CreateReplicationInstanceResponseOutputTypeDef,
-    DeleteReplicationInstanceResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    ModifyReplicationInstanceResponseOutputTypeDef,
-    RebootReplicationInstanceResponseOutputTypeDef,
-    DescribeRecommendationsResponseOutputTypeDef,
+    DescribeReplicationsResponseTypeDef,
+    StartReplicationResponseTypeDef,
+    StopReplicationResponseTypeDef,
+    CancelReplicationTaskAssessmentRunResponseTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
+    StartReplicationTaskAssessmentRunResponseTypeDef,
+    CreateReplicationTaskResponseTypeDef,
+    DeleteReplicationTaskResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    ModifyReplicationTaskResponseTypeDef,
+    MoveReplicationTaskResponseTypeDef,
+    StartReplicationTaskAssessmentResponseTypeDef,
+    StartReplicationTaskResponseTypeDef,
+    StopReplicationTaskResponseTypeDef,
+    DescribeFleetAdvisorSchemasResponseTypeDef,
+    CreateReplicationSubnetGroupResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    ModifyReplicationSubnetGroupResponseTypeDef,
+    ReplicationInstanceTypeDef,
+    RecommendationTypeDef,
+    CreateReplicationInstanceResponseTypeDef,
+    DeleteReplicationInstanceResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    ModifyReplicationInstanceResponseTypeDef,
+    RebootReplicationInstanceResponseTypeDef,
+    DescribeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaOutputTypeDef:
+def get_structure() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dms-1.28.3.post1/README.md` & `mypy-boto3-dms-1.28.3.post2/README.md`

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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -440,27 +440,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_dms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
-    AccountQuotaOutputTypeDef,
+    AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    AvailabilityZoneOutputTypeDef,
-    BatchStartRecommendationsErrorEntryOutputTypeDef,
+    AvailabilityZoneTypeDef,
+    BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
-    CertificateOutputTypeDef,
-    CollectorHealthCheckOutputTypeDef,
-    InventoryDataOutputTypeDef,
-    CollectorShortInfoResponseOutputTypeDef,
+    CertificateTypeDef,
+    CollectorHealthCheckTypeDef,
+    InventoryDataTypeDef,
+    CollectorShortInfoResponseTypeDef,
     ComputeConfigOutputTypeDef,
     ComputeConfigTypeDef,
-    ConnectionOutputTypeDef,
+    ConnectionTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
     KafkaSettingsTypeDef,
@@ -472,60 +472,60 @@
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
-    EventSubscriptionOutputTypeDef,
+    EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseOutputTypeDef,
-    DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
-    ServerShortInfoResponseOutputTypeDef,
-    DatabaseShortInfoResponseOutputTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    DatabaseInstanceSoftwareDetailsResponseTypeDef,
+    ServerShortInfoResponseTypeDef,
+    DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
-    EndpointSettingOutputTypeDef,
-    SupportedEndpointTypeOutputTypeDef,
-    EventCategoryGroupOutputTypeDef,
-    EventOutputTypeDef,
+    EndpointSettingTypeDef,
+    SupportedEndpointTypeTypeDef,
+    EventCategoryGroupTypeDef,
+    EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
-    FleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    FleetAdvisorSchemaObjectResponseOutputTypeDef,
+    FleetAdvisorLsaAnalysisResponseTypeDef,
+    FleetAdvisorSchemaObjectResponseTypeDef,
     DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
-    OrderableReplicationInstanceOutputTypeDef,
-    LimitationOutputTypeDef,
+    OrderableReplicationInstanceTypeDef,
+    LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
-    RefreshSchemasStatusOutputTypeDef,
+    RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
-    ReplicationInstanceTaskLogOutputTypeDef,
-    TableStatisticsOutputTypeDef,
+    ReplicationInstanceTaskLogTypeDef,
+    TableStatisticsTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
-    ReplicationTaskAssessmentResultOutputTypeDef,
-    ReplicationTaskIndividualAssessmentOutputTypeDef,
+    ReplicationTaskAssessmentResultTypeDef,
+    ReplicationTaskIndividualAssessmentTypeDef,
     DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
+    DescribeSchemasResponseTypeDef,
     DmsTransferSettingsOutputTypeDef,
     DocDbSettingsOutputTypeDef,
     DynamoDbSettingsOutputTypeDef,
     ElasticsearchSettingsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GcpMySQLSettingsOutputTypeDef,
     IBMDb2SettingsOutputTypeDef,
@@ -546,69 +546,69 @@
     TagOutputTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
     PaginatorConfigTypeDef,
-    PendingMaintenanceActionOutputTypeDef,
-    ProvisionDataOutputTypeDef,
-    RdsConfigurationOutputTypeDef,
-    RdsRequirementsOutputTypeDef,
+    PendingMaintenanceActionTypeDef,
+    ProvisionDataTypeDef,
+    RdsConfigurationTypeDef,
+    RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsOutputTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadReplicationTablesResponseOutputTypeDef,
-    ReloadTablesResponseOutputTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ReplicationPendingModifiedValuesOutputTypeDef,
-    VpcSecurityGroupMembershipOutputTypeDef,
-    ReplicationStatsOutputTypeDef,
-    ReplicationTaskAssessmentRunProgressOutputTypeDef,
-    ReplicationTaskStatsOutputTypeDef,
+    ReplicationPendingModifiedValuesTypeDef,
+    VpcSecurityGroupMembershipTypeDef,
+    ReplicationStatsTypeDef,
+    ReplicationTaskAssessmentRunProgressTypeDef,
+    ReplicationTaskStatsTypeDef,
     ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    SchemaShortInfoResponseOutputTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    SchemaShortInfoResponseTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
-    DescribeAccountAttributesResponseOutputTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    SubnetOutputTypeDef,
-    BatchStartRecommendationsResponseOutputTypeDef,
-    DeleteCertificateResponseOutputTypeDef,
-    DescribeCertificatesResponseOutputTypeDef,
-    ImportCertificateResponseOutputTypeDef,
-    CollectorResponseOutputTypeDef,
-    ReplicationConfigOutputTypeDef,
+    SubnetTypeDef,
+    BatchStartRecommendationsResponseTypeDef,
+    DeleteCertificateResponseTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    ImportCertificateResponseTypeDef,
+    CollectorResponseTypeDef,
+    ReplicationConfigTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
     ModifyReplicationConfigMessageRequestTypeDef,
-    DeleteConnectionResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    TestConnectionResponseOutputTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    TestConnectionResponseTypeDef,
     CreateEndpointMessageRequestTypeDef,
     ModifyEndpointMessageRequestTypeDef,
-    CreateEventSubscriptionResponseOutputTypeDef,
-    DeleteEventSubscriptionResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    ModifyEventSubscriptionResponseOutputTypeDef,
-    DatabaseResponseOutputTypeDef,
+    CreateEventSubscriptionResponseTypeDef,
+    DeleteEventSubscriptionResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    ModifyEventSubscriptionResponseTypeDef,
+    DatabaseResponseTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
     DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
     DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
@@ -642,87 +642,87 @@
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef,
-    DescribeEndpointSettingsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventCategoriesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribeRecommendationLimitationsResponseOutputTypeDef,
-    DescribeRefreshSchemasStatusResponseOutputTypeDef,
-    RefreshSchemasResponseOutputTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
-    DescribeReplicationTableStatisticsResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
-    EndpointOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ResourcePendingMaintenanceActionsOutputTypeDef,
-    RdsRecommendationOutputTypeDef,
+    DescribeEndpointSettingsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventCategoriesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribeRecommendationLimitationsResponseTypeDef,
+    DescribeRefreshSchemasStatusResponseTypeDef,
+    RefreshSchemasResponseTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
+    EndpointTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResourcePendingMaintenanceActionsTypeDef,
+    RdsRecommendationTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadReplicationTablesMessageRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
-    ReplicationOutputTypeDef,
-    ReplicationTaskAssessmentRunOutputTypeDef,
-    ReplicationTaskOutputTypeDef,
-    SchemaResponseOutputTypeDef,
-    ReplicationSubnetGroupOutputTypeDef,
-    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
-    CreateReplicationConfigResponseOutputTypeDef,
-    DeleteReplicationConfigResponseOutputTypeDef,
-    DescribeReplicationConfigsResponseOutputTypeDef,
-    ModifyReplicationConfigResponseOutputTypeDef,
-    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
-    CreateEndpointResponseOutputTypeDef,
-    DeleteEndpointResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    ModifyEndpointResponseOutputTypeDef,
-    ApplyPendingMaintenanceActionResponseOutputTypeDef,
-    DescribePendingMaintenanceActionsResponseOutputTypeDef,
-    RecommendationDataOutputTypeDef,
+    ReplicationTypeDef,
+    ReplicationTaskAssessmentRunTypeDef,
+    ReplicationTaskTypeDef,
+    SchemaResponseTypeDef,
+    ReplicationSubnetGroupTypeDef,
+    DescribeFleetAdvisorCollectorsResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    DeleteEndpointResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    ModifyEndpointResponseTypeDef,
+    ApplyPendingMaintenanceActionResponseTypeDef,
+    DescribePendingMaintenanceActionsResponseTypeDef,
+    RecommendationDataTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
-    DescribeReplicationsResponseOutputTypeDef,
-    StartReplicationResponseOutputTypeDef,
-    StopReplicationResponseOutputTypeDef,
-    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
-    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
-    CreateReplicationTaskResponseOutputTypeDef,
-    DeleteReplicationTaskResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    ModifyReplicationTaskResponseOutputTypeDef,
-    MoveReplicationTaskResponseOutputTypeDef,
-    StartReplicationTaskAssessmentResponseOutputTypeDef,
-    StartReplicationTaskResponseOutputTypeDef,
-    StopReplicationTaskResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
-    CreateReplicationSubnetGroupResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    ModifyReplicationSubnetGroupResponseOutputTypeDef,
-    ReplicationInstanceOutputTypeDef,
-    RecommendationOutputTypeDef,
-    CreateReplicationInstanceResponseOutputTypeDef,
-    DeleteReplicationInstanceResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    ModifyReplicationInstanceResponseOutputTypeDef,
-    RebootReplicationInstanceResponseOutputTypeDef,
-    DescribeRecommendationsResponseOutputTypeDef,
+    DescribeReplicationsResponseTypeDef,
+    StartReplicationResponseTypeDef,
+    StopReplicationResponseTypeDef,
+    CancelReplicationTaskAssessmentRunResponseTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
+    StartReplicationTaskAssessmentRunResponseTypeDef,
+    CreateReplicationTaskResponseTypeDef,
+    DeleteReplicationTaskResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    ModifyReplicationTaskResponseTypeDef,
+    MoveReplicationTaskResponseTypeDef,
+    StartReplicationTaskAssessmentResponseTypeDef,
+    StartReplicationTaskResponseTypeDef,
+    StopReplicationTaskResponseTypeDef,
+    DescribeFleetAdvisorSchemasResponseTypeDef,
+    CreateReplicationSubnetGroupResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    ModifyReplicationSubnetGroupResponseTypeDef,
+    ReplicationInstanceTypeDef,
+    RecommendationTypeDef,
+    CreateReplicationInstanceResponseTypeDef,
+    DeleteReplicationInstanceResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    ModifyReplicationInstanceResponseTypeDef,
+    RebootReplicationInstanceResponseTypeDef,
+    DescribeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaOutputTypeDef:
+def get_structure() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__init__.pyi` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/__main__.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.DatabaseMigrationService 1.28.3\nVersion:        "
-        " 1.28.3.post1\nBuilder version: 7.14.7\nDocs:           "
+        " 1.28.3.post2\nBuilder version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,113 +39,113 @@
     DescribeReplicationSubnetGroupsPaginator,
     DescribeReplicationTaskAssessmentResultsPaginator,
     DescribeReplicationTasksPaginator,
     DescribeSchemasPaginator,
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
-    ApplyPendingMaintenanceActionResponseOutputTypeDef,
-    BatchStartRecommendationsResponseOutputTypeDef,
-    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
+    ApplyPendingMaintenanceActionResponseTypeDef,
+    BatchStartRecommendationsResponseTypeDef,
+    CancelReplicationTaskAssessmentRunResponseTypeDef,
     ComputeConfigTypeDef,
-    CreateEndpointResponseOutputTypeDef,
-    CreateEventSubscriptionResponseOutputTypeDef,
-    CreateFleetAdvisorCollectorResponseOutputTypeDef,
-    CreateReplicationConfigResponseOutputTypeDef,
-    CreateReplicationInstanceResponseOutputTypeDef,
-    CreateReplicationSubnetGroupResponseOutputTypeDef,
-    CreateReplicationTaskResponseOutputTypeDef,
-    DeleteCertificateResponseOutputTypeDef,
-    DeleteConnectionResponseOutputTypeDef,
-    DeleteEndpointResponseOutputTypeDef,
-    DeleteEventSubscriptionResponseOutputTypeDef,
-    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
-    DeleteReplicationConfigResponseOutputTypeDef,
-    DeleteReplicationInstanceResponseOutputTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DeleteReplicationTaskResponseOutputTypeDef,
-    DescribeAccountAttributesResponseOutputTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
-    DescribeCertificatesResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    DescribeEndpointSettingsResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventCategoriesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
-    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribePendingMaintenanceActionsResponseOutputTypeDef,
-    DescribeRecommendationLimitationsResponseOutputTypeDef,
-    DescribeRecommendationsResponseOutputTypeDef,
-    DescribeRefreshSchemasStatusResponseOutputTypeDef,
-    DescribeReplicationConfigsResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
-    DescribeReplicationsResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    DescribeReplicationTableStatisticsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEventSubscriptionResponseTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
+    CreateReplicationInstanceResponseTypeDef,
+    CreateReplicationSubnetGroupResponseTypeDef,
+    CreateReplicationTaskResponseTypeDef,
+    DeleteCertificateResponseTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DeleteEndpointResponseTypeDef,
+    DeleteEventSubscriptionResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
+    DeleteReplicationInstanceResponseTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseTypeDef,
+    DeleteReplicationTaskResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    DescribeEndpointSettingsResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventCategoriesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    DescribeFleetAdvisorCollectorsResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
+    DescribeFleetAdvisorSchemasResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribePendingMaintenanceActionsResponseTypeDef,
+    DescribeRecommendationLimitationsResponseTypeDef,
+    DescribeRecommendationsResponseTypeDef,
+    DescribeRefreshSchemasStatusResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationsResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
-    ImportCertificateResponseOutputTypeDef,
+    ImportCertificateResponseTypeDef,
     KafkaSettingsTypeDef,
     KinesisSettingsTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MicrosoftSQLServerSettingsTypeDef,
-    ModifyEndpointResponseOutputTypeDef,
-    ModifyEventSubscriptionResponseOutputTypeDef,
-    ModifyReplicationConfigResponseOutputTypeDef,
-    ModifyReplicationInstanceResponseOutputTypeDef,
-    ModifyReplicationSubnetGroupResponseOutputTypeDef,
-    ModifyReplicationTaskResponseOutputTypeDef,
+    ModifyEndpointResponseTypeDef,
+    ModifyEventSubscriptionResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
+    ModifyReplicationInstanceResponseTypeDef,
+    ModifyReplicationSubnetGroupResponseTypeDef,
+    ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
-    MoveReplicationTaskResponseOutputTypeDef,
+    MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
-    RebootReplicationInstanceResponseOutputTypeDef,
+    RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
-    RefreshSchemasResponseOutputTypeDef,
-    ReloadReplicationTablesResponseOutputTypeDef,
-    ReloadTablesResponseOutputTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    RefreshSchemasResponseTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     S3SettingsTypeDef,
     StartRecommendationsRequestEntryTypeDef,
-    StartReplicationResponseOutputTypeDef,
-    StartReplicationTaskAssessmentResponseOutputTypeDef,
-    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
-    StartReplicationTaskResponseOutputTypeDef,
-    StopReplicationResponseOutputTypeDef,
-    StopReplicationTaskResponseOutputTypeDef,
+    StartReplicationResponseTypeDef,
+    StartReplicationTaskAssessmentResponseTypeDef,
+    StartReplicationTaskAssessmentRunResponseTypeDef,
+    StartReplicationTaskResponseTypeDef,
+    StopReplicationResponseTypeDef,
+    StopReplicationTaskResponseTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
-    TestConnectionResponseOutputTypeDef,
+    TestConnectionResponseTypeDef,
     TimestreamSettingsTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
     ReplicationTaskReadyWaiter,
@@ -226,26 +226,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.add_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#add_tags_to_resource)
         """
 
     def apply_pending_maintenance_action(
         self, *, ReplicationInstanceArn: str, ApplyAction: str, OptInType: str
-    ) -> ApplyPendingMaintenanceActionResponseOutputTypeDef:
+    ) -> ApplyPendingMaintenanceActionResponseTypeDef:
         """
         Applies a pending maintenance action to a resource (for example, to a
         replication instance).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.apply_pending_maintenance_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#apply_pending_maintenance_action)
         """
 
     def batch_start_recommendations(
         self, *, Data: Sequence[StartRecommendationsRequestEntryTypeDef] = ...
-    ) -> BatchStartRecommendationsResponseOutputTypeDef:
+    ) -> BatchStartRecommendationsResponseTypeDef:
         """
         Starts the analysis of up to 20 source databases to recommend target engines for
         each source database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.batch_start_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#batch_start_recommendations)
         """
@@ -256,15 +256,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#can_paginate)
         """
 
     def cancel_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> CancelReplicationTaskAssessmentRunResponseOutputTypeDef:
+    ) -> CancelReplicationTaskAssessmentRunResponseTypeDef:
         """
         Cancels a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.cancel_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#cancel_replication_task_assessment_run)
         """
 
@@ -310,15 +310,15 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> CreateEndpointResponseOutputTypeDef:
+    ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_endpoint)
         """
 
@@ -328,30 +328,30 @@
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventSubscriptionResponseOutputTypeDef:
+    ) -> CreateEventSubscriptionResponseTypeDef:
         """
         Creates an DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_event_subscription)
         """
 
     def create_fleet_advisor_collector(
         self,
         *,
         CollectorName: str,
         ServiceAccessRoleArn: str,
         S3BucketName: str,
         Description: str = ...
-    ) -> CreateFleetAdvisorCollectorResponseOutputTypeDef:
+    ) -> CreateFleetAdvisorCollectorResponseTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_fleet_advisor_collector)
         """
 
@@ -364,15 +364,15 @@
         ComputeConfig: ComputeConfigTypeDef,
         ReplicationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ResourceIdentifier: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationConfigResponseOutputTypeDef:
+    ) -> CreateReplicationConfigResponseTypeDef:
         """
         Creates a configuration that you can later provide to configure and start an DMS
         Serverless replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_config)
         """
@@ -392,30 +392,30 @@
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         PubliclyAccessible: bool = ...,
         DnsNameServers: str = ...,
         ResourceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> CreateReplicationInstanceResponseOutputTypeDef:
+    ) -> CreateReplicationInstanceResponseTypeDef:
         """
         Creates the replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_instance)
         """
 
     def create_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         ReplicationSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationSubnetGroupResponseOutputTypeDef:
+    ) -> CreateReplicationSubnetGroupResponseTypeDef:
         """
         Creates a replication subnet group given a list of the subnet IDs in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_subnet_group)
         """
 
@@ -431,51 +431,51 @@
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
         ResourceIdentifier: str = ...
-    ) -> CreateReplicationTaskResponseOutputTypeDef:
+    ) -> CreateReplicationTaskResponseTypeDef:
         """
         Creates a replication task using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_task)
         """
 
-    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseOutputTypeDef:
+    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseTypeDef:
         """
         Deletes the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_certificate)
         """
 
     def delete_connection(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> DeleteConnectionResponseOutputTypeDef:
+    ) -> DeleteConnectionResponseTypeDef:
         """
         Deletes the connection between a replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_connection)
         """
 
-    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseOutputTypeDef:
+    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseTypeDef:
         """
         Deletes the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_endpoint)
         """
 
     def delete_event_subscription(
         self, *, SubscriptionName: str
-    ) -> DeleteEventSubscriptionResponseOutputTypeDef:
+    ) -> DeleteEventSubscriptionResponseTypeDef:
         """
         Deletes an DMS event subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_event_subscription)
         """
 
@@ -487,35 +487,35 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_collector)
         """
 
     def delete_fleet_advisor_databases(
         self, *, DatabaseIds: Sequence[str]
-    ) -> DeleteFleetAdvisorDatabasesResponseOutputTypeDef:
+    ) -> DeleteFleetAdvisorDatabasesResponseTypeDef:
         """
         Deletes the specified Fleet Advisor collector databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_databases)
         """
 
     def delete_replication_config(
         self, *, ReplicationConfigArn: str
-    ) -> DeleteReplicationConfigResponseOutputTypeDef:
+    ) -> DeleteReplicationConfigResponseTypeDef:
         """
         Deletes an DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_config)
         """
 
     def delete_replication_instance(
         self, *, ReplicationInstanceArn: str
-    ) -> DeleteReplicationInstanceResponseOutputTypeDef:
+    ) -> DeleteReplicationInstanceResponseTypeDef:
         """
         Deletes the specified replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_instance)
         """
 
@@ -527,33 +527,33 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_subnet_group)
         """
 
     def delete_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> DeleteReplicationTaskResponseOutputTypeDef:
+    ) -> DeleteReplicationTaskResponseTypeDef:
         """
         Deletes the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task)
         """
 
     def delete_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> DeleteReplicationTaskAssessmentRunResponseOutputTypeDef:
+    ) -> DeleteReplicationTaskAssessmentRunResponseTypeDef:
         """
         Deletes the record of a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task_assessment_run)
         """
 
-    def describe_account_attributes(self) -> DescribeAccountAttributesResponseOutputTypeDef:
+    def describe_account_attributes(self) -> DescribeAccountAttributesResponseTypeDef:
         """
         Lists all of the DMS attributes for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_account_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_account_attributes)
         """
 
@@ -563,78 +563,78 @@
         ReplicationTaskArn: str = ...,
         ReplicationInstanceArn: str = ...,
         SourceEngineName: str = ...,
         TargetEngineName: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeApplicableIndividualAssessmentsResponseOutputTypeDef:
+    ) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:
         """
         Provides a list of individual assessments that you can specify for a new
         premigration assessment run, given one or more parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_applicable_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_applicable_individual_assessments)
         """
 
     def describe_certificates(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeCertificatesResponseOutputTypeDef:
+    ) -> DescribeCertificatesResponseTypeDef:
         """
         Provides a description of the certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_certificates)
         """
 
     def describe_connections(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeConnectionsResponseOutputTypeDef:
+    ) -> DescribeConnectionsResponseTypeDef:
         """
         Describes the status of the connections that have been made between the
         replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_connections)
         """
 
     def describe_endpoint_settings(
         self, *, EngineName: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointSettingsResponseOutputTypeDef:
+    ) -> DescribeEndpointSettingsResponseTypeDef:
         """
         Returns information about the possible endpoint settings available when you
         create an endpoint for a specific database engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_settings)
         """
 
     def describe_endpoint_types(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointTypesResponseOutputTypeDef:
+    ) -> DescribeEndpointTypesResponseTypeDef:
         """
         Returns information about the type of endpoints available.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_types)
         """
 
     def describe_endpoints(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointsResponseOutputTypeDef:
+    ) -> DescribeEndpointsResponseTypeDef:
         """
         Returns information about the endpoints for your account in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoints)
         """
 
     def describe_event_categories(
         self, *, SourceType: str = ..., Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeEventCategoriesResponseOutputTypeDef:
+    ) -> DescribeEventCategoriesResponseTypeDef:
         """
         Lists categories for all event source types, or, if specified, for a specified
         source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_categories)
         """
@@ -642,15 +642,15 @@
     def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventSubscriptionsResponseOutputTypeDef:
+    ) -> DescribeEventSubscriptionsResponseTypeDef:
         """
         Lists all the event subscriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_subscriptions)
         """
 
@@ -662,77 +662,77 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventsResponseOutputTypeDef:
+    ) -> DescribeEventsResponseTypeDef:
         """
         Lists events for a given source identifier and source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_events)
         """
 
     def describe_fleet_advisor_collectors(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorCollectorsResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorCollectorsResponseTypeDef:
         """
         Returns a list of the Fleet Advisor collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_collectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_collectors)
         """
 
     def describe_fleet_advisor_databases(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorDatabasesResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorDatabasesResponseTypeDef:
         """
         Returns a list of Fleet Advisor databases in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_databases)
         """
 
     def describe_fleet_advisor_lsa_analysis(
         self, *, MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorLsaAnalysisResponseTypeDef:
         """
         Provides descriptions of large-scale assessment (LSA) analyses produced by your
         Fleet Advisor collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_lsa_analysis)
         """
 
     def describe_fleet_advisor_schema_object_summary(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef:
         """
         Provides descriptions of the schemas discovered by your Fleet Advisor
         collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schema_object_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schema_object_summary)
         """
 
     def describe_fleet_advisor_schemas(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemasResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorSchemasResponseTypeDef:
         """
         Returns a list of schemas detected by Fleet Advisor Collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schemas)
         """
 
     def describe_orderable_replication_instances(
         self, *, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeOrderableReplicationInstancesResponseOutputTypeDef:
+    ) -> DescribeOrderableReplicationInstancesResponseTypeDef:
         """
         Returns information about the replication instance types that can be created in
         the specified region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_orderable_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_orderable_replication_instances)
         """
@@ -740,190 +740,190 @@
     def describe_pending_maintenance_actions(
         self,
         *,
         ReplicationInstanceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
-    ) -> DescribePendingMaintenanceActionsResponseOutputTypeDef:
+    ) -> DescribePendingMaintenanceActionsResponseTypeDef:
         """
         For internal use only See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/dms-2016-01-01/DescribePendingMaintenanceActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_pending_maintenance_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_pending_maintenance_actions)
         """
 
     def describe_recommendation_limitations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationLimitationsResponseOutputTypeDef:
+    ) -> DescribeRecommendationLimitationsResponseTypeDef:
         """
         Returns a paginated list of limitations for recommendations of target Amazon Web
         Services engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendation_limitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendation_limitations)
         """
 
     def describe_recommendations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationsResponseOutputTypeDef:
+    ) -> DescribeRecommendationsResponseTypeDef:
         """
         Returns a paginated list of target engine recommendations for your source
         databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendations)
         """
 
     def describe_refresh_schemas_status(
         self, *, EndpointArn: str
-    ) -> DescribeRefreshSchemasStatusResponseOutputTypeDef:
+    ) -> DescribeRefreshSchemasStatusResponseTypeDef:
         """
         Returns the status of the RefreshSchemas operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_refresh_schemas_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_refresh_schemas_status)
         """
 
     def describe_replication_configs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationConfigsResponseOutputTypeDef:
+    ) -> DescribeReplicationConfigsResponseTypeDef:
         """
         Returns one or more existing DMS Serverless replication configurations as a list
         of structures.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_configs)
         """
 
     def describe_replication_instance_task_logs(
         self, *, ReplicationInstanceArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstanceTaskLogsResponseOutputTypeDef:
+    ) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:
         """
         Returns information about the task logs for the specified task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instance_task_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instance_task_logs)
         """
 
     def describe_replication_instances(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstancesResponseOutputTypeDef:
+    ) -> DescribeReplicationInstancesResponseTypeDef:
         """
         Returns information about replication instances for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instances)
         """
 
     def describe_replication_subnet_groups(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationSubnetGroupsResponseOutputTypeDef:
+    ) -> DescribeReplicationSubnetGroupsResponseTypeDef:
         """
         Returns information about the replication subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_subnet_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_subnet_groups)
         """
 
     def describe_replication_table_statistics(
         self,
         *,
         ReplicationConfigArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeReplicationTableStatisticsResponseOutputTypeDef:
+    ) -> DescribeReplicationTableStatisticsResponseTypeDef:
         """
         Returns table and schema statistics for one or more provisioned replications
         that use a given DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_table_statistics)
         """
 
     def describe_replication_task_assessment_results(
         self, *, ReplicationTaskArn: str = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef:
+    ) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:
         """
         Returns the task assessment results from the Amazon S3 bucket that DMS creates
         in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_results)
         """
 
     def describe_replication_task_assessment_runs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef:
+    ) -> DescribeReplicationTaskAssessmentRunsResponseTypeDef:
         """
         Returns a paginated list of premigration assessment runs based on filter
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_runs)
         """
 
     def describe_replication_task_individual_assessments(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef:
+    ) -> DescribeReplicationTaskIndividualAssessmentsResponseTypeDef:
         """
         Returns a paginated list of individual assessments based on filter settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_individual_assessments)
         """
 
     def describe_replication_tasks(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...
-    ) -> DescribeReplicationTasksResponseOutputTypeDef:
+    ) -> DescribeReplicationTasksResponseTypeDef:
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_tasks)
         """
 
     def describe_replications(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationsResponseOutputTypeDef:
+    ) -> DescribeReplicationsResponseTypeDef:
         """
         Provides details on replication progress by returning status information for one
         or more provisioned DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replications)
         """
 
     def describe_schemas(
         self, *, EndpointArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeSchemasResponseOutputTypeDef:
+    ) -> DescribeSchemasResponseTypeDef:
         """
         Returns information about the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_schemas)
         """
 
     def describe_table_statistics(
         self,
         *,
         ReplicationTaskArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeTableStatisticsResponseOutputTypeDef:
+    ) -> DescribeTableStatisticsResponseTypeDef:
         """
         Returns table statistics on the database migration task, including table name,
         rows inserted, rows updated, and rows deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_table_statistics)
         """
@@ -945,25 +945,25 @@
     def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
         CertificateWallet: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ImportCertificateResponseOutputTypeDef:
+    ) -> ImportCertificateResponseTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#import_certificate)
         """
 
     def list_tags_for_resource(
         self, *, ResourceArn: str = ..., ResourceArnList: Sequence[str] = ...
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all metadata tags attached to an DMS resource, including replication
         instance, endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#list_tags_for_resource)
         """
@@ -1001,15 +1001,15 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> ModifyEndpointResponseOutputTypeDef:
+    ) -> ModifyEndpointResponseTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_endpoint)
         """
 
@@ -1017,15 +1017,15 @@
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         Enabled: bool = ...
-    ) -> ModifyEventSubscriptionResponseOutputTypeDef:
+    ) -> ModifyEventSubscriptionResponseTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_event_subscription)
         """
 
@@ -1037,15 +1037,15 @@
         ReplicationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ComputeConfig: ComputeConfigTypeDef = ...,
         SourceEndpointArn: str = ...,
         TargetEndpointArn: str = ...
-    ) -> ModifyReplicationConfigResponseOutputTypeDef:
+    ) -> ModifyReplicationConfigResponseTypeDef:
         """
         Modifies an existing DMS Serverless replication configuration that you can use
         to start a replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_config)
         """
@@ -1061,29 +1061,29 @@
         PreferredMaintenanceWindow: str = ...,
         MultiAZ: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         AutoMinorVersionUpgrade: bool = ...,
         ReplicationInstanceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> ModifyReplicationInstanceResponseOutputTypeDef:
+    ) -> ModifyReplicationInstanceResponseTypeDef:
         """
         Modifies the replication instance to apply new settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_instance)
         """
 
     def modify_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         SubnetIds: Sequence[str],
         ReplicationSubnetGroupDescription: str = ...
-    ) -> ModifyReplicationSubnetGroupResponseOutputTypeDef:
+    ) -> ModifyReplicationSubnetGroupResponseTypeDef:
         """
         Modifies the settings for the specified replication subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_subnet_group)
         """
 
@@ -1095,79 +1095,79 @@
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         TaskData: str = ...
-    ) -> ModifyReplicationTaskResponseOutputTypeDef:
+    ) -> ModifyReplicationTaskResponseTypeDef:
         """
         Modifies the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_task)
         """
 
     def move_replication_task(
         self, *, ReplicationTaskArn: str, TargetReplicationInstanceArn: str
-    ) -> MoveReplicationTaskResponseOutputTypeDef:
+    ) -> MoveReplicationTaskResponseTypeDef:
         """
         Moves a replication task from its current replication instance to a different
         target replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.move_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#move_replication_task)
         """
 
     def reboot_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         ForceFailover: bool = ...,
         ForcePlannedFailover: bool = ...
-    ) -> RebootReplicationInstanceResponseOutputTypeDef:
+    ) -> RebootReplicationInstanceResponseTypeDef:
         """
         Reboots a replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reboot_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reboot_replication_instance)
         """
 
     def refresh_schemas(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> RefreshSchemasResponseOutputTypeDef:
+    ) -> RefreshSchemasResponseTypeDef:
         """
         Populates the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.refresh_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#refresh_schemas)
         """
 
     def reload_replication_tables(
         self,
         *,
         ReplicationConfigArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadReplicationTablesResponseOutputTypeDef:
+    ) -> ReloadReplicationTablesResponseTypeDef:
         """
         Reloads the target database table with the source data for a given DMS
         Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_replication_tables)
         """
 
     def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadTablesResponseOutputTypeDef:
+    ) -> ReloadTablesResponseTypeDef:
         """
         Reloads the target database table with the source data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_tables)
         """
 
@@ -1178,15 +1178,15 @@
         Removes metadata tags from an DMS resource, including replication instance,
         endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.remove_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#remove_tags_from_resource)
         """
 
-    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseOutputTypeDef:
+    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseTypeDef:
         """
         Runs large-scale assessment (LSA) analysis on every Fleet Advisor collector in
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.run_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#run_fleet_advisor_lsa_analysis)
         """
@@ -1206,15 +1206,15 @@
         self,
         *,
         ReplicationConfigArn: str,
         StartReplicationType: str,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationResponseOutputTypeDef:
+    ) -> StartReplicationResponseTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS connects to the source
         endpoint and collects the metadata to analyze the replication workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication)
         """
@@ -1223,25 +1223,25 @@
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationTaskResponseOutputTypeDef:
+    ) -> StartReplicationTaskResponseTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task)
         """
 
     def start_replication_task_assessment(
         self, *, ReplicationTaskArn: str
-    ) -> StartReplicationTaskAssessmentResponseOutputTypeDef:
+    ) -> StartReplicationTaskAssessmentResponseTypeDef:
         """
         Starts the replication task assessment for unsupported data types in the source
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment)
         """
@@ -1254,57 +1254,55 @@
         ResultLocationBucket: str,
         AssessmentRunName: str,
         ResultLocationFolder: str = ...,
         ResultEncryptionMode: str = ...,
         ResultKmsKeyArn: str = ...,
         IncludeOnly: Sequence[str] = ...,
         Exclude: Sequence[str] = ...
-    ) -> StartReplicationTaskAssessmentRunResponseOutputTypeDef:
+    ) -> StartReplicationTaskAssessmentRunResponseTypeDef:
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment_run)
         """
 
-    def stop_replication(
-        self, *, ReplicationConfigArn: str
-    ) -> StopReplicationResponseOutputTypeDef:
+    def stop_replication(self, *, ReplicationConfigArn: str) -> StopReplicationResponseTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS stops any and all
         ongoing DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication)
         """
 
     def stop_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> StopReplicationTaskResponseOutputTypeDef:
+    ) -> StopReplicationTaskResponseTypeDef:
         """
         Stops the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication_task)
         """
 
     def test_connection(
         self, *, ReplicationInstanceArn: str, EndpointArn: str
-    ) -> TestConnectionResponseOutputTypeDef:
+    ) -> TestConnectionResponseTypeDef:
         """
         Tests the connection between the replication instance and the endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.test_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#test_connection)
         """
 
     def update_subscriptions_to_event_bridge(
         self, *, ForceMove: bool = ...
-    ) -> UpdateSubscriptionsToEventBridgeResponseOutputTypeDef:
+    ) -> UpdateSubscriptionsToEventBridgeResponseTypeDef:
         """
         Migrates 10 active and enabled Amazon SNS subscriptions at a time and converts
         them to corresponding Amazon EventBridge rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.update_subscriptions_to_event_bridge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#update_subscriptions_to_event_bridge)
         """
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/client.pyi` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -39,113 +39,113 @@
     DescribeReplicationSubnetGroupsPaginator,
     DescribeReplicationTaskAssessmentResultsPaginator,
     DescribeReplicationTasksPaginator,
     DescribeSchemasPaginator,
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
-    ApplyPendingMaintenanceActionResponseOutputTypeDef,
-    BatchStartRecommendationsResponseOutputTypeDef,
-    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
+    ApplyPendingMaintenanceActionResponseTypeDef,
+    BatchStartRecommendationsResponseTypeDef,
+    CancelReplicationTaskAssessmentRunResponseTypeDef,
     ComputeConfigTypeDef,
-    CreateEndpointResponseOutputTypeDef,
-    CreateEventSubscriptionResponseOutputTypeDef,
-    CreateFleetAdvisorCollectorResponseOutputTypeDef,
-    CreateReplicationConfigResponseOutputTypeDef,
-    CreateReplicationInstanceResponseOutputTypeDef,
-    CreateReplicationSubnetGroupResponseOutputTypeDef,
-    CreateReplicationTaskResponseOutputTypeDef,
-    DeleteCertificateResponseOutputTypeDef,
-    DeleteConnectionResponseOutputTypeDef,
-    DeleteEndpointResponseOutputTypeDef,
-    DeleteEventSubscriptionResponseOutputTypeDef,
-    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
-    DeleteReplicationConfigResponseOutputTypeDef,
-    DeleteReplicationInstanceResponseOutputTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DeleteReplicationTaskResponseOutputTypeDef,
-    DescribeAccountAttributesResponseOutputTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
-    DescribeCertificatesResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    DescribeEndpointSettingsResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventCategoriesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
-    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribePendingMaintenanceActionsResponseOutputTypeDef,
-    DescribeRecommendationLimitationsResponseOutputTypeDef,
-    DescribeRecommendationsResponseOutputTypeDef,
-    DescribeRefreshSchemasStatusResponseOutputTypeDef,
-    DescribeReplicationConfigsResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
-    DescribeReplicationsResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    DescribeReplicationTableStatisticsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEventSubscriptionResponseTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
+    CreateReplicationInstanceResponseTypeDef,
+    CreateReplicationSubnetGroupResponseTypeDef,
+    CreateReplicationTaskResponseTypeDef,
+    DeleteCertificateResponseTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DeleteEndpointResponseTypeDef,
+    DeleteEventSubscriptionResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
+    DeleteReplicationInstanceResponseTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseTypeDef,
+    DeleteReplicationTaskResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    DescribeEndpointSettingsResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventCategoriesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    DescribeFleetAdvisorCollectorsResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
+    DescribeFleetAdvisorSchemasResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribePendingMaintenanceActionsResponseTypeDef,
+    DescribeRecommendationLimitationsResponseTypeDef,
+    DescribeRecommendationsResponseTypeDef,
+    DescribeRefreshSchemasStatusResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationsResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
-    ImportCertificateResponseOutputTypeDef,
+    ImportCertificateResponseTypeDef,
     KafkaSettingsTypeDef,
     KinesisSettingsTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MicrosoftSQLServerSettingsTypeDef,
-    ModifyEndpointResponseOutputTypeDef,
-    ModifyEventSubscriptionResponseOutputTypeDef,
-    ModifyReplicationConfigResponseOutputTypeDef,
-    ModifyReplicationInstanceResponseOutputTypeDef,
-    ModifyReplicationSubnetGroupResponseOutputTypeDef,
-    ModifyReplicationTaskResponseOutputTypeDef,
+    ModifyEndpointResponseTypeDef,
+    ModifyEventSubscriptionResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
+    ModifyReplicationInstanceResponseTypeDef,
+    ModifyReplicationSubnetGroupResponseTypeDef,
+    ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
-    MoveReplicationTaskResponseOutputTypeDef,
+    MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
-    RebootReplicationInstanceResponseOutputTypeDef,
+    RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
-    RefreshSchemasResponseOutputTypeDef,
-    ReloadReplicationTablesResponseOutputTypeDef,
-    ReloadTablesResponseOutputTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
+    RefreshSchemasResponseTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     S3SettingsTypeDef,
     StartRecommendationsRequestEntryTypeDef,
-    StartReplicationResponseOutputTypeDef,
-    StartReplicationTaskAssessmentResponseOutputTypeDef,
-    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
-    StartReplicationTaskResponseOutputTypeDef,
-    StopReplicationResponseOutputTypeDef,
-    StopReplicationTaskResponseOutputTypeDef,
+    StartReplicationResponseTypeDef,
+    StartReplicationTaskAssessmentResponseTypeDef,
+    StartReplicationTaskAssessmentRunResponseTypeDef,
+    StartReplicationTaskResponseTypeDef,
+    StopReplicationResponseTypeDef,
+    StopReplicationTaskResponseTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
-    TestConnectionResponseOutputTypeDef,
+    TestConnectionResponseTypeDef,
     TimestreamSettingsTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
     ReplicationTaskReadyWaiter,
@@ -220,25 +220,25 @@
         subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.add_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#add_tags_to_resource)
         """
     def apply_pending_maintenance_action(
         self, *, ReplicationInstanceArn: str, ApplyAction: str, OptInType: str
-    ) -> ApplyPendingMaintenanceActionResponseOutputTypeDef:
+    ) -> ApplyPendingMaintenanceActionResponseTypeDef:
         """
         Applies a pending maintenance action to a resource (for example, to a
         replication instance).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.apply_pending_maintenance_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#apply_pending_maintenance_action)
         """
     def batch_start_recommendations(
         self, *, Data: Sequence[StartRecommendationsRequestEntryTypeDef] = ...
-    ) -> BatchStartRecommendationsResponseOutputTypeDef:
+    ) -> BatchStartRecommendationsResponseTypeDef:
         """
         Starts the analysis of up to 20 source databases to recommend target engines for
         each source database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.batch_start_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#batch_start_recommendations)
         """
@@ -247,15 +247,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#can_paginate)
         """
     def cancel_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> CancelReplicationTaskAssessmentRunResponseOutputTypeDef:
+    ) -> CancelReplicationTaskAssessmentRunResponseTypeDef:
         """
         Cancels a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.cancel_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#cancel_replication_task_assessment_run)
         """
     def close(self) -> None:
@@ -299,15 +299,15 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> CreateEndpointResponseOutputTypeDef:
+    ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_endpoint)
         """
     def create_event_subscription(
@@ -316,29 +316,29 @@
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventSubscriptionResponseOutputTypeDef:
+    ) -> CreateEventSubscriptionResponseTypeDef:
         """
         Creates an DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_event_subscription)
         """
     def create_fleet_advisor_collector(
         self,
         *,
         CollectorName: str,
         ServiceAccessRoleArn: str,
         S3BucketName: str,
         Description: str = ...
-    ) -> CreateFleetAdvisorCollectorResponseOutputTypeDef:
+    ) -> CreateFleetAdvisorCollectorResponseTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_fleet_advisor_collector)
         """
     def create_replication_config(
@@ -350,15 +350,15 @@
         ComputeConfig: ComputeConfigTypeDef,
         ReplicationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ResourceIdentifier: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationConfigResponseOutputTypeDef:
+    ) -> CreateReplicationConfigResponseTypeDef:
         """
         Creates a configuration that you can later provide to configure and start an DMS
         Serverless replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_config)
         """
@@ -377,29 +377,29 @@
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         PubliclyAccessible: bool = ...,
         DnsNameServers: str = ...,
         ResourceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> CreateReplicationInstanceResponseOutputTypeDef:
+    ) -> CreateReplicationInstanceResponseTypeDef:
         """
         Creates the replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_instance)
         """
     def create_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         ReplicationSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateReplicationSubnetGroupResponseOutputTypeDef:
+    ) -> CreateReplicationSubnetGroupResponseTypeDef:
         """
         Creates a replication subnet group given a list of the subnet IDs in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_subnet_group)
         """
     def create_replication_task(
@@ -414,47 +414,47 @@
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
         ResourceIdentifier: str = ...
-    ) -> CreateReplicationTaskResponseOutputTypeDef:
+    ) -> CreateReplicationTaskResponseTypeDef:
         """
         Creates a replication task using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#create_replication_task)
         """
-    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseOutputTypeDef:
+    def delete_certificate(self, *, CertificateArn: str) -> DeleteCertificateResponseTypeDef:
         """
         Deletes the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_certificate)
         """
     def delete_connection(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> DeleteConnectionResponseOutputTypeDef:
+    ) -> DeleteConnectionResponseTypeDef:
         """
         Deletes the connection between a replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_connection)
         """
-    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseOutputTypeDef:
+    def delete_endpoint(self, *, EndpointArn: str) -> DeleteEndpointResponseTypeDef:
         """
         Deletes the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_endpoint)
         """
     def delete_event_subscription(
         self, *, SubscriptionName: str
-    ) -> DeleteEventSubscriptionResponseOutputTypeDef:
+    ) -> DeleteEventSubscriptionResponseTypeDef:
         """
         Deletes an DMS event subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_event_subscription)
         """
     def delete_fleet_advisor_collector(
@@ -464,33 +464,33 @@
         Deletes the specified Fleet Advisor collector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_collector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_collector)
         """
     def delete_fleet_advisor_databases(
         self, *, DatabaseIds: Sequence[str]
-    ) -> DeleteFleetAdvisorDatabasesResponseOutputTypeDef:
+    ) -> DeleteFleetAdvisorDatabasesResponseTypeDef:
         """
         Deletes the specified Fleet Advisor collector databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_fleet_advisor_databases)
         """
     def delete_replication_config(
         self, *, ReplicationConfigArn: str
-    ) -> DeleteReplicationConfigResponseOutputTypeDef:
+    ) -> DeleteReplicationConfigResponseTypeDef:
         """
         Deletes an DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_config)
         """
     def delete_replication_instance(
         self, *, ReplicationInstanceArn: str
-    ) -> DeleteReplicationInstanceResponseOutputTypeDef:
+    ) -> DeleteReplicationInstanceResponseTypeDef:
         """
         Deletes the specified replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_instance)
         """
     def delete_replication_subnet_group(
@@ -500,31 +500,31 @@
         Deletes a subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_subnet_group)
         """
     def delete_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> DeleteReplicationTaskResponseOutputTypeDef:
+    ) -> DeleteReplicationTaskResponseTypeDef:
         """
         Deletes the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task)
         """
     def delete_replication_task_assessment_run(
         self, *, ReplicationTaskAssessmentRunArn: str
-    ) -> DeleteReplicationTaskAssessmentRunResponseOutputTypeDef:
+    ) -> DeleteReplicationTaskAssessmentRunResponseTypeDef:
         """
         Deletes the record of a single premigration assessment run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#delete_replication_task_assessment_run)
         """
-    def describe_account_attributes(self) -> DescribeAccountAttributesResponseOutputTypeDef:
+    def describe_account_attributes(self) -> DescribeAccountAttributesResponseTypeDef:
         """
         Lists all of the DMS attributes for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_account_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_account_attributes)
         """
     def describe_applicable_individual_assessments(
@@ -533,87 +533,87 @@
         ReplicationTaskArn: str = ...,
         ReplicationInstanceArn: str = ...,
         SourceEngineName: str = ...,
         TargetEngineName: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeApplicableIndividualAssessmentsResponseOutputTypeDef:
+    ) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:
         """
         Provides a list of individual assessments that you can specify for a new
         premigration assessment run, given one or more parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_applicable_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_applicable_individual_assessments)
         """
     def describe_certificates(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeCertificatesResponseOutputTypeDef:
+    ) -> DescribeCertificatesResponseTypeDef:
         """
         Provides a description of the certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_certificates)
         """
     def describe_connections(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeConnectionsResponseOutputTypeDef:
+    ) -> DescribeConnectionsResponseTypeDef:
         """
         Describes the status of the connections that have been made between the
         replication instance and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_connections)
         """
     def describe_endpoint_settings(
         self, *, EngineName: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointSettingsResponseOutputTypeDef:
+    ) -> DescribeEndpointSettingsResponseTypeDef:
         """
         Returns information about the possible endpoint settings available when you
         create an endpoint for a specific database engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_settings)
         """
     def describe_endpoint_types(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointTypesResponseOutputTypeDef:
+    ) -> DescribeEndpointTypesResponseTypeDef:
         """
         Returns information about the type of endpoints available.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoint_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoint_types)
         """
     def describe_endpoints(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeEndpointsResponseOutputTypeDef:
+    ) -> DescribeEndpointsResponseTypeDef:
         """
         Returns information about the endpoints for your account in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_endpoints)
         """
     def describe_event_categories(
         self, *, SourceType: str = ..., Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeEventCategoriesResponseOutputTypeDef:
+    ) -> DescribeEventCategoriesResponseTypeDef:
         """
         Lists categories for all event source types, or, if specified, for a specified
         source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_categories)
         """
     def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventSubscriptionsResponseOutputTypeDef:
+    ) -> DescribeEventSubscriptionsResponseTypeDef:
         """
         Lists all the event subscriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_event_subscriptions)
         """
     def describe_events(
@@ -624,246 +624,246 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
-    ) -> DescribeEventsResponseOutputTypeDef:
+    ) -> DescribeEventsResponseTypeDef:
         """
         Lists events for a given source identifier and source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_events)
         """
     def describe_fleet_advisor_collectors(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorCollectorsResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorCollectorsResponseTypeDef:
         """
         Returns a list of the Fleet Advisor collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_collectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_collectors)
         """
     def describe_fleet_advisor_databases(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorDatabasesResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorDatabasesResponseTypeDef:
         """
         Returns a list of Fleet Advisor databases in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_databases)
         """
     def describe_fleet_advisor_lsa_analysis(
         self, *, MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorLsaAnalysisResponseTypeDef:
         """
         Provides descriptions of large-scale assessment (LSA) analyses produced by your
         Fleet Advisor collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_lsa_analysis)
         """
     def describe_fleet_advisor_schema_object_summary(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef:
         """
         Provides descriptions of the schemas discovered by your Fleet Advisor
         collectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schema_object_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schema_object_summary)
         """
     def describe_fleet_advisor_schemas(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeFleetAdvisorSchemasResponseOutputTypeDef:
+    ) -> DescribeFleetAdvisorSchemasResponseTypeDef:
         """
         Returns a list of schemas detected by Fleet Advisor Collectors in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_fleet_advisor_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_fleet_advisor_schemas)
         """
     def describe_orderable_replication_instances(
         self, *, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeOrderableReplicationInstancesResponseOutputTypeDef:
+    ) -> DescribeOrderableReplicationInstancesResponseTypeDef:
         """
         Returns information about the replication instance types that can be created in
         the specified region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_orderable_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_orderable_replication_instances)
         """
     def describe_pending_maintenance_actions(
         self,
         *,
         ReplicationInstanceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
-    ) -> DescribePendingMaintenanceActionsResponseOutputTypeDef:
+    ) -> DescribePendingMaintenanceActionsResponseTypeDef:
         """
         For internal use only See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/dms-2016-01-01/DescribePendingMaintenanceActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_pending_maintenance_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_pending_maintenance_actions)
         """
     def describe_recommendation_limitations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationLimitationsResponseOutputTypeDef:
+    ) -> DescribeRecommendationLimitationsResponseTypeDef:
         """
         Returns a paginated list of limitations for recommendations of target Amazon Web
         Services engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendation_limitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendation_limitations)
         """
     def describe_recommendations(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., NextToken: str = ...
-    ) -> DescribeRecommendationsResponseOutputTypeDef:
+    ) -> DescribeRecommendationsResponseTypeDef:
         """
         Returns a paginated list of target engine recommendations for your source
         databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_recommendations)
         """
     def describe_refresh_schemas_status(
         self, *, EndpointArn: str
-    ) -> DescribeRefreshSchemasStatusResponseOutputTypeDef:
+    ) -> DescribeRefreshSchemasStatusResponseTypeDef:
         """
         Returns the status of the RefreshSchemas operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_refresh_schemas_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_refresh_schemas_status)
         """
     def describe_replication_configs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationConfigsResponseOutputTypeDef:
+    ) -> DescribeReplicationConfigsResponseTypeDef:
         """
         Returns one or more existing DMS Serverless replication configurations as a list
         of structures.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_configs)
         """
     def describe_replication_instance_task_logs(
         self, *, ReplicationInstanceArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstanceTaskLogsResponseOutputTypeDef:
+    ) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:
         """
         Returns information about the task logs for the specified task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instance_task_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instance_task_logs)
         """
     def describe_replication_instances(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationInstancesResponseOutputTypeDef:
+    ) -> DescribeReplicationInstancesResponseTypeDef:
         """
         Returns information about replication instances for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_instances)
         """
     def describe_replication_subnet_groups(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationSubnetGroupsResponseOutputTypeDef:
+    ) -> DescribeReplicationSubnetGroupsResponseTypeDef:
         """
         Returns information about the replication subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_subnet_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_subnet_groups)
         """
     def describe_replication_table_statistics(
         self,
         *,
         ReplicationConfigArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeReplicationTableStatisticsResponseOutputTypeDef:
+    ) -> DescribeReplicationTableStatisticsResponseTypeDef:
         """
         Returns table and schema statistics for one or more provisioned replications
         that use a given DMS Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_table_statistics)
         """
     def describe_replication_task_assessment_results(
         self, *, ReplicationTaskArn: str = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef:
+    ) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:
         """
         Returns the task assessment results from the Amazon S3 bucket that DMS creates
         in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_results)
         """
     def describe_replication_task_assessment_runs(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef:
+    ) -> DescribeReplicationTaskAssessmentRunsResponseTypeDef:
         """
         Returns a paginated list of premigration assessment runs based on filter
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_assessment_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_assessment_runs)
         """
     def describe_replication_task_individual_assessments(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef:
+    ) -> DescribeReplicationTaskIndividualAssessmentsResponseTypeDef:
         """
         Returns a paginated list of individual assessments based on filter settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_task_individual_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_task_individual_assessments)
         """
     def describe_replication_tasks(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...
-    ) -> DescribeReplicationTasksResponseOutputTypeDef:
+    ) -> DescribeReplicationTasksResponseTypeDef:
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replication_tasks)
         """
     def describe_replications(
         self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeReplicationsResponseOutputTypeDef:
+    ) -> DescribeReplicationsResponseTypeDef:
         """
         Provides details on replication progress by returning status information for one
         or more provisioned DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_replications)
         """
     def describe_schemas(
         self, *, EndpointArn: str, MaxRecords: int = ..., Marker: str = ...
-    ) -> DescribeSchemasResponseOutputTypeDef:
+    ) -> DescribeSchemasResponseTypeDef:
         """
         Returns information about the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_schemas)
         """
     def describe_table_statistics(
         self,
         *,
         ReplicationTaskArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
-    ) -> DescribeTableStatisticsResponseOutputTypeDef:
+    ) -> DescribeTableStatisticsResponseTypeDef:
         """
         Returns table statistics on the database migration task, including table name,
         rows inserted, rows updated, and rows deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_table_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#describe_table_statistics)
         """
@@ -883,24 +883,24 @@
     def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
         CertificateWallet: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ImportCertificateResponseOutputTypeDef:
+    ) -> ImportCertificateResponseTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#import_certificate)
         """
     def list_tags_for_resource(
         self, *, ResourceArn: str = ..., ResourceArnList: Sequence[str] = ...
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all metadata tags attached to an DMS resource, including replication
         instance, endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#list_tags_for_resource)
         """
@@ -937,30 +937,30 @@
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
         TimestreamSettings: TimestreamSettingsTypeDef = ...
-    ) -> ModifyEndpointResponseOutputTypeDef:
+    ) -> ModifyEndpointResponseTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_endpoint)
         """
     def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         Enabled: bool = ...
-    ) -> ModifyEventSubscriptionResponseOutputTypeDef:
+    ) -> ModifyEventSubscriptionResponseTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_event_subscription)
         """
     def modify_replication_config(
@@ -971,15 +971,15 @@
         ReplicationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ComputeConfig: ComputeConfigTypeDef = ...,
         SourceEndpointArn: str = ...,
         TargetEndpointArn: str = ...
-    ) -> ModifyReplicationConfigResponseOutputTypeDef:
+    ) -> ModifyReplicationConfigResponseTypeDef:
         """
         Modifies an existing DMS Serverless replication configuration that you can use
         to start a replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_config)
         """
@@ -994,28 +994,28 @@
         PreferredMaintenanceWindow: str = ...,
         MultiAZ: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         AutoMinorVersionUpgrade: bool = ...,
         ReplicationInstanceIdentifier: str = ...,
         NetworkType: str = ...
-    ) -> ModifyReplicationInstanceResponseOutputTypeDef:
+    ) -> ModifyReplicationInstanceResponseTypeDef:
         """
         Modifies the replication instance to apply new settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_instance)
         """
     def modify_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         SubnetIds: Sequence[str],
         ReplicationSubnetGroupDescription: str = ...
-    ) -> ModifyReplicationSubnetGroupResponseOutputTypeDef:
+    ) -> ModifyReplicationSubnetGroupResponseTypeDef:
         """
         Modifies the settings for the specified replication subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_subnet_group)
         """
     def modify_replication_task(
@@ -1026,74 +1026,74 @@
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         TaskData: str = ...
-    ) -> ModifyReplicationTaskResponseOutputTypeDef:
+    ) -> ModifyReplicationTaskResponseTypeDef:
         """
         Modifies the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#modify_replication_task)
         """
     def move_replication_task(
         self, *, ReplicationTaskArn: str, TargetReplicationInstanceArn: str
-    ) -> MoveReplicationTaskResponseOutputTypeDef:
+    ) -> MoveReplicationTaskResponseTypeDef:
         """
         Moves a replication task from its current replication instance to a different
         target replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.move_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#move_replication_task)
         """
     def reboot_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         ForceFailover: bool = ...,
         ForcePlannedFailover: bool = ...
-    ) -> RebootReplicationInstanceResponseOutputTypeDef:
+    ) -> RebootReplicationInstanceResponseTypeDef:
         """
         Reboots a replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reboot_replication_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reboot_replication_instance)
         """
     def refresh_schemas(
         self, *, EndpointArn: str, ReplicationInstanceArn: str
-    ) -> RefreshSchemasResponseOutputTypeDef:
+    ) -> RefreshSchemasResponseTypeDef:
         """
         Populates the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.refresh_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#refresh_schemas)
         """
     def reload_replication_tables(
         self,
         *,
         ReplicationConfigArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadReplicationTablesResponseOutputTypeDef:
+    ) -> ReloadReplicationTablesResponseTypeDef:
         """
         Reloads the target database table with the source data for a given DMS
         Serverless replication configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_replication_tables)
         """
     def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
-    ) -> ReloadTablesResponseOutputTypeDef:
+    ) -> ReloadTablesResponseTypeDef:
         """
         Reloads the target database table with the source data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#reload_tables)
         """
     def remove_tags_from_resource(
@@ -1102,15 +1102,15 @@
         """
         Removes metadata tags from an DMS resource, including replication instance,
         endpoint, subnet group, and migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.remove_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#remove_tags_from_resource)
         """
-    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseOutputTypeDef:
+    def run_fleet_advisor_lsa_analysis(self) -> RunFleetAdvisorLsaAnalysisResponseTypeDef:
         """
         Runs large-scale assessment (LSA) analysis on every Fleet Advisor collector in
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.run_fleet_advisor_lsa_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#run_fleet_advisor_lsa_analysis)
         """
@@ -1128,15 +1128,15 @@
         self,
         *,
         ReplicationConfigArn: str,
         StartReplicationType: str,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationResponseOutputTypeDef:
+    ) -> StartReplicationResponseTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS connects to the source
         endpoint and collects the metadata to analyze the replication workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication)
         """
@@ -1144,24 +1144,24 @@
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: Union[datetime, str] = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
-    ) -> StartReplicationTaskResponseOutputTypeDef:
+    ) -> StartReplicationTaskResponseTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task)
         """
     def start_replication_task_assessment(
         self, *, ReplicationTaskArn: str
-    ) -> StartReplicationTaskAssessmentResponseOutputTypeDef:
+    ) -> StartReplicationTaskAssessmentResponseTypeDef:
         """
         Starts the replication task assessment for unsupported data types in the source
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment)
         """
@@ -1173,53 +1173,51 @@
         ResultLocationBucket: str,
         AssessmentRunName: str,
         ResultLocationFolder: str = ...,
         ResultEncryptionMode: str = ...,
         ResultKmsKeyArn: str = ...,
         IncludeOnly: Sequence[str] = ...,
         Exclude: Sequence[str] = ...
-    ) -> StartReplicationTaskAssessmentRunResponseOutputTypeDef:
+    ) -> StartReplicationTaskAssessmentRunResponseTypeDef:
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#start_replication_task_assessment_run)
         """
-    def stop_replication(
-        self, *, ReplicationConfigArn: str
-    ) -> StopReplicationResponseOutputTypeDef:
+    def stop_replication(self, *, ReplicationConfigArn: str) -> StopReplicationResponseTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS stops any and all
         ongoing DMS Serverless replications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication)
         """
     def stop_replication_task(
         self, *, ReplicationTaskArn: str
-    ) -> StopReplicationTaskResponseOutputTypeDef:
+    ) -> StopReplicationTaskResponseTypeDef:
         """
         Stops the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#stop_replication_task)
         """
     def test_connection(
         self, *, ReplicationInstanceArn: str, EndpointArn: str
-    ) -> TestConnectionResponseOutputTypeDef:
+    ) -> TestConnectionResponseTypeDef:
         """
         Tests the connection between the replication instance and the endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.test_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#test_connection)
         """
     def update_subscriptions_to_event_bridge(
         self, *, ForceMove: bool = ...
-    ) -> UpdateSubscriptionsToEventBridgeResponseOutputTypeDef:
+    ) -> UpdateSubscriptionsToEventBridgeResponseTypeDef:
         """
         Migrates 10 active and enabled Amazon SNS subscriptions at a time and converts
         them to corresponding Amazon EventBridge rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.update_subscriptions_to_event_bridge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/client/#update_subscriptions_to_event_bridge)
         """
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/literals.pyi` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,37 +46,36 @@
 import sys
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeCertificatesResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeCertificatesPaginator",
     "DescribeConnectionsPaginator",
     "DescribeEndpointTypesPaginator",
     "DescribeEndpointsPaginator",
     "DescribeEventSubscriptionsPaginator",
     "DescribeEventsPaginator",
@@ -85,116 +84,108 @@
     "DescribeReplicationSubnetGroupsPaginator",
     "DescribeReplicationTaskAssessmentResultsPaginator",
     "DescribeReplicationTasksPaginator",
     "DescribeSchemasPaginator",
     "DescribeTableStatisticsPaginator",
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
 class DescribeCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeCertificatesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
-
 class DescribeConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeConnectionsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
-
 class DescribeEndpointTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointTypesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
-
 class DescribeEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
-
 class DescribeEventSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventSubscriptionsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
-
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
     """
 
     def paginate(
@@ -204,131 +195,124 @@
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
-
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
-
 class DescribeReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationInstancesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
-
 class DescribeReplicationSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
-
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
         self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
-
 class DescribeReplicationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTasksResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
-
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
         self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeSchemasResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
-
 class DescribeTableStatisticsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeTableStatisticsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/paginator.pyi` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,36 +46,37 @@
 import sys
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeCertificatesResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeCertificatesPaginator",
     "DescribeConnectionsPaginator",
     "DescribeEndpointTypesPaginator",
     "DescribeEndpointsPaginator",
     "DescribeEventSubscriptionsPaginator",
     "DescribeEventsPaginator",
@@ -84,108 +85,116 @@
     "DescribeReplicationSubnetGroupsPaginator",
     "DescribeReplicationTaskAssessmentResultsPaginator",
     "DescribeReplicationTasksPaginator",
     "DescribeSchemasPaginator",
     "DescribeTableStatisticsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeCertificatesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
+
 class DescribeConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeConnectionsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
+
 class DescribeEndpointTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointTypesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
+
 class DescribeEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEndpointsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
+
 class DescribeEventSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventSubscriptionsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
+
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
     """
 
     def paginate(
@@ -195,124 +204,131 @@
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeEventsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
+
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
+
 class DescribeReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationInstancesResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
+
 class DescribeReplicationSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
+
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
         self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
+
 class DescribeReplicationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeReplicationTasksResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
+
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
         self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeSchemasResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
+
 class DescribeTableStatisticsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeTableStatisticsResponseOutputTypeDef]:
+    ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dms.type_defs import AccountQuotaOutputTypeDef
+    from mypy_boto3_dms.type_defs import AccountQuotaTypeDef
 
-    data: AccountQuotaOutputTypeDef = {...}
+    data: AccountQuotaTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -61,27 +61,27 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccountQuotaOutputTypeDef",
+    "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "AvailabilityZoneOutputTypeDef",
-    "BatchStartRecommendationsErrorEntryOutputTypeDef",
+    "AvailabilityZoneTypeDef",
+    "BatchStartRecommendationsErrorEntryTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
-    "CertificateOutputTypeDef",
-    "CollectorHealthCheckOutputTypeDef",
-    "InventoryDataOutputTypeDef",
-    "CollectorShortInfoResponseOutputTypeDef",
+    "CertificateTypeDef",
+    "CollectorHealthCheckTypeDef",
+    "InventoryDataTypeDef",
+    "CollectorShortInfoResponseTypeDef",
     "ComputeConfigOutputTypeDef",
     "ComputeConfigTypeDef",
-    "ConnectionOutputTypeDef",
+    "ConnectionTypeDef",
     "DmsTransferSettingsTypeDef",
     "DocDbSettingsTypeDef",
     "DynamoDbSettingsTypeDef",
     "ElasticsearchSettingsTypeDef",
     "GcpMySQLSettingsTypeDef",
     "IBMDb2SettingsTypeDef",
     "KafkaSettingsTypeDef",
@@ -93,60 +93,60 @@
     "OracleSettingsTypeDef",
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "TimestreamSettingsTypeDef",
-    "EventSubscriptionOutputTypeDef",
+    "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
-    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
-    "ServerShortInfoResponseOutputTypeDef",
-    "DatabaseShortInfoResponseOutputTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
+    "ServerShortInfoResponseTypeDef",
+    "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
-    "EndpointSettingOutputTypeDef",
-    "SupportedEndpointTypeOutputTypeDef",
-    "EventCategoryGroupOutputTypeDef",
-    "EventOutputTypeDef",
+    "EndpointSettingTypeDef",
+    "SupportedEndpointTypeTypeDef",
+    "EventCategoryGroupTypeDef",
+    "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
-    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
-    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
+    "FleetAdvisorLsaAnalysisResponseTypeDef",
+    "FleetAdvisorSchemaObjectResponseTypeDef",
     "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
-    "OrderableReplicationInstanceOutputTypeDef",
-    "LimitationOutputTypeDef",
+    "OrderableReplicationInstanceTypeDef",
+    "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
-    "RefreshSchemasStatusOutputTypeDef",
+    "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
-    "ReplicationInstanceTaskLogOutputTypeDef",
-    "TableStatisticsOutputTypeDef",
+    "ReplicationInstanceTaskLogTypeDef",
+    "TableStatisticsTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
-    "ReplicationTaskAssessmentResultOutputTypeDef",
-    "ReplicationTaskIndividualAssessmentOutputTypeDef",
+    "ReplicationTaskAssessmentResultTypeDef",
+    "ReplicationTaskIndividualAssessmentTypeDef",
     "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "DescribeSchemasResponseOutputTypeDef",
+    "DescribeSchemasResponseTypeDef",
     "DmsTransferSettingsOutputTypeDef",
     "DocDbSettingsOutputTypeDef",
     "DynamoDbSettingsOutputTypeDef",
     "ElasticsearchSettingsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GcpMySQLSettingsOutputTypeDef",
     "IBMDb2SettingsOutputTypeDef",
@@ -167,69 +167,69 @@
     "TagOutputTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PendingMaintenanceActionOutputTypeDef",
-    "ProvisionDataOutputTypeDef",
-    "RdsConfigurationOutputTypeDef",
-    "RdsRequirementsOutputTypeDef",
+    "PendingMaintenanceActionTypeDef",
+    "ProvisionDataTypeDef",
+    "RdsConfigurationTypeDef",
+    "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsOutputTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
-    "ReloadReplicationTablesResponseOutputTypeDef",
-    "ReloadTablesResponseOutputTypeDef",
+    "ReloadReplicationTablesResponseTypeDef",
+    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ReplicationPendingModifiedValuesOutputTypeDef",
-    "VpcSecurityGroupMembershipOutputTypeDef",
-    "ReplicationStatsOutputTypeDef",
-    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
-    "ReplicationTaskStatsOutputTypeDef",
+    "ReplicationPendingModifiedValuesTypeDef",
+    "VpcSecurityGroupMembershipTypeDef",
+    "ReplicationStatsTypeDef",
+    "ReplicationTaskAssessmentRunProgressTypeDef",
+    "ReplicationTaskStatsTypeDef",
     "ResponseMetadataTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
-    "SchemaShortInfoResponseOutputTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    "SchemaShortInfoResponseTypeDef",
     "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
-    "DescribeAccountAttributesResponseOutputTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "SubnetOutputTypeDef",
-    "BatchStartRecommendationsResponseOutputTypeDef",
-    "DeleteCertificateResponseOutputTypeDef",
-    "DescribeCertificatesResponseOutputTypeDef",
-    "ImportCertificateResponseOutputTypeDef",
-    "CollectorResponseOutputTypeDef",
-    "ReplicationConfigOutputTypeDef",
+    "SubnetTypeDef",
+    "BatchStartRecommendationsResponseTypeDef",
+    "DeleteCertificateResponseTypeDef",
+    "DescribeCertificatesResponseTypeDef",
+    "ImportCertificateResponseTypeDef",
+    "CollectorResponseTypeDef",
+    "ReplicationConfigTypeDef",
     "CreateReplicationConfigMessageRequestTypeDef",
     "ModifyReplicationConfigMessageRequestTypeDef",
-    "DeleteConnectionResponseOutputTypeDef",
-    "DescribeConnectionsResponseOutputTypeDef",
-    "TestConnectionResponseOutputTypeDef",
+    "DeleteConnectionResponseTypeDef",
+    "DescribeConnectionsResponseTypeDef",
+    "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
-    "CreateEventSubscriptionResponseOutputTypeDef",
-    "DeleteEventSubscriptionResponseOutputTypeDef",
-    "DescribeEventSubscriptionsResponseOutputTypeDef",
-    "ModifyEventSubscriptionResponseOutputTypeDef",
-    "DatabaseResponseOutputTypeDef",
+    "CreateEventSubscriptionResponseTypeDef",
+    "DeleteEventSubscriptionResponseTypeDef",
+    "DescribeEventSubscriptionsResponseTypeDef",
+    "ModifyEventSubscriptionResponseTypeDef",
+    "DatabaseResponseTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
     "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
     "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
@@ -263,87 +263,87 @@
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef",
-    "DescribeEndpointSettingsResponseOutputTypeDef",
-    "DescribeEndpointTypesResponseOutputTypeDef",
-    "DescribeEventCategoriesResponseOutputTypeDef",
-    "DescribeEventsResponseOutputTypeDef",
-    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
-    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
-    "DescribeRecommendationLimitationsResponseOutputTypeDef",
-    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
-    "RefreshSchemasResponseOutputTypeDef",
-    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
-    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
-    "DescribeTableStatisticsResponseOutputTypeDef",
-    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
-    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
-    "EndpointOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
-    "ResourcePendingMaintenanceActionsOutputTypeDef",
-    "RdsRecommendationOutputTypeDef",
+    "DescribeEndpointSettingsResponseTypeDef",
+    "DescribeEndpointTypesResponseTypeDef",
+    "DescribeEventCategoriesResponseTypeDef",
+    "DescribeEventsResponseTypeDef",
+    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
+    "DescribeOrderableReplicationInstancesResponseTypeDef",
+    "DescribeRecommendationLimitationsResponseTypeDef",
+    "DescribeRefreshSchemasStatusResponseTypeDef",
+    "RefreshSchemasResponseTypeDef",
+    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
+    "DescribeReplicationTableStatisticsResponseTypeDef",
+    "DescribeTableStatisticsResponseTypeDef",
+    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
+    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
+    "EndpointTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResourcePendingMaintenanceActionsTypeDef",
+    "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadReplicationTablesMessageRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
-    "ReplicationOutputTypeDef",
-    "ReplicationTaskAssessmentRunOutputTypeDef",
-    "ReplicationTaskOutputTypeDef",
-    "SchemaResponseOutputTypeDef",
-    "ReplicationSubnetGroupOutputTypeDef",
-    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
-    "CreateReplicationConfigResponseOutputTypeDef",
-    "DeleteReplicationConfigResponseOutputTypeDef",
-    "DescribeReplicationConfigsResponseOutputTypeDef",
-    "ModifyReplicationConfigResponseOutputTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
-    "CreateEndpointResponseOutputTypeDef",
-    "DeleteEndpointResponseOutputTypeDef",
-    "DescribeEndpointsResponseOutputTypeDef",
-    "ModifyEndpointResponseOutputTypeDef",
-    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
-    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
-    "RecommendationDataOutputTypeDef",
+    "ReplicationTypeDef",
+    "ReplicationTaskAssessmentRunTypeDef",
+    "ReplicationTaskTypeDef",
+    "SchemaResponseTypeDef",
+    "ReplicationSubnetGroupTypeDef",
+    "DescribeFleetAdvisorCollectorsResponseTypeDef",
+    "CreateReplicationConfigResponseTypeDef",
+    "DeleteReplicationConfigResponseTypeDef",
+    "DescribeReplicationConfigsResponseTypeDef",
+    "ModifyReplicationConfigResponseTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "DeleteEndpointResponseTypeDef",
+    "DescribeEndpointsResponseTypeDef",
+    "ModifyEndpointResponseTypeDef",
+    "ApplyPendingMaintenanceActionResponseTypeDef",
+    "DescribePendingMaintenanceActionsResponseTypeDef",
+    "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
-    "DescribeReplicationsResponseOutputTypeDef",
-    "StartReplicationResponseOutputTypeDef",
-    "StopReplicationResponseOutputTypeDef",
-    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
-    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
-    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
-    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
-    "CreateReplicationTaskResponseOutputTypeDef",
-    "DeleteReplicationTaskResponseOutputTypeDef",
-    "DescribeReplicationTasksResponseOutputTypeDef",
-    "ModifyReplicationTaskResponseOutputTypeDef",
-    "MoveReplicationTaskResponseOutputTypeDef",
-    "StartReplicationTaskAssessmentResponseOutputTypeDef",
-    "StartReplicationTaskResponseOutputTypeDef",
-    "StopReplicationTaskResponseOutputTypeDef",
-    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
-    "CreateReplicationSubnetGroupResponseOutputTypeDef",
-    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
-    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
-    "ReplicationInstanceOutputTypeDef",
-    "RecommendationOutputTypeDef",
-    "CreateReplicationInstanceResponseOutputTypeDef",
-    "DeleteReplicationInstanceResponseOutputTypeDef",
-    "DescribeReplicationInstancesResponseOutputTypeDef",
-    "ModifyReplicationInstanceResponseOutputTypeDef",
-    "RebootReplicationInstanceResponseOutputTypeDef",
-    "DescribeRecommendationsResponseOutputTypeDef",
+    "DescribeReplicationsResponseTypeDef",
+    "StartReplicationResponseTypeDef",
+    "StopReplicationResponseTypeDef",
+    "CancelReplicationTaskAssessmentRunResponseTypeDef",
+    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
+    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
+    "StartReplicationTaskAssessmentRunResponseTypeDef",
+    "CreateReplicationTaskResponseTypeDef",
+    "DeleteReplicationTaskResponseTypeDef",
+    "DescribeReplicationTasksResponseTypeDef",
+    "ModifyReplicationTaskResponseTypeDef",
+    "MoveReplicationTaskResponseTypeDef",
+    "StartReplicationTaskAssessmentResponseTypeDef",
+    "StartReplicationTaskResponseTypeDef",
+    "StopReplicationTaskResponseTypeDef",
+    "DescribeFleetAdvisorSchemasResponseTypeDef",
+    "CreateReplicationSubnetGroupResponseTypeDef",
+    "DescribeReplicationSubnetGroupsResponseTypeDef",
+    "ModifyReplicationSubnetGroupResponseTypeDef",
+    "ReplicationInstanceTypeDef",
+    "RecommendationTypeDef",
+    "CreateReplicationInstanceResponseTypeDef",
+    "DeleteReplicationInstanceResponseTypeDef",
+    "DescribeReplicationInstancesResponseTypeDef",
+    "ModifyReplicationInstanceResponseTypeDef",
+    "RebootReplicationInstanceResponseTypeDef",
+    "DescribeRecommendationsResponseTypeDef",
 )
 
-AccountQuotaOutputTypeDef = TypedDict(
-    "AccountQuotaOutputTypeDef",
+AccountQuotaTypeDef = TypedDict(
+    "AccountQuotaTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
 )
 
@@ -362,73 +362,73 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
     },
 )
 
-AvailabilityZoneOutputTypeDef = TypedDict(
-    "AvailabilityZoneOutputTypeDef",
+AvailabilityZoneTypeDef = TypedDict(
+    "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
 )
 
-BatchStartRecommendationsErrorEntryOutputTypeDef = TypedDict(
-    "BatchStartRecommendationsErrorEntryOutputTypeDef",
+BatchStartRecommendationsErrorEntryTypeDef = TypedDict(
+    "BatchStartRecommendationsErrorEntryTypeDef",
     {
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
 )
 
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
 )
 
-CertificateOutputTypeDef = TypedDict(
-    "CertificateOutputTypeDef",
+CertificateTypeDef = TypedDict(
+    "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateCreationDate": datetime,
         "CertificatePem": str,
         "CertificateWallet": bytes,
         "CertificateArn": str,
         "CertificateOwner": str,
         "ValidFromDate": datetime,
         "ValidToDate": datetime,
         "SigningAlgorithm": str,
         "KeyLength": int,
     },
 )
 
-CollectorHealthCheckOutputTypeDef = TypedDict(
-    "CollectorHealthCheckOutputTypeDef",
+CollectorHealthCheckTypeDef = TypedDict(
+    "CollectorHealthCheckTypeDef",
     {
         "CollectorStatus": CollectorStatusType,
         "LocalCollectorS3Access": bool,
         "WebCollectorS3Access": bool,
         "WebCollectorGrantedRoleBasedAccess": bool,
     },
 )
 
-InventoryDataOutputTypeDef = TypedDict(
-    "InventoryDataOutputTypeDef",
+InventoryDataTypeDef = TypedDict(
+    "InventoryDataTypeDef",
     {
         "NumberOfDatabases": int,
         "NumberOfSchemas": int,
     },
 )
 
-CollectorShortInfoResponseOutputTypeDef = TypedDict(
-    "CollectorShortInfoResponseOutputTypeDef",
+CollectorShortInfoResponseTypeDef = TypedDict(
+    "CollectorShortInfoResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
 )
 
 ComputeConfigOutputTypeDef = TypedDict(
@@ -458,16 +458,16 @@
         "PreferredMaintenanceWindow": str,
         "ReplicationSubnetGroupId": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-ConnectionOutputTypeDef = TypedDict(
-    "ConnectionOutputTypeDef",
+ConnectionTypeDef = TypedDict(
+    "ConnectionTypeDef",
     {
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
         "EndpointIdentifier": str,
         "ReplicationInstanceIdentifier": str,
@@ -933,16 +933,16 @@
 
 class TimestreamSettingsTypeDef(
     _RequiredTimestreamSettingsTypeDef, _OptionalTimestreamSettingsTypeDef
 ):
     pass
 
 
-EventSubscriptionOutputTypeDef = TypedDict(
-    "EventSubscriptionOutputTypeDef",
+EventSubscriptionTypeDef = TypedDict(
+    "EventSubscriptionTypeDef",
     {
         "CustomerAwsId": str,
         "CustSubscriptionId": str,
         "SnsTopicArn": str,
         "Status": str,
         "SubscriptionCreationTime": str,
         "SourceType": str,
@@ -972,50 +972,50 @@
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
 
-CreateFleetAdvisorCollectorResponseOutputTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "Description": str,
         "ServiceAccessRoleArn": str,
         "S3BucketName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseInstanceSoftwareDetailsResponseOutputTypeDef = TypedDict(
-    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
+DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
+    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
         "SupportLevel": str,
         "OsArchitecture": int,
         "Tooltip": str,
     },
 )
 
-ServerShortInfoResponseOutputTypeDef = TypedDict(
-    "ServerShortInfoResponseOutputTypeDef",
+ServerShortInfoResponseTypeDef = TypedDict(
+    "ServerShortInfoResponseTypeDef",
     {
         "ServerId": str,
         "IpAddress": str,
         "ServerName": str,
     },
 )
 
-DatabaseShortInfoResponseOutputTypeDef = TypedDict(
-    "DatabaseShortInfoResponseOutputTypeDef",
+DatabaseShortInfoResponseTypeDef = TypedDict(
+    "DatabaseShortInfoResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
         "DatabaseEngine": str,
     },
 )
@@ -1059,16 +1059,16 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
-DeleteFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     {
         "DatabaseIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
@@ -1116,16 +1116,16 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeApplicableIndividualAssessmentsResponseOutputTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
         "IndividualAssessmentNames": List[str],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1165,50 +1165,50 @@
 class DescribeEndpointSettingsMessageRequestTypeDef(
     _RequiredDescribeEndpointSettingsMessageRequestTypeDef,
     _OptionalDescribeEndpointSettingsMessageRequestTypeDef,
 ):
     pass
 
 
-EndpointSettingOutputTypeDef = TypedDict(
-    "EndpointSettingOutputTypeDef",
+EndpointSettingTypeDef = TypedDict(
+    "EndpointSettingTypeDef",
     {
         "Name": str,
         "Type": EndpointSettingTypeValueType,
         "EnumValues": List[str],
         "Sensitive": bool,
         "Units": str,
         "Applicability": str,
         "IntValueMin": int,
         "IntValueMax": int,
         "DefaultValue": str,
     },
 )
 
-SupportedEndpointTypeOutputTypeDef = TypedDict(
-    "SupportedEndpointTypeOutputTypeDef",
+SupportedEndpointTypeTypeDef = TypedDict(
+    "SupportedEndpointTypeTypeDef",
     {
         "EngineName": str,
         "SupportsCDC": bool,
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
 )
 
-EventCategoryGroupOutputTypeDef = TypedDict(
-    "EventCategoryGroupOutputTypeDef",
+EventCategoryGroupTypeDef = TypedDict(
+    "EventCategoryGroupTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
 )
 
-EventOutputTypeDef = TypedDict(
-    "EventOutputTypeDef",
+EventTypeDef = TypedDict(
+    "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
     },
@@ -1219,24 +1219,24 @@
     {
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-FleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
-    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
+FleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "FleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
     },
 )
 
-FleetAdvisorSchemaObjectResponseOutputTypeDef = TypedDict(
-    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
+FleetAdvisorSchemaObjectResponseTypeDef = TypedDict(
+    "FleetAdvisorSchemaObjectResponseTypeDef",
     {
         "SchemaId": str,
         "ObjectType": str,
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
@@ -1255,31 +1255,31 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-OrderableReplicationInstanceOutputTypeDef = TypedDict(
-    "OrderableReplicationInstanceOutputTypeDef",
+OrderableReplicationInstanceTypeDef = TypedDict(
+    "OrderableReplicationInstanceTypeDef",
     {
         "EngineVersion": str,
         "ReplicationInstanceClass": str,
         "StorageType": str,
         "MinAllocatedStorage": int,
         "MaxAllocatedStorage": int,
         "DefaultAllocatedStorage": int,
         "IncludedAllocatedStorage": int,
         "AvailabilityZones": List[str],
         "ReleaseStatus": ReleaseStatusValuesType,
     },
 )
 
-LimitationOutputTypeDef = TypedDict(
-    "LimitationOutputTypeDef",
+LimitationTypeDef = TypedDict(
+    "LimitationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "Name": str,
         "Description": str,
         "Impact": str,
         "Type": str,
@@ -1289,16 +1289,16 @@
 DescribeRefreshSchemasStatusMessageRequestTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
-RefreshSchemasStatusOutputTypeDef = TypedDict(
-    "RefreshSchemasStatusOutputTypeDef",
+RefreshSchemasStatusTypeDef = TypedDict(
+    "RefreshSchemasStatusTypeDef",
     {
         "EndpointArn": str,
         "ReplicationInstanceArn": str,
         "Status": RefreshSchemasStatusTypeValueType,
         "LastRefreshDate": datetime,
         "LastFailureMessage": str,
     },
@@ -1323,25 +1323,25 @@
 class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(
     _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     _OptionalDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
 ):
     pass
 
 
-ReplicationInstanceTaskLogOutputTypeDef = TypedDict(
-    "ReplicationInstanceTaskLogOutputTypeDef",
+ReplicationInstanceTaskLogTypeDef = TypedDict(
+    "ReplicationInstanceTaskLogTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
 )
 
-TableStatisticsOutputTypeDef = TypedDict(
-    "TableStatisticsOutputTypeDef",
+TableStatisticsTypeDef = TypedDict(
+    "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
         "Updates": int,
         "Ddls": int,
@@ -1380,29 +1380,29 @@
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-ReplicationTaskAssessmentResultOutputTypeDef = TypedDict(
-    "ReplicationTaskAssessmentResultOutputTypeDef",
+ReplicationTaskAssessmentResultTypeDef = TypedDict(
+    "ReplicationTaskAssessmentResultTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "ReplicationTaskArn": str,
         "ReplicationTaskLastAssessmentDate": datetime,
         "AssessmentStatus": str,
         "AssessmentResultsFile": str,
         "AssessmentResults": str,
         "S3ObjectUrl": str,
     },
 )
 
-ReplicationTaskIndividualAssessmentOutputTypeDef = TypedDict(
-    "ReplicationTaskIndividualAssessmentOutputTypeDef",
+ReplicationTaskIndividualAssessmentTypeDef = TypedDict(
+    "ReplicationTaskIndividualAssessmentTypeDef",
     {
         "ReplicationTaskIndividualAssessmentArn": str,
         "ReplicationTaskAssessmentRunArn": str,
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
@@ -1448,16 +1448,16 @@
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
 
-DescribeSchemasResponseOutputTypeDef = TypedDict(
-    "DescribeSchemasResponseOutputTypeDef",
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
     {
         "Marker": str,
         "Schemas": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2010,55 +2010,55 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PendingMaintenanceActionOutputTypeDef = TypedDict(
-    "PendingMaintenanceActionOutputTypeDef",
+PendingMaintenanceActionTypeDef = TypedDict(
+    "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
 )
 
-ProvisionDataOutputTypeDef = TypedDict(
-    "ProvisionDataOutputTypeDef",
+ProvisionDataTypeDef = TypedDict(
+    "ProvisionDataTypeDef",
     {
         "ProvisionState": str,
         "ProvisionedCapacityUnits": int,
         "DateProvisioned": datetime,
         "IsNewProvisioningAvailable": bool,
         "DateNewProvisioningDataAvailable": datetime,
         "ReasonForNewProvisioningData": str,
     },
 )
 
-RdsConfigurationOutputTypeDef = TypedDict(
-    "RdsConfigurationOutputTypeDef",
+RdsConfigurationTypeDef = TypedDict(
+    "RdsConfigurationTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
 )
 
-RdsRequirementsOutputTypeDef = TypedDict(
-    "RdsRequirementsOutputTypeDef",
+RdsRequirementsTypeDef = TypedDict(
+    "RdsRequirementsTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
@@ -2117,59 +2117,59 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
-ReloadReplicationTablesResponseOutputTypeDef = TypedDict(
-    "ReloadReplicationTablesResponseOutputTypeDef",
+ReloadReplicationTablesResponseTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseTypeDef",
     {
         "ReplicationConfigArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReloadTablesResponseOutputTypeDef = TypedDict(
-    "ReloadTablesResponseOutputTypeDef",
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ReplicationPendingModifiedValuesOutputTypeDef = TypedDict(
-    "ReplicationPendingModifiedValuesOutputTypeDef",
+ReplicationPendingModifiedValuesTypeDef = TypedDict(
+    "ReplicationPendingModifiedValuesTypeDef",
     {
         "ReplicationInstanceClass": str,
         "AllocatedStorage": int,
         "MultiAZ": bool,
         "EngineVersion": str,
         "NetworkType": str,
     },
 )
 
-VpcSecurityGroupMembershipOutputTypeDef = TypedDict(
-    "VpcSecurityGroupMembershipOutputTypeDef",
+VpcSecurityGroupMembershipTypeDef = TypedDict(
+    "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
 )
 
-ReplicationStatsOutputTypeDef = TypedDict(
-    "ReplicationStatsOutputTypeDef",
+ReplicationStatsTypeDef = TypedDict(
+    "ReplicationStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -2177,24 +2177,24 @@
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunProgressOutputTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
+ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunProgressTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
 )
 
-ReplicationTaskStatsOutputTypeDef = TypedDict(
-    "ReplicationTaskStatsOutputTypeDef",
+ReplicationTaskStatsTypeDef = TypedDict(
+    "ReplicationTaskStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -2213,25 +2213,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RunFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SchemaShortInfoResponseOutputTypeDef = TypedDict(
-    "SchemaShortInfoResponseOutputTypeDef",
+SchemaShortInfoResponseTypeDef = TypedDict(
+    "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
     },
@@ -2348,26 +2348,26 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
-UpdateSubscriptionsToEventBridgeResponseOutputTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     {
         "Result": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccountAttributesResponseOutputTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseOutputTypeDef",
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
     {
-        "AccountQuotas": List[AccountQuotaOutputTypeDef],
+        "AccountQuotas": List[AccountQuotaTypeDef],
         "UniqueAccountIdentifier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
@@ -2516,77 +2516,77 @@
 
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
 
-SubnetOutputTypeDef = TypedDict(
-    "SubnetOutputTypeDef",
+SubnetTypeDef = TypedDict(
+    "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
-        "SubnetAvailabilityZone": AvailabilityZoneOutputTypeDef,
+        "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
 )
 
-BatchStartRecommendationsResponseOutputTypeDef = TypedDict(
-    "BatchStartRecommendationsResponseOutputTypeDef",
+BatchStartRecommendationsResponseTypeDef = TypedDict(
+    "BatchStartRecommendationsResponseTypeDef",
     {
-        "ErrorEntries": List[BatchStartRecommendationsErrorEntryOutputTypeDef],
+        "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteCertificateResponseOutputTypeDef = TypedDict(
-    "DeleteCertificateResponseOutputTypeDef",
+DeleteCertificateResponseTypeDef = TypedDict(
+    "DeleteCertificateResponseTypeDef",
     {
-        "Certificate": CertificateOutputTypeDef,
+        "Certificate": CertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCertificatesResponseOutputTypeDef = TypedDict(
-    "DescribeCertificatesResponseOutputTypeDef",
+DescribeCertificatesResponseTypeDef = TypedDict(
+    "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
-        "Certificates": List[CertificateOutputTypeDef],
+        "Certificates": List[CertificateTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ImportCertificateResponseOutputTypeDef = TypedDict(
-    "ImportCertificateResponseOutputTypeDef",
+ImportCertificateResponseTypeDef = TypedDict(
+    "ImportCertificateResponseTypeDef",
     {
-        "Certificate": CertificateOutputTypeDef,
+        "Certificate": CertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CollectorResponseOutputTypeDef = TypedDict(
-    "CollectorResponseOutputTypeDef",
+CollectorResponseTypeDef = TypedDict(
+    "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "CollectorVersion": str,
         "VersionStatus": VersionStatusType,
         "Description": str,
         "S3BucketName": str,
         "ServiceAccessRoleArn": str,
-        "CollectorHealthCheck": CollectorHealthCheckOutputTypeDef,
+        "CollectorHealthCheck": CollectorHealthCheckTypeDef,
         "LastDataReceived": str,
         "RegisteredDate": str,
         "CreatedDate": str,
         "ModifiedDate": str,
-        "InventoryData": InventoryDataOutputTypeDef,
+        "InventoryData": InventoryDataTypeDef,
     },
 )
 
-ReplicationConfigOutputTypeDef = TypedDict(
-    "ReplicationConfigOutputTypeDef",
+ReplicationConfigTypeDef = TypedDict(
+    "ReplicationConfigTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "ReplicationConfigArn": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationType": MigrationTypeValueType,
         "ComputeConfig": ComputeConfigOutputTypeDef,
@@ -2653,35 +2653,35 @@
 class ModifyReplicationConfigMessageRequestTypeDef(
     _RequiredModifyReplicationConfigMessageRequestTypeDef,
     _OptionalModifyReplicationConfigMessageRequestTypeDef,
 ):
     pass
 
 
-DeleteConnectionResponseOutputTypeDef = TypedDict(
-    "DeleteConnectionResponseOutputTypeDef",
+DeleteConnectionResponseTypeDef = TypedDict(
+    "DeleteConnectionResponseTypeDef",
     {
-        "Connection": ConnectionOutputTypeDef,
+        "Connection": ConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeConnectionsResponseOutputTypeDef = TypedDict(
-    "DescribeConnectionsResponseOutputTypeDef",
+DescribeConnectionsResponseTypeDef = TypedDict(
+    "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
-        "Connections": List[ConnectionOutputTypeDef],
+        "Connections": List[ConnectionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestConnectionResponseOutputTypeDef = TypedDict(
-    "TestConnectionResponseOutputTypeDef",
+TestConnectionResponseTypeDef = TypedDict(
+    "TestConnectionResponseTypeDef",
     {
-        "Connection": ConnectionOutputTypeDef,
+        "Connection": ConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
@@ -2785,57 +2785,57 @@
 
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
     pass
 
 
-CreateEventSubscriptionResponseOutputTypeDef = TypedDict(
-    "CreateEventSubscriptionResponseOutputTypeDef",
+CreateEventSubscriptionResponseTypeDef = TypedDict(
+    "CreateEventSubscriptionResponseTypeDef",
     {
-        "EventSubscription": EventSubscriptionOutputTypeDef,
+        "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEventSubscriptionResponseOutputTypeDef = TypedDict(
-    "DeleteEventSubscriptionResponseOutputTypeDef",
+DeleteEventSubscriptionResponseTypeDef = TypedDict(
+    "DeleteEventSubscriptionResponseTypeDef",
     {
-        "EventSubscription": EventSubscriptionOutputTypeDef,
+        "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventSubscriptionsResponseOutputTypeDef = TypedDict(
-    "DescribeEventSubscriptionsResponseOutputTypeDef",
+DescribeEventSubscriptionsResponseTypeDef = TypedDict(
+    "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
-        "EventSubscriptionsList": List[EventSubscriptionOutputTypeDef],
+        "EventSubscriptionsList": List[EventSubscriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEventSubscriptionResponseOutputTypeDef = TypedDict(
-    "ModifyEventSubscriptionResponseOutputTypeDef",
+ModifyEventSubscriptionResponseTypeDef = TypedDict(
+    "ModifyEventSubscriptionResponseTypeDef",
     {
-        "EventSubscription": EventSubscriptionOutputTypeDef,
+        "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseResponseOutputTypeDef = TypedDict(
-    "DatabaseResponseOutputTypeDef",
+DatabaseResponseTypeDef = TypedDict(
+    "DatabaseResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "IpAddress": str,
         "NumberOfSchemas": int,
-        "Server": ServerShortInfoResponseOutputTypeDef,
-        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
-        "Collectors": List[CollectorShortInfoResponseOutputTypeDef],
+        "Server": ServerShortInfoResponseTypeDef,
+        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
+        "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
 )
 
 DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -3301,154 +3301,152 @@
         "Marker": str,
         "WithoutSettings": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEndpointSettingsResponseOutputTypeDef = TypedDict(
-    "DescribeEndpointSettingsResponseOutputTypeDef",
+DescribeEndpointSettingsResponseTypeDef = TypedDict(
+    "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
-        "EndpointSettings": List[EndpointSettingOutputTypeDef],
+        "EndpointSettings": List[EndpointSettingTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointTypesResponseOutputTypeDef = TypedDict(
-    "DescribeEndpointTypesResponseOutputTypeDef",
+DescribeEndpointTypesResponseTypeDef = TypedDict(
+    "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
-        "SupportedEndpointTypes": List[SupportedEndpointTypeOutputTypeDef],
+        "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventCategoriesResponseOutputTypeDef = TypedDict(
-    "DescribeEventCategoriesResponseOutputTypeDef",
+DescribeEventCategoriesResponseTypeDef = TypedDict(
+    "DescribeEventCategoriesResponseTypeDef",
     {
-        "EventCategoryGroupList": List[EventCategoryGroupOutputTypeDef],
+        "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventsResponseOutputTypeDef = TypedDict(
-    "DescribeEventsResponseOutputTypeDef",
+DescribeEventsResponseTypeDef = TypedDict(
+    "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
-        "Events": List[EventOutputTypeDef],
+        "Events": List[EventTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
-        "Analysis": List[FleetAdvisorLsaAnalysisResponseOutputTypeDef],
+        "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
+DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
-        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseOutputTypeDef],
+        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOrderableReplicationInstancesResponseOutputTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
+DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
-        "OrderableReplicationInstances": List[OrderableReplicationInstanceOutputTypeDef],
+        "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationLimitationsResponseOutputTypeDef = TypedDict(
-    "DescribeRecommendationLimitationsResponseOutputTypeDef",
+DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
+    "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
-        "Limitations": List[LimitationOutputTypeDef],
+        "Limitations": List[LimitationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRefreshSchemasStatusResponseOutputTypeDef = TypedDict(
-    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
+DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
+    "DescribeRefreshSchemasStatusResponseTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RefreshSchemasResponseOutputTypeDef = TypedDict(
-    "RefreshSchemasResponseOutputTypeDef",
+RefreshSchemasResponseTypeDef = TypedDict(
+    "RefreshSchemasResponseTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstanceTaskLogsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
+DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
+    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
-        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogOutputTypeDef],
+        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTableStatisticsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
+DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeReplicationTableStatisticsResponseTypeDef",
     {
         "ReplicationConfigArn": str,
         "Marker": str,
-        "ReplicationTableStatistics": List[TableStatisticsOutputTypeDef],
+        "ReplicationTableStatistics": List[TableStatisticsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTableStatisticsResponseOutputTypeDef = TypedDict(
-    "DescribeTableStatisticsResponseOutputTypeDef",
+DescribeTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
-        "TableStatistics": List[TableStatisticsOutputTypeDef],
+        "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
+DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
-        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultOutputTypeDef],
+        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
+DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskIndividualAssessments": List[
-            ReplicationTaskIndividualAssessmentOutputTypeDef
-        ],
+        "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EndpointOutputTypeDef = TypedDict(
-    "EndpointOutputTypeDef",
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
     {
         "EndpointIdentifier": str,
         "EndpointType": ReplicationEndpointTypeValueType,
         "EngineName": str,
         "EngineDisplayName": str,
         "Username": str,
         "ServerName": str,
@@ -3481,35 +3479,35 @@
         "DocDbSettings": DocDbSettingsOutputTypeDef,
         "RedisSettings": RedisSettingsOutputTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsOutputTypeDef,
         "TimestreamSettings": TimestreamSettingsOutputTypeDef,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourcePendingMaintenanceActionsOutputTypeDef = TypedDict(
-    "ResourcePendingMaintenanceActionsOutputTypeDef",
+ResourcePendingMaintenanceActionsTypeDef = TypedDict(
+    "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
-        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionOutputTypeDef],
+        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
 )
 
-RdsRecommendationOutputTypeDef = TypedDict(
-    "RdsRecommendationOutputTypeDef",
+RdsRecommendationTypeDef = TypedDict(
+    "RdsRecommendationTypeDef",
     {
-        "RequirementsToTarget": RdsRequirementsOutputTypeDef,
-        "TargetConfiguration": RdsConfigurationOutputTypeDef,
+        "RequirementsToTarget": RdsRequirementsTypeDef,
+        "TargetConfiguration": RdsConfigurationTypeDef,
     },
 )
 
 StartRecommendationsRequestEntryTypeDef = TypedDict(
     "StartRecommendationsRequestEntryTypeDef",
     {
         "DatabaseId": str,
@@ -3566,58 +3564,58 @@
 
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
 
-ReplicationOutputTypeDef = TypedDict(
-    "ReplicationOutputTypeDef",
+ReplicationTypeDef = TypedDict(
+    "ReplicationTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "ReplicationConfigArn": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationType": MigrationTypeValueType,
         "Status": str,
-        "ProvisionData": ProvisionDataOutputTypeDef,
+        "ProvisionData": ProvisionDataTypeDef,
         "StopReason": str,
         "FailureMessages": List[str],
-        "ReplicationStats": ReplicationStatsOutputTypeDef,
+        "ReplicationStats": ReplicationStatsTypeDef,
         "StartReplicationType": str,
         "CdcStartTime": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationCreateTime": datetime,
         "ReplicationUpdateTime": datetime,
         "ReplicationLastStopTime": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunOutputTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunOutputTypeDef",
+ReplicationTaskAssessmentRunTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
-        "AssessmentProgress": ReplicationTaskAssessmentRunProgressOutputTypeDef,
+        "AssessmentProgress": ReplicationTaskAssessmentRunProgressTypeDef,
         "LastFailureMessage": str,
         "ServiceAccessRoleArn": str,
         "ResultLocationBucket": str,
         "ResultLocationFolder": str,
         "ResultEncryptionMode": str,
         "ResultKmsKeyArn": str,
         "AssessmentRunName": str,
     },
 )
 
-ReplicationTaskOutputTypeDef = TypedDict(
-    "ReplicationTaskOutputTypeDef",
+ReplicationTaskTypeDef = TypedDict(
+    "ReplicationTaskTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationInstanceArn": str,
         "MigrationType": MigrationTypeValueType,
         "TableMappings": str,
@@ -3627,333 +3625,333 @@
         "StopReason": str,
         "ReplicationTaskCreationDate": datetime,
         "ReplicationTaskStartDate": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationTaskArn": str,
-        "ReplicationTaskStats": ReplicationTaskStatsOutputTypeDef,
+        "ReplicationTaskStats": ReplicationTaskStatsTypeDef,
         "TaskData": str,
         "TargetReplicationInstanceArn": str,
     },
 )
 
-SchemaResponseOutputTypeDef = TypedDict(
-    "SchemaResponseOutputTypeDef",
+SchemaResponseTypeDef = TypedDict(
+    "SchemaResponseTypeDef",
     {
         "CodeLineCount": int,
         "CodeSize": int,
         "Complexity": str,
-        "Server": ServerShortInfoResponseOutputTypeDef,
-        "DatabaseInstance": DatabaseShortInfoResponseOutputTypeDef,
+        "Server": ServerShortInfoResponseTypeDef,
+        "DatabaseInstance": DatabaseShortInfoResponseTypeDef,
         "SchemaId": str,
         "SchemaName": str,
-        "OriginalSchema": SchemaShortInfoResponseOutputTypeDef,
+        "OriginalSchema": SchemaShortInfoResponseTypeDef,
         "Similarity": float,
     },
 )
 
-ReplicationSubnetGroupOutputTypeDef = TypedDict(
-    "ReplicationSubnetGroupOutputTypeDef",
+ReplicationSubnetGroupTypeDef = TypedDict(
+    "ReplicationSubnetGroupTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
-        "Subnets": List[SubnetOutputTypeDef],
+        "Subnets": List[SubnetTypeDef],
         "SupportedNetworkTypes": List[str],
     },
 )
 
-DescribeFleetAdvisorCollectorsResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
+DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
-        "Collectors": List[CollectorResponseOutputTypeDef],
+        "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationConfigResponseOutputTypeDef = TypedDict(
-    "CreateReplicationConfigResponseOutputTypeDef",
+CreateReplicationConfigResponseTypeDef = TypedDict(
+    "CreateReplicationConfigResponseTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationConfigResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationConfigResponseOutputTypeDef",
+DeleteReplicationConfigResponseTypeDef = TypedDict(
+    "DeleteReplicationConfigResponseTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationConfigsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationConfigsResponseOutputTypeDef",
+DescribeReplicationConfigsResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationConfigs": List[ReplicationConfigOutputTypeDef],
+        "ReplicationConfigs": List[ReplicationConfigTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationConfigResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationConfigResponseOutputTypeDef",
+ModifyReplicationConfigResponseTypeDef = TypedDict(
+    "ModifyReplicationConfigResponseTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
+DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     {
-        "Databases": List[DatabaseResponseOutputTypeDef],
+        "Databases": List[DatabaseResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointResponseOutputTypeDef = TypedDict(
-    "CreateEndpointResponseOutputTypeDef",
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
     {
-        "Endpoint": EndpointOutputTypeDef,
+        "Endpoint": EndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEndpointResponseOutputTypeDef = TypedDict(
-    "DeleteEndpointResponseOutputTypeDef",
+DeleteEndpointResponseTypeDef = TypedDict(
+    "DeleteEndpointResponseTypeDef",
     {
-        "Endpoint": EndpointOutputTypeDef,
+        "Endpoint": EndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointsResponseOutputTypeDef = TypedDict(
-    "DescribeEndpointsResponseOutputTypeDef",
+DescribeEndpointsResponseTypeDef = TypedDict(
+    "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
-        "Endpoints": List[EndpointOutputTypeDef],
+        "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEndpointResponseOutputTypeDef = TypedDict(
-    "ModifyEndpointResponseOutputTypeDef",
+ModifyEndpointResponseTypeDef = TypedDict(
+    "ModifyEndpointResponseTypeDef",
     {
-        "Endpoint": EndpointOutputTypeDef,
+        "Endpoint": EndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ApplyPendingMaintenanceActionResponseOutputTypeDef = TypedDict(
-    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
+ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
+    "ApplyPendingMaintenanceActionResponseTypeDef",
     {
-        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsOutputTypeDef,
+        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePendingMaintenanceActionsResponseOutputTypeDef = TypedDict(
-    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
+DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsResponseTypeDef",
     {
-        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsOutputTypeDef],
+        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommendationDataOutputTypeDef = TypedDict(
-    "RecommendationDataOutputTypeDef",
+RecommendationDataTypeDef = TypedDict(
+    "RecommendationDataTypeDef",
     {
-        "RdsEngine": RdsRecommendationOutputTypeDef,
+        "RdsEngine": RdsRecommendationTypeDef,
     },
 )
 
 BatchStartRecommendationsRequestRequestTypeDef = TypedDict(
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
     total=False,
 )
 
-DescribeReplicationsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationsResponseOutputTypeDef",
+DescribeReplicationsResponseTypeDef = TypedDict(
+    "DescribeReplicationsResponseTypeDef",
     {
         "Marker": str,
-        "Replications": List[ReplicationOutputTypeDef],
+        "Replications": List[ReplicationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationResponseOutputTypeDef = TypedDict(
-    "StartReplicationResponseOutputTypeDef",
+StartReplicationResponseTypeDef = TypedDict(
+    "StartReplicationResponseTypeDef",
     {
-        "Replication": ReplicationOutputTypeDef,
+        "Replication": ReplicationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationResponseOutputTypeDef = TypedDict(
-    "StopReplicationResponseOutputTypeDef",
+StopReplicationResponseTypeDef = TypedDict(
+    "StopReplicationResponseTypeDef",
     {
-        "Replication": ReplicationOutputTypeDef,
+        "Replication": ReplicationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
-    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
+CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
+    "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
+DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
+    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
+DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunOutputTypeDef],
+        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
+StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationTaskResponseOutputTypeDef = TypedDict(
-    "CreateReplicationTaskResponseOutputTypeDef",
+CreateReplicationTaskResponseTypeDef = TypedDict(
+    "CreateReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationTaskResponseOutputTypeDef",
+DeleteReplicationTaskResponseTypeDef = TypedDict(
+    "DeleteReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTasksResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTasksResponseOutputTypeDef",
+DescribeReplicationTasksResponseTypeDef = TypedDict(
+    "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationTasks": List[ReplicationTaskOutputTypeDef],
+        "ReplicationTasks": List[ReplicationTaskTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationTaskResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationTaskResponseOutputTypeDef",
+ModifyReplicationTaskResponseTypeDef = TypedDict(
+    "ModifyReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MoveReplicationTaskResponseOutputTypeDef = TypedDict(
-    "MoveReplicationTaskResponseOutputTypeDef",
+MoveReplicationTaskResponseTypeDef = TypedDict(
+    "MoveReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentResponseOutputTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentResponseOutputTypeDef",
+StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskResponseOutputTypeDef = TypedDict(
-    "StartReplicationTaskResponseOutputTypeDef",
+StartReplicationTaskResponseTypeDef = TypedDict(
+    "StartReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationTaskResponseOutputTypeDef = TypedDict(
-    "StopReplicationTaskResponseOutputTypeDef",
+StopReplicationTaskResponseTypeDef = TypedDict(
+    "StopReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemasResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
+DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
-        "FleetAdvisorSchemas": List[SchemaResponseOutputTypeDef],
+        "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
-    "CreateReplicationSubnetGroupResponseOutputTypeDef",
+CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
+    "CreateReplicationSubnetGroupResponseTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationSubnetGroupsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
+DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationSubnetGroups": List[ReplicationSubnetGroupOutputTypeDef],
+        "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
+ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
+    "ModifyReplicationSubnetGroupResponseTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicationInstanceOutputTypeDef = TypedDict(
-    "ReplicationInstanceOutputTypeDef",
+ReplicationInstanceTypeDef = TypedDict(
+    "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
         "ReplicationInstanceStatus": str,
         "AllocatedStorage": int,
         "InstanceCreateTime": datetime,
-        "VpcSecurityGroups": List[VpcSecurityGroupMembershipOutputTypeDef],
+        "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "AvailabilityZone": str,
-        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
         "PreferredMaintenanceWindow": str,
-        "PendingModifiedValues": ReplicationPendingModifiedValuesOutputTypeDef,
+        "PendingModifiedValues": ReplicationPendingModifiedValuesTypeDef,
         "MultiAZ": bool,
         "EngineVersion": str,
         "AutoMinorVersionUpgrade": bool,
         "KmsKeyId": str,
         "ReplicationInstanceArn": str,
         "ReplicationInstancePublicIpAddress": str,
         "ReplicationInstancePrivateIpAddress": str,
@@ -3964,69 +3962,69 @@
         "SecondaryAvailabilityZone": str,
         "FreeUntil": datetime,
         "DnsNameServers": str,
         "NetworkType": str,
     },
 )
 
-RecommendationOutputTypeDef = TypedDict(
-    "RecommendationOutputTypeDef",
+RecommendationTypeDef = TypedDict(
+    "RecommendationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "CreatedDate": str,
         "Status": str,
         "Preferred": bool,
         "Settings": RecommendationSettingsOutputTypeDef,
-        "Data": RecommendationDataOutputTypeDef,
+        "Data": RecommendationDataTypeDef,
     },
 )
 
-CreateReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "CreateReplicationInstanceResponseOutputTypeDef",
+CreateReplicationInstanceResponseTypeDef = TypedDict(
+    "CreateReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationInstanceResponseOutputTypeDef",
+DeleteReplicationInstanceResponseTypeDef = TypedDict(
+    "DeleteReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstancesResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationInstancesResponseOutputTypeDef",
+DescribeReplicationInstancesResponseTypeDef = TypedDict(
+    "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationInstances": List[ReplicationInstanceOutputTypeDef],
+        "ReplicationInstances": List[ReplicationInstanceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationInstanceResponseOutputTypeDef",
+ModifyReplicationInstanceResponseTypeDef = TypedDict(
+    "ModifyReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RebootReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "RebootReplicationInstanceResponseOutputTypeDef",
+RebootReplicationInstanceResponseTypeDef = TypedDict(
+    "RebootReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationsResponseOutputTypeDef = TypedDict(
-    "DescribeRecommendationsResponseOutputTypeDef",
+DescribeRecommendationsResponseTypeDef = TypedDict(
+    "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "Recommendations": List[RecommendationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/type_defs.pyi` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dms.type_defs import AccountQuotaOutputTypeDef
+    from mypy_boto3_dms.type_defs import AccountQuotaTypeDef
 
-    data: AccountQuotaOutputTypeDef = {...}
+    data: AccountQuotaTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -60,27 +60,27 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccountQuotaOutputTypeDef",
+    "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "AvailabilityZoneOutputTypeDef",
-    "BatchStartRecommendationsErrorEntryOutputTypeDef",
+    "AvailabilityZoneTypeDef",
+    "BatchStartRecommendationsErrorEntryTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
-    "CertificateOutputTypeDef",
-    "CollectorHealthCheckOutputTypeDef",
-    "InventoryDataOutputTypeDef",
-    "CollectorShortInfoResponseOutputTypeDef",
+    "CertificateTypeDef",
+    "CollectorHealthCheckTypeDef",
+    "InventoryDataTypeDef",
+    "CollectorShortInfoResponseTypeDef",
     "ComputeConfigOutputTypeDef",
     "ComputeConfigTypeDef",
-    "ConnectionOutputTypeDef",
+    "ConnectionTypeDef",
     "DmsTransferSettingsTypeDef",
     "DocDbSettingsTypeDef",
     "DynamoDbSettingsTypeDef",
     "ElasticsearchSettingsTypeDef",
     "GcpMySQLSettingsTypeDef",
     "IBMDb2SettingsTypeDef",
     "KafkaSettingsTypeDef",
@@ -92,60 +92,60 @@
     "OracleSettingsTypeDef",
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "TimestreamSettingsTypeDef",
-    "EventSubscriptionOutputTypeDef",
+    "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
-    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
-    "ServerShortInfoResponseOutputTypeDef",
-    "DatabaseShortInfoResponseOutputTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
+    "ServerShortInfoResponseTypeDef",
+    "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
-    "EndpointSettingOutputTypeDef",
-    "SupportedEndpointTypeOutputTypeDef",
-    "EventCategoryGroupOutputTypeDef",
-    "EventOutputTypeDef",
+    "EndpointSettingTypeDef",
+    "SupportedEndpointTypeTypeDef",
+    "EventCategoryGroupTypeDef",
+    "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
-    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
-    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
+    "FleetAdvisorLsaAnalysisResponseTypeDef",
+    "FleetAdvisorSchemaObjectResponseTypeDef",
     "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
-    "OrderableReplicationInstanceOutputTypeDef",
-    "LimitationOutputTypeDef",
+    "OrderableReplicationInstanceTypeDef",
+    "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
-    "RefreshSchemasStatusOutputTypeDef",
+    "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
-    "ReplicationInstanceTaskLogOutputTypeDef",
-    "TableStatisticsOutputTypeDef",
+    "ReplicationInstanceTaskLogTypeDef",
+    "TableStatisticsTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
-    "ReplicationTaskAssessmentResultOutputTypeDef",
-    "ReplicationTaskIndividualAssessmentOutputTypeDef",
+    "ReplicationTaskAssessmentResultTypeDef",
+    "ReplicationTaskIndividualAssessmentTypeDef",
     "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "DescribeSchemasResponseOutputTypeDef",
+    "DescribeSchemasResponseTypeDef",
     "DmsTransferSettingsOutputTypeDef",
     "DocDbSettingsOutputTypeDef",
     "DynamoDbSettingsOutputTypeDef",
     "ElasticsearchSettingsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GcpMySQLSettingsOutputTypeDef",
     "IBMDb2SettingsOutputTypeDef",
@@ -166,69 +166,69 @@
     "TagOutputTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PendingMaintenanceActionOutputTypeDef",
-    "ProvisionDataOutputTypeDef",
-    "RdsConfigurationOutputTypeDef",
-    "RdsRequirementsOutputTypeDef",
+    "PendingMaintenanceActionTypeDef",
+    "ProvisionDataTypeDef",
+    "RdsConfigurationTypeDef",
+    "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsOutputTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
-    "ReloadReplicationTablesResponseOutputTypeDef",
-    "ReloadTablesResponseOutputTypeDef",
+    "ReloadReplicationTablesResponseTypeDef",
+    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ReplicationPendingModifiedValuesOutputTypeDef",
-    "VpcSecurityGroupMembershipOutputTypeDef",
-    "ReplicationStatsOutputTypeDef",
-    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
-    "ReplicationTaskStatsOutputTypeDef",
+    "ReplicationPendingModifiedValuesTypeDef",
+    "VpcSecurityGroupMembershipTypeDef",
+    "ReplicationStatsTypeDef",
+    "ReplicationTaskAssessmentRunProgressTypeDef",
+    "ReplicationTaskStatsTypeDef",
     "ResponseMetadataTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
-    "SchemaShortInfoResponseOutputTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    "SchemaShortInfoResponseTypeDef",
     "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
-    "DescribeAccountAttributesResponseOutputTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "SubnetOutputTypeDef",
-    "BatchStartRecommendationsResponseOutputTypeDef",
-    "DeleteCertificateResponseOutputTypeDef",
-    "DescribeCertificatesResponseOutputTypeDef",
-    "ImportCertificateResponseOutputTypeDef",
-    "CollectorResponseOutputTypeDef",
-    "ReplicationConfigOutputTypeDef",
+    "SubnetTypeDef",
+    "BatchStartRecommendationsResponseTypeDef",
+    "DeleteCertificateResponseTypeDef",
+    "DescribeCertificatesResponseTypeDef",
+    "ImportCertificateResponseTypeDef",
+    "CollectorResponseTypeDef",
+    "ReplicationConfigTypeDef",
     "CreateReplicationConfigMessageRequestTypeDef",
     "ModifyReplicationConfigMessageRequestTypeDef",
-    "DeleteConnectionResponseOutputTypeDef",
-    "DescribeConnectionsResponseOutputTypeDef",
-    "TestConnectionResponseOutputTypeDef",
+    "DeleteConnectionResponseTypeDef",
+    "DescribeConnectionsResponseTypeDef",
+    "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
-    "CreateEventSubscriptionResponseOutputTypeDef",
-    "DeleteEventSubscriptionResponseOutputTypeDef",
-    "DescribeEventSubscriptionsResponseOutputTypeDef",
-    "ModifyEventSubscriptionResponseOutputTypeDef",
-    "DatabaseResponseOutputTypeDef",
+    "CreateEventSubscriptionResponseTypeDef",
+    "DeleteEventSubscriptionResponseTypeDef",
+    "DescribeEventSubscriptionsResponseTypeDef",
+    "ModifyEventSubscriptionResponseTypeDef",
+    "DatabaseResponseTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
     "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
     "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
@@ -262,87 +262,87 @@
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef",
-    "DescribeEndpointSettingsResponseOutputTypeDef",
-    "DescribeEndpointTypesResponseOutputTypeDef",
-    "DescribeEventCategoriesResponseOutputTypeDef",
-    "DescribeEventsResponseOutputTypeDef",
-    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
-    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
-    "DescribeRecommendationLimitationsResponseOutputTypeDef",
-    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
-    "RefreshSchemasResponseOutputTypeDef",
-    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
-    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
-    "DescribeTableStatisticsResponseOutputTypeDef",
-    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
-    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
-    "EndpointOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
-    "ResourcePendingMaintenanceActionsOutputTypeDef",
-    "RdsRecommendationOutputTypeDef",
+    "DescribeEndpointSettingsResponseTypeDef",
+    "DescribeEndpointTypesResponseTypeDef",
+    "DescribeEventCategoriesResponseTypeDef",
+    "DescribeEventsResponseTypeDef",
+    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
+    "DescribeOrderableReplicationInstancesResponseTypeDef",
+    "DescribeRecommendationLimitationsResponseTypeDef",
+    "DescribeRefreshSchemasStatusResponseTypeDef",
+    "RefreshSchemasResponseTypeDef",
+    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
+    "DescribeReplicationTableStatisticsResponseTypeDef",
+    "DescribeTableStatisticsResponseTypeDef",
+    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
+    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
+    "EndpointTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResourcePendingMaintenanceActionsTypeDef",
+    "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadReplicationTablesMessageRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
-    "ReplicationOutputTypeDef",
-    "ReplicationTaskAssessmentRunOutputTypeDef",
-    "ReplicationTaskOutputTypeDef",
-    "SchemaResponseOutputTypeDef",
-    "ReplicationSubnetGroupOutputTypeDef",
-    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
-    "CreateReplicationConfigResponseOutputTypeDef",
-    "DeleteReplicationConfigResponseOutputTypeDef",
-    "DescribeReplicationConfigsResponseOutputTypeDef",
-    "ModifyReplicationConfigResponseOutputTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
-    "CreateEndpointResponseOutputTypeDef",
-    "DeleteEndpointResponseOutputTypeDef",
-    "DescribeEndpointsResponseOutputTypeDef",
-    "ModifyEndpointResponseOutputTypeDef",
-    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
-    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
-    "RecommendationDataOutputTypeDef",
+    "ReplicationTypeDef",
+    "ReplicationTaskAssessmentRunTypeDef",
+    "ReplicationTaskTypeDef",
+    "SchemaResponseTypeDef",
+    "ReplicationSubnetGroupTypeDef",
+    "DescribeFleetAdvisorCollectorsResponseTypeDef",
+    "CreateReplicationConfigResponseTypeDef",
+    "DeleteReplicationConfigResponseTypeDef",
+    "DescribeReplicationConfigsResponseTypeDef",
+    "ModifyReplicationConfigResponseTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "DeleteEndpointResponseTypeDef",
+    "DescribeEndpointsResponseTypeDef",
+    "ModifyEndpointResponseTypeDef",
+    "ApplyPendingMaintenanceActionResponseTypeDef",
+    "DescribePendingMaintenanceActionsResponseTypeDef",
+    "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
-    "DescribeReplicationsResponseOutputTypeDef",
-    "StartReplicationResponseOutputTypeDef",
-    "StopReplicationResponseOutputTypeDef",
-    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
-    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
-    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
-    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
-    "CreateReplicationTaskResponseOutputTypeDef",
-    "DeleteReplicationTaskResponseOutputTypeDef",
-    "DescribeReplicationTasksResponseOutputTypeDef",
-    "ModifyReplicationTaskResponseOutputTypeDef",
-    "MoveReplicationTaskResponseOutputTypeDef",
-    "StartReplicationTaskAssessmentResponseOutputTypeDef",
-    "StartReplicationTaskResponseOutputTypeDef",
-    "StopReplicationTaskResponseOutputTypeDef",
-    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
-    "CreateReplicationSubnetGroupResponseOutputTypeDef",
-    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
-    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
-    "ReplicationInstanceOutputTypeDef",
-    "RecommendationOutputTypeDef",
-    "CreateReplicationInstanceResponseOutputTypeDef",
-    "DeleteReplicationInstanceResponseOutputTypeDef",
-    "DescribeReplicationInstancesResponseOutputTypeDef",
-    "ModifyReplicationInstanceResponseOutputTypeDef",
-    "RebootReplicationInstanceResponseOutputTypeDef",
-    "DescribeRecommendationsResponseOutputTypeDef",
+    "DescribeReplicationsResponseTypeDef",
+    "StartReplicationResponseTypeDef",
+    "StopReplicationResponseTypeDef",
+    "CancelReplicationTaskAssessmentRunResponseTypeDef",
+    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
+    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
+    "StartReplicationTaskAssessmentRunResponseTypeDef",
+    "CreateReplicationTaskResponseTypeDef",
+    "DeleteReplicationTaskResponseTypeDef",
+    "DescribeReplicationTasksResponseTypeDef",
+    "ModifyReplicationTaskResponseTypeDef",
+    "MoveReplicationTaskResponseTypeDef",
+    "StartReplicationTaskAssessmentResponseTypeDef",
+    "StartReplicationTaskResponseTypeDef",
+    "StopReplicationTaskResponseTypeDef",
+    "DescribeFleetAdvisorSchemasResponseTypeDef",
+    "CreateReplicationSubnetGroupResponseTypeDef",
+    "DescribeReplicationSubnetGroupsResponseTypeDef",
+    "ModifyReplicationSubnetGroupResponseTypeDef",
+    "ReplicationInstanceTypeDef",
+    "RecommendationTypeDef",
+    "CreateReplicationInstanceResponseTypeDef",
+    "DeleteReplicationInstanceResponseTypeDef",
+    "DescribeReplicationInstancesResponseTypeDef",
+    "ModifyReplicationInstanceResponseTypeDef",
+    "RebootReplicationInstanceResponseTypeDef",
+    "DescribeRecommendationsResponseTypeDef",
 )
 
-AccountQuotaOutputTypeDef = TypedDict(
-    "AccountQuotaOutputTypeDef",
+AccountQuotaTypeDef = TypedDict(
+    "AccountQuotaTypeDef",
     {
         "AccountQuotaName": str,
         "Used": int,
         "Max": int,
     },
 )
 
@@ -361,73 +361,73 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
     },
 )
 
-AvailabilityZoneOutputTypeDef = TypedDict(
-    "AvailabilityZoneOutputTypeDef",
+AvailabilityZoneTypeDef = TypedDict(
+    "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
 )
 
-BatchStartRecommendationsErrorEntryOutputTypeDef = TypedDict(
-    "BatchStartRecommendationsErrorEntryOutputTypeDef",
+BatchStartRecommendationsErrorEntryTypeDef = TypedDict(
+    "BatchStartRecommendationsErrorEntryTypeDef",
     {
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
 )
 
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
 )
 
-CertificateOutputTypeDef = TypedDict(
-    "CertificateOutputTypeDef",
+CertificateTypeDef = TypedDict(
+    "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateCreationDate": datetime,
         "CertificatePem": str,
         "CertificateWallet": bytes,
         "CertificateArn": str,
         "CertificateOwner": str,
         "ValidFromDate": datetime,
         "ValidToDate": datetime,
         "SigningAlgorithm": str,
         "KeyLength": int,
     },
 )
 
-CollectorHealthCheckOutputTypeDef = TypedDict(
-    "CollectorHealthCheckOutputTypeDef",
+CollectorHealthCheckTypeDef = TypedDict(
+    "CollectorHealthCheckTypeDef",
     {
         "CollectorStatus": CollectorStatusType,
         "LocalCollectorS3Access": bool,
         "WebCollectorS3Access": bool,
         "WebCollectorGrantedRoleBasedAccess": bool,
     },
 )
 
-InventoryDataOutputTypeDef = TypedDict(
-    "InventoryDataOutputTypeDef",
+InventoryDataTypeDef = TypedDict(
+    "InventoryDataTypeDef",
     {
         "NumberOfDatabases": int,
         "NumberOfSchemas": int,
     },
 )
 
-CollectorShortInfoResponseOutputTypeDef = TypedDict(
-    "CollectorShortInfoResponseOutputTypeDef",
+CollectorShortInfoResponseTypeDef = TypedDict(
+    "CollectorShortInfoResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
 )
 
 ComputeConfigOutputTypeDef = TypedDict(
@@ -457,16 +457,16 @@
         "PreferredMaintenanceWindow": str,
         "ReplicationSubnetGroupId": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-ConnectionOutputTypeDef = TypedDict(
-    "ConnectionOutputTypeDef",
+ConnectionTypeDef = TypedDict(
+    "ConnectionTypeDef",
     {
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
         "EndpointIdentifier": str,
         "ReplicationInstanceIdentifier": str,
@@ -924,16 +924,16 @@
 )
 
 class TimestreamSettingsTypeDef(
     _RequiredTimestreamSettingsTypeDef, _OptionalTimestreamSettingsTypeDef
 ):
     pass
 
-EventSubscriptionOutputTypeDef = TypedDict(
-    "EventSubscriptionOutputTypeDef",
+EventSubscriptionTypeDef = TypedDict(
+    "EventSubscriptionTypeDef",
     {
         "CustomerAwsId": str,
         "CustSubscriptionId": str,
         "SnsTopicArn": str,
         "Status": str,
         "SubscriptionCreationTime": str,
         "SourceType": str,
@@ -961,50 +961,50 @@
 
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
-CreateFleetAdvisorCollectorResponseOutputTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseOutputTypeDef",
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "Description": str,
         "ServiceAccessRoleArn": str,
         "S3BucketName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseInstanceSoftwareDetailsResponseOutputTypeDef = TypedDict(
-    "DatabaseInstanceSoftwareDetailsResponseOutputTypeDef",
+DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
+    "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
         "SupportLevel": str,
         "OsArchitecture": int,
         "Tooltip": str,
     },
 )
 
-ServerShortInfoResponseOutputTypeDef = TypedDict(
-    "ServerShortInfoResponseOutputTypeDef",
+ServerShortInfoResponseTypeDef = TypedDict(
+    "ServerShortInfoResponseTypeDef",
     {
         "ServerId": str,
         "IpAddress": str,
         "ServerName": str,
     },
 )
 
-DatabaseShortInfoResponseOutputTypeDef = TypedDict(
-    "DatabaseShortInfoResponseOutputTypeDef",
+DatabaseShortInfoResponseTypeDef = TypedDict(
+    "DatabaseShortInfoResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
         "DatabaseEngine": str,
     },
 )
@@ -1048,16 +1048,16 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
-DeleteFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseOutputTypeDef",
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     {
         "DatabaseIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
@@ -1105,16 +1105,16 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeApplicableIndividualAssessmentsResponseOutputTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseOutputTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
         "IndividualAssessmentNames": List[str],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1152,50 +1152,50 @@
 
 class DescribeEndpointSettingsMessageRequestTypeDef(
     _RequiredDescribeEndpointSettingsMessageRequestTypeDef,
     _OptionalDescribeEndpointSettingsMessageRequestTypeDef,
 ):
     pass
 
-EndpointSettingOutputTypeDef = TypedDict(
-    "EndpointSettingOutputTypeDef",
+EndpointSettingTypeDef = TypedDict(
+    "EndpointSettingTypeDef",
     {
         "Name": str,
         "Type": EndpointSettingTypeValueType,
         "EnumValues": List[str],
         "Sensitive": bool,
         "Units": str,
         "Applicability": str,
         "IntValueMin": int,
         "IntValueMax": int,
         "DefaultValue": str,
     },
 )
 
-SupportedEndpointTypeOutputTypeDef = TypedDict(
-    "SupportedEndpointTypeOutputTypeDef",
+SupportedEndpointTypeTypeDef = TypedDict(
+    "SupportedEndpointTypeTypeDef",
     {
         "EngineName": str,
         "SupportsCDC": bool,
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
 )
 
-EventCategoryGroupOutputTypeDef = TypedDict(
-    "EventCategoryGroupOutputTypeDef",
+EventCategoryGroupTypeDef = TypedDict(
+    "EventCategoryGroupTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
 )
 
-EventOutputTypeDef = TypedDict(
-    "EventOutputTypeDef",
+EventTypeDef = TypedDict(
+    "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
     },
@@ -1206,24 +1206,24 @@
     {
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-FleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
-    "FleetAdvisorLsaAnalysisResponseOutputTypeDef",
+FleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "FleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
     },
 )
 
-FleetAdvisorSchemaObjectResponseOutputTypeDef = TypedDict(
-    "FleetAdvisorSchemaObjectResponseOutputTypeDef",
+FleetAdvisorSchemaObjectResponseTypeDef = TypedDict(
+    "FleetAdvisorSchemaObjectResponseTypeDef",
     {
         "SchemaId": str,
         "ObjectType": str,
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
@@ -1242,31 +1242,31 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-OrderableReplicationInstanceOutputTypeDef = TypedDict(
-    "OrderableReplicationInstanceOutputTypeDef",
+OrderableReplicationInstanceTypeDef = TypedDict(
+    "OrderableReplicationInstanceTypeDef",
     {
         "EngineVersion": str,
         "ReplicationInstanceClass": str,
         "StorageType": str,
         "MinAllocatedStorage": int,
         "MaxAllocatedStorage": int,
         "DefaultAllocatedStorage": int,
         "IncludedAllocatedStorage": int,
         "AvailabilityZones": List[str],
         "ReleaseStatus": ReleaseStatusValuesType,
     },
 )
 
-LimitationOutputTypeDef = TypedDict(
-    "LimitationOutputTypeDef",
+LimitationTypeDef = TypedDict(
+    "LimitationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "Name": str,
         "Description": str,
         "Impact": str,
         "Type": str,
@@ -1276,16 +1276,16 @@
 DescribeRefreshSchemasStatusMessageRequestTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
-RefreshSchemasStatusOutputTypeDef = TypedDict(
-    "RefreshSchemasStatusOutputTypeDef",
+RefreshSchemasStatusTypeDef = TypedDict(
+    "RefreshSchemasStatusTypeDef",
     {
         "EndpointArn": str,
         "ReplicationInstanceArn": str,
         "Status": RefreshSchemasStatusTypeValueType,
         "LastRefreshDate": datetime,
         "LastFailureMessage": str,
     },
@@ -1308,25 +1308,25 @@
 
 class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(
     _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     _OptionalDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
 ):
     pass
 
-ReplicationInstanceTaskLogOutputTypeDef = TypedDict(
-    "ReplicationInstanceTaskLogOutputTypeDef",
+ReplicationInstanceTaskLogTypeDef = TypedDict(
+    "ReplicationInstanceTaskLogTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
 )
 
-TableStatisticsOutputTypeDef = TypedDict(
-    "TableStatisticsOutputTypeDef",
+TableStatisticsTypeDef = TypedDict(
+    "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
         "Updates": int,
         "Ddls": int,
@@ -1365,29 +1365,29 @@
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-ReplicationTaskAssessmentResultOutputTypeDef = TypedDict(
-    "ReplicationTaskAssessmentResultOutputTypeDef",
+ReplicationTaskAssessmentResultTypeDef = TypedDict(
+    "ReplicationTaskAssessmentResultTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "ReplicationTaskArn": str,
         "ReplicationTaskLastAssessmentDate": datetime,
         "AssessmentStatus": str,
         "AssessmentResultsFile": str,
         "AssessmentResults": str,
         "S3ObjectUrl": str,
     },
 )
 
-ReplicationTaskIndividualAssessmentOutputTypeDef = TypedDict(
-    "ReplicationTaskIndividualAssessmentOutputTypeDef",
+ReplicationTaskIndividualAssessmentTypeDef = TypedDict(
+    "ReplicationTaskIndividualAssessmentTypeDef",
     {
         "ReplicationTaskIndividualAssessmentArn": str,
         "ReplicationTaskAssessmentRunArn": str,
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
@@ -1429,16 +1429,16 @@
 )
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
-DescribeSchemasResponseOutputTypeDef = TypedDict(
-    "DescribeSchemasResponseOutputTypeDef",
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
     {
         "Marker": str,
         "Schemas": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1983,55 +1983,55 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PendingMaintenanceActionOutputTypeDef = TypedDict(
-    "PendingMaintenanceActionOutputTypeDef",
+PendingMaintenanceActionTypeDef = TypedDict(
+    "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
 )
 
-ProvisionDataOutputTypeDef = TypedDict(
-    "ProvisionDataOutputTypeDef",
+ProvisionDataTypeDef = TypedDict(
+    "ProvisionDataTypeDef",
     {
         "ProvisionState": str,
         "ProvisionedCapacityUnits": int,
         "DateProvisioned": datetime,
         "IsNewProvisioningAvailable": bool,
         "DateNewProvisioningDataAvailable": datetime,
         "ReasonForNewProvisioningData": str,
     },
 )
 
-RdsConfigurationOutputTypeDef = TypedDict(
-    "RdsConfigurationOutputTypeDef",
+RdsConfigurationTypeDef = TypedDict(
+    "RdsConfigurationTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
         "EngineVersion": str,
     },
 )
 
-RdsRequirementsOutputTypeDef = TypedDict(
-    "RdsRequirementsOutputTypeDef",
+RdsRequirementsTypeDef = TypedDict(
+    "RdsRequirementsTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
@@ -2088,59 +2088,59 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
-ReloadReplicationTablesResponseOutputTypeDef = TypedDict(
-    "ReloadReplicationTablesResponseOutputTypeDef",
+ReloadReplicationTablesResponseTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseTypeDef",
     {
         "ReplicationConfigArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReloadTablesResponseOutputTypeDef = TypedDict(
-    "ReloadTablesResponseOutputTypeDef",
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ReplicationPendingModifiedValuesOutputTypeDef = TypedDict(
-    "ReplicationPendingModifiedValuesOutputTypeDef",
+ReplicationPendingModifiedValuesTypeDef = TypedDict(
+    "ReplicationPendingModifiedValuesTypeDef",
     {
         "ReplicationInstanceClass": str,
         "AllocatedStorage": int,
         "MultiAZ": bool,
         "EngineVersion": str,
         "NetworkType": str,
     },
 )
 
-VpcSecurityGroupMembershipOutputTypeDef = TypedDict(
-    "VpcSecurityGroupMembershipOutputTypeDef",
+VpcSecurityGroupMembershipTypeDef = TypedDict(
+    "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
 )
 
-ReplicationStatsOutputTypeDef = TypedDict(
-    "ReplicationStatsOutputTypeDef",
+ReplicationStatsTypeDef = TypedDict(
+    "ReplicationStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -2148,24 +2148,24 @@
         "StartDate": datetime,
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunProgressOutputTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunProgressOutputTypeDef",
+ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunProgressTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
 )
 
-ReplicationTaskStatsOutputTypeDef = TypedDict(
-    "ReplicationTaskStatsOutputTypeDef",
+ReplicationTaskStatsTypeDef = TypedDict(
+    "ReplicationTaskStatsTypeDef",
     {
         "FullLoadProgressPercent": int,
         "ElapsedTimeMillis": int,
         "TablesLoaded": int,
         "TablesLoading": int,
         "TablesQueued": int,
         "TablesErrored": int,
@@ -2184,25 +2184,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RunFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "LsaAnalysisId": str,
         "Status": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SchemaShortInfoResponseOutputTypeDef = TypedDict(
-    "SchemaShortInfoResponseOutputTypeDef",
+SchemaShortInfoResponseTypeDef = TypedDict(
+    "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseIpAddress": str,
     },
@@ -2313,26 +2313,26 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
-UpdateSubscriptionsToEventBridgeResponseOutputTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseOutputTypeDef",
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     {
         "Result": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccountAttributesResponseOutputTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseOutputTypeDef",
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
     {
-        "AccountQuotas": List[AccountQuotaOutputTypeDef],
+        "AccountQuotas": List[AccountQuotaTypeDef],
         "UniqueAccountIdentifier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
@@ -2471,77 +2471,77 @@
 )
 
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
-SubnetOutputTypeDef = TypedDict(
-    "SubnetOutputTypeDef",
+SubnetTypeDef = TypedDict(
+    "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
-        "SubnetAvailabilityZone": AvailabilityZoneOutputTypeDef,
+        "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
 )
 
-BatchStartRecommendationsResponseOutputTypeDef = TypedDict(
-    "BatchStartRecommendationsResponseOutputTypeDef",
+BatchStartRecommendationsResponseTypeDef = TypedDict(
+    "BatchStartRecommendationsResponseTypeDef",
     {
-        "ErrorEntries": List[BatchStartRecommendationsErrorEntryOutputTypeDef],
+        "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteCertificateResponseOutputTypeDef = TypedDict(
-    "DeleteCertificateResponseOutputTypeDef",
+DeleteCertificateResponseTypeDef = TypedDict(
+    "DeleteCertificateResponseTypeDef",
     {
-        "Certificate": CertificateOutputTypeDef,
+        "Certificate": CertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCertificatesResponseOutputTypeDef = TypedDict(
-    "DescribeCertificatesResponseOutputTypeDef",
+DescribeCertificatesResponseTypeDef = TypedDict(
+    "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
-        "Certificates": List[CertificateOutputTypeDef],
+        "Certificates": List[CertificateTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ImportCertificateResponseOutputTypeDef = TypedDict(
-    "ImportCertificateResponseOutputTypeDef",
+ImportCertificateResponseTypeDef = TypedDict(
+    "ImportCertificateResponseTypeDef",
     {
-        "Certificate": CertificateOutputTypeDef,
+        "Certificate": CertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CollectorResponseOutputTypeDef = TypedDict(
-    "CollectorResponseOutputTypeDef",
+CollectorResponseTypeDef = TypedDict(
+    "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
         "CollectorVersion": str,
         "VersionStatus": VersionStatusType,
         "Description": str,
         "S3BucketName": str,
         "ServiceAccessRoleArn": str,
-        "CollectorHealthCheck": CollectorHealthCheckOutputTypeDef,
+        "CollectorHealthCheck": CollectorHealthCheckTypeDef,
         "LastDataReceived": str,
         "RegisteredDate": str,
         "CreatedDate": str,
         "ModifiedDate": str,
-        "InventoryData": InventoryDataOutputTypeDef,
+        "InventoryData": InventoryDataTypeDef,
     },
 )
 
-ReplicationConfigOutputTypeDef = TypedDict(
-    "ReplicationConfigOutputTypeDef",
+ReplicationConfigTypeDef = TypedDict(
+    "ReplicationConfigTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "ReplicationConfigArn": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationType": MigrationTypeValueType,
         "ComputeConfig": ComputeConfigOutputTypeDef,
@@ -2604,35 +2604,35 @@
 
 class ModifyReplicationConfigMessageRequestTypeDef(
     _RequiredModifyReplicationConfigMessageRequestTypeDef,
     _OptionalModifyReplicationConfigMessageRequestTypeDef,
 ):
     pass
 
-DeleteConnectionResponseOutputTypeDef = TypedDict(
-    "DeleteConnectionResponseOutputTypeDef",
+DeleteConnectionResponseTypeDef = TypedDict(
+    "DeleteConnectionResponseTypeDef",
     {
-        "Connection": ConnectionOutputTypeDef,
+        "Connection": ConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeConnectionsResponseOutputTypeDef = TypedDict(
-    "DescribeConnectionsResponseOutputTypeDef",
+DescribeConnectionsResponseTypeDef = TypedDict(
+    "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
-        "Connections": List[ConnectionOutputTypeDef],
+        "Connections": List[ConnectionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestConnectionResponseOutputTypeDef = TypedDict(
-    "TestConnectionResponseOutputTypeDef",
+TestConnectionResponseTypeDef = TypedDict(
+    "TestConnectionResponseTypeDef",
     {
-        "Connection": ConnectionOutputTypeDef,
+        "Connection": ConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
@@ -2732,57 +2732,57 @@
 )
 
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
     pass
 
-CreateEventSubscriptionResponseOutputTypeDef = TypedDict(
-    "CreateEventSubscriptionResponseOutputTypeDef",
+CreateEventSubscriptionResponseTypeDef = TypedDict(
+    "CreateEventSubscriptionResponseTypeDef",
     {
-        "EventSubscription": EventSubscriptionOutputTypeDef,
+        "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEventSubscriptionResponseOutputTypeDef = TypedDict(
-    "DeleteEventSubscriptionResponseOutputTypeDef",
+DeleteEventSubscriptionResponseTypeDef = TypedDict(
+    "DeleteEventSubscriptionResponseTypeDef",
     {
-        "EventSubscription": EventSubscriptionOutputTypeDef,
+        "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventSubscriptionsResponseOutputTypeDef = TypedDict(
-    "DescribeEventSubscriptionsResponseOutputTypeDef",
+DescribeEventSubscriptionsResponseTypeDef = TypedDict(
+    "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
-        "EventSubscriptionsList": List[EventSubscriptionOutputTypeDef],
+        "EventSubscriptionsList": List[EventSubscriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEventSubscriptionResponseOutputTypeDef = TypedDict(
-    "ModifyEventSubscriptionResponseOutputTypeDef",
+ModifyEventSubscriptionResponseTypeDef = TypedDict(
+    "ModifyEventSubscriptionResponseTypeDef",
     {
-        "EventSubscription": EventSubscriptionOutputTypeDef,
+        "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseResponseOutputTypeDef = TypedDict(
-    "DatabaseResponseOutputTypeDef",
+DatabaseResponseTypeDef = TypedDict(
+    "DatabaseResponseTypeDef",
     {
         "DatabaseId": str,
         "DatabaseName": str,
         "IpAddress": str,
         "NumberOfSchemas": int,
-        "Server": ServerShortInfoResponseOutputTypeDef,
-        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
-        "Collectors": List[CollectorShortInfoResponseOutputTypeDef],
+        "Server": ServerShortInfoResponseTypeDef,
+        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
+        "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
 )
 
 DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -3242,154 +3242,152 @@
         "Marker": str,
         "WithoutSettings": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEndpointSettingsResponseOutputTypeDef = TypedDict(
-    "DescribeEndpointSettingsResponseOutputTypeDef",
+DescribeEndpointSettingsResponseTypeDef = TypedDict(
+    "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
-        "EndpointSettings": List[EndpointSettingOutputTypeDef],
+        "EndpointSettings": List[EndpointSettingTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointTypesResponseOutputTypeDef = TypedDict(
-    "DescribeEndpointTypesResponseOutputTypeDef",
+DescribeEndpointTypesResponseTypeDef = TypedDict(
+    "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
-        "SupportedEndpointTypes": List[SupportedEndpointTypeOutputTypeDef],
+        "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventCategoriesResponseOutputTypeDef = TypedDict(
-    "DescribeEventCategoriesResponseOutputTypeDef",
+DescribeEventCategoriesResponseTypeDef = TypedDict(
+    "DescribeEventCategoriesResponseTypeDef",
     {
-        "EventCategoryGroupList": List[EventCategoryGroupOutputTypeDef],
+        "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEventsResponseOutputTypeDef = TypedDict(
-    "DescribeEventsResponseOutputTypeDef",
+DescribeEventsResponseTypeDef = TypedDict(
+    "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
-        "Events": List[EventOutputTypeDef],
+        "Events": List[EventTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef",
+DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
-        "Analysis": List[FleetAdvisorLsaAnalysisResponseOutputTypeDef],
+        "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef",
+DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
-        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseOutputTypeDef],
+        "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOrderableReplicationInstancesResponseOutputTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesResponseOutputTypeDef",
+DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
-        "OrderableReplicationInstances": List[OrderableReplicationInstanceOutputTypeDef],
+        "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationLimitationsResponseOutputTypeDef = TypedDict(
-    "DescribeRecommendationLimitationsResponseOutputTypeDef",
+DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
+    "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
-        "Limitations": List[LimitationOutputTypeDef],
+        "Limitations": List[LimitationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRefreshSchemasStatusResponseOutputTypeDef = TypedDict(
-    "DescribeRefreshSchemasStatusResponseOutputTypeDef",
+DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
+    "DescribeRefreshSchemasStatusResponseTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RefreshSchemasResponseOutputTypeDef = TypedDict(
-    "RefreshSchemasResponseOutputTypeDef",
+RefreshSchemasResponseTypeDef = TypedDict(
+    "RefreshSchemasResponseTypeDef",
     {
-        "RefreshSchemasStatus": RefreshSchemasStatusOutputTypeDef,
+        "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstanceTaskLogsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationInstanceTaskLogsResponseOutputTypeDef",
+DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
+    "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
-        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogOutputTypeDef],
+        "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTableStatisticsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTableStatisticsResponseOutputTypeDef",
+DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeReplicationTableStatisticsResponseTypeDef",
     {
         "ReplicationConfigArn": str,
         "Marker": str,
-        "ReplicationTableStatistics": List[TableStatisticsOutputTypeDef],
+        "ReplicationTableStatistics": List[TableStatisticsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTableStatisticsResponseOutputTypeDef = TypedDict(
-    "DescribeTableStatisticsResponseOutputTypeDef",
+DescribeTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
-        "TableStatistics": List[TableStatisticsOutputTypeDef],
+        "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef",
+DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
-        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultOutputTypeDef],
+        "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef",
+DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskIndividualAssessments": List[
-            ReplicationTaskIndividualAssessmentOutputTypeDef
-        ],
+        "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EndpointOutputTypeDef = TypedDict(
-    "EndpointOutputTypeDef",
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
     {
         "EndpointIdentifier": str,
         "EndpointType": ReplicationEndpointTypeValueType,
         "EngineName": str,
         "EngineDisplayName": str,
         "Username": str,
         "ServerName": str,
@@ -3422,35 +3420,35 @@
         "DocDbSettings": DocDbSettingsOutputTypeDef,
         "RedisSettings": RedisSettingsOutputTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsOutputTypeDef,
         "TimestreamSettings": TimestreamSettingsOutputTypeDef,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourcePendingMaintenanceActionsOutputTypeDef = TypedDict(
-    "ResourcePendingMaintenanceActionsOutputTypeDef",
+ResourcePendingMaintenanceActionsTypeDef = TypedDict(
+    "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
-        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionOutputTypeDef],
+        "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
 )
 
-RdsRecommendationOutputTypeDef = TypedDict(
-    "RdsRecommendationOutputTypeDef",
+RdsRecommendationTypeDef = TypedDict(
+    "RdsRecommendationTypeDef",
     {
-        "RequirementsToTarget": RdsRequirementsOutputTypeDef,
-        "TargetConfiguration": RdsConfigurationOutputTypeDef,
+        "RequirementsToTarget": RdsRequirementsTypeDef,
+        "TargetConfiguration": RdsConfigurationTypeDef,
     },
 )
 
 StartRecommendationsRequestEntryTypeDef = TypedDict(
     "StartRecommendationsRequestEntryTypeDef",
     {
         "DatabaseId": str,
@@ -3503,58 +3501,58 @@
 )
 
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
-ReplicationOutputTypeDef = TypedDict(
-    "ReplicationOutputTypeDef",
+ReplicationTypeDef = TypedDict(
+    "ReplicationTypeDef",
     {
         "ReplicationConfigIdentifier": str,
         "ReplicationConfigArn": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationType": MigrationTypeValueType,
         "Status": str,
-        "ProvisionData": ProvisionDataOutputTypeDef,
+        "ProvisionData": ProvisionDataTypeDef,
         "StopReason": str,
         "FailureMessages": List[str],
-        "ReplicationStats": ReplicationStatsOutputTypeDef,
+        "ReplicationStats": ReplicationStatsTypeDef,
         "StartReplicationType": str,
         "CdcStartTime": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationCreateTime": datetime,
         "ReplicationUpdateTime": datetime,
         "ReplicationLastStopTime": datetime,
     },
 )
 
-ReplicationTaskAssessmentRunOutputTypeDef = TypedDict(
-    "ReplicationTaskAssessmentRunOutputTypeDef",
+ReplicationTaskAssessmentRunTypeDef = TypedDict(
+    "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
-        "AssessmentProgress": ReplicationTaskAssessmentRunProgressOutputTypeDef,
+        "AssessmentProgress": ReplicationTaskAssessmentRunProgressTypeDef,
         "LastFailureMessage": str,
         "ServiceAccessRoleArn": str,
         "ResultLocationBucket": str,
         "ResultLocationFolder": str,
         "ResultEncryptionMode": str,
         "ResultKmsKeyArn": str,
         "AssessmentRunName": str,
     },
 )
 
-ReplicationTaskOutputTypeDef = TypedDict(
-    "ReplicationTaskOutputTypeDef",
+ReplicationTaskTypeDef = TypedDict(
+    "ReplicationTaskTypeDef",
     {
         "ReplicationTaskIdentifier": str,
         "SourceEndpointArn": str,
         "TargetEndpointArn": str,
         "ReplicationInstanceArn": str,
         "MigrationType": MigrationTypeValueType,
         "TableMappings": str,
@@ -3564,333 +3562,333 @@
         "StopReason": str,
         "ReplicationTaskCreationDate": datetime,
         "ReplicationTaskStartDate": datetime,
         "CdcStartPosition": str,
         "CdcStopPosition": str,
         "RecoveryCheckpoint": str,
         "ReplicationTaskArn": str,
-        "ReplicationTaskStats": ReplicationTaskStatsOutputTypeDef,
+        "ReplicationTaskStats": ReplicationTaskStatsTypeDef,
         "TaskData": str,
         "TargetReplicationInstanceArn": str,
     },
 )
 
-SchemaResponseOutputTypeDef = TypedDict(
-    "SchemaResponseOutputTypeDef",
+SchemaResponseTypeDef = TypedDict(
+    "SchemaResponseTypeDef",
     {
         "CodeLineCount": int,
         "CodeSize": int,
         "Complexity": str,
-        "Server": ServerShortInfoResponseOutputTypeDef,
-        "DatabaseInstance": DatabaseShortInfoResponseOutputTypeDef,
+        "Server": ServerShortInfoResponseTypeDef,
+        "DatabaseInstance": DatabaseShortInfoResponseTypeDef,
         "SchemaId": str,
         "SchemaName": str,
-        "OriginalSchema": SchemaShortInfoResponseOutputTypeDef,
+        "OriginalSchema": SchemaShortInfoResponseTypeDef,
         "Similarity": float,
     },
 )
 
-ReplicationSubnetGroupOutputTypeDef = TypedDict(
-    "ReplicationSubnetGroupOutputTypeDef",
+ReplicationSubnetGroupTypeDef = TypedDict(
+    "ReplicationSubnetGroupTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
-        "Subnets": List[SubnetOutputTypeDef],
+        "Subnets": List[SubnetTypeDef],
         "SupportedNetworkTypes": List[str],
     },
 )
 
-DescribeFleetAdvisorCollectorsResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorCollectorsResponseOutputTypeDef",
+DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
-        "Collectors": List[CollectorResponseOutputTypeDef],
+        "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationConfigResponseOutputTypeDef = TypedDict(
-    "CreateReplicationConfigResponseOutputTypeDef",
+CreateReplicationConfigResponseTypeDef = TypedDict(
+    "CreateReplicationConfigResponseTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationConfigResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationConfigResponseOutputTypeDef",
+DeleteReplicationConfigResponseTypeDef = TypedDict(
+    "DeleteReplicationConfigResponseTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationConfigsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationConfigsResponseOutputTypeDef",
+DescribeReplicationConfigsResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationConfigs": List[ReplicationConfigOutputTypeDef],
+        "ReplicationConfigs": List[ReplicationConfigTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationConfigResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationConfigResponseOutputTypeDef",
+ModifyReplicationConfigResponseTypeDef = TypedDict(
+    "ModifyReplicationConfigResponseTypeDef",
     {
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorDatabasesResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseOutputTypeDef",
+DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     {
-        "Databases": List[DatabaseResponseOutputTypeDef],
+        "Databases": List[DatabaseResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointResponseOutputTypeDef = TypedDict(
-    "CreateEndpointResponseOutputTypeDef",
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
     {
-        "Endpoint": EndpointOutputTypeDef,
+        "Endpoint": EndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteEndpointResponseOutputTypeDef = TypedDict(
-    "DeleteEndpointResponseOutputTypeDef",
+DeleteEndpointResponseTypeDef = TypedDict(
+    "DeleteEndpointResponseTypeDef",
     {
-        "Endpoint": EndpointOutputTypeDef,
+        "Endpoint": EndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEndpointsResponseOutputTypeDef = TypedDict(
-    "DescribeEndpointsResponseOutputTypeDef",
+DescribeEndpointsResponseTypeDef = TypedDict(
+    "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
-        "Endpoints": List[EndpointOutputTypeDef],
+        "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyEndpointResponseOutputTypeDef = TypedDict(
-    "ModifyEndpointResponseOutputTypeDef",
+ModifyEndpointResponseTypeDef = TypedDict(
+    "ModifyEndpointResponseTypeDef",
     {
-        "Endpoint": EndpointOutputTypeDef,
+        "Endpoint": EndpointTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ApplyPendingMaintenanceActionResponseOutputTypeDef = TypedDict(
-    "ApplyPendingMaintenanceActionResponseOutputTypeDef",
+ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
+    "ApplyPendingMaintenanceActionResponseTypeDef",
     {
-        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsOutputTypeDef,
+        "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePendingMaintenanceActionsResponseOutputTypeDef = TypedDict(
-    "DescribePendingMaintenanceActionsResponseOutputTypeDef",
+DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsResponseTypeDef",
     {
-        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsOutputTypeDef],
+        "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommendationDataOutputTypeDef = TypedDict(
-    "RecommendationDataOutputTypeDef",
+RecommendationDataTypeDef = TypedDict(
+    "RecommendationDataTypeDef",
     {
-        "RdsEngine": RdsRecommendationOutputTypeDef,
+        "RdsEngine": RdsRecommendationTypeDef,
     },
 )
 
 BatchStartRecommendationsRequestRequestTypeDef = TypedDict(
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
     total=False,
 )
 
-DescribeReplicationsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationsResponseOutputTypeDef",
+DescribeReplicationsResponseTypeDef = TypedDict(
+    "DescribeReplicationsResponseTypeDef",
     {
         "Marker": str,
-        "Replications": List[ReplicationOutputTypeDef],
+        "Replications": List[ReplicationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationResponseOutputTypeDef = TypedDict(
-    "StartReplicationResponseOutputTypeDef",
+StartReplicationResponseTypeDef = TypedDict(
+    "StartReplicationResponseTypeDef",
     {
-        "Replication": ReplicationOutputTypeDef,
+        "Replication": ReplicationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationResponseOutputTypeDef = TypedDict(
-    "StopReplicationResponseOutputTypeDef",
+StopReplicationResponseTypeDef = TypedDict(
+    "StopReplicationResponseTypeDef",
     {
-        "Replication": ReplicationOutputTypeDef,
+        "Replication": ReplicationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CancelReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
-    "CancelReplicationTaskAssessmentRunResponseOutputTypeDef",
+CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
+    "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationTaskAssessmentRunResponseOutputTypeDef",
+DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
+    "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef",
+DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunOutputTypeDef],
+        "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentRunResponseOutputTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentRunResponseOutputTypeDef",
+StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
-        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunOutputTypeDef,
+        "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationTaskResponseOutputTypeDef = TypedDict(
-    "CreateReplicationTaskResponseOutputTypeDef",
+CreateReplicationTaskResponseTypeDef = TypedDict(
+    "CreateReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationTaskResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationTaskResponseOutputTypeDef",
+DeleteReplicationTaskResponseTypeDef = TypedDict(
+    "DeleteReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationTasksResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationTasksResponseOutputTypeDef",
+DescribeReplicationTasksResponseTypeDef = TypedDict(
+    "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationTasks": List[ReplicationTaskOutputTypeDef],
+        "ReplicationTasks": List[ReplicationTaskTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationTaskResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationTaskResponseOutputTypeDef",
+ModifyReplicationTaskResponseTypeDef = TypedDict(
+    "ModifyReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MoveReplicationTaskResponseOutputTypeDef = TypedDict(
-    "MoveReplicationTaskResponseOutputTypeDef",
+MoveReplicationTaskResponseTypeDef = TypedDict(
+    "MoveReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskAssessmentResponseOutputTypeDef = TypedDict(
-    "StartReplicationTaskAssessmentResponseOutputTypeDef",
+StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
+    "StartReplicationTaskAssessmentResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReplicationTaskResponseOutputTypeDef = TypedDict(
-    "StartReplicationTaskResponseOutputTypeDef",
+StartReplicationTaskResponseTypeDef = TypedDict(
+    "StartReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopReplicationTaskResponseOutputTypeDef = TypedDict(
-    "StopReplicationTaskResponseOutputTypeDef",
+StopReplicationTaskResponseTypeDef = TypedDict(
+    "StopReplicationTaskResponseTypeDef",
     {
-        "ReplicationTask": ReplicationTaskOutputTypeDef,
+        "ReplicationTask": ReplicationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetAdvisorSchemasResponseOutputTypeDef = TypedDict(
-    "DescribeFleetAdvisorSchemasResponseOutputTypeDef",
+DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
-        "FleetAdvisorSchemas": List[SchemaResponseOutputTypeDef],
+        "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
-    "CreateReplicationSubnetGroupResponseOutputTypeDef",
+CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
+    "CreateReplicationSubnetGroupResponseTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationSubnetGroupsResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsResponseOutputTypeDef",
+DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationSubnetGroups": List[ReplicationSubnetGroupOutputTypeDef],
+        "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationSubnetGroupResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationSubnetGroupResponseOutputTypeDef",
+ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
+    "ModifyReplicationSubnetGroupResponseTypeDef",
     {
-        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReplicationInstanceOutputTypeDef = TypedDict(
-    "ReplicationInstanceOutputTypeDef",
+ReplicationInstanceTypeDef = TypedDict(
+    "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
         "ReplicationInstanceStatus": str,
         "AllocatedStorage": int,
         "InstanceCreateTime": datetime,
-        "VpcSecurityGroups": List[VpcSecurityGroupMembershipOutputTypeDef],
+        "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "AvailabilityZone": str,
-        "ReplicationSubnetGroup": ReplicationSubnetGroupOutputTypeDef,
+        "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
         "PreferredMaintenanceWindow": str,
-        "PendingModifiedValues": ReplicationPendingModifiedValuesOutputTypeDef,
+        "PendingModifiedValues": ReplicationPendingModifiedValuesTypeDef,
         "MultiAZ": bool,
         "EngineVersion": str,
         "AutoMinorVersionUpgrade": bool,
         "KmsKeyId": str,
         "ReplicationInstanceArn": str,
         "ReplicationInstancePublicIpAddress": str,
         "ReplicationInstancePrivateIpAddress": str,
@@ -3901,69 +3899,69 @@
         "SecondaryAvailabilityZone": str,
         "FreeUntil": datetime,
         "DnsNameServers": str,
         "NetworkType": str,
     },
 )
 
-RecommendationOutputTypeDef = TypedDict(
-    "RecommendationOutputTypeDef",
+RecommendationTypeDef = TypedDict(
+    "RecommendationTypeDef",
     {
         "DatabaseId": str,
         "EngineName": str,
         "CreatedDate": str,
         "Status": str,
         "Preferred": bool,
         "Settings": RecommendationSettingsOutputTypeDef,
-        "Data": RecommendationDataOutputTypeDef,
+        "Data": RecommendationDataTypeDef,
     },
 )
 
-CreateReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "CreateReplicationInstanceResponseOutputTypeDef",
+CreateReplicationInstanceResponseTypeDef = TypedDict(
+    "CreateReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "DeleteReplicationInstanceResponseOutputTypeDef",
+DeleteReplicationInstanceResponseTypeDef = TypedDict(
+    "DeleteReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReplicationInstancesResponseOutputTypeDef = TypedDict(
-    "DescribeReplicationInstancesResponseOutputTypeDef",
+DescribeReplicationInstancesResponseTypeDef = TypedDict(
+    "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
-        "ReplicationInstances": List[ReplicationInstanceOutputTypeDef],
+        "ReplicationInstances": List[ReplicationInstanceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "ModifyReplicationInstanceResponseOutputTypeDef",
+ModifyReplicationInstanceResponseTypeDef = TypedDict(
+    "ModifyReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RebootReplicationInstanceResponseOutputTypeDef = TypedDict(
-    "RebootReplicationInstanceResponseOutputTypeDef",
+RebootReplicationInstanceResponseTypeDef = TypedDict(
+    "RebootReplicationInstanceResponseTypeDef",
     {
-        "ReplicationInstance": ReplicationInstanceOutputTypeDef,
+        "ReplicationInstance": ReplicationInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecommendationsResponseOutputTypeDef = TypedDict(
-    "DescribeRecommendationsResponseOutputTypeDef",
+DescribeRecommendationsResponseTypeDef = TypedDict(
+    "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
-        "Recommendations": List[RecommendationOutputTypeDef],
+        "Recommendations": List[RecommendationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.py` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms/waiter.pyi` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/PKG-INFO` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,27 +472,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_dms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
-    AccountQuotaOutputTypeDef,
+    AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    AvailabilityZoneOutputTypeDef,
-    BatchStartRecommendationsErrorEntryOutputTypeDef,
+    AvailabilityZoneTypeDef,
+    BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
-    CertificateOutputTypeDef,
-    CollectorHealthCheckOutputTypeDef,
-    InventoryDataOutputTypeDef,
-    CollectorShortInfoResponseOutputTypeDef,
+    CertificateTypeDef,
+    CollectorHealthCheckTypeDef,
+    InventoryDataTypeDef,
+    CollectorShortInfoResponseTypeDef,
     ComputeConfigOutputTypeDef,
     ComputeConfigTypeDef,
-    ConnectionOutputTypeDef,
+    ConnectionTypeDef,
     DmsTransferSettingsTypeDef,
     DocDbSettingsTypeDef,
     DynamoDbSettingsTypeDef,
     ElasticsearchSettingsTypeDef,
     GcpMySQLSettingsTypeDef,
     IBMDb2SettingsTypeDef,
     KafkaSettingsTypeDef,
@@ -504,60 +504,60 @@
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     TimestreamSettingsTypeDef,
-    EventSubscriptionOutputTypeDef,
+    EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseOutputTypeDef,
-    DatabaseInstanceSoftwareDetailsResponseOutputTypeDef,
-    ServerShortInfoResponseOutputTypeDef,
-    DatabaseShortInfoResponseOutputTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    DatabaseInstanceSoftwareDetailsResponseTypeDef,
+    ServerShortInfoResponseTypeDef,
+    DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseOutputTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationConfigMessageRequestTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseOutputTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
-    EndpointSettingOutputTypeDef,
-    SupportedEndpointTypeOutputTypeDef,
-    EventCategoryGroupOutputTypeDef,
-    EventOutputTypeDef,
+    EndpointSettingTypeDef,
+    SupportedEndpointTypeTypeDef,
+    EventCategoryGroupTypeDef,
+    EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
-    FleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    FleetAdvisorSchemaObjectResponseOutputTypeDef,
+    FleetAdvisorLsaAnalysisResponseTypeDef,
+    FleetAdvisorSchemaObjectResponseTypeDef,
     DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
-    OrderableReplicationInstanceOutputTypeDef,
-    LimitationOutputTypeDef,
+    OrderableReplicationInstanceTypeDef,
+    LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
-    RefreshSchemasStatusOutputTypeDef,
+    RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
-    ReplicationInstanceTaskLogOutputTypeDef,
-    TableStatisticsOutputTypeDef,
+    ReplicationInstanceTaskLogTypeDef,
+    TableStatisticsTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
-    ReplicationTaskAssessmentResultOutputTypeDef,
-    ReplicationTaskIndividualAssessmentOutputTypeDef,
+    ReplicationTaskAssessmentResultTypeDef,
+    ReplicationTaskIndividualAssessmentTypeDef,
     DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseOutputTypeDef,
+    DescribeSchemasResponseTypeDef,
     DmsTransferSettingsOutputTypeDef,
     DocDbSettingsOutputTypeDef,
     DynamoDbSettingsOutputTypeDef,
     ElasticsearchSettingsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GcpMySQLSettingsOutputTypeDef,
     IBMDb2SettingsOutputTypeDef,
@@ -578,69 +578,69 @@
     TagOutputTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
     PaginatorConfigTypeDef,
-    PendingMaintenanceActionOutputTypeDef,
-    ProvisionDataOutputTypeDef,
-    RdsConfigurationOutputTypeDef,
-    RdsRequirementsOutputTypeDef,
+    PendingMaintenanceActionTypeDef,
+    ProvisionDataTypeDef,
+    RdsConfigurationTypeDef,
+    RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsOutputTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadReplicationTablesResponseOutputTypeDef,
-    ReloadTablesResponseOutputTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ReplicationPendingModifiedValuesOutputTypeDef,
-    VpcSecurityGroupMembershipOutputTypeDef,
-    ReplicationStatsOutputTypeDef,
-    ReplicationTaskAssessmentRunProgressOutputTypeDef,
-    ReplicationTaskStatsOutputTypeDef,
+    ReplicationPendingModifiedValuesTypeDef,
+    VpcSecurityGroupMembershipTypeDef,
+    ReplicationStatsTypeDef,
+    ReplicationTaskAssessmentRunProgressTypeDef,
+    ReplicationTaskStatsTypeDef,
     ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    SchemaShortInfoResponseOutputTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    SchemaShortInfoResponseTypeDef,
     StartReplicationMessageRequestTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseOutputTypeDef,
-    DescribeAccountAttributesResponseOutputTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    SubnetOutputTypeDef,
-    BatchStartRecommendationsResponseOutputTypeDef,
-    DeleteCertificateResponseOutputTypeDef,
-    DescribeCertificatesResponseOutputTypeDef,
-    ImportCertificateResponseOutputTypeDef,
-    CollectorResponseOutputTypeDef,
-    ReplicationConfigOutputTypeDef,
+    SubnetTypeDef,
+    BatchStartRecommendationsResponseTypeDef,
+    DeleteCertificateResponseTypeDef,
+    DescribeCertificatesResponseTypeDef,
+    ImportCertificateResponseTypeDef,
+    CollectorResponseTypeDef,
+    ReplicationConfigTypeDef,
     CreateReplicationConfigMessageRequestTypeDef,
     ModifyReplicationConfigMessageRequestTypeDef,
-    DeleteConnectionResponseOutputTypeDef,
-    DescribeConnectionsResponseOutputTypeDef,
-    TestConnectionResponseOutputTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DescribeConnectionsResponseTypeDef,
+    TestConnectionResponseTypeDef,
     CreateEndpointMessageRequestTypeDef,
     ModifyEndpointMessageRequestTypeDef,
-    CreateEventSubscriptionResponseOutputTypeDef,
-    DeleteEventSubscriptionResponseOutputTypeDef,
-    DescribeEventSubscriptionsResponseOutputTypeDef,
-    ModifyEventSubscriptionResponseOutputTypeDef,
-    DatabaseResponseOutputTypeDef,
+    CreateEventSubscriptionResponseTypeDef,
+    DeleteEventSubscriptionResponseTypeDef,
+    DescribeEventSubscriptionsResponseTypeDef,
+    ModifyEventSubscriptionResponseTypeDef,
+    DatabaseResponseTypeDef,
     DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
     DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
     DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
@@ -674,87 +674,87 @@
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef,
-    DescribeEndpointSettingsResponseOutputTypeDef,
-    DescribeEndpointTypesResponseOutputTypeDef,
-    DescribeEventCategoriesResponseOutputTypeDef,
-    DescribeEventsResponseOutputTypeDef,
-    DescribeFleetAdvisorLsaAnalysisResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemaObjectSummaryResponseOutputTypeDef,
-    DescribeOrderableReplicationInstancesResponseOutputTypeDef,
-    DescribeRecommendationLimitationsResponseOutputTypeDef,
-    DescribeRefreshSchemasStatusResponseOutputTypeDef,
-    RefreshSchemasResponseOutputTypeDef,
-    DescribeReplicationInstanceTaskLogsResponseOutputTypeDef,
-    DescribeReplicationTableStatisticsResponseOutputTypeDef,
-    DescribeTableStatisticsResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentResultsResponseOutputTypeDef,
-    DescribeReplicationTaskIndividualAssessmentsResponseOutputTypeDef,
-    EndpointOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ResourcePendingMaintenanceActionsOutputTypeDef,
-    RdsRecommendationOutputTypeDef,
+    DescribeEndpointSettingsResponseTypeDef,
+    DescribeEndpointTypesResponseTypeDef,
+    DescribeEventCategoriesResponseTypeDef,
+    DescribeEventsResponseTypeDef,
+    DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
+    DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
+    DescribeOrderableReplicationInstancesResponseTypeDef,
+    DescribeRecommendationLimitationsResponseTypeDef,
+    DescribeRefreshSchemasStatusResponseTypeDef,
+    RefreshSchemasResponseTypeDef,
+    DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
+    DescribeTableStatisticsResponseTypeDef,
+    DescribeReplicationTaskAssessmentResultsResponseTypeDef,
+    DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
+    EndpointTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResourcePendingMaintenanceActionsTypeDef,
+    RdsRecommendationTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadReplicationTablesMessageRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
-    ReplicationOutputTypeDef,
-    ReplicationTaskAssessmentRunOutputTypeDef,
-    ReplicationTaskOutputTypeDef,
-    SchemaResponseOutputTypeDef,
-    ReplicationSubnetGroupOutputTypeDef,
-    DescribeFleetAdvisorCollectorsResponseOutputTypeDef,
-    CreateReplicationConfigResponseOutputTypeDef,
-    DeleteReplicationConfigResponseOutputTypeDef,
-    DescribeReplicationConfigsResponseOutputTypeDef,
-    ModifyReplicationConfigResponseOutputTypeDef,
-    DescribeFleetAdvisorDatabasesResponseOutputTypeDef,
-    CreateEndpointResponseOutputTypeDef,
-    DeleteEndpointResponseOutputTypeDef,
-    DescribeEndpointsResponseOutputTypeDef,
-    ModifyEndpointResponseOutputTypeDef,
-    ApplyPendingMaintenanceActionResponseOutputTypeDef,
-    DescribePendingMaintenanceActionsResponseOutputTypeDef,
-    RecommendationDataOutputTypeDef,
+    ReplicationTypeDef,
+    ReplicationTaskAssessmentRunTypeDef,
+    ReplicationTaskTypeDef,
+    SchemaResponseTypeDef,
+    ReplicationSubnetGroupTypeDef,
+    DescribeFleetAdvisorCollectorsResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    DeleteEndpointResponseTypeDef,
+    DescribeEndpointsResponseTypeDef,
+    ModifyEndpointResponseTypeDef,
+    ApplyPendingMaintenanceActionResponseTypeDef,
+    DescribePendingMaintenanceActionsResponseTypeDef,
+    RecommendationDataTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
-    DescribeReplicationsResponseOutputTypeDef,
-    StartReplicationResponseOutputTypeDef,
-    StopReplicationResponseOutputTypeDef,
-    CancelReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DeleteReplicationTaskAssessmentRunResponseOutputTypeDef,
-    DescribeReplicationTaskAssessmentRunsResponseOutputTypeDef,
-    StartReplicationTaskAssessmentRunResponseOutputTypeDef,
-    CreateReplicationTaskResponseOutputTypeDef,
-    DeleteReplicationTaskResponseOutputTypeDef,
-    DescribeReplicationTasksResponseOutputTypeDef,
-    ModifyReplicationTaskResponseOutputTypeDef,
-    MoveReplicationTaskResponseOutputTypeDef,
-    StartReplicationTaskAssessmentResponseOutputTypeDef,
-    StartReplicationTaskResponseOutputTypeDef,
-    StopReplicationTaskResponseOutputTypeDef,
-    DescribeFleetAdvisorSchemasResponseOutputTypeDef,
-    CreateReplicationSubnetGroupResponseOutputTypeDef,
-    DescribeReplicationSubnetGroupsResponseOutputTypeDef,
-    ModifyReplicationSubnetGroupResponseOutputTypeDef,
-    ReplicationInstanceOutputTypeDef,
-    RecommendationOutputTypeDef,
-    CreateReplicationInstanceResponseOutputTypeDef,
-    DeleteReplicationInstanceResponseOutputTypeDef,
-    DescribeReplicationInstancesResponseOutputTypeDef,
-    ModifyReplicationInstanceResponseOutputTypeDef,
-    RebootReplicationInstanceResponseOutputTypeDef,
-    DescribeRecommendationsResponseOutputTypeDef,
+    DescribeReplicationsResponseTypeDef,
+    StartReplicationResponseTypeDef,
+    StopReplicationResponseTypeDef,
+    CancelReplicationTaskAssessmentRunResponseTypeDef,
+    DeleteReplicationTaskAssessmentRunResponseTypeDef,
+    DescribeReplicationTaskAssessmentRunsResponseTypeDef,
+    StartReplicationTaskAssessmentRunResponseTypeDef,
+    CreateReplicationTaskResponseTypeDef,
+    DeleteReplicationTaskResponseTypeDef,
+    DescribeReplicationTasksResponseTypeDef,
+    ModifyReplicationTaskResponseTypeDef,
+    MoveReplicationTaskResponseTypeDef,
+    StartReplicationTaskAssessmentResponseTypeDef,
+    StartReplicationTaskResponseTypeDef,
+    StopReplicationTaskResponseTypeDef,
+    DescribeFleetAdvisorSchemasResponseTypeDef,
+    CreateReplicationSubnetGroupResponseTypeDef,
+    DescribeReplicationSubnetGroupsResponseTypeDef,
+    ModifyReplicationSubnetGroupResponseTypeDef,
+    ReplicationInstanceTypeDef,
+    RecommendationTypeDef,
+    CreateReplicationInstanceResponseTypeDef,
+    DeleteReplicationInstanceResponseTypeDef,
+    DescribeReplicationInstancesResponseTypeDef,
+    ModifyReplicationInstanceResponseTypeDef,
+    RebootReplicationInstanceResponseTypeDef,
+    DescribeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaOutputTypeDef:
+def get_structure() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dms-1.28.3.post1/mypy_boto3_dms.egg-info/SOURCES.txt` & `mypy-boto3-dms-1.28.3.post2/mypy_boto3_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.28.3.post1/setup.py` & `mypy-boto3-dms-1.28.3.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dms",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DatabaseMigrationService 1.28.3 service generated with"
-        " mypy-boto3-builder 7.14.7"
+        " mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

