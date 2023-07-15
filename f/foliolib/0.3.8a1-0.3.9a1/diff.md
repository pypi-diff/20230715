# Comparing `tmp/foliolib-0.3.8a1.tar.gz` & `tmp/foliolib-0.3.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliolib-0.3.8a1.tar", last modified: Mon Jul 10 17:46:11 2023, max compression
+gzip compressed data, was "foliolib-0.3.9a1.tar", last modified: Sat Jul 15 07:29:52 2023, max compression
```

## Comparing `foliolib-0.3.8a1.tar` & `foliolib-0.3.9a1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.8a1/COPYING
--rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.8a1/MANIFEST.in
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2752 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2012 2023-07-10 17:43:35.000000 foliolib-0.3.8a1/README.rst
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.371590 foliolib-0.3.8a1/foliolib/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.8a1/foliolib/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-07-10 17:46:09.000000 foliolib-0.3.8a1/foliolib/__version__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.371590 foliolib-0.3.8a1/foliolib/apiBuilder/
--rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.8a1/foliolib/apiBuilder/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.8a1/foliolib/apiBuilder/build_api.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.8a1/foliolib/apiBuilder/cli.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.375590 foliolib-0.3.8a1/foliolib/cli/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3820 2023-06-16 04:28:16.000000 foliolib-0.3.8a1/foliolib/cli/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.375590 foliolib-0.3.8a1/foliolib/cli/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.8a1/foliolib/cli/folio/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.8a1/foliolib/cli/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.8a1/foliolib/cli/main.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.8a1/foliolib/cli/main_err.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.8a1/foliolib/cli/main_noauth.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.8a1/foliolib/cli/module.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.8a1/foliolib/cli/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.8a1/foliolib/cli/orderedGroup.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3892 2023-05-29 05:12:42.000000 foliolib-0.3.8a1/foliolib/cli/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.8a1/foliolib/cli/server.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.8a1/foliolib/cli/tenant.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12652 2023-05-26 13:04:01.000000 foliolib-0.3.8a1/foliolib/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.8a1/foliolib/exceptions.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.375590 foliolib-0.3.8a1/foliolib/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.8a1/foliolib/folio/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.379590 foliolib-0.3.8a1/foliolib/folio/api/
--rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.8a1/foliolib/folio/api/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/audit.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/authtoken.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7100 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/bulkOperations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/calendar.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    40915 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/circulation.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/circulationStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/configuration.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16302 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/consortia.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/copycat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/courses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataExport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataExportSpring.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataExportWorker.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/dataImportConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/diConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/ebsconet.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/email.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5628 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/entitiesLinks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/ermUsage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5745 2023-07-10 17:25:42.000000 foliolib-0.3.8a1/foliolib/folio/api/ermUsageHarvester.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/eusageReports.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/eventConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/feesfines.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/finance.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-07-10 17:25:43.000000 foliolib-0.3.8a1/foliolib/folio/api/financeStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-07-10 17:25:44.000000 foliolib-0.3.8a1/foliolib/folio/api/fincConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/folioCustomFields.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/folioSpringBase.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-07-10 17:25:41.000000 foliolib-0.3.8a1/foliolib/folio/api/folioVertxLib.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-07-10 17:25:44.000000 foliolib-0.3.8a1/foliolib/folio/api/gobi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-07-10 17:25:44.000000 foliolib-0.3.8a1/foliolib/folio/api/idmConnect.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-07-10 17:26:02.000000 foliolib-0.3.8a1/foliolib/folio/api/innReach.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-07-10 17:26:02.000000 foliolib-0.3.8a1/foliolib/folio/api/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/inventoryStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/inventoryUpdate.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/invoice.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/invoiceStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/kbEbscoJava.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/ldp.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/licenses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/login.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/loginSaml.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-07-10 17:26:03.000000 foliolib-0.3.8a1/foliolib/folio/api/marccat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/metaStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/notes.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/notify.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12602 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/oaiPmh.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/orders.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/ordersStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/organizations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/organizationsStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/passwordValidator.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-07-10 17:26:04.000000 foliolib-0.3.8a1/foliolib/folio/api/patron.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/patronBlocks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/permissions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/pubsub.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4777 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/quickMarc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/remoteStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/reservoir.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/rtac.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    18371 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/search.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/sender.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/settings.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/sharedIndex.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-07-10 17:26:05.000000 foliolib-0.3.8a1/foliolib/folio/api/sourceRecordManager.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    29289 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/sourceRecordStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/tags.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/templateEngine.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/userImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24695 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/users.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-07-10 17:26:06.000000 foliolib-0.3.8a1/foliolib/folio/api/usersBl.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.8a1/foliolib/folio/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.8a1/foliolib/folio/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.8a1/foliolib/folio/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.8a1/foliolib/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.8a1/foliolib/folio/inventoryReferenceData.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.8a1/foliolib/folio/users.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.379590 foliolib-0.3.8a1/foliolib/helper/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.8a1/foliolib/helper/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-06-29 05:24:34.000000 foliolib-0.3.8a1/foliolib/helper/database.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.8a1/foliolib/helper/folio.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.8a1/foliolib/helper/modules.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.8a1/foliolib/helper/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6637 2023-05-27 07:21:39.000000 foliolib-0.3.8a1/foliolib/helper/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1518 2023-06-23 09:49:22.000000 foliolib-0.3.8a1/foliolib/helper/tenant.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/foliolib/okapi/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.8a1/foliolib/okapi/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.8a1/foliolib/okapi/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.8a1/foliolib/okapi/kubeClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.8a1/foliolib/okapi/misc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    39439 2023-06-16 08:13:58.000000 foliolib-0.3.8a1/foliolib/okapi/okapiClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.8a1/foliolib/okapi/okapiModule.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17123 2023-06-22 08:42:17.000000 foliolib-0.3.8a1/foliolib/okapi/okapiModuleKubernetes.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-10 17:46:11.371590 foliolib-0.3.8a1/foliolib.egg-info/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2752 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/SOURCES.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/dependency_links.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/entry_points.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/requires.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-07-10 17:46:11.000000 foliolib-0.3.8a1/foliolib.egg-info/top_level.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.8a1/requirements.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-07-10 17:46:11.383590 foliolib-0.3.8a1/setup.cfg
--rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2023-05-29 06:44:32.000000 foliolib-0.3.8a1/setup.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.410090 foliolib-0.3.9a1/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.9a1/COPYING
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.9a1/MANIFEST.in
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2753 2023-07-15 07:29:52.410090 foliolib-0.3.9a1/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2013 2023-07-14 07:29:20.000000 foliolib-0.3.9a1/README.rst
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.402090 foliolib-0.3.9a1/foliolib/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.9a1/foliolib/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-07-15 07:29:49.000000 foliolib-0.3.9a1/foliolib/__version__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.402090 foliolib-0.3.9a1/foliolib/apiBuilder/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.9a1/foliolib/apiBuilder/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.9a1/foliolib/apiBuilder/build_api.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.9a1/foliolib/apiBuilder/cli.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.402090 foliolib-0.3.9a1/foliolib/cli/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3820 2023-06-16 04:28:16.000000 foliolib-0.3.9a1/foliolib/cli/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.402090 foliolib-0.3.9a1/foliolib/cli/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1541 2023-07-11 10:00:13.000000 foliolib-0.3.9a1/foliolib/cli/folio/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3433 2023-07-12 05:56:16.000000 foliolib-0.3.9a1/foliolib/cli/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.9a1/foliolib/cli/main.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.9a1/foliolib/cli/main_err.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.9a1/foliolib/cli/main_noauth.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.9a1/foliolib/cli/module.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.9a1/foliolib/cli/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.9a1/foliolib/cli/orderedGroup.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3892 2023-07-14 03:48:00.000000 foliolib-0.3.9a1/foliolib/cli/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.9a1/foliolib/cli/server.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.9a1/foliolib/cli/tenant.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13254 2023-07-15 06:44:14.000000 foliolib-0.3.9a1/foliolib/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.9a1/foliolib/exceptions.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.402090 foliolib-0.3.9a1/foliolib/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.9a1/foliolib/folio/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.410090 foliolib-0.3.9a1/foliolib/folio/api/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.9a1/foliolib/folio/api/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/audit.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/authtoken.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7100 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/bulkOperations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/calendar.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    40915 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/circulation.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/circulationStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/configuration.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16302 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/consortia.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/copycat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/courses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/dataExport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/dataExportSpring.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/dataExportWorker.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/dataImportConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/diConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/ebsconet.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/email.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5628 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/entitiesLinks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/ermUsage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5745 2023-07-10 17:25:42.000000 foliolib-0.3.9a1/foliolib/folio/api/ermUsageHarvester.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-07-10 17:25:43.000000 foliolib-0.3.9a1/foliolib/folio/api/eusageReports.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-07-10 17:25:43.000000 foliolib-0.3.9a1/foliolib/folio/api/eventConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-07-10 17:25:43.000000 foliolib-0.3.9a1/foliolib/folio/api/feesfines.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-07-10 17:25:43.000000 foliolib-0.3.9a1/foliolib/folio/api/finance.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-07-10 17:25:43.000000 foliolib-0.3.9a1/foliolib/folio/api/financeStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-07-10 17:25:44.000000 foliolib-0.3.9a1/foliolib/folio/api/fincConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/folioCustomFields.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/folioSpringBase.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-07-10 17:25:41.000000 foliolib-0.3.9a1/foliolib/folio/api/folioVertxLib.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-07-10 17:25:44.000000 foliolib-0.3.9a1/foliolib/folio/api/gobi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-07-10 17:25:44.000000 foliolib-0.3.9a1/foliolib/folio/api/idmConnect.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-07-10 17:26:02.000000 foliolib-0.3.9a1/foliolib/folio/api/innReach.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-07-10 17:26:02.000000 foliolib-0.3.9a1/foliolib/folio/api/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/inventoryStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/inventoryUpdate.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/invoice.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/invoiceStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/kbEbscoJava.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/ldp.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/licenses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/login.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/loginSaml.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-07-10 17:26:03.000000 foliolib-0.3.9a1/foliolib/folio/api/marccat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/metaStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/notes.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/notify.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12602 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/oaiPmh.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/orders.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/ordersStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/organizations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/organizationsStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/passwordValidator.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-07-10 17:26:04.000000 foliolib-0.3.9a1/foliolib/folio/api/patron.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/patronBlocks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/permissions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/pubsub.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4777 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/quickMarc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/remoteStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/reservoir.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/rtac.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    18371 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/search.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/sender.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/settings.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/sharedIndex.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-07-10 17:26:05.000000 foliolib-0.3.9a1/foliolib/folio/api/sourceRecordManager.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    29289 2023-07-10 17:26:06.000000 foliolib-0.3.9a1/foliolib/folio/api/sourceRecordStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-07-10 17:26:06.000000 foliolib-0.3.9a1/foliolib/folio/api/tags.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-07-10 17:26:06.000000 foliolib-0.3.9a1/foliolib/folio/api/templateEngine.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-07-10 17:26:06.000000 foliolib-0.3.9a1/foliolib/folio/api/userImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24695 2023-07-10 17:26:06.000000 foliolib-0.3.9a1/foliolib/folio/api/users.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-07-10 17:26:06.000000 foliolib-0.3.9a1/foliolib/folio/api/usersBl.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.9a1/foliolib/folio/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.9a1/foliolib/folio/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.9a1/foliolib/folio/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.9a1/foliolib/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.9a1/foliolib/folio/inventoryReferenceData.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.9a1/foliolib/folio/users.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.410090 foliolib-0.3.9a1/foliolib/helper/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1436 2023-07-13 08:08:57.000000 foliolib-0.3.9a1/foliolib/helper/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9225 2023-07-14 07:35:11.000000 foliolib-0.3.9a1/foliolib/helper/database.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3572 2023-07-14 08:44:58.000000 foliolib-0.3.9a1/foliolib/helper/folio.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5212 2023-07-14 06:23:10.000000 foliolib-0.3.9a1/foliolib/helper/modules.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3827 2023-07-13 16:48:50.000000 foliolib-0.3.9a1/foliolib/helper/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9347 2023-07-14 06:23:10.000000 foliolib-0.3.9a1/foliolib/helper/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1918 2023-07-14 06:27:21.000000 foliolib-0.3.9a1/foliolib/helper/tenant.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.410090 foliolib-0.3.9a1/foliolib/okapi/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.9a1/foliolib/okapi/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.9a1/foliolib/okapi/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16413 2023-07-15 06:48:17.000000 foliolib-0.3.9a1/foliolib/okapi/kubeClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.9a1/foliolib/okapi/misc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    39244 2023-07-14 06:23:10.000000 foliolib-0.3.9a1/foliolib/okapi/okapiClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-07-13 16:49:11.000000 foliolib-0.3.9a1/foliolib/okapi/okapiModule.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    18331 2023-07-15 07:26:25.000000 foliolib-0.3.9a1/foliolib/okapi/okapiModuleKubernetes.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-07-15 07:29:52.402090 foliolib-0.3.9a1/foliolib.egg-info/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2753 2023-07-15 07:29:52.000000 foliolib-0.3.9a1/foliolib.egg-info/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-07-15 07:29:52.000000 foliolib-0.3.9a1/foliolib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-07-15 07:29:52.000000 foliolib-0.3.9a1/foliolib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-07-15 07:29:52.000000 foliolib-0.3.9a1/foliolib.egg-info/entry_points.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-07-15 07:29:52.000000 foliolib-0.3.9a1/foliolib.egg-info/requires.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-07-15 07:29:52.000000 foliolib-0.3.9a1/foliolib.egg-info/top_level.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.9a1/requirements.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-07-15 07:29:52.410090 foliolib-0.3.9a1/setup.cfg
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2023-05-29 06:44:32.000000 foliolib-0.3.9a1/setup.py
```

### Comparing `foliolib-0.3.8a1/COPYING` & `foliolib-0.3.9a1/COPYING`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/PKG-INFO` & `foliolib-0.3.9a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.8a1
+Version: 0.3.9a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -81,15 +81,15 @@
 
     >>> from foliolib import server
     >>> from foliolib.folio.users import Users
     >>> from foliolib.folio.api.inventory import Inventory
     >>>
     >>> server("myServer")
     >>>
-    >>> Users("TenantId").login("UserId","Password")
+    >>> Users("TenantId").login("UserId", "Password")
     >>> inventory = Inventory("TenantId")
     >>> instances = inventory.get_instances(query="title==*")
     >>> print(instances)
 
 Also foliolib provides a command line interface:
 
 .. code-block:: bash
```

### Comparing `foliolib-0.3.8a1/README.rst` & `foliolib-0.3.9a1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     >>> from foliolib import server
     >>> from foliolib.folio.users import Users
     >>> from foliolib.folio.api.inventory import Inventory
     >>>
     >>> server("myServer")
     >>>
-    >>> Users("TenantId").login("UserId","Password")
+    >>> Users("TenantId").login("UserId", "Password")
     >>> inventory = Inventory("TenantId")
     >>> instances = inventory.get_instances(query="title==*")
     >>> print(instances)
 
 Also foliolib provides a command line interface:
 
 .. code-block:: bash
```

### Comparing `foliolib-0.3.8a1/foliolib/__init__.py` & `foliolib-0.3.9a1/foliolib/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/apiBuilder/build_api.py` & `foliolib-0.3.9a1/foliolib/apiBuilder/build_api.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/apiBuilder/cli.py` & `foliolib-0.3.9a1/foliolib/apiBuilder/cli.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/__init__.py` & `foliolib-0.3.9a1/foliolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/folio/__init__.py` & `foliolib-0.3.9a1/foliolib/cli/folio/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2022 Tobias Weber <tobi-weber@gmx.de>
 
 import click
+from foliolib.cli.folio.inventory import inventory
 from foliolib.folio.users import Users
 from foliolib.helper.folio import create_superuser
 
 from ..orderedGroup import OrderedGroup
 
 
 @click.group(cls=OrderedGroup)
@@ -15,15 +16,15 @@
 
 
 @folio.command()
 @click.argument("tenantid")
 @click.option("-u", "--user", default="folio_admin", help=" ", show_default=True)
 @click.option("-p", "--password", default="admin", help=" ", show_default=True)
 def login(**kwargs):
-    """Login into a tenant
+    """Log into a tenant
 
     TENANTID\tThe tenant id.
     """
     print("Login %s with %s:%s" % (kwargs["tenantid"],
                                    kwargs["user"],
                                    kwargs["password"]))
 
@@ -40,7 +41,10 @@
     TENANTID\tThe tenant id.
     """
     print("Create superuser %s:%s for tenant %s" % (kwargs["user"],
                                                     kwargs["password"],
                                                     kwargs["tenantid"]))
     create_superuser(kwargs["tenantid"],
                      kwargs["user"], kwargs["password"])
+
+
+folio.add_command(inventory)
```

### Comparing `foliolib-0.3.8a1/foliolib/cli/main.py` & `foliolib-0.3.9a1/foliolib/cli/main.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/main_noauth.py` & `foliolib-0.3.9a1/foliolib/cli/main_noauth.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/module.py` & `foliolib-0.3.9a1/foliolib/cli/module.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/okapi.py` & `foliolib-0.3.9a1/foliolib/cli/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/platform.py` & `foliolib-0.3.9a1/foliolib/cli/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         _kwargs["simulate"] = True
     if kwargs["no_invoke"]:
         _kwargs["invoke"] = False
     if kwargs["no_npmsnapshot"]:
         _kwargs["npmSnapshot"] = False
     if kwargs["no_prerelease"]:
         _kwargs["preRelease"] = False
-    install_platform(kwargs["platform"], kwargs["node"], kwargs["tenantid"],
+    install_platform(kwargs["platform"], kwargs["tenantid"], kwargs["node"],
                      loadSample=kwargs["loadsample"],
                      loadReference=kwargs["loadreference"],
                      deploy_async=kwargs["deployasync"],
                      **_kwargs)
 
 
 @platform.command()
@@ -89,10 +89,10 @@
         _kwargs["simulate"] = True
     if kwargs["no_invoke"]:
         _kwargs["invoke"] = False
     if kwargs["no_npmsnapshot"]:
         _kwargs["npmSnapshot"] = False
     if kwargs["no_prerelease"]:
         _kwargs["preRelease"] = False
-    upgrade_platform(kwargs["platform"], kwargs["node"], kwargs["tenant"],
+    upgrade_platform(kwargs["platform"], kwargs["tenant"], kwargs["node"],
                      deploy_async=kwargs["deployasync"],
                      exclude=kwargs["exclude"], **_kwargs)
```

### Comparing `foliolib-0.3.8a1/foliolib/cli/server.py` & `foliolib-0.3.9a1/foliolib/cli/server.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/cli/tenant.py` & `foliolib-0.3.9a1/foliolib/cli/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/config.py` & `foliolib-0.3.9a1/foliolib/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020 Tobias Weber <tobi-weber@gmx.de>
+# Copyright (C) 2023 Tobias Weber <tobi-weber@gmx.de>
 
 
 import configparser
 import logging
 import os
 import pathlib
+from typing import Any, Union
 
 from foliolib.exceptions import ServerConfigNotFound
 
 log = logging.getLogger("foliolib.config")
 
 
 class Config:
@@ -37,15 +38,15 @@
         """Get current server name.
 
         Returns:
             str: Current server name.
         """
         return self._server
 
-    def set_server(self, name):
+    def set_server(self, name: str):
         """Set current server name.
 
         Args:
             name (str): Server name
 
         Raises:
             ServerConfigNotFound: Server config not found.
@@ -230,32 +231,51 @@
             bool: Wether foliolib env is enabled.
         """
         is_foliolib_env = self.__servercfg.get(
             "Okapi", "foliolibEnv", fallback=False)
 
         return is_foliolib_env
 
-    def get_env(self, as_dict=False):
+    def get_env(self, as_dict: bool = False):
+        """get global enviroment variables.
+
+        Args:
+            as_dict (bool, optional): Defaults to False.
+
+        Returns:
+            Union[dict, list]: dict, if as_dict is True, else list with enviroments variables.
+        """
         if self.is_foliolib_env():
             if as_dict:
                 return {k: v for k, v in self.__servercfg["Env"].items()}
             else:
                 return [{"name": k, "value": v}
                         for k, v in self.__servercfg["Env"].items()]
         else:
             if as_dict:
                 return {}
             else:
                 return []
 
-    def set_env(self, key, value):
+    def set_env(self, key: str, value: Any):
+        """Set enviroment variable.
+
+        Args:
+            key (str): Name of the enviroment variable.
+            value (Any): Value of the enviroment variable.
+        """
         if self.is_foliolib_env():
             self.set_servercfg("Env", key, value)
 
-    def delete_env(self, key):
+    def delete_env(self, key: str):
+        """Delete enviroment variable.
+
+        Args:
+            key (str): Name of the enviroment variable.
+        """
         if self.is_foliolib_env():
             self.remove_servercfg("Env", key)
 
     def get_confdir(self):
         """Get the configuration directory
 
         Returns:
@@ -350,17 +370,17 @@
         sdir = os.path.join(self.get_confdir(), self.get_server())
         fpath = os.path.join(sdir, "server.conf")
         log.debug("Load config from %s", fpath)
         self.__servercfg.read(fpath)
 
 
 def server(name: str, logging_level: str = "INFO"):
-    """ Load server sonfig for given name.
+    """ Load server config for given name.
 
     Args:
         name (str): Name of the server config.
         logging_level (str, optional): INFO, WARNING, ERROR or DEBUG. Defaults to "INFO".
     """
     from foliolib import set_logging
     set_logging(level=logging_level)
     Config().set_server(name)
-    print("Server is %s" % name)
+    log.info("Server is %s" % name)
```

### Comparing `foliolib-0.3.8a1/foliolib/exceptions.py` & `foliolib-0.3.9a1/foliolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/__init__.py` & `foliolib-0.3.9a1/foliolib/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/audit.py` & `foliolib-0.3.9a1/foliolib/folio/api/audit.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/authtoken.py` & `foliolib-0.3.9a1/foliolib/folio/api/authtoken.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/bulkOperations.py` & `foliolib-0.3.9a1/foliolib/folio/api/bulkOperations.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/calendar.py` & `foliolib-0.3.9a1/foliolib/folio/api/calendar.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/circulation.py` & `foliolib-0.3.9a1/foliolib/folio/api/circulation.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/circulationStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/circulationStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/configuration.py` & `foliolib-0.3.9a1/foliolib/folio/api/configuration.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/consortia.py` & `foliolib-0.3.9a1/foliolib/folio/api/consortia.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/copycat.py` & `foliolib-0.3.9a1/foliolib/folio/api/copycat.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/courses.py` & `foliolib-0.3.9a1/foliolib/folio/api/courses.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/dataExport.py` & `foliolib-0.3.9a1/foliolib/folio/api/dataExport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/dataExportSpring.py` & `foliolib-0.3.9a1/foliolib/folio/api/dataExportSpring.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/dataExportWorker.py` & `foliolib-0.3.9a1/foliolib/folio/api/dataExportWorker.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/dataImport.py` & `foliolib-0.3.9a1/foliolib/folio/api/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/dataImportConverterStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/dataImportConverterStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/diConverterStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/diConverterStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/ebsconet.py` & `foliolib-0.3.9a1/foliolib/folio/api/ebsconet.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/email.py` & `foliolib-0.3.9a1/foliolib/folio/api/email.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/entitiesLinks.py` & `foliolib-0.3.9a1/foliolib/folio/api/entitiesLinks.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/ermUsage.py` & `foliolib-0.3.9a1/foliolib/folio/api/ermUsage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/ermUsageHarvester.py` & `foliolib-0.3.9a1/foliolib/folio/api/ermUsageHarvester.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/eusageReports.py` & `foliolib-0.3.9a1/foliolib/folio/api/eusageReports.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/eventConfig.py` & `foliolib-0.3.9a1/foliolib/folio/api/eventConfig.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/feesfines.py` & `foliolib-0.3.9a1/foliolib/folio/api/feesfines.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/finance.py` & `foliolib-0.3.9a1/foliolib/folio/api/finance.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/financeStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/financeStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/fincConfig.py` & `foliolib-0.3.9a1/foliolib/folio/api/fincConfig.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/folioCustomFields.py` & `foliolib-0.3.9a1/foliolib/folio/api/folioCustomFields.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/folioSpringBase.py` & `foliolib-0.3.9a1/foliolib/folio/api/folioSpringBase.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/folioVertxLib.py` & `foliolib-0.3.9a1/foliolib/folio/api/folioVertxLib.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/gobi.py` & `foliolib-0.3.9a1/foliolib/folio/api/gobi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/idmConnect.py` & `foliolib-0.3.9a1/foliolib/folio/api/idmConnect.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/innReach.py` & `foliolib-0.3.9a1/foliolib/folio/api/innReach.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/inventory.py` & `foliolib-0.3.9a1/foliolib/folio/api/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/inventoryStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/inventoryStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/inventoryUpdate.py` & `foliolib-0.3.9a1/foliolib/folio/api/inventoryUpdate.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/invoice.py` & `foliolib-0.3.9a1/foliolib/folio/api/invoice.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/invoiceStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/invoiceStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/kbEbscoJava.py` & `foliolib-0.3.9a1/foliolib/folio/api/kbEbscoJava.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/ldp.py` & `foliolib-0.3.9a1/foliolib/folio/api/ldp.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/licenses.py` & `foliolib-0.3.9a1/foliolib/folio/api/licenses.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/login.py` & `foliolib-0.3.9a1/foliolib/folio/api/login.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/loginSaml.py` & `foliolib-0.3.9a1/foliolib/folio/api/loginSaml.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/marccat.py` & `foliolib-0.3.9a1/foliolib/folio/api/marccat.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/metaStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/metaStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/notes.py` & `foliolib-0.3.9a1/foliolib/folio/api/notes.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/notify.py` & `foliolib-0.3.9a1/foliolib/folio/api/notify.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/oaiPmh.py` & `foliolib-0.3.9a1/foliolib/folio/api/oaiPmh.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/orders.py` & `foliolib-0.3.9a1/foliolib/folio/api/orders.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/ordersStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/ordersStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/organizations.py` & `foliolib-0.3.9a1/foliolib/folio/api/organizations.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/organizationsStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/organizationsStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/passwordValidator.py` & `foliolib-0.3.9a1/foliolib/folio/api/passwordValidator.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/patron.py` & `foliolib-0.3.9a1/foliolib/folio/api/patron.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/patronBlocks.py` & `foliolib-0.3.9a1/foliolib/folio/api/patronBlocks.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/permissions.py` & `foliolib-0.3.9a1/foliolib/folio/api/permissions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/pubsub.py` & `foliolib-0.3.9a1/foliolib/folio/api/pubsub.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/quickMarc.py` & `foliolib-0.3.9a1/foliolib/folio/api/quickMarc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/remoteStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/remoteStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/reservoir.py` & `foliolib-0.3.9a1/foliolib/folio/api/reservoir.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/rtac.py` & `foliolib-0.3.9a1/foliolib/folio/api/rtac.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/search.py` & `foliolib-0.3.9a1/foliolib/folio/api/search.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/sender.py` & `foliolib-0.3.9a1/foliolib/folio/api/sender.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/settings.py` & `foliolib-0.3.9a1/foliolib/folio/api/settings.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/sharedIndex.py` & `foliolib-0.3.9a1/foliolib/folio/api/sharedIndex.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/sourceRecordManager.py` & `foliolib-0.3.9a1/foliolib/folio/api/sourceRecordManager.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/sourceRecordStorage.py` & `foliolib-0.3.9a1/foliolib/folio/api/sourceRecordStorage.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/tags.py` & `foliolib-0.3.9a1/foliolib/folio/api/tags.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/templateEngine.py` & `foliolib-0.3.9a1/foliolib/folio/api/templateEngine.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/userImport.py` & `foliolib-0.3.9a1/foliolib/folio/api/userImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/users.py` & `foliolib-0.3.9a1/foliolib/folio/api/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/api/usersBl.py` & `foliolib-0.3.9a1/foliolib/folio/api/usersBl.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/config.py` & `foliolib-0.3.9a1/foliolib/folio/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/dataImport.py` & `foliolib-0.3.9a1/foliolib/folio/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/inventory.py` & `foliolib-0.3.9a1/foliolib/folio/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/inventoryReferenceData.py` & `foliolib-0.3.9a1/foliolib/folio/inventoryReferenceData.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/folio/users.py` & `foliolib-0.3.9a1/foliolib/folio/users.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/helper/__init__.py` & `foliolib-0.3.9a1/foliolib/helper/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import base64
 import re
 
 from foliolib.config import Config
 
 
 def get_node():
+    """Get first okapi node.
+
+    Returns:
+        str: node id
+    """
     from foliolib.okapi.okapiClient import OkapiClient
     try:
         nodes = OkapiClient().get_nodes()
     except:
         nodes = []
     try:
         host = Config().servercfg().get("Okapi", "host")
@@ -30,15 +35,23 @@
     for node in nodes:
         if "nodeId" in node:
             return node["nodeId"]
 
     return host
 
 
-def split_modid(modid):
+def split_modid(modid: str):
+    """Split Module id in name and version
+
+    Args:
+        modid (str): Module id
+
+    Returns:
+        tuple: Tuple with module name and id
+    """
     m = re.search(r"-\d+.\d+.\d+", modid)
     if m is not None:
         version = m.group(0)
         modname = modid.replace(version, "")
         version = version[1:]
         return modname, version
     else:
```

### Comparing `foliolib-0.3.8a1/foliolib/helper/database.py` & `foliolib-0.3.9a1/foliolib/helper/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2021 Tobias Weber <tobi-weber@gmx.de>
+# Copyright (C) 2023 Tobias Weber <tobi-weber@gmx.de>
 
 import logging
 
 from foliolib.config import Config
 
 log = logging.getLogger("foliolib.helper.database")
 
@@ -12,200 +12,204 @@
     import psycopg2
     from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
 except:
     log.debug("Cannot import postgres client. You have to install psycopg2.")
 
 
 class Postgres:
-    """Example:
+    """
+    Postgres config can be defined in $HOME/.foliolib/[SERVERNAME]/server.conf:
+
+    .. code-block:: cfg
+
+        [Postgres]
+        host = localhost
+        port = 5432
+        user = postgres
+        password = password
+
+
+    Example:
+
+    .. code-block:: python
+
+        with Postgres(database="okapi_modules") as pg:
+            print(pg.get_schemas())
+            pg.cursor.execute("SELECT * FROM TABLENAME;")
+            print(pg.cursor.fetchall())
 
-    with Postgres(databas="okapi_modules") as pg:
-        print(pg.get_schemas)
     """
 
     def __init__(self, user: str = None, password: str = None, database: str = "postgres",
                  host: str = None, port: str = None) -> None:
         self._host = host or Config().servercfg().get(
             "Postgres", "host", fallback="localhost")
         self._port = port or Config().servercfg().get(
             "Postgres", "port", fallback="5432")
         self._user = user or Config().servercfg().get(
             "Postgres", "user", fallback="postgres")
         self._password = password or Config().servercfg().get(
             "Postgres", "password", fallback="postgres")
         self._database = database
         self._con = None
+        self.cursor = None
 
     def open(self):
         try:
-            log.info("Open postgres database %s on %s:%s with user %s:%s",
-                     self._database, self._host, self._port, self._user, self._password)
+            log.debug("Open postgres database %s on %s:%s with user %s:%s",
+                      self._database, self._host, self._port, self._user, self._password)
             self._con = psycopg2.connect(database=self._database, user=self._user,
                                          password=self._password, host=self._host,
                                          port=self._port)
             self._con.set_isolation_level(ISOLATION_LEVEL_AUTOCOMMIT)
+            self.cursor = self._con.cursor()
         except psycopg2.OperationalError as err:
             log.error("Postgresql: %s", err)
 
     def close(self):
         if self._con is not None:
             self._con.close()
 
-    def cursor(self):
-        return self._con.cursor()
-
     def is_open(self):
         return False if self._con is None else True
 
     def get_databases(self):
-        with self.cursor() as c:
-            c.execute("SELECT datname FROM pg_database")
-            dbs = c.fetchall()
-            return [d[0] for d in dbs]
+        self.cursor.execute("SELECT datname FROM pg_database")
+        dbs = self.cursor.fetchall()
+        return [d[0] for d in dbs]
 
     def create_database(self, dbname: str, user: str):
-        with self.cursor() as c:
-            c.execute(f"CREATE DATABASE {dbname} WITH OWNER {user};")
+        self.cursor.execute(f"CREATE DATABASE {dbname} WITH OWNER {user};")
 
     def drop_database(self, dbname: str, force=False):
-        with self.cursor() as c:
-            c.execute(f"DROP DATABASE {dbname};")
+        self.cursor.execute(f"DROP DATABASE {dbname};")
 
     def get_schemas(self):
         pg_schemas = ["pg_toast",
                       "pg_temp_1",
                       "pg_toast_temp_1",
                       "pg_catalog",
                       # "public",
                       "information_schema"]
-        with self.cursor() as c:
-            c.execute("select schema_name from information_schema.schemata;")
-            schemas = c.fetchall()
-            schemas = [s[0] for s in schemas if s[0] not in pg_schemas]
-            return schemas
+        self.cursor.execute(
+            "select schema_name from information_schema.schemata;")
+        schemas = self.cursor.fetchall()
+        schemas = [s[0] for s in schemas if s[0] not in pg_schemas]
+        return schemas
 
     def create_schema(self, schema: str, user: str = None):
-        with self.cursor() as c:
-            if user is None:
-                log.info("Create Schema %s", schema)
-                c.execute(f"CREATE SCHEMA {schema};")
-            else:
-                log.info("Create Schema %s for user %s", schema, user)
-                c.execute(f"CREATE SCHEMA {schema} AUTHORIZATION {user};")
+        if user is None:
+            log.info("Create Schema %s", schema)
+            self.cursor.execute(f"CREATE SCHEMA {schema};")
+        else:
+            log.info("Create Schema %s for user %s", schema, user)
+            self.cursor.execute(
+                f"CREATE SCHEMA {schema} AUTHORIZATION {user};")
 
     def drop_schema(self, schema: str):
-        with self.cursor() as c:
-            c.execute(f"drop schema {schema} cascade")
+        self.cursor.execute(f"drop schema {schema} cascade")
 
     def get_tables(self, schema: str):
-        with self.cursor() as c:
-            c.execute(f"select * from pg_tables where schemaname='{schema}';")
-            tables = c.fetchall()
-            tables = [t[1] for t in tables]
+        self.cursor.execute(
+            f"select * from pg_tables where schemaname='{schema}';")
+        tables = c.fetchall()
+        tables = [t[1] for t in tables]
 
-            return tables
+        return tables
 
     def get_table_column_names(self, table: str, schema: str = None):
         table = f"{schema}.{table}" if schema else table
         log.debug("Get column names from table %s", table)
-        with self.cursor() as c:
-            s = "SELECT column_name FROM INFORMATION_SCHEMA.COLUMNS WHERE "
-            s += f"table_name = '{table}';"
-            c.execute(s)
-            r = c.fetchall()
-            return r
+        s = "SELECT column_name FROM INFORMATION_SCHEMA.COLUMNS WHERE "
+        s += f"table_name = '{table}';"
+        self.cursor.execute(s)
+        r = self.cursor.fetchall()
+        return r
 
     def get_table_data(self, table: str, schema: str = None, id_=None):
         table = f"{schema}.{table}" if schema else table
         log.debug("Get data from table %s", table)
-        with self.cursor() as c:
-            s = f"SELECT * FROM {table}"
-            if id_ is not None:
-                s += f" WHERE id={id_}"
-            c.execute(s + ";")
-            r = c.fetchall()
-            return r
+        s = f"SELECT * FROM {table}"
+        if id_ is not None:
+            s += f" WHERE id={id_}"
+        self.cursor.execute(s + ";")
+        r = self.cursor.fetchall()
+        return r
 
     def get_table_row_count(self, table: str, schema: str = None):
         table = f"{schema}.{table}" if schema else table
         log.debug("Get row count from table %s", table)
-        with self.cursor() as c:
-            c.execute(f"SELECT count(*) FROM {table};")
-            r = c.fetchall()[0][0]
-            return r
+        self.cursor.execute(f"SELECT count(*) FROM {table};")
+        r = self.cursor.fetchall()[0][0]
+        return r
 
     def delete_rows_from_table(self, table: str, schema: str = None,
                                ids=[]):
         table = f"{schema}.{table}" if schema else table
-        with self.cursor() as c:
-            for id_ in ids:
-                log.debug("Delete %s in table %s", (id_, table))
-                c.execute(f"DELETE FROM {table} WHERE id={id_};")
+        for id_ in ids:
+            log.debug("Delete %s in table %s", (id_, table))
+            self.cursor.execute(f"DELETE FROM {table} WHERE id={id_};")
 
     def clear_table(self, table: str, schema: str = None):
         table = f"{schema}.{table}" if schema else table
         log.debug("Clear table %s", table)
-        with self._con.cursor() as c:
-            c.execute(f"TRUNCATE TABLE {table} CONTINUE IDENTITY CASCADE;")
+        self.cursor.execute(
+            f"TRUNCATE TABLE {table} CONTINUE IDENTITY CASCADE;")
 
     def drop_table(self, table: str, schema: str = None):
         table = f"{schema}.{table}" if schema else table
         log.debug("Drop table %s", table)
-        with self._con.cursor() as c:
-            c.execute(f"DROP TABLE {table};")
+        self.cursor.execute(f"DROP TABLE {table};")
 
     def get_users(self):
-        with self.cursor() as c:
-            c.execute("""select usesysid as user_id,
-                        usename as username,
-                        usesuper as is_superuser,
-                        passwd as password_md5,
-                        valuntil as password_expiration
-                        from pg_shadow
-                        order by usename;""")
-            users = c.fetchall()
-            return [u[1] for u in users]
+        self.cursor.execute("""select usesysid as user_id,
+                    usename as username,
+                    usesuper as is_superuser,
+                    passwd as password_md5,
+                    valuntil as password_expiration
+                    from pg_shadow
+                    order by usename;""")
+        users = self.cursor.fetchall()
+        return [u[1] for u in users]
 
     def create_user(self, user: str, password: str, roles: list = []):
-        with self.cursor() as c:
-            c.execute(
-                f"CREATE ROLE {user} WITH PASSWORD '{password}' {' '.join(roles)};")
+        self.cursor.execute(
+            f"CREATE ROLE {user} WITH PASSWORD '{password}' {' '.join(roles)};")
 
     def drop_user(self, user: str):
-        with self.cursor() as c:
-            c.execute(f"""REVOKE ALL PRIVILEGES ON ALL TABLES IN SCHEMA public FROM {user};
-                        REVOKE ALL PRIVILEGES ON ALL SEQUENCES IN SCHEMA public FROM {user};
-                        REVOKE ALL PRIVILEGES ON ALL FUNCTIONS IN SCHEMA public FROM {user};
-                        DROP USER {user};""")
+        self.cursor.execute(f"""REVOKE ALL PRIVILEGES ON ALL TABLES IN SCHEMA public FROM {user};
+                    REVOKE ALL PRIVILEGES ON ALL SEQUENCES IN SCHEMA public FROM {user};
+                    REVOKE ALL PRIVILEGES ON ALL FUNCTIONS IN SCHEMA public FROM {user};
+                    DROP USER {user};""")
 
     def drop_schema(self, schema: str):
-        with self.cursor() as c:
-            c.execute(f"drop schema {schema} cascade")
-            self._con.commit()
+        self.cursor.execute(f"drop schema {schema} cascade")
+        self._con.commit()
 
     def drop_users_for_tenant(self, tenant: str):
         for user in self.get_users():
             if tenant in user:
                 self.drop_user(user)
 
     def get_descriptors(self):
-        with self._con.cursor() as c:
-            c.execute("SELECT * FROM modules;")
-            descriptors = {}
-            for d in c.fetchall():
-                descriptors[d[0]["id"]] = d[0]
-            return descriptors
+        self.cursor.execute("SELECT * FROM modules;")
+        descriptors = {}
+        for d in self.cursor.fetchall():
+            descriptors[d[0]["id"]] = d[0]
+        return descriptors
 
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if exc_type is not None:
             log.error("%s: %s", exc_type, exc_value)
+        if not self.cursor.closed:
+            self.cursor.close()
         self.close()
 
 
 def create_okapi_db(user: str = "okapi", password: str = "okapi25",
                     database: str = "okapi"):
     # pylint: disable=no-member
     with Postgres() as pg:
```

### Comparing `foliolib-0.3.8a1/foliolib/helper/folio.py` & `foliolib-0.3.9a1/foliolib/helper/folio.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 from foliolib.folio.exceptions import UserNotFound
 from foliolib.folio.users import Users
 from foliolib.okapi.okapiClient import OkapiClient
 
 log = logging.getLogger("foliolib.helper.okapi")
 
 
-def create_superuser(tenant: str, username: str = "admin",
-                     password: str = "folio"):
+def create_superuser(tenant: str, username: str,
+                     password: str):
     """Create a superuser for a tenant.
 
     Args:
         tenant (str): tenant id.
-        username (str, optional): username. Defaults to "admin".
-        password (str, optional): password. Defaults to "folio".
+        username (str, optional): username..
+        password (str, optional): password..
 
     Returns:
-        [type]: [description]
+        dict: User object
     """
     okapi = OkapiClient()
 
     log.info("Disable authtoken for tenant.")
     try:
         mod_authtoken = okapi.get_tenant_interface(tenant, "authtoken")[0]
         disabled_mods = okapi.disable_module(mod_authtoken["id"], tenant)
```

### Comparing `foliolib-0.3.8a1/foliolib/helper/okapi.py` & `foliolib-0.3.9a1/foliolib/helper/okapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2021 Tobias Weber <tobi-weber@gmx.de>
+# Copyright (C) 2023 Tobias Weber <tobi-weber@gmx.de>
 
 import logging
-import pprint
 
 from foliolib.config import Config
 from foliolib.folio.users import Users
 from foliolib.helper import split_modid
 from foliolib.okapi.okapiClient import OkapiClient
 from foliolib.okapi.okapiModule import (create_okapiModules,
                                         sort_modules_by_requirements)
@@ -24,20 +23,20 @@
     log.info("Logging in supertenant")
     userService = Users("supertenant")
     token = userService.login(username, password)
     if token is None:
         log.error("Login failed")
 
 
-def secure_supertenant(username: str = "okapi_admin", password: str = "admin"):
+def secure_supertenant(username: str, password: str):
     """Secure supertenant.
 
     Args:
-        username (str, optional): username for supertenant. Defaults to "okapi_admin".
-        password (str, optional): password supertenant. Defaults to "admin".
+        username (str): username for supertenant.
+        password (str): password supertenant.
     """
     tenant = "supertenant"
     permissions = [
         "okapi.all",
         "okapi.proxy.pull.modules.post",
         "perms.all",
         "login.all",
```

### Comparing `foliolib-0.3.8a1/foliolib/helper/tenant.py` & `foliolib-0.3.9a1/foliolib/helper/tenant.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,18 +9,27 @@
 from foliolib.okapi.okapiModule import (OkapiModule,
                                         sort_modules_by_requirements)
 
 log = logging.getLogger("foliolib.helper.okapi")
 
 
 def uninstall_tenant(tenantid, **kwargs):
-    """Disable all modules of a tenant.
+    """Disable all modules of a tenant and remove tenant.
 
     Args:
         tenantid ([type]): tenant id.
+        **kwargs (properties): Keyword Arguments
+
+    Keyword Args:
+        invoke (boolean): default = true
+                    Whether to invoke for tenant init/permissions/purge
+        purge (boolean): default = false
+                    Disabled modules will also be purged.
+        simulate (boolean): default = false
+                    Whether the installation is simulated
     """
     okapi = OkapiClient()
 
     descriptors = okapi.get_tenant_modules(tenantid, full=True)
     modules = sort_modules_by_requirements(
         [OkapiModule(descriptor) for descriptor in descriptors]
     )
```

### Comparing `foliolib-0.3.8a1/foliolib/okapi/__init__.py` & `foliolib-0.3.9a1/foliolib/okapi/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/okapi/exceptions.py` & `foliolib-0.3.9a1/foliolib/okapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/okapi/kubeClient.py` & `foliolib-0.3.9a1/foliolib/okapi/kubeClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,14 +388,19 @@
                 return True
         return False
 
 
 class KubeAdmin(KubeClient):
 
     def __init__(self, kube_config: str = None):
+        """Manage folio in kubernetes.
+
+        Args:
+            kube_config (str, optional): Path to kube config. Defaults to None.
+        """
         super().__init__(kube_config)
         self.__apps_v1 = client.AppsV1Api()
         self.__core_v1 = client.CoreV1Api()
         self.__dnames = {}
         self.__snames = {}
 
     def stop_folio(self):
```

### Comparing `foliolib-0.3.8a1/foliolib/okapi/misc.py` & `foliolib-0.3.9a1/foliolib/okapi/misc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/foliolib/okapi/okapiClient.py` & `foliolib-0.3.9a1/foliolib/okapi/okapiClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020 Tobias Weber <tobi-weber@gmx.de>
+# Copyright (C) 2023 Tobias Weber <tobi-weber@gmx.de>
 
 import json
 import logging
 import os
 from typing import Union
 from urllib.parse import urlencode, urljoin
 
@@ -276,15 +276,15 @@
         return self.request("GET", "/_/discovery/modules")
 
     def deploy_module(self, modId: Union[str, okapiModule.OkapiModule], node: str = None):
         """Deploy a module.
 
         Args:
             modId (Union[str, OkapiModule]): Module id or instance of OkapiModule.
-            node (str): The node on which module should be deployed. Default first node from nodes list.
+            node (str): The node id on which module should be deployed. Default first node from nodes list.
 
         Returns:
             dict: Deployment descriptor.
         """
         if isinstance(modId, okapiModule.OkapiModule):
             modId = modId.get_id()
         descriptor = self.get_module(modId)
@@ -554,18 +554,14 @@
 
         Args:
             modId (str): Module id
             tenantId (str): Tenant id
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
-            async (boolean): default = false
-                        Whether to uninstall in the background
-            deploy (boolean): default = false
-                        Whether to undeploy
             ignoreErrors (boolean): default = false
                         Okapi 4.2.0 and later, it is possible to ignore errors during the install operation. This is done by supplying parameter ignoreErrors=true.
                         In this case, Okapi will try to upgrade all modules in the modules list, regardless if one of them fails. However, for individual modules,
                         if they fail, their upgrade will not be commited.
                         This is an experimental parameter which was added to be able to inspect all problem(s) with module upgrade(s).
             invoke (boolean): default = true
                         Whether to invoke for tenant init/permissions/purge
```

### Comparing `foliolib-0.3.8a1/foliolib/okapi/okapiModule.py` & `foliolib-0.3.9a1/foliolib/okapi/okapiModule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2020 Tobias Weber <tobi-weber@gmx.de>
+# Copyright (C) 2023 Tobias Weber <tobi-weber@gmx.de>
 
 import json
 import logging
 import os
 from configparser import NoOptionError
 from typing import List, Union
```

### Comparing `foliolib-0.3.8a1/foliolib/okapi/okapiModuleKubernetes.py` & `foliolib-0.3.9a1/foliolib/okapi/okapiModuleKubernetes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2022 Tobias Weber <tobi-weber@gmx.de>
 
 import logging
 import math
+from typing import Union
 
 from foliolib.config import Config
 from foliolib.helper import split_modid
 from foliolib.okapi.okapiModule import OkapiModule
 
 from . import GLOBAL_ENV_NAME_KUBERNETES, get_hazelcast_xml
 
 log = logging.getLogger("foliolib.okapi.okapiModuleKuberenetes")
 
 
 class OkapiModuleKubernetes:
+    """Defines an okapi module for Kubernetes.
+    """
 
-    def __init__(self, modId):
-        module = OkapiModule(modId)
-        self._modId = modId
-        self._name, self._version = split_modid(modId)
+    def __init__(self, module: Union[dict, str]):
+        """
+        Args:
+            module (Union[dict, str]): Module id or instance of OkapiModule.
+        """
+        if isinstance(module, OkapiModule):
+            self._modId = module.get_id()
+        elif isinstance(module, str):
+            self._modId = module
+            module = OkapiModule(module)
+        self._name, self._version = split_modid(self._modId)
         self._docker_image = module.get_docker_image()
         docker_args = module.get_docker_args()
         self._kind = "Deployment"
         self._memory = docker_args["memory"]
         self._port = docker_args["port"]
         self._protocol = docker_args["protocol"]
         self._env = module.get_env()
         self.healthCheck = True
         self.podAntiAffinity = True
-        modcfg = Config().modulescfg(modId)
+        modcfg = Config().modulescfg(self._modId)
         servercfg = Config().servercfg()
         self._namespace = servercfg.get(
             "Kubernetes", "namespace", fallback="folio")
         self.imagePullSecret = servercfg.get(
             "Kubernetes", "imagePullSecret", fallback=None)
 
         self._replicas = servercfg.getint("Kubernetes", "replicas", fallback=1)
@@ -55,20 +65,35 @@
                     "Kubernetes", "healthCheck", fallback=True)
                 self.podAntiAffinity = modcfg.getboolean(
                     "Kubernetes", "podAntiAffinity", fallback=True)
                 self.imagePullSecret = modcfg.get(
                     "Kubernetes", "imagePullSecret", fallback=self.imagePullSecret)
 
     def get_kind(self):
+        """Get resource kind.
+
+        Returns:
+            str: Deployment or StatefulSet
+        """
         return self._kind
 
     def get_rfc_name(self):
+        """Get module id as rfc name.
+
+        Returns:
+            str: rfc name.
+        """
         return self._modId.replace(".", "-")
 
     def get_service(self):
+        """Get Kubernetes service definition for the module.
+
+        Returns:
+            dict: Kubernetes service definition.
+        """
         service = {
             "apiVersion": "v1",
             "kind": "Service",
             "metadata": {
                 "name": self.get_rfc_name(),
                 "labels": {
                     "run": self._modId,
@@ -93,14 +118,19 @@
         if self._kind == "StatefulSet":
             service["spec"]["clusterIP"] = "None"
             # service["spec"]["ports"][0]["targetPort"] = self._port
 
         return service
 
     def get_deployment(self):
+        """Get Kubernetes deployment or statefulset definition for the module.
+
+        Returns:
+            dict: Kubernetes deployment or statefulset definition.
+        """
         deployment = {
             "apiVersion": "apps/v1",
             "kind": self._kind,
             "metadata": {
                 "name": self.get_rfc_name()
             },
             "spec": {
@@ -141,20 +171,20 @@
                     }
                 }
             }
         }
 
         volume = self.volume()
         hazelcast = self.hazelcast()
-        securityContext = self.securityContext()
-        deployment["spec"]["template"]["spec"]["containers"][0]["resources"] = self.resources()
+        securityContext = self.__securityContext()
+        deployment["spec"]["template"]["spec"]["containers"][0]["resources"] = self.__resources()
         if self.healthCheck:
-            deployment["spec"]["template"]["spec"]["containers"][0]["startupProbe"] = self.startupProbe()
-            deployment["spec"]["template"]["spec"]["containers"][0]["livenessProbe"] = self.livenessProbe()
-            deployment["spec"]["template"]["spec"]["containers"][0]["readinessProbe"] = self.readinessProbe()
+            deployment["spec"]["template"]["spec"]["containers"][0]["startupProbe"] = self.__startupProbe()
+            deployment["spec"]["template"]["spec"]["containers"][0]["livenessProbe"] = self.__livenessProbe()
+            deployment["spec"]["template"]["spec"]["containers"][0]["readinessProbe"] = self.__readinessProbe()
         if volume or hazelcast:
             deployment["spec"]["template"]["spec"]["containers"][0]["volumeMounts"] = []
             deployment["spec"]["template"]["spec"]["volumes"] = []
         if volume:
             deployment["spec"]["template"]["spec"]["containers"][0]["volumeMounts"].append(
                 volume["mount"])
             deployment["spec"]["template"]["spec"]["volumes"].append(
@@ -202,37 +232,102 @@
             }
         if self.imagePullSecret:
             deployment["spec"]["template"]["spec"]["imagePullSecrets"] = [{
                 "name": self.imagePullSecret}]
 
         return deployment
 
-    def _healthProbe(self):
+    def volume(self):
+        """Get Kubernetes PersistentVolumeClaim definition.
+
+        Returns:
+            dict: Kubernetes PersistentVolumeClaim definition.
+        """
+        conf = Config().modulescfg(self._modId)
+        name = f"{self._modId}-data"
+        name = "%s-data" % self._modId.replace(".", "-")
+        mountPath = None
+        size = None
+        volume = {}
+        if conf is not None:
+            if conf.has_section("Volume"):
+                mountPath = conf.get("Volume", "mountPath")
+                storageClassName = conf.get(
+                    "Volume", "storageClassName", fallback=None)
+                size = conf.get("Volume", "size")
+
+                volume["claim"] = {"name": name,
+                                   "persistentVolumeClaim": {"claimName": name}
+                                   }
+                volume["mount"] = {"mountPath": mountPath,
+                                   "name": name
+
+                                   }
+                volume["persistentVolumeClaim"] = {"apiVersion": "v1",
+                                                   "kind": "PersistentVolumeClaim",
+                                                   "metadata": {"name": name,
+                                                                "labels":  {"app": self._modId}},
+                                                   "spec": {"accessModes": ["ReadWriteOnce"],
+                                                            "resources": {"requests": {"storage": size}},
+                                                            }
+                                                   }
+                if storageClassName is not None:
+                    volume["persistentVolumeClaim"]["spec"]["storageClassName"] = storageClassName
+
+        return volume
+
+    def hazelcast(self):
+        """Get Kubernetes ConfigMap definition for Hazelcast.
+
+        Returns:
+            dict: Kubernetes ConfigMap definition for Hazelcast.
+        """
+        conf = Config().modulescfg(self._modId)
+        if conf is not None and conf.getboolean(
+                "Kubernetes", "hazelcast", fallback=False):
+            name = f"{self._modId}-hazelcast-xml"
+            return {
+                "name": name,
+                "data": {"hazelcast.xml": get_hazelcast_xml(self.get_rfc_name(), self._namespace)},
+                "mount": {"name": "hazelcast-xml",
+                          "mountPath": "/etc/hazelcast",
+                          "readOnly": True},
+                "volume": {"name": "hazelcast-xml",
+                           "configMap": {"name": name}},
+                "ports": [{"containerPort": 5701},
+                          {"containerPort": 5702},
+                          {"containerPort": 5703},
+                          {"containerPort": 5704},
+                          {"containerPort": 54327}]
+            }
+        return None
+
+    def __healthProbe(self):
         return {"httpGet": {"path": "admin/health",
                             "port": self._port,
                             "scheme": "HTTP"
                             }
                 }
 
-    def startupProbe(self):
+    def __startupProbe(self):
         conf = Config().modulescfg(self._modId)
         failureThreshold = 60
         periodSeconds = 10
         if conf is not None:
             failureThreshold = conf.get(
                 "StartupProbe", "failureThreshold", fallback=failureThreshold)
             periodSeconds = conf.get(
                 "StartupProbe", "periodSeconds", fallback=periodSeconds)
-        data = self._healthProbe()
+        data = self.__healthProbe()
         data["failureThreshold"] = failureThreshold
         data["periodSeconds"] = periodSeconds
 
         return data
 
-    def livenessProbe(self):
+    def __livenessProbe(self):
         conf = Config().modulescfg(self._modId)
         failureThreshold = 3
         initialDelaySeconds = 45
         periodSeconds = 60
         successThreshold = 1
         timeoutSeconds = 5
         if conf is not None:
@@ -242,24 +337,24 @@
                 "LivenessProbe", "initialDelaySeconds", fallback=initialDelaySeconds)
             periodSeconds = conf.get(
                 "LivenessProbe", "periodSeconds", fallback=periodSeconds)
             successThreshold = conf.get(
                 "LivenessProbe", "successThreshold", fallback=successThreshold)
             timeoutSeconds = conf.get(
                 "LivenessProbe", "timeoutSeconds", fallback=timeoutSeconds)
-        data = self._healthProbe()
+        data = self.__healthProbe()
         data["failureThreshold"] = failureThreshold
         data["initialDelaySeconds"] = initialDelaySeconds
         data["periodSeconds"] = periodSeconds
         data["successThreshold"] = successThreshold
         data["timeoutSeconds"] = timeoutSeconds
 
         return data
 
-    def readinessProbe(self):
+    def __readinessProbe(self):
         conf = Config().modulescfg(self._modId)
         failureThreshold = 3
         initialDelaySeconds = 45
         periodSeconds = 60
         successThreshold = 1
         timeoutSeconds = 5
         if conf is not None:
@@ -269,24 +364,24 @@
                 "ReadinessProbe", "initialDelaySeconds", fallback=initialDelaySeconds)
             periodSeconds = conf.get(
                 "ReadinessProbe", "periodSeconds", fallback=periodSeconds)
             successThreshold = conf.get(
                 "ReadinessProbe", "successThreshold", fallback=successThreshold)
             timeoutSeconds = conf.get(
                 "ReadinessProbe", "timeoutSeconds", fallback=timeoutSeconds)
-        data = self._healthProbe()
+        data = self.__healthProbe()
         data["failureThreshold"] = failureThreshold
         data["initialDelaySeconds"] = initialDelaySeconds
         data["periodSeconds"] = periodSeconds
         data["successThreshold"] = successThreshold
         data["timeoutSeconds"] = timeoutSeconds
 
         return data
 
-    def resources(self):
+    def __resources(self):
         conf = Config().modulescfg(self._modId)
         module = OkapiModule(self._modId)
         min_cpu = "10m"
         max_cpu = 0
         memory = module.get_docker_args()["memory"]
         if memory is not None:
             memoryRequestPercentage = Config().servercfg().getint(
@@ -326,70 +421,15 @@
                 limits["cpu"] = max_cpu
             if max_memory:
                 limits["memory"] = max_memory
             resources["limits"] = limits
 
         return resources
 
-    def volume(self):
-        conf = Config().modulescfg(self._modId)
-        name = f"{self._modId}-data"
-        name = "%s-data" % self._modId.replace(".", "-")
-        mountPath = None
-        size = None
-        volume = {}
-        if conf is not None:
-            if conf.has_section("Volume"):
-                mountPath = conf.get("Volume", "mountPath")
-                storageClassName = conf.get(
-                    "Volume", "storageClassName", fallback=None)
-                size = conf.get("Volume", "size")
-
-                volume["claim"] = {"name": name,
-                                   "persistentVolumeClaim": {"claimName": name}
-                                   }
-                volume["mount"] = {"mountPath": mountPath,
-                                   "name": name
-
-                                   }
-                volume["persistentVolumeClaim"] = {"apiVersion": "v1",
-                                                   "kind": "PersistentVolumeClaim",
-                                                   "metadata": {"name": name,
-                                                                "labels":  {"app": self._modId}},
-                                                   "spec": {"accessModes": ["ReadWriteOnce"],
-                                                            "resources": {"requests": {"storage": size}},
-                                                            }
-                                                   }
-                if storageClassName is not None:
-                    volume["persistentVolumeClaim"]["spec"]["storageClassName"] = storageClassName
-
-        return volume
-
-    def hazelcast(self):
-        conf = Config().modulescfg(self._modId)
-        if conf is not None and conf.getboolean(
-                "Kubernetes", "hazelcast", fallback=False):
-            name = f"{self._modId}-hazelcast-xml"
-            return {
-                "name": name,
-                "data": {"hazelcast.xml": get_hazelcast_xml(self.get_rfc_name(), self._namespace)},
-                "mount": {"name": "hazelcast-xml",
-                          "mountPath": "/etc/hazelcast",
-                          "readOnly": True},
-                "volume": {"name": "hazelcast-xml",
-                           "configMap": {"name": name}},
-                "ports": [{"containerPort": 5701},
-                          {"containerPort": 5702},
-                          {"containerPort": 5703},
-                          {"containerPort": 5704},
-                          {"containerPort": 54327}]
-            }
-        return None
-
-    def securityContext(self):
+    def __securityContext(self):
         conf = Config().modulescfg(self._modId)
         sc = {}
         if conf is not None:
             if conf.has_section("SecurityContext"):
                 runAsUser = conf.getint(
                     "SecurityContext", "runAsUser", fallback=None)
                 runAsNonRoot = conf.getboolean(
```

### Comparing `foliolib-0.3.8a1/foliolib.egg-info/PKG-INFO` & `foliolib-0.3.9a1/foliolib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.8a1
+Version: 0.3.9a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -81,15 +81,15 @@
 
     >>> from foliolib import server
     >>> from foliolib.folio.users import Users
     >>> from foliolib.folio.api.inventory import Inventory
     >>>
     >>> server("myServer")
     >>>
-    >>> Users("TenantId").login("UserId","Password")
+    >>> Users("TenantId").login("UserId", "Password")
     >>> inventory = Inventory("TenantId")
     >>> instances = inventory.get_instances(query="title==*")
     >>> print(instances)
 
 Also foliolib provides a command line interface:
 
 .. code-block:: bash
```

### Comparing `foliolib-0.3.8a1/foliolib.egg-info/SOURCES.txt` & `foliolib-0.3.9a1/foliolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.8a1/setup.cfg` & `foliolib-0.3.9a1/setup.cfg`

 * *Files identical despite different names*

