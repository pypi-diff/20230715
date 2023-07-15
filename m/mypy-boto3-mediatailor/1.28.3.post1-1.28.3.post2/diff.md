# Comparing `tmp/mypy-boto3-mediatailor-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-mediatailor-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediatailor-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:02 2023, max compression
+gzip compressed data, was "mypy-boto3-mediatailor-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:35 2023, max compression
```

## Comparing `mypy-boto3-mediatailor-1.28.3.post1.tar` & `mypy-boto3-mediatailor-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.967727 mypy-boto3-mediatailor-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-14 16:18:02.963726 mypy-boto3-mediatailor-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.963726 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33957 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33898 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-14 16:16:51.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57550 2023-07-14 16:16:52.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57500 2023-07-14 16:16:51.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.963726 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 16:18:02.000000 mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:02.967727 mypy-boto3-mediatailor-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-14 16:16:50.000000 mypy-boto3-mediatailor-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.158395 mypy-boto3-mediatailor-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-07-15 06:38:35.158395 mypy-boto3-mediatailor-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.150394 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33557 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33498 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56596 2023-07-15 06:37:25.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56546 2023-07-15 06:37:23.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.158395 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-07-15 06:38:34.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-15 06:38:35.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:34.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:34.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:34.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 06:38:34.000000 mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:35.158395 mypy-boto3-mediatailor-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-15 06:37:22.000000 mypy-boto3-mediatailor-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/LICENSE` & `mypy-boto3-mediatailor-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/PKG-INFO` & `mypy-boto3-mediatailor-1.28.3.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
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
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,42 +374,42 @@
     SlateSourceOutputTypeDef,
     SpliceInsertMessageOutputTypeDef,
     KeyValuePairTypeDef,
     SlateSourceTypeDef,
     SpliceInsertMessageTypeDef,
     AdMarkerPassthroughOutputTypeDef,
     AdMarkerPassthroughTypeDef,
-    AlertOutputTypeDef,
+    AlertTypeDef,
     AvailMatchingCriteriaOutputTypeDef,
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionOutputTypeDef,
     AvailSuppressionTypeDef,
     BumperOutputTypeDef,
     BumperTypeDef,
     CdnConfigurationOutputTypeDef,
     CdnConfigurationTypeDef,
-    LogConfigurationForChannelOutputTypeDef,
+    LogConfigurationForChannelTypeDef,
     ClipRangeOutputTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ConfigureLogsForChannelResponseOutputTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     HttpPackageConfigurationTypeDef,
     HttpPackageConfigurationOutputTypeDef,
     PrefetchRetrievalTypeDef,
     PrefetchRetrievalOutputTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     DefaultSegmentDeliveryConfigurationOutputTypeDef,
     HttpConfigurationOutputTypeDef,
     SegmentDeliveryConfigurationOutputTypeDef,
     DashConfigurationForPutTypeDef,
-    DashConfigurationOutputTypeDef,
+    DashConfigurationTypeDef,
     DashPlaylistSettingsOutputTypeDef,
     DashPlaylistSettingsTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteLiveSourceRequestRequestTypeDef,
     DeletePlaybackConfigurationRequestRequestTypeDef,
     DeletePrefetchScheduleRequestRequestTypeDef,
@@ -419,21 +419,21 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseOutputTypeDef,
+    GetChannelPolicyResponseTypeDef,
     GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
-    HlsConfigurationOutputTypeDef,
+    HlsConfigurationTypeDef,
     LivePreRollConfigurationOutputTypeDef,
-    LogConfigurationOutputTypeDef,
+    LogConfigurationTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
     HlsPlaylistSettingsOutputTypeDef,
     HlsPlaylistSettingsTypeDef,
     ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
@@ -442,88 +442,88 @@
     ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
     ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
     LivePreRollConfigurationTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    ScheduleAdBreakOutputTypeDef,
+    ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorOutputTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
     AccessConfigurationOutputTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesOutputTypeDef,
     ManifestProcessingRulesTypeDef,
-    ListAlertsResponseOutputTypeDef,
+    ListAlertsResponseTypeDef,
     PrefetchConsumptionOutputTypeDef,
     PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
     CreateVodSourceRequestRequestTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
-    CreateLiveSourceResponseOutputTypeDef,
-    CreateVodSourceResponseOutputTypeDef,
-    DescribeLiveSourceResponseOutputTypeDef,
-    DescribeVodSourceResponseOutputTypeDef,
-    LiveSourceOutputTypeDef,
-    UpdateLiveSourceResponseOutputTypeDef,
-    UpdateVodSourceResponseOutputTypeDef,
-    VodSourceOutputTypeDef,
-    ResponseOutputItemOutputTypeDef,
+    CreateLiveSourceResponseTypeDef,
+    CreateVodSourceResponseTypeDef,
+    DescribeLiveSourceResponseTypeDef,
+    DescribeVodSourceResponseTypeDef,
+    LiveSourceTypeDef,
+    UpdateLiveSourceResponseTypeDef,
+    UpdateVodSourceResponseTypeDef,
+    VodSourceTypeDef,
+    ResponseOutputItemTypeDef,
     RequestOutputItemTypeDef,
-    ScheduleEntryOutputTypeDef,
+    ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageOutputTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    CreateSourceLocationResponseOutputTypeDef,
-    DescribeSourceLocationResponseOutputTypeDef,
-    SourceLocationOutputTypeDef,
-    UpdateSourceLocationResponseOutputTypeDef,
+    CreateSourceLocationResponseTypeDef,
+    DescribeSourceLocationResponseTypeDef,
+    SourceLocationTypeDef,
+    UpdateSourceLocationResponseTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
-    GetPlaybackConfigurationResponseOutputTypeDef,
-    PlaybackConfigurationOutputTypeDef,
-    PutPlaybackConfigurationResponseOutputTypeDef,
+    GetPlaybackConfigurationResponseTypeDef,
+    PlaybackConfigurationTypeDef,
+    PutPlaybackConfigurationResponseTypeDef,
     PutPlaybackConfigurationRequestRequestTypeDef,
-    CreatePrefetchScheduleResponseOutputTypeDef,
-    GetPrefetchScheduleResponseOutputTypeDef,
-    PrefetchScheduleOutputTypeDef,
+    CreatePrefetchScheduleResponseTypeDef,
+    GetPrefetchScheduleResponseTypeDef,
+    PrefetchScheduleTypeDef,
     CreatePrefetchScheduleRequestRequestTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
-    ChannelOutputTypeDef,
-    CreateChannelResponseOutputTypeDef,
-    DescribeChannelResponseOutputTypeDef,
-    UpdateChannelResponseOutputTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
+    ChannelTypeDef,
+    CreateChannelResponseTypeDef,
+    DescribeChannelResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    GetChannelScheduleResponseOutputTypeDef,
+    GetChannelScheduleResponseTypeDef,
     AdBreakOutputTypeDef,
     AdBreakTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    CreateProgramResponseOutputTypeDef,
-    DescribeProgramResponseOutputTypeDef,
-    UpdateProgramResponseOutputTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    CreateProgramResponseTypeDef,
+    DescribeProgramResponseTypeDef,
+    UpdateProgramResponseTypeDef,
     CreateProgramRequestRequestTypeDef,
     UpdateProgramRequestRequestTypeDef,
 )
 
 
 def get_structure() -> SecretsManagerAccessTokenConfigurationOutputTypeDef:
     return {...}
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/README.md` & `mypy-boto3-mediatailor-1.28.3.post2/README.md`

 * *Files 10% similar despite different names*

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
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,42 +342,42 @@
     SlateSourceOutputTypeDef,
     SpliceInsertMessageOutputTypeDef,
     KeyValuePairTypeDef,
     SlateSourceTypeDef,
     SpliceInsertMessageTypeDef,
     AdMarkerPassthroughOutputTypeDef,
     AdMarkerPassthroughTypeDef,
-    AlertOutputTypeDef,
+    AlertTypeDef,
     AvailMatchingCriteriaOutputTypeDef,
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionOutputTypeDef,
     AvailSuppressionTypeDef,
     BumperOutputTypeDef,
     BumperTypeDef,
     CdnConfigurationOutputTypeDef,
     CdnConfigurationTypeDef,
-    LogConfigurationForChannelOutputTypeDef,
+    LogConfigurationForChannelTypeDef,
     ClipRangeOutputTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ConfigureLogsForChannelResponseOutputTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     HttpPackageConfigurationTypeDef,
     HttpPackageConfigurationOutputTypeDef,
     PrefetchRetrievalTypeDef,
     PrefetchRetrievalOutputTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     DefaultSegmentDeliveryConfigurationOutputTypeDef,
     HttpConfigurationOutputTypeDef,
     SegmentDeliveryConfigurationOutputTypeDef,
     DashConfigurationForPutTypeDef,
-    DashConfigurationOutputTypeDef,
+    DashConfigurationTypeDef,
     DashPlaylistSettingsOutputTypeDef,
     DashPlaylistSettingsTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteLiveSourceRequestRequestTypeDef,
     DeletePlaybackConfigurationRequestRequestTypeDef,
     DeletePrefetchScheduleRequestRequestTypeDef,
@@ -387,21 +387,21 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseOutputTypeDef,
+    GetChannelPolicyResponseTypeDef,
     GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
-    HlsConfigurationOutputTypeDef,
+    HlsConfigurationTypeDef,
     LivePreRollConfigurationOutputTypeDef,
-    LogConfigurationOutputTypeDef,
+    LogConfigurationTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
     HlsPlaylistSettingsOutputTypeDef,
     HlsPlaylistSettingsTypeDef,
     ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
@@ -410,88 +410,88 @@
     ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
     ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
     LivePreRollConfigurationTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    ScheduleAdBreakOutputTypeDef,
+    ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorOutputTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
     AccessConfigurationOutputTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesOutputTypeDef,
     ManifestProcessingRulesTypeDef,
-    ListAlertsResponseOutputTypeDef,
+    ListAlertsResponseTypeDef,
     PrefetchConsumptionOutputTypeDef,
     PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
     CreateVodSourceRequestRequestTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
-    CreateLiveSourceResponseOutputTypeDef,
-    CreateVodSourceResponseOutputTypeDef,
-    DescribeLiveSourceResponseOutputTypeDef,
-    DescribeVodSourceResponseOutputTypeDef,
-    LiveSourceOutputTypeDef,
-    UpdateLiveSourceResponseOutputTypeDef,
-    UpdateVodSourceResponseOutputTypeDef,
-    VodSourceOutputTypeDef,
-    ResponseOutputItemOutputTypeDef,
+    CreateLiveSourceResponseTypeDef,
+    CreateVodSourceResponseTypeDef,
+    DescribeLiveSourceResponseTypeDef,
+    DescribeVodSourceResponseTypeDef,
+    LiveSourceTypeDef,
+    UpdateLiveSourceResponseTypeDef,
+    UpdateVodSourceResponseTypeDef,
+    VodSourceTypeDef,
+    ResponseOutputItemTypeDef,
     RequestOutputItemTypeDef,
-    ScheduleEntryOutputTypeDef,
+    ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageOutputTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    CreateSourceLocationResponseOutputTypeDef,
-    DescribeSourceLocationResponseOutputTypeDef,
-    SourceLocationOutputTypeDef,
-    UpdateSourceLocationResponseOutputTypeDef,
+    CreateSourceLocationResponseTypeDef,
+    DescribeSourceLocationResponseTypeDef,
+    SourceLocationTypeDef,
+    UpdateSourceLocationResponseTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
-    GetPlaybackConfigurationResponseOutputTypeDef,
-    PlaybackConfigurationOutputTypeDef,
-    PutPlaybackConfigurationResponseOutputTypeDef,
+    GetPlaybackConfigurationResponseTypeDef,
+    PlaybackConfigurationTypeDef,
+    PutPlaybackConfigurationResponseTypeDef,
     PutPlaybackConfigurationRequestRequestTypeDef,
-    CreatePrefetchScheduleResponseOutputTypeDef,
-    GetPrefetchScheduleResponseOutputTypeDef,
-    PrefetchScheduleOutputTypeDef,
+    CreatePrefetchScheduleResponseTypeDef,
+    GetPrefetchScheduleResponseTypeDef,
+    PrefetchScheduleTypeDef,
     CreatePrefetchScheduleRequestRequestTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
-    ChannelOutputTypeDef,
-    CreateChannelResponseOutputTypeDef,
-    DescribeChannelResponseOutputTypeDef,
-    UpdateChannelResponseOutputTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
+    ChannelTypeDef,
+    CreateChannelResponseTypeDef,
+    DescribeChannelResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    GetChannelScheduleResponseOutputTypeDef,
+    GetChannelScheduleResponseTypeDef,
     AdBreakOutputTypeDef,
     AdBreakTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    CreateProgramResponseOutputTypeDef,
-    DescribeProgramResponseOutputTypeDef,
-    UpdateProgramResponseOutputTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    CreateProgramResponseTypeDef,
+    DescribeProgramResponseTypeDef,
+    UpdateProgramResponseTypeDef,
     CreateProgramRequestRequestTypeDef,
     UpdateProgramRequestRequestTypeDef,
 )
 
 
 def get_structure() -> SecretsManagerAccessTokenConfigurationOutputTypeDef:
     return {...}
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.py` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__init__.pyi` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/__main__.py` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaTailor 1.28.3\nVersion:         1.28.3.post1\nBuilder"
-        " version: 7.14.7\nDocs:           "
+        "Type annotations for boto3.MediaTailor 1.28.3\nVersion:         1.28.3.post2\nBuilder"
+        " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\nOther"
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

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.py` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,59 +31,59 @@
 )
 from .type_defs import (
     AccessConfigurationTypeDef,
     AdBreakTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
-    ConfigureLogsForChannelResponseOutputTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
-    CreateChannelResponseOutputTypeDef,
-    CreateLiveSourceResponseOutputTypeDef,
-    CreatePrefetchScheduleResponseOutputTypeDef,
-    CreateProgramResponseOutputTypeDef,
-    CreateSourceLocationResponseOutputTypeDef,
-    CreateVodSourceResponseOutputTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateLiveSourceResponseTypeDef,
+    CreatePrefetchScheduleResponseTypeDef,
+    CreateProgramResponseTypeDef,
+    CreateSourceLocationResponseTypeDef,
+    CreateVodSourceResponseTypeDef,
     DashConfigurationForPutTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
-    DescribeChannelResponseOutputTypeDef,
-    DescribeLiveSourceResponseOutputTypeDef,
-    DescribeProgramResponseOutputTypeDef,
-    DescribeSourceLocationResponseOutputTypeDef,
-    DescribeVodSourceResponseOutputTypeDef,
+    DescribeChannelResponseTypeDef,
+    DescribeLiveSourceResponseTypeDef,
+    DescribeProgramResponseTypeDef,
+    DescribeSourceLocationResponseTypeDef,
+    DescribeVodSourceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseOutputTypeDef,
-    GetChannelScheduleResponseOutputTypeDef,
-    GetPlaybackConfigurationResponseOutputTypeDef,
-    GetPrefetchScheduleResponseOutputTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetChannelScheduleResponseTypeDef,
+    GetPlaybackConfigurationResponseTypeDef,
+    GetPrefetchScheduleResponseTypeDef,
     HttpConfigurationTypeDef,
     HttpPackageConfigurationTypeDef,
-    ListAlertsResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
+    ListAlertsResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
     LivePreRollConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     PrefetchRetrievalTypeDef,
-    PutPlaybackConfigurationResponseOutputTypeDef,
+    PutPlaybackConfigurationResponseTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
-    UpdateChannelResponseOutputTypeDef,
-    UpdateLiveSourceResponseOutputTypeDef,
-    UpdateProgramResponseOutputTypeDef,
+    UpdateChannelResponseTypeDef,
+    UpdateLiveSourceResponseTypeDef,
+    UpdateProgramResponseTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    UpdateSourceLocationResponseOutputTypeDef,
-    UpdateVodSourceResponseOutputTypeDef,
+    UpdateSourceLocationResponseTypeDef,
+    UpdateVodSourceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -135,25 +135,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#close)
         """
 
     def configure_logs_for_channel(
         self, *, ChannelName: str, LogTypes: Sequence[Literal["AS_RUN"]]
-    ) -> ConfigureLogsForChannelResponseOutputTypeDef:
+    ) -> ConfigureLogsForChannelResponseTypeDef:
         """
         Configures Amazon CloudWatch log settings for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_channel)
         """
 
     def configure_logs_for_playback_configuration(
         self, *, PercentEnabled: int, PlaybackConfigurationName: str
-    ) -> ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef:
+    ) -> ConfigureLogsForPlaybackConfigurationResponseTypeDef:
         """
         Amazon CloudWatch log settings for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_playback_configuration)
         """
 
@@ -162,30 +162,30 @@
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         PlaybackMode: PlaybackModeType,
         FillerSlate: SlateSourceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Tier: TierType = ...
-    ) -> CreateChannelResponseOutputTypeDef:
+    ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_channel)
         """
 
     def create_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateLiveSourceResponseOutputTypeDef:
+    ) -> CreateLiveSourceResponseTypeDef:
         """
         The live source configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_live_source)
         """
 
@@ -193,15 +193,15 @@
         self,
         *,
         Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
         Retrieval: PrefetchRetrievalTypeDef,
         StreamId: str = ...
-    ) -> CreatePrefetchScheduleResponseOutputTypeDef:
+    ) -> CreatePrefetchScheduleResponseTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_prefetch_schedule)
         """
 
@@ -211,15 +211,15 @@
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
         AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
         VodSourceName: str = ...
-    ) -> CreateProgramResponseOutputTypeDef:
+    ) -> CreateProgramResponseTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_program)
         """
 
@@ -228,30 +228,30 @@
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateSourceLocationResponseOutputTypeDef:
+    ) -> CreateSourceLocationResponseTypeDef:
         """
         Creates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_source_location)
         """
 
     def create_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVodSourceResponseOutputTypeDef:
+    ) -> CreateVodSourceResponseTypeDef:
         """
         The VOD source configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_vod_source)
         """
 
@@ -317,55 +317,55 @@
         """
         The video on demand (VOD) source to delete.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#delete_vod_source)
         """
 
-    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseOutputTypeDef:
+    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseTypeDef:
         """
         Describes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_channel)
         """
 
     def describe_live_source(
         self, *, LiveSourceName: str, SourceLocationName: str
-    ) -> DescribeLiveSourceResponseOutputTypeDef:
+    ) -> DescribeLiveSourceResponseTypeDef:
         """
         The live source to describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_live_source)
         """
 
     def describe_program(
         self, *, ChannelName: str, ProgramName: str
-    ) -> DescribeProgramResponseOutputTypeDef:
+    ) -> DescribeProgramResponseTypeDef:
         """
         Describes a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_program)
         """
 
     def describe_source_location(
         self, *, SourceLocationName: str
-    ) -> DescribeSourceLocationResponseOutputTypeDef:
+    ) -> DescribeSourceLocationResponseTypeDef:
         """
         Describes a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_source_location)
         """
 
     def describe_vod_source(
         self, *, SourceLocationName: str, VodSourceName: str
-    ) -> DescribeVodSourceResponseOutputTypeDef:
+    ) -> DescribeVodSourceResponseTypeDef:
         """
         Provides details about a specific video on demand (VOD) source in a specific
         source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_vod_source)
         """
@@ -380,137 +380,133 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#generate_presigned_url)
         """
 
-    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseOutputTypeDef:
+    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseTypeDef:
         """
         Returns the channel's IAM policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_policy)
         """
 
     def get_channel_schedule(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> GetChannelScheduleResponseOutputTypeDef:
+    ) -> GetChannelScheduleResponseTypeDef:
         """
         Retrieves information about your channel's schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_schedule)
         """
 
-    def get_playback_configuration(
-        self, *, Name: str
-    ) -> GetPlaybackConfigurationResponseOutputTypeDef:
+    def get_playback_configuration(self, *, Name: str) -> GetPlaybackConfigurationResponseTypeDef:
         """
         Retrieves a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_playback_configuration)
         """
 
     def get_prefetch_schedule(
         self, *, Name: str, PlaybackConfigurationName: str
-    ) -> GetPrefetchScheduleResponseOutputTypeDef:
+    ) -> GetPrefetchScheduleResponseTypeDef:
         """
         Retrieves a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_prefetch_schedule)
         """
 
     def list_alerts(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAlertsResponseOutputTypeDef:
+    ) -> ListAlertsResponseTypeDef:
         """
         Lists the alerts that are associated with a MediaTailor channel assembly
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_alerts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_alerts)
         """
 
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListChannelsResponseOutputTypeDef:
+    ) -> ListChannelsResponseTypeDef:
         """
         Retrieves information about the channels that are associated with the current
         AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_channels)
         """
 
     def list_live_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListLiveSourcesResponseOutputTypeDef:
+    ) -> ListLiveSourcesResponseTypeDef:
         """
         Lists the live sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_live_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_live_sources)
         """
 
     def list_playback_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListPlaybackConfigurationsResponseOutputTypeDef:
+    ) -> ListPlaybackConfigurationsResponseTypeDef:
         """
         Retrieves existing playback configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_playback_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_playback_configurations)
         """
 
     def list_prefetch_schedules(
         self,
         *,
         PlaybackConfigurationName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         StreamId: str = ...
-    ) -> ListPrefetchSchedulesResponseOutputTypeDef:
+    ) -> ListPrefetchSchedulesResponseTypeDef:
         """
         Lists the prefetch schedules for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_prefetch_schedules)
         """
 
     def list_source_locations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListSourceLocationsResponseOutputTypeDef:
+    ) -> ListSourceLocationsResponseTypeDef:
         """
         Lists the source locations for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_source_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_source_locations)
         """
 
-    def list_tags_for_resource(
-        self, *, ResourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         A list of tags that are associated with this resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_tags_for_resource)
         """
 
     def list_vod_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListVodSourcesResponseOutputTypeDef:
+    ) -> ListVodSourcesResponseTypeDef:
         """
         Lists the VOD sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_vod_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_vod_sources)
         """
 
@@ -535,15 +531,15 @@
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
         VideoContentSourceUrl: str = ...
-    ) -> PutPlaybackConfigurationResponseOutputTypeDef:
+    ) -> PutPlaybackConfigurationResponseTypeDef:
         """
         Creates a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#put_playback_configuration)
         """
 
@@ -585,44 +581,44 @@
 
     def update_channel(
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         FillerSlate: SlateSourceTypeDef = ...
-    ) -> UpdateChannelResponseOutputTypeDef:
+    ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_channel)
         """
 
     def update_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str
-    ) -> UpdateLiveSourceResponseOutputTypeDef:
+    ) -> UpdateLiveSourceResponseTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_live_source)
         """
 
     def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
         AdBreaks: Sequence[AdBreakTypeDef] = ...
-    ) -> UpdateProgramResponseOutputTypeDef:
+    ) -> UpdateProgramResponseTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_program)
         """
 
@@ -630,29 +626,29 @@
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...
-    ) -> UpdateSourceLocationResponseOutputTypeDef:
+    ) -> UpdateSourceLocationResponseTypeDef:
         """
         Updates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_source_location)
         """
 
     def update_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str
-    ) -> UpdateVodSourceResponseOutputTypeDef:
+    ) -> UpdateVodSourceResponseTypeDef:
         """
         Updates a VOD source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_vod_source)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/client.pyi` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/client.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -31,59 +31,59 @@
 )
 from .type_defs import (
     AccessConfigurationTypeDef,
     AdBreakTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
-    ConfigureLogsForChannelResponseOutputTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
-    CreateChannelResponseOutputTypeDef,
-    CreateLiveSourceResponseOutputTypeDef,
-    CreatePrefetchScheduleResponseOutputTypeDef,
-    CreateProgramResponseOutputTypeDef,
-    CreateSourceLocationResponseOutputTypeDef,
-    CreateVodSourceResponseOutputTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateLiveSourceResponseTypeDef,
+    CreatePrefetchScheduleResponseTypeDef,
+    CreateProgramResponseTypeDef,
+    CreateSourceLocationResponseTypeDef,
+    CreateVodSourceResponseTypeDef,
     DashConfigurationForPutTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
-    DescribeChannelResponseOutputTypeDef,
-    DescribeLiveSourceResponseOutputTypeDef,
-    DescribeProgramResponseOutputTypeDef,
-    DescribeSourceLocationResponseOutputTypeDef,
-    DescribeVodSourceResponseOutputTypeDef,
+    DescribeChannelResponseTypeDef,
+    DescribeLiveSourceResponseTypeDef,
+    DescribeProgramResponseTypeDef,
+    DescribeSourceLocationResponseTypeDef,
+    DescribeVodSourceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetChannelPolicyResponseOutputTypeDef,
-    GetChannelScheduleResponseOutputTypeDef,
-    GetPlaybackConfigurationResponseOutputTypeDef,
-    GetPrefetchScheduleResponseOutputTypeDef,
+    GetChannelPolicyResponseTypeDef,
+    GetChannelScheduleResponseTypeDef,
+    GetPlaybackConfigurationResponseTypeDef,
+    GetPrefetchScheduleResponseTypeDef,
     HttpConfigurationTypeDef,
     HttpPackageConfigurationTypeDef,
-    ListAlertsResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
+    ListAlertsResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
     LivePreRollConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     PrefetchRetrievalTypeDef,
-    PutPlaybackConfigurationResponseOutputTypeDef,
+    PutPlaybackConfigurationResponseTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
-    UpdateChannelResponseOutputTypeDef,
-    UpdateLiveSourceResponseOutputTypeDef,
-    UpdateProgramResponseOutputTypeDef,
+    UpdateChannelResponseTypeDef,
+    UpdateLiveSourceResponseTypeDef,
+    UpdateProgramResponseTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    UpdateSourceLocationResponseOutputTypeDef,
-    UpdateVodSourceResponseOutputTypeDef,
+    UpdateSourceLocationResponseTypeDef,
+    UpdateVodSourceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -128,24 +128,24 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#close)
         """
     def configure_logs_for_channel(
         self, *, ChannelName: str, LogTypes: Sequence[Literal["AS_RUN"]]
-    ) -> ConfigureLogsForChannelResponseOutputTypeDef:
+    ) -> ConfigureLogsForChannelResponseTypeDef:
         """
         Configures Amazon CloudWatch log settings for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_channel)
         """
     def configure_logs_for_playback_configuration(
         self, *, PercentEnabled: int, PlaybackConfigurationName: str
-    ) -> ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef:
+    ) -> ConfigureLogsForPlaybackConfigurationResponseTypeDef:
         """
         Amazon CloudWatch log settings for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#configure_logs_for_playback_configuration)
         """
     def create_channel(
@@ -153,44 +153,44 @@
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         PlaybackMode: PlaybackModeType,
         FillerSlate: SlateSourceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Tier: TierType = ...
-    ) -> CreateChannelResponseOutputTypeDef:
+    ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_channel)
         """
     def create_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateLiveSourceResponseOutputTypeDef:
+    ) -> CreateLiveSourceResponseTypeDef:
         """
         The live source configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_live_source)
         """
     def create_prefetch_schedule(
         self,
         *,
         Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
         Retrieval: PrefetchRetrievalTypeDef,
         StreamId: str = ...
-    ) -> CreatePrefetchScheduleResponseOutputTypeDef:
+    ) -> CreatePrefetchScheduleResponseTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_prefetch_schedule)
         """
     def create_program(
@@ -199,15 +199,15 @@
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
         AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
         VodSourceName: str = ...
-    ) -> CreateProgramResponseOutputTypeDef:
+    ) -> CreateProgramResponseTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_program)
         """
     def create_source_location(
@@ -215,29 +215,29 @@
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> CreateSourceLocationResponseOutputTypeDef:
+    ) -> CreateSourceLocationResponseTypeDef:
         """
         Creates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_source_location)
         """
     def create_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str,
         Tags: Mapping[str, str] = ...
-    ) -> CreateVodSourceResponseOutputTypeDef:
+    ) -> CreateVodSourceResponseTypeDef:
         """
         The VOD source configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#create_vod_source)
         """
     def delete_channel(self, *, ChannelName: str) -> Dict[str, Any]:
@@ -294,51 +294,51 @@
     def delete_vod_source(self, *, SourceLocationName: str, VodSourceName: str) -> Dict[str, Any]:
         """
         The video on demand (VOD) source to delete.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#delete_vod_source)
         """
-    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseOutputTypeDef:
+    def describe_channel(self, *, ChannelName: str) -> DescribeChannelResponseTypeDef:
         """
         Describes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_channel)
         """
     def describe_live_source(
         self, *, LiveSourceName: str, SourceLocationName: str
-    ) -> DescribeLiveSourceResponseOutputTypeDef:
+    ) -> DescribeLiveSourceResponseTypeDef:
         """
         The live source to describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_live_source)
         """
     def describe_program(
         self, *, ChannelName: str, ProgramName: str
-    ) -> DescribeProgramResponseOutputTypeDef:
+    ) -> DescribeProgramResponseTypeDef:
         """
         Describes a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_program)
         """
     def describe_source_location(
         self, *, SourceLocationName: str
-    ) -> DescribeSourceLocationResponseOutputTypeDef:
+    ) -> DescribeSourceLocationResponseTypeDef:
         """
         Describes a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_source_location)
         """
     def describe_vod_source(
         self, *, SourceLocationName: str, VodSourceName: str
-    ) -> DescribeVodSourceResponseOutputTypeDef:
+    ) -> DescribeVodSourceResponseTypeDef:
         """
         Provides details about a specific video on demand (VOD) source in a specific
         source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#describe_vod_source)
         """
@@ -351,126 +351,122 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#generate_presigned_url)
         """
-    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseOutputTypeDef:
+    def get_channel_policy(self, *, ChannelName: str) -> GetChannelPolicyResponseTypeDef:
         """
         Returns the channel's IAM policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_policy)
         """
     def get_channel_schedule(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> GetChannelScheduleResponseOutputTypeDef:
+    ) -> GetChannelScheduleResponseTypeDef:
         """
         Retrieves information about your channel's schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_channel_schedule)
         """
-    def get_playback_configuration(
-        self, *, Name: str
-    ) -> GetPlaybackConfigurationResponseOutputTypeDef:
+    def get_playback_configuration(self, *, Name: str) -> GetPlaybackConfigurationResponseTypeDef:
         """
         Retrieves a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_playback_configuration)
         """
     def get_prefetch_schedule(
         self, *, Name: str, PlaybackConfigurationName: str
-    ) -> GetPrefetchScheduleResponseOutputTypeDef:
+    ) -> GetPrefetchScheduleResponseTypeDef:
         """
         Retrieves a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_prefetch_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#get_prefetch_schedule)
         """
     def list_alerts(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAlertsResponseOutputTypeDef:
+    ) -> ListAlertsResponseTypeDef:
         """
         Lists the alerts that are associated with a MediaTailor channel assembly
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_alerts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_alerts)
         """
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListChannelsResponseOutputTypeDef:
+    ) -> ListChannelsResponseTypeDef:
         """
         Retrieves information about the channels that are associated with the current
         AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_channels)
         """
     def list_live_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListLiveSourcesResponseOutputTypeDef:
+    ) -> ListLiveSourcesResponseTypeDef:
         """
         Lists the live sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_live_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_live_sources)
         """
     def list_playback_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListPlaybackConfigurationsResponseOutputTypeDef:
+    ) -> ListPlaybackConfigurationsResponseTypeDef:
         """
         Retrieves existing playback configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_playback_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_playback_configurations)
         """
     def list_prefetch_schedules(
         self,
         *,
         PlaybackConfigurationName: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         StreamId: str = ...
-    ) -> ListPrefetchSchedulesResponseOutputTypeDef:
+    ) -> ListPrefetchSchedulesResponseTypeDef:
         """
         Lists the prefetch schedules for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_prefetch_schedules)
         """
     def list_source_locations(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListSourceLocationsResponseOutputTypeDef:
+    ) -> ListSourceLocationsResponseTypeDef:
         """
         Lists the source locations for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_source_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_source_locations)
         """
-    def list_tags_for_resource(
-        self, *, ResourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         A list of tags that are associated with this resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_tags_for_resource)
         """
     def list_vod_sources(
         self, *, SourceLocationName: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListVodSourcesResponseOutputTypeDef:
+    ) -> ListVodSourcesResponseTypeDef:
         """
         Lists the VOD sources contained in a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_vod_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#list_vod_sources)
         """
     def put_channel_policy(self, *, ChannelName: str, Policy: str) -> Dict[str, Any]:
@@ -493,15 +489,15 @@
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
         VideoContentSourceUrl: str = ...
-    ) -> PutPlaybackConfigurationResponseOutputTypeDef:
+    ) -> PutPlaybackConfigurationResponseTypeDef:
         """
         Creates a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#put_playback_configuration)
         """
     def start_channel(self, *, ChannelName: str) -> Dict[str, Any]:
@@ -538,70 +534,70 @@
         """
     def update_channel(
         self,
         *,
         ChannelName: str,
         Outputs: Sequence[RequestOutputItemTypeDef],
         FillerSlate: SlateSourceTypeDef = ...
-    ) -> UpdateChannelResponseOutputTypeDef:
+    ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_channel)
         """
     def update_live_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         LiveSourceName: str,
         SourceLocationName: str
-    ) -> UpdateLiveSourceResponseOutputTypeDef:
+    ) -> UpdateLiveSourceResponseTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_live_source)
         """
     def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
         AdBreaks: Sequence[AdBreakTypeDef] = ...
-    ) -> UpdateProgramResponseOutputTypeDef:
+    ) -> UpdateProgramResponseTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_program)
         """
     def update_source_location(
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
         SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...
-    ) -> UpdateSourceLocationResponseOutputTypeDef:
+    ) -> UpdateSourceLocationResponseTypeDef:
         """
         Updates a source location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_source_location)
         """
     def update_vod_source(
         self,
         *,
         HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],
         SourceLocationName: str,
         VodSourceName: str
-    ) -> UpdateVodSourceResponseOutputTypeDef:
+    ) -> UpdateVodSourceResponseTypeDef:
         """
         Updates a VOD source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_vod_source)
         """
     @overload
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.py` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/literals.pyi` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.py` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    GetChannelScheduleResponseOutputTypeDef,
-    ListAlertsResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
+    GetChannelScheduleResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "GetChannelSchedulePaginator",
     "ListAlertsPaginator",
     "ListChannelsPaginator",
@@ -79,75 +79,75 @@
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetChannelScheduleResponseOutputTypeDef]:
+    ) -> _PageIterator[GetChannelScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
 
 class ListAlertsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAlertsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAlertsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListChannelsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
         """
 
 
 class ListLiveSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLiveSourcesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLiveSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
         """
 
 
 class ListPlaybackConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPlaybackConfigurationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPlaybackConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
         """
 
 
 class ListPrefetchSchedulesPaginator(Paginator):
@@ -158,42 +158,42 @@
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPrefetchSchedulesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPrefetchSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
 
 class ListSourceLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSourceLocationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSourceLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
         """
 
 
 class ListVodSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVodSourcesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListVodSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/paginator.pyi` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    GetChannelScheduleResponseOutputTypeDef,
-    ListAlertsResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
+    GetChannelScheduleResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "GetChannelSchedulePaginator",
     "ListAlertsPaginator",
     "ListChannelsPaginator",
@@ -76,71 +76,71 @@
 
     def paginate(
         self,
         *,
         ChannelName: str,
         DurationMinutes: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetChannelScheduleResponseOutputTypeDef]:
+    ) -> _PageIterator[GetChannelScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.GetChannelSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#getchannelschedulepaginator)
         """
 
 class ListAlertsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAlertsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAlertsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListAlerts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listalertspaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListChannelsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listchannelspaginator)
         """
 
 class ListLiveSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLiveSourcesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListLiveSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListLiveSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listlivesourcespaginator)
         """
 
 class ListPlaybackConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPlaybackConfigurationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPlaybackConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPlaybackConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listplaybackconfigurationspaginator)
         """
 
 class ListPrefetchSchedulesPaginator(Paginator):
     """
@@ -150,40 +150,40 @@
 
     def paginate(
         self,
         *,
         PlaybackConfigurationName: str,
         StreamId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPrefetchSchedulesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPrefetchSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListPrefetchSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listprefetchschedulespaginator)
         """
 
 class ListSourceLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSourceLocationsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSourceLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListSourceLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listsourcelocationspaginator)
         """
 
 class ListVodSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
     """
 
     def paginate(
         self, *, SourceLocationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVodSourcesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListVodSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Paginator.ListVodSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/paginators/#listvodsourcespaginator)
         """
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.py` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,42 +48,42 @@
     "SlateSourceOutputTypeDef",
     "SpliceInsertMessageOutputTypeDef",
     "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughOutputTypeDef",
     "AdMarkerPassthroughTypeDef",
-    "AlertOutputTypeDef",
+    "AlertTypeDef",
     "AvailMatchingCriteriaOutputTypeDef",
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionOutputTypeDef",
     "AvailSuppressionTypeDef",
     "BumperOutputTypeDef",
     "BumperTypeDef",
     "CdnConfigurationOutputTypeDef",
     "CdnConfigurationTypeDef",
-    "LogConfigurationForChannelOutputTypeDef",
+    "LogConfigurationForChannelTypeDef",
     "ClipRangeOutputTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
-    "ConfigureLogsForChannelResponseOutputTypeDef",
+    "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
-    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "HttpPackageConfigurationTypeDef",
     "HttpPackageConfigurationOutputTypeDef",
     "PrefetchRetrievalTypeDef",
     "PrefetchRetrievalOutputTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
     "DefaultSegmentDeliveryConfigurationOutputTypeDef",
     "HttpConfigurationOutputTypeDef",
     "SegmentDeliveryConfigurationOutputTypeDef",
     "DashConfigurationForPutTypeDef",
-    "DashConfigurationOutputTypeDef",
+    "DashConfigurationTypeDef",
     "DashPlaylistSettingsOutputTypeDef",
     "DashPlaylistSettingsTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteLiveSourceRequestRequestTypeDef",
     "DeletePlaybackConfigurationRequestRequestTypeDef",
     "DeletePrefetchScheduleRequestRequestTypeDef",
@@ -93,21 +93,21 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeLiveSourceRequestRequestTypeDef",
     "DescribeProgramRequestRequestTypeDef",
     "DescribeSourceLocationRequestRequestTypeDef",
     "DescribeVodSourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "GetChannelPolicyResponseOutputTypeDef",
+    "GetChannelPolicyResponseTypeDef",
     "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     "GetChannelScheduleRequestRequestTypeDef",
     "GetPlaybackConfigurationRequestRequestTypeDef",
-    "HlsConfigurationOutputTypeDef",
+    "HlsConfigurationTypeDef",
     "LivePreRollConfigurationOutputTypeDef",
-    "LogConfigurationOutputTypeDef",
+    "LogConfigurationTypeDef",
     "GetPrefetchScheduleRequestRequestTypeDef",
     "HlsPlaylistSettingsOutputTypeDef",
     "HlsPlaylistSettingsTypeDef",
     "ListAlertsRequestListAlertsPaginateTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
@@ -116,88 +116,88 @@
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
     "ListPrefetchSchedulesRequestRequestTypeDef",
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListSourceLocationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "ListVodSourcesRequestRequestTypeDef",
     "LivePreRollConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ScheduleAdBreakOutputTypeDef",
+    "ScheduleAdBreakTypeDef",
     "TransitionTypeDef",
     "SegmentationDescriptorOutputTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
     "AccessConfigurationOutputTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesOutputTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "ListAlertsResponseOutputTypeDef",
+    "ListAlertsResponseTypeDef",
     "PrefetchConsumptionOutputTypeDef",
     "PrefetchConsumptionTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
     "CreateVodSourceRequestRequestTypeDef",
     "UpdateLiveSourceRequestRequestTypeDef",
     "UpdateVodSourceRequestRequestTypeDef",
-    "CreateLiveSourceResponseOutputTypeDef",
-    "CreateVodSourceResponseOutputTypeDef",
-    "DescribeLiveSourceResponseOutputTypeDef",
-    "DescribeVodSourceResponseOutputTypeDef",
-    "LiveSourceOutputTypeDef",
-    "UpdateLiveSourceResponseOutputTypeDef",
-    "UpdateVodSourceResponseOutputTypeDef",
-    "VodSourceOutputTypeDef",
-    "ResponseOutputItemOutputTypeDef",
+    "CreateLiveSourceResponseTypeDef",
+    "CreateVodSourceResponseTypeDef",
+    "DescribeLiveSourceResponseTypeDef",
+    "DescribeVodSourceResponseTypeDef",
+    "LiveSourceTypeDef",
+    "UpdateLiveSourceResponseTypeDef",
+    "UpdateVodSourceResponseTypeDef",
+    "VodSourceTypeDef",
+    "ResponseOutputItemTypeDef",
     "RequestOutputItemTypeDef",
-    "ScheduleEntryOutputTypeDef",
+    "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
     "TimeSignalMessageOutputTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
-    "CreateSourceLocationResponseOutputTypeDef",
-    "DescribeSourceLocationResponseOutputTypeDef",
-    "SourceLocationOutputTypeDef",
-    "UpdateSourceLocationResponseOutputTypeDef",
+    "CreateSourceLocationResponseTypeDef",
+    "DescribeSourceLocationResponseTypeDef",
+    "SourceLocationTypeDef",
+    "UpdateSourceLocationResponseTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
-    "GetPlaybackConfigurationResponseOutputTypeDef",
-    "PlaybackConfigurationOutputTypeDef",
-    "PutPlaybackConfigurationResponseOutputTypeDef",
+    "GetPlaybackConfigurationResponseTypeDef",
+    "PlaybackConfigurationTypeDef",
+    "PutPlaybackConfigurationResponseTypeDef",
     "PutPlaybackConfigurationRequestRequestTypeDef",
-    "CreatePrefetchScheduleResponseOutputTypeDef",
-    "GetPrefetchScheduleResponseOutputTypeDef",
-    "PrefetchScheduleOutputTypeDef",
+    "CreatePrefetchScheduleResponseTypeDef",
+    "GetPrefetchScheduleResponseTypeDef",
+    "PrefetchScheduleTypeDef",
     "CreatePrefetchScheduleRequestRequestTypeDef",
-    "ListLiveSourcesResponseOutputTypeDef",
-    "ListVodSourcesResponseOutputTypeDef",
-    "ChannelOutputTypeDef",
-    "CreateChannelResponseOutputTypeDef",
-    "DescribeChannelResponseOutputTypeDef",
-    "UpdateChannelResponseOutputTypeDef",
+    "ListLiveSourcesResponseTypeDef",
+    "ListVodSourcesResponseTypeDef",
+    "ChannelTypeDef",
+    "CreateChannelResponseTypeDef",
+    "DescribeChannelResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "GetChannelScheduleResponseOutputTypeDef",
+    "GetChannelScheduleResponseTypeDef",
     "AdBreakOutputTypeDef",
     "AdBreakTypeDef",
-    "ListSourceLocationsResponseOutputTypeDef",
-    "ListPlaybackConfigurationsResponseOutputTypeDef",
-    "ListPrefetchSchedulesResponseOutputTypeDef",
-    "ListChannelsResponseOutputTypeDef",
-    "CreateProgramResponseOutputTypeDef",
-    "DescribeProgramResponseOutputTypeDef",
-    "UpdateProgramResponseOutputTypeDef",
+    "ListSourceLocationsResponseTypeDef",
+    "ListPlaybackConfigurationsResponseTypeDef",
+    "ListPrefetchSchedulesResponseTypeDef",
+    "ListChannelsResponseTypeDef",
+    "CreateProgramResponseTypeDef",
+    "DescribeProgramResponseTypeDef",
+    "UpdateProgramResponseTypeDef",
     "CreateProgramRequestRequestTypeDef",
     "UpdateProgramRequestRequestTypeDef",
 )
 
 SecretsManagerAccessTokenConfigurationOutputTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationOutputTypeDef",
     {
@@ -282,16 +282,16 @@
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AlertOutputTypeDef = TypedDict(
-    "AlertOutputTypeDef",
+AlertTypeDef = TypedDict(
+    "AlertTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
         "Category": AlertCategoryType,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
@@ -363,16 +363,16 @@
     {
         "AdSegmentUrlPrefix": str,
         "ContentSegmentUrlPrefix": str,
     },
     total=False,
 )
 
-LogConfigurationForChannelOutputTypeDef = TypedDict(
-    "LogConfigurationForChannelOutputTypeDef",
+LogConfigurationForChannelTypeDef = TypedDict(
+    "LogConfigurationForChannelTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
 )
 
 ClipRangeOutputTypeDef = TypedDict(
     "ClipRangeOutputTypeDef",
@@ -392,16 +392,16 @@
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
 
-ConfigureLogsForChannelResponseOutputTypeDef = TypedDict(
-    "ConfigureLogsForChannelResponseOutputTypeDef",
+ConfigureLogsForChannelResponseTypeDef = TypedDict(
+    "ConfigureLogsForChannelResponseTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -409,16 +409,16 @@
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
     },
 )
 
-ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef = TypedDict(
-    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
+ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -522,16 +522,16 @@
     {
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
     total=False,
 )
 
-DashConfigurationOutputTypeDef = TypedDict(
-    "DashConfigurationOutputTypeDef",
+DashConfigurationTypeDef = TypedDict(
+    "DashConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
 )
 
@@ -664,16 +664,16 @@
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 
-GetChannelPolicyResponseOutputTypeDef = TypedDict(
-    "GetChannelPolicyResponseOutputTypeDef",
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -726,31 +726,31 @@
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-HlsConfigurationOutputTypeDef = TypedDict(
-    "HlsConfigurationOutputTypeDef",
+HlsConfigurationTypeDef = TypedDict(
+    "HlsConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
     },
 )
 
 LivePreRollConfigurationOutputTypeDef = TypedDict(
     "LivePreRollConfigurationOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
         "MaxDurationSeconds": int,
     },
 )
 
-LogConfigurationOutputTypeDef = TypedDict(
-    "LogConfigurationOutputTypeDef",
+LogConfigurationTypeDef = TypedDict(
+    "LogConfigurationTypeDef",
     {
         "PercentEnabled": int,
     },
 )
 
 GetPrefetchScheduleRequestRequestTypeDef = TypedDict(
     "GetPrefetchScheduleRequestRequestTypeDef",
@@ -966,16 +966,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
@@ -1056,16 +1056,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ScheduleAdBreakOutputTypeDef = TypedDict(
-    "ScheduleAdBreakOutputTypeDef",
+ScheduleAdBreakTypeDef = TypedDict(
+    "ScheduleAdBreakTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
@@ -1190,18 +1190,18 @@
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
     total=False,
 )
 
-ListAlertsResponseOutputTypeDef = TypedDict(
-    "ListAlertsResponseOutputTypeDef",
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
     {
-        "Items": List[AlertOutputTypeDef],
+        "Items": List[AlertTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PrefetchConsumptionOutputTypeDef = TypedDict(
     "PrefetchConsumptionOutputTypeDef",
@@ -1294,126 +1294,126 @@
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
-CreateLiveSourceResponseOutputTypeDef = TypedDict(
-    "CreateLiveSourceResponseOutputTypeDef",
+CreateLiveSourceResponseTypeDef = TypedDict(
+    "CreateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVodSourceResponseOutputTypeDef = TypedDict(
-    "CreateVodSourceResponseOutputTypeDef",
+CreateVodSourceResponseTypeDef = TypedDict(
+    "CreateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLiveSourceResponseOutputTypeDef = TypedDict(
-    "DescribeLiveSourceResponseOutputTypeDef",
+DescribeLiveSourceResponseTypeDef = TypedDict(
+    "DescribeLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVodSourceResponseOutputTypeDef = TypedDict(
-    "DescribeVodSourceResponseOutputTypeDef",
+DescribeVodSourceResponseTypeDef = TypedDict(
+    "DescribeVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-LiveSourceOutputTypeDef = TypedDict(
-    "LiveSourceOutputTypeDef",
+LiveSourceTypeDef = TypedDict(
+    "LiveSourceTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
     },
 )
 
-UpdateLiveSourceResponseOutputTypeDef = TypedDict(
-    "UpdateLiveSourceResponseOutputTypeDef",
+UpdateLiveSourceResponseTypeDef = TypedDict(
+    "UpdateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVodSourceResponseOutputTypeDef = TypedDict(
-    "UpdateVodSourceResponseOutputTypeDef",
+UpdateVodSourceResponseTypeDef = TypedDict(
+    "UpdateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VodSourceOutputTypeDef = TypedDict(
-    "VodSourceOutputTypeDef",
+VodSourceTypeDef = TypedDict(
+    "VodSourceTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
     },
 )
 
-ResponseOutputItemOutputTypeDef = TypedDict(
-    "ResponseOutputItemOutputTypeDef",
+ResponseOutputItemTypeDef = TypedDict(
+    "ResponseOutputItemTypeDef",
     {
         "DashPlaylistSettings": DashPlaylistSettingsOutputTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsOutputTypeDef,
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
@@ -1438,24 +1438,24 @@
 
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
 
-ScheduleEntryOutputTypeDef = TypedDict(
-    "ScheduleEntryOutputTypeDef",
+ScheduleEntryTypeDef = TypedDict(
+    "ScheduleEntryTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "Arn": str,
         "ChannelName": str,
         "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduleAdBreaks": List[ScheduleAdBreakOutputTypeDef],
+        "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
 _RequiredScheduleConfigurationTypeDef = TypedDict(
@@ -1499,63 +1499,63 @@
     {
         "ClipRange": ClipRangeTypeDef,
         "Transition": UpdateProgramTransitionTypeDef,
     },
     total=False,
 )
 
-CreateSourceLocationResponseOutputTypeDef = TypedDict(
-    "CreateSourceLocationResponseOutputTypeDef",
+CreateSourceLocationResponseTypeDef = TypedDict(
+    "CreateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSourceLocationResponseOutputTypeDef = TypedDict(
-    "DescribeSourceLocationResponseOutputTypeDef",
+DescribeSourceLocationResponseTypeDef = TypedDict(
+    "DescribeSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SourceLocationOutputTypeDef = TypedDict(
-    "SourceLocationOutputTypeDef",
+SourceLocationTypeDef = TypedDict(
+    "SourceLocationTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
     },
 )
 
-UpdateSourceLocationResponseOutputTypeDef = TypedDict(
-    "UpdateSourceLocationResponseOutputTypeDef",
+UpdateSourceLocationResponseTypeDef = TypedDict(
+    "UpdateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
@@ -1613,77 +1613,77 @@
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
 
-GetPlaybackConfigurationResponseOutputTypeDef = TypedDict(
-    "GetPlaybackConfigurationResponseOutputTypeDef",
+GetPlaybackConfigurationResponseTypeDef = TypedDict(
+    "GetPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionOutputTypeDef,
         "Bumper": BumperOutputTypeDef,
         "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationOutputTypeDef,
-        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "DashConfiguration": DashConfigurationTypeDef,
+        "HlsConfiguration": HlsConfigurationTypeDef,
         "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
-        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PlaybackConfigurationOutputTypeDef = TypedDict(
-    "PlaybackConfigurationOutputTypeDef",
+PlaybackConfigurationTypeDef = TypedDict(
+    "PlaybackConfigurationTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionOutputTypeDef,
         "Bumper": BumperOutputTypeDef,
         "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationOutputTypeDef,
-        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "DashConfiguration": DashConfigurationTypeDef,
+        "HlsConfiguration": HlsConfigurationTypeDef,
         "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
-        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
 )
 
-PutPlaybackConfigurationResponseOutputTypeDef = TypedDict(
-    "PutPlaybackConfigurationResponseOutputTypeDef",
+PutPlaybackConfigurationResponseTypeDef = TypedDict(
+    "PutPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionOutputTypeDef,
         "Bumper": BumperOutputTypeDef,
         "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationOutputTypeDef,
-        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "DashConfiguration": DashConfigurationTypeDef,
+        "HlsConfiguration": HlsConfigurationTypeDef,
         "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
-        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
@@ -1724,42 +1724,42 @@
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePrefetchScheduleResponseOutputTypeDef = TypedDict(
-    "CreatePrefetchScheduleResponseOutputTypeDef",
+CreatePrefetchScheduleResponseTypeDef = TypedDict(
+    "CreatePrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalOutputTypeDef,
         "StreamId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPrefetchScheduleResponseOutputTypeDef = TypedDict(
-    "GetPrefetchScheduleResponseOutputTypeDef",
+GetPrefetchScheduleResponseTypeDef = TypedDict(
+    "GetPrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalOutputTypeDef,
         "StreamId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PrefetchScheduleOutputTypeDef = TypedDict(
-    "PrefetchScheduleOutputTypeDef",
+PrefetchScheduleTypeDef = TypedDict(
+    "PrefetchScheduleTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalOutputTypeDef,
         "StreamId": str,
@@ -1787,94 +1787,94 @@
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
 
-ListLiveSourcesResponseOutputTypeDef = TypedDict(
-    "ListLiveSourcesResponseOutputTypeDef",
+ListLiveSourcesResponseTypeDef = TypedDict(
+    "ListLiveSourcesResponseTypeDef",
     {
-        "Items": List[LiveSourceOutputTypeDef],
+        "Items": List[LiveSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVodSourcesResponseOutputTypeDef = TypedDict(
-    "ListVodSourcesResponseOutputTypeDef",
+ListVodSourcesResponseTypeDef = TypedDict(
+    "ListVodSourcesResponseTypeDef",
     {
-        "Items": List[VodSourceOutputTypeDef],
+        "Items": List[VodSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ChannelOutputTypeDef = TypedDict(
-    "ChannelOutputTypeDef",
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "LogConfiguration": LogConfigurationForChannelTypeDef,
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
     },
 )
 
-CreateChannelResponseOutputTypeDef = TypedDict(
-    "CreateChannelResponseOutputTypeDef",
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeChannelResponseOutputTypeDef = TypedDict(
-    "DescribeChannelResponseOutputTypeDef",
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "LogConfiguration": LogConfigurationForChannelTypeDef,
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelResponseOutputTypeDef = TypedDict(
-    "UpdateChannelResponseOutputTypeDef",
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1921,18 +1921,18 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-GetChannelScheduleResponseOutputTypeDef = TypedDict(
-    "GetChannelScheduleResponseOutputTypeDef",
+GetChannelScheduleResponseTypeDef = TypedDict(
+    "GetChannelScheduleResponseTypeDef",
     {
-        "Items": List[ScheduleEntryOutputTypeDef],
+        "Items": List[ScheduleEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdBreakOutputTypeDef = TypedDict(
     "AdBreakOutputTypeDef",
@@ -1955,52 +1955,52 @@
         "Slate": SlateSourceTypeDef,
         "SpliceInsertMessage": SpliceInsertMessageTypeDef,
         "TimeSignalMessage": TimeSignalMessageTypeDef,
     },
     total=False,
 )
 
-ListSourceLocationsResponseOutputTypeDef = TypedDict(
-    "ListSourceLocationsResponseOutputTypeDef",
+ListSourceLocationsResponseTypeDef = TypedDict(
+    "ListSourceLocationsResponseTypeDef",
     {
-        "Items": List[SourceLocationOutputTypeDef],
+        "Items": List[SourceLocationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPlaybackConfigurationsResponseOutputTypeDef = TypedDict(
-    "ListPlaybackConfigurationsResponseOutputTypeDef",
+ListPlaybackConfigurationsResponseTypeDef = TypedDict(
+    "ListPlaybackConfigurationsResponseTypeDef",
     {
-        "Items": List[PlaybackConfigurationOutputTypeDef],
+        "Items": List[PlaybackConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPrefetchSchedulesResponseOutputTypeDef = TypedDict(
-    "ListPrefetchSchedulesResponseOutputTypeDef",
+ListPrefetchSchedulesResponseTypeDef = TypedDict(
+    "ListPrefetchSchedulesResponseTypeDef",
     {
-        "Items": List[PrefetchScheduleOutputTypeDef],
+        "Items": List[PrefetchScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListChannelsResponseOutputTypeDef = TypedDict(
-    "ListChannelsResponseOutputTypeDef",
+ListChannelsResponseTypeDef = TypedDict(
+    "ListChannelsResponseTypeDef",
     {
-        "Items": List[ChannelOutputTypeDef],
+        "Items": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProgramResponseOutputTypeDef = TypedDict(
-    "CreateProgramResponseOutputTypeDef",
+CreateProgramResponseTypeDef = TypedDict(
+    "CreateProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
@@ -2009,16 +2009,16 @@
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeProgramResponseOutputTypeDef = TypedDict(
-    "DescribeProgramResponseOutputTypeDef",
+DescribeProgramResponseTypeDef = TypedDict(
+    "DescribeProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
@@ -2027,16 +2027,16 @@
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateProgramResponseOutputTypeDef = TypedDict(
-    "UpdateProgramResponseOutputTypeDef",
+UpdateProgramResponseTypeDef = TypedDict(
+    "UpdateProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor/type_defs.pyi` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -47,42 +47,42 @@
     "SlateSourceOutputTypeDef",
     "SpliceInsertMessageOutputTypeDef",
     "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughOutputTypeDef",
     "AdMarkerPassthroughTypeDef",
-    "AlertOutputTypeDef",
+    "AlertTypeDef",
     "AvailMatchingCriteriaOutputTypeDef",
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionOutputTypeDef",
     "AvailSuppressionTypeDef",
     "BumperOutputTypeDef",
     "BumperTypeDef",
     "CdnConfigurationOutputTypeDef",
     "CdnConfigurationTypeDef",
-    "LogConfigurationForChannelOutputTypeDef",
+    "LogConfigurationForChannelTypeDef",
     "ClipRangeOutputTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
-    "ConfigureLogsForChannelResponseOutputTypeDef",
+    "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
-    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "HttpPackageConfigurationTypeDef",
     "HttpPackageConfigurationOutputTypeDef",
     "PrefetchRetrievalTypeDef",
     "PrefetchRetrievalOutputTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
     "DefaultSegmentDeliveryConfigurationOutputTypeDef",
     "HttpConfigurationOutputTypeDef",
     "SegmentDeliveryConfigurationOutputTypeDef",
     "DashConfigurationForPutTypeDef",
-    "DashConfigurationOutputTypeDef",
+    "DashConfigurationTypeDef",
     "DashPlaylistSettingsOutputTypeDef",
     "DashPlaylistSettingsTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteLiveSourceRequestRequestTypeDef",
     "DeletePlaybackConfigurationRequestRequestTypeDef",
     "DeletePrefetchScheduleRequestRequestTypeDef",
@@ -92,21 +92,21 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeLiveSourceRequestRequestTypeDef",
     "DescribeProgramRequestRequestTypeDef",
     "DescribeSourceLocationRequestRequestTypeDef",
     "DescribeVodSourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
-    "GetChannelPolicyResponseOutputTypeDef",
+    "GetChannelPolicyResponseTypeDef",
     "GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     "GetChannelScheduleRequestRequestTypeDef",
     "GetPlaybackConfigurationRequestRequestTypeDef",
-    "HlsConfigurationOutputTypeDef",
+    "HlsConfigurationTypeDef",
     "LivePreRollConfigurationOutputTypeDef",
-    "LogConfigurationOutputTypeDef",
+    "LogConfigurationTypeDef",
     "GetPrefetchScheduleRequestRequestTypeDef",
     "HlsPlaylistSettingsOutputTypeDef",
     "HlsPlaylistSettingsTypeDef",
     "ListAlertsRequestListAlertsPaginateTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
@@ -115,88 +115,88 @@
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     "ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef",
     "ListPrefetchSchedulesRequestRequestTypeDef",
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListSourceLocationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "ListVodSourcesRequestRequestTypeDef",
     "LivePreRollConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ScheduleAdBreakOutputTypeDef",
+    "ScheduleAdBreakTypeDef",
     "TransitionTypeDef",
     "SegmentationDescriptorOutputTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
     "AccessConfigurationOutputTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesOutputTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "ListAlertsResponseOutputTypeDef",
+    "ListAlertsResponseTypeDef",
     "PrefetchConsumptionOutputTypeDef",
     "PrefetchConsumptionTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
     "CreateVodSourceRequestRequestTypeDef",
     "UpdateLiveSourceRequestRequestTypeDef",
     "UpdateVodSourceRequestRequestTypeDef",
-    "CreateLiveSourceResponseOutputTypeDef",
-    "CreateVodSourceResponseOutputTypeDef",
-    "DescribeLiveSourceResponseOutputTypeDef",
-    "DescribeVodSourceResponseOutputTypeDef",
-    "LiveSourceOutputTypeDef",
-    "UpdateLiveSourceResponseOutputTypeDef",
-    "UpdateVodSourceResponseOutputTypeDef",
-    "VodSourceOutputTypeDef",
-    "ResponseOutputItemOutputTypeDef",
+    "CreateLiveSourceResponseTypeDef",
+    "CreateVodSourceResponseTypeDef",
+    "DescribeLiveSourceResponseTypeDef",
+    "DescribeVodSourceResponseTypeDef",
+    "LiveSourceTypeDef",
+    "UpdateLiveSourceResponseTypeDef",
+    "UpdateVodSourceResponseTypeDef",
+    "VodSourceTypeDef",
+    "ResponseOutputItemTypeDef",
     "RequestOutputItemTypeDef",
-    "ScheduleEntryOutputTypeDef",
+    "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
     "TimeSignalMessageOutputTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
-    "CreateSourceLocationResponseOutputTypeDef",
-    "DescribeSourceLocationResponseOutputTypeDef",
-    "SourceLocationOutputTypeDef",
-    "UpdateSourceLocationResponseOutputTypeDef",
+    "CreateSourceLocationResponseTypeDef",
+    "DescribeSourceLocationResponseTypeDef",
+    "SourceLocationTypeDef",
+    "UpdateSourceLocationResponseTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
-    "GetPlaybackConfigurationResponseOutputTypeDef",
-    "PlaybackConfigurationOutputTypeDef",
-    "PutPlaybackConfigurationResponseOutputTypeDef",
+    "GetPlaybackConfigurationResponseTypeDef",
+    "PlaybackConfigurationTypeDef",
+    "PutPlaybackConfigurationResponseTypeDef",
     "PutPlaybackConfigurationRequestRequestTypeDef",
-    "CreatePrefetchScheduleResponseOutputTypeDef",
-    "GetPrefetchScheduleResponseOutputTypeDef",
-    "PrefetchScheduleOutputTypeDef",
+    "CreatePrefetchScheduleResponseTypeDef",
+    "GetPrefetchScheduleResponseTypeDef",
+    "PrefetchScheduleTypeDef",
     "CreatePrefetchScheduleRequestRequestTypeDef",
-    "ListLiveSourcesResponseOutputTypeDef",
-    "ListVodSourcesResponseOutputTypeDef",
-    "ChannelOutputTypeDef",
-    "CreateChannelResponseOutputTypeDef",
-    "DescribeChannelResponseOutputTypeDef",
-    "UpdateChannelResponseOutputTypeDef",
+    "ListLiveSourcesResponseTypeDef",
+    "ListVodSourcesResponseTypeDef",
+    "ChannelTypeDef",
+    "CreateChannelResponseTypeDef",
+    "DescribeChannelResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "GetChannelScheduleResponseOutputTypeDef",
+    "GetChannelScheduleResponseTypeDef",
     "AdBreakOutputTypeDef",
     "AdBreakTypeDef",
-    "ListSourceLocationsResponseOutputTypeDef",
-    "ListPlaybackConfigurationsResponseOutputTypeDef",
-    "ListPrefetchSchedulesResponseOutputTypeDef",
-    "ListChannelsResponseOutputTypeDef",
-    "CreateProgramResponseOutputTypeDef",
-    "DescribeProgramResponseOutputTypeDef",
-    "UpdateProgramResponseOutputTypeDef",
+    "ListSourceLocationsResponseTypeDef",
+    "ListPlaybackConfigurationsResponseTypeDef",
+    "ListPrefetchSchedulesResponseTypeDef",
+    "ListChannelsResponseTypeDef",
+    "CreateProgramResponseTypeDef",
+    "DescribeProgramResponseTypeDef",
+    "UpdateProgramResponseTypeDef",
     "CreateProgramRequestRequestTypeDef",
     "UpdateProgramRequestRequestTypeDef",
 )
 
 SecretsManagerAccessTokenConfigurationOutputTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationOutputTypeDef",
     {
@@ -281,16 +281,16 @@
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AlertOutputTypeDef = TypedDict(
-    "AlertOutputTypeDef",
+AlertTypeDef = TypedDict(
+    "AlertTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
         "Category": AlertCategoryType,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
@@ -362,16 +362,16 @@
     {
         "AdSegmentUrlPrefix": str,
         "ContentSegmentUrlPrefix": str,
     },
     total=False,
 )
 
-LogConfigurationForChannelOutputTypeDef = TypedDict(
-    "LogConfigurationForChannelOutputTypeDef",
+LogConfigurationForChannelTypeDef = TypedDict(
+    "LogConfigurationForChannelTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
 )
 
 ClipRangeOutputTypeDef = TypedDict(
     "ClipRangeOutputTypeDef",
@@ -391,16 +391,16 @@
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
 
-ConfigureLogsForChannelResponseOutputTypeDef = TypedDict(
-    "ConfigureLogsForChannelResponseOutputTypeDef",
+ConfigureLogsForChannelResponseTypeDef = TypedDict(
+    "ConfigureLogsForChannelResponseTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -408,16 +408,16 @@
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
     },
 )
 
-ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef = TypedDict(
-    "ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef",
+ConfigureLogsForPlaybackConfigurationResponseTypeDef = TypedDict(
+    "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     {
         "PercentEnabled": int,
         "PlaybackConfigurationName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -519,16 +519,16 @@
     {
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
     total=False,
 )
 
-DashConfigurationOutputTypeDef = TypedDict(
-    "DashConfigurationOutputTypeDef",
+DashConfigurationTypeDef = TypedDict(
+    "DashConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
         "MpdLocation": str,
         "OriginManifestType": OriginManifestTypeType,
     },
 )
 
@@ -661,16 +661,16 @@
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
     },
 )
 
-GetChannelPolicyResponseOutputTypeDef = TypedDict(
-    "GetChannelPolicyResponseOutputTypeDef",
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -719,31 +719,31 @@
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-HlsConfigurationOutputTypeDef = TypedDict(
-    "HlsConfigurationOutputTypeDef",
+HlsConfigurationTypeDef = TypedDict(
+    "HlsConfigurationTypeDef",
     {
         "ManifestEndpointPrefix": str,
     },
 )
 
 LivePreRollConfigurationOutputTypeDef = TypedDict(
     "LivePreRollConfigurationOutputTypeDef",
     {
         "AdDecisionServerUrl": str,
         "MaxDurationSeconds": int,
     },
 )
 
-LogConfigurationOutputTypeDef = TypedDict(
-    "LogConfigurationOutputTypeDef",
+LogConfigurationTypeDef = TypedDict(
+    "LogConfigurationTypeDef",
     {
         "PercentEnabled": int,
     },
 )
 
 GetPrefetchScheduleRequestRequestTypeDef = TypedDict(
     "GetPrefetchScheduleRequestRequestTypeDef",
@@ -947,16 +947,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef = TypedDict(
@@ -1033,16 +1033,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ScheduleAdBreakOutputTypeDef = TypedDict(
-    "ScheduleAdBreakOutputTypeDef",
+ScheduleAdBreakTypeDef = TypedDict(
+    "ScheduleAdBreakTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
@@ -1165,18 +1165,18 @@
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
     total=False,
 )
 
-ListAlertsResponseOutputTypeDef = TypedDict(
-    "ListAlertsResponseOutputTypeDef",
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
     {
-        "Items": List[AlertOutputTypeDef],
+        "Items": List[AlertTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PrefetchConsumptionOutputTypeDef = TypedDict(
     "PrefetchConsumptionOutputTypeDef",
@@ -1263,126 +1263,126 @@
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
-CreateLiveSourceResponseOutputTypeDef = TypedDict(
-    "CreateLiveSourceResponseOutputTypeDef",
+CreateLiveSourceResponseTypeDef = TypedDict(
+    "CreateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVodSourceResponseOutputTypeDef = TypedDict(
-    "CreateVodSourceResponseOutputTypeDef",
+CreateVodSourceResponseTypeDef = TypedDict(
+    "CreateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLiveSourceResponseOutputTypeDef = TypedDict(
-    "DescribeLiveSourceResponseOutputTypeDef",
+DescribeLiveSourceResponseTypeDef = TypedDict(
+    "DescribeLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVodSourceResponseOutputTypeDef = TypedDict(
-    "DescribeVodSourceResponseOutputTypeDef",
+DescribeVodSourceResponseTypeDef = TypedDict(
+    "DescribeVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-LiveSourceOutputTypeDef = TypedDict(
-    "LiveSourceOutputTypeDef",
+LiveSourceTypeDef = TypedDict(
+    "LiveSourceTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
     },
 )
 
-UpdateLiveSourceResponseOutputTypeDef = TypedDict(
-    "UpdateLiveSourceResponseOutputTypeDef",
+UpdateLiveSourceResponseTypeDef = TypedDict(
+    "UpdateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "LiveSourceName": str,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVodSourceResponseOutputTypeDef = TypedDict(
-    "UpdateVodSourceResponseOutputTypeDef",
+UpdateVodSourceResponseTypeDef = TypedDict(
+    "UpdateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VodSourceOutputTypeDef = TypedDict(
-    "VodSourceOutputTypeDef",
+VodSourceTypeDef = TypedDict(
+    "VodSourceTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationOutputTypeDef],
         "LastModifiedTime": datetime,
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "VodSourceName": str,
     },
 )
 
-ResponseOutputItemOutputTypeDef = TypedDict(
-    "ResponseOutputItemOutputTypeDef",
+ResponseOutputItemTypeDef = TypedDict(
+    "ResponseOutputItemTypeDef",
     {
         "DashPlaylistSettings": DashPlaylistSettingsOutputTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsOutputTypeDef,
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
@@ -1405,24 +1405,24 @@
 )
 
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
-ScheduleEntryOutputTypeDef = TypedDict(
-    "ScheduleEntryOutputTypeDef",
+ScheduleEntryTypeDef = TypedDict(
+    "ScheduleEntryTypeDef",
     {
         "ApproximateDurationSeconds": int,
         "ApproximateStartTime": datetime,
         "Arn": str,
         "ChannelName": str,
         "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduleAdBreaks": List[ScheduleAdBreakOutputTypeDef],
+        "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "SourceLocationName": str,
         "VodSourceName": str,
     },
 )
 
 _RequiredScheduleConfigurationTypeDef = TypedDict(
@@ -1464,63 +1464,63 @@
     {
         "ClipRange": ClipRangeTypeDef,
         "Transition": UpdateProgramTransitionTypeDef,
     },
     total=False,
 )
 
-CreateSourceLocationResponseOutputTypeDef = TypedDict(
-    "CreateSourceLocationResponseOutputTypeDef",
+CreateSourceLocationResponseTypeDef = TypedDict(
+    "CreateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSourceLocationResponseOutputTypeDef = TypedDict(
-    "DescribeSourceLocationResponseOutputTypeDef",
+DescribeSourceLocationResponseTypeDef = TypedDict(
+    "DescribeSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SourceLocationOutputTypeDef = TypedDict(
-    "SourceLocationOutputTypeDef",
+SourceLocationTypeDef = TypedDict(
+    "SourceLocationTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationOutputTypeDef],
         "SourceLocationName": str,
         "Tags": Dict[str, str],
     },
 )
 
-UpdateSourceLocationResponseOutputTypeDef = TypedDict(
-    "UpdateSourceLocationResponseOutputTypeDef",
+UpdateSourceLocationResponseTypeDef = TypedDict(
+    "UpdateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationOutputTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationOutputTypeDef,
         "HttpConfiguration": HttpConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
@@ -1574,77 +1574,77 @@
 
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
-GetPlaybackConfigurationResponseOutputTypeDef = TypedDict(
-    "GetPlaybackConfigurationResponseOutputTypeDef",
+GetPlaybackConfigurationResponseTypeDef = TypedDict(
+    "GetPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionOutputTypeDef,
         "Bumper": BumperOutputTypeDef,
         "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationOutputTypeDef,
-        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "DashConfiguration": DashConfigurationTypeDef,
+        "HlsConfiguration": HlsConfigurationTypeDef,
         "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
-        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PlaybackConfigurationOutputTypeDef = TypedDict(
-    "PlaybackConfigurationOutputTypeDef",
+PlaybackConfigurationTypeDef = TypedDict(
+    "PlaybackConfigurationTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionOutputTypeDef,
         "Bumper": BumperOutputTypeDef,
         "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationOutputTypeDef,
-        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "DashConfiguration": DashConfigurationTypeDef,
+        "HlsConfiguration": HlsConfigurationTypeDef,
         "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
-        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
 )
 
-PutPlaybackConfigurationResponseOutputTypeDef = TypedDict(
-    "PutPlaybackConfigurationResponseOutputTypeDef",
+PutPlaybackConfigurationResponseTypeDef = TypedDict(
+    "PutPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionOutputTypeDef,
         "Bumper": BumperOutputTypeDef,
         "CdnConfiguration": CdnConfigurationOutputTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
-        "DashConfiguration": DashConfigurationOutputTypeDef,
-        "HlsConfiguration": HlsConfigurationOutputTypeDef,
+        "DashConfiguration": DashConfigurationTypeDef,
+        "HlsConfiguration": HlsConfigurationTypeDef,
         "LivePreRollConfiguration": LivePreRollConfigurationOutputTypeDef,
-        "LogConfiguration": LogConfigurationOutputTypeDef,
+        "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesOutputTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
         "SessionInitializationEndpointPrefix": str,
         "SlateAdUrl": str,
@@ -1683,42 +1683,42 @@
 
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
-CreatePrefetchScheduleResponseOutputTypeDef = TypedDict(
-    "CreatePrefetchScheduleResponseOutputTypeDef",
+CreatePrefetchScheduleResponseTypeDef = TypedDict(
+    "CreatePrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalOutputTypeDef,
         "StreamId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPrefetchScheduleResponseOutputTypeDef = TypedDict(
-    "GetPrefetchScheduleResponseOutputTypeDef",
+GetPrefetchScheduleResponseTypeDef = TypedDict(
+    "GetPrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalOutputTypeDef,
         "StreamId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PrefetchScheduleOutputTypeDef = TypedDict(
-    "PrefetchScheduleOutputTypeDef",
+PrefetchScheduleTypeDef = TypedDict(
+    "PrefetchScheduleTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionOutputTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalOutputTypeDef,
         "StreamId": str,
@@ -1744,94 +1744,94 @@
 
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
-ListLiveSourcesResponseOutputTypeDef = TypedDict(
-    "ListLiveSourcesResponseOutputTypeDef",
+ListLiveSourcesResponseTypeDef = TypedDict(
+    "ListLiveSourcesResponseTypeDef",
     {
-        "Items": List[LiveSourceOutputTypeDef],
+        "Items": List[LiveSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVodSourcesResponseOutputTypeDef = TypedDict(
-    "ListVodSourcesResponseOutputTypeDef",
+ListVodSourcesResponseTypeDef = TypedDict(
+    "ListVodSourcesResponseTypeDef",
     {
-        "Items": List[VodSourceOutputTypeDef],
+        "Items": List[VodSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ChannelOutputTypeDef = TypedDict(
-    "ChannelOutputTypeDef",
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "LogConfiguration": LogConfigurationForChannelTypeDef,
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
     },
 )
 
-CreateChannelResponseOutputTypeDef = TypedDict(
-    "CreateChannelResponseOutputTypeDef",
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeChannelResponseOutputTypeDef = TypedDict(
-    "DescribeChannelResponseOutputTypeDef",
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "LogConfiguration": LogConfigurationForChannelOutputTypeDef,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "LogConfiguration": LogConfigurationForChannelTypeDef,
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelResponseOutputTypeDef = TypedDict(
-    "UpdateChannelResponseOutputTypeDef",
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
         "FillerSlate": SlateSourceOutputTypeDef,
         "LastModifiedTime": datetime,
-        "Outputs": List[ResponseOutputItemOutputTypeDef],
+        "Outputs": List[ResponseOutputItemTypeDef],
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1874,18 +1874,18 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-GetChannelScheduleResponseOutputTypeDef = TypedDict(
-    "GetChannelScheduleResponseOutputTypeDef",
+GetChannelScheduleResponseTypeDef = TypedDict(
+    "GetChannelScheduleResponseTypeDef",
     {
-        "Items": List[ScheduleEntryOutputTypeDef],
+        "Items": List[ScheduleEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdBreakOutputTypeDef = TypedDict(
     "AdBreakOutputTypeDef",
@@ -1908,52 +1908,52 @@
         "Slate": SlateSourceTypeDef,
         "SpliceInsertMessage": SpliceInsertMessageTypeDef,
         "TimeSignalMessage": TimeSignalMessageTypeDef,
     },
     total=False,
 )
 
-ListSourceLocationsResponseOutputTypeDef = TypedDict(
-    "ListSourceLocationsResponseOutputTypeDef",
+ListSourceLocationsResponseTypeDef = TypedDict(
+    "ListSourceLocationsResponseTypeDef",
     {
-        "Items": List[SourceLocationOutputTypeDef],
+        "Items": List[SourceLocationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPlaybackConfigurationsResponseOutputTypeDef = TypedDict(
-    "ListPlaybackConfigurationsResponseOutputTypeDef",
+ListPlaybackConfigurationsResponseTypeDef = TypedDict(
+    "ListPlaybackConfigurationsResponseTypeDef",
     {
-        "Items": List[PlaybackConfigurationOutputTypeDef],
+        "Items": List[PlaybackConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPrefetchSchedulesResponseOutputTypeDef = TypedDict(
-    "ListPrefetchSchedulesResponseOutputTypeDef",
+ListPrefetchSchedulesResponseTypeDef = TypedDict(
+    "ListPrefetchSchedulesResponseTypeDef",
     {
-        "Items": List[PrefetchScheduleOutputTypeDef],
+        "Items": List[PrefetchScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListChannelsResponseOutputTypeDef = TypedDict(
-    "ListChannelsResponseOutputTypeDef",
+ListChannelsResponseTypeDef = TypedDict(
+    "ListChannelsResponseTypeDef",
     {
-        "Items": List[ChannelOutputTypeDef],
+        "Items": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProgramResponseOutputTypeDef = TypedDict(
-    "CreateProgramResponseOutputTypeDef",
+CreateProgramResponseTypeDef = TypedDict(
+    "CreateProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
@@ -1962,16 +1962,16 @@
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeProgramResponseOutputTypeDef = TypedDict(
-    "DescribeProgramResponseOutputTypeDef",
+DescribeProgramResponseTypeDef = TypedDict(
+    "DescribeProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
@@ -1980,16 +1980,16 @@
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateProgramResponseOutputTypeDef = TypedDict(
-    "UpdateProgramResponseOutputTypeDef",
+UpdateProgramResponseTypeDef = TypedDict(
+    "UpdateProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakOutputTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeOutputTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/PKG-INFO` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
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
 [mypy-boto3-mediatailor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,42 +374,42 @@
     SlateSourceOutputTypeDef,
     SpliceInsertMessageOutputTypeDef,
     KeyValuePairTypeDef,
     SlateSourceTypeDef,
     SpliceInsertMessageTypeDef,
     AdMarkerPassthroughOutputTypeDef,
     AdMarkerPassthroughTypeDef,
-    AlertOutputTypeDef,
+    AlertTypeDef,
     AvailMatchingCriteriaOutputTypeDef,
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionOutputTypeDef,
     AvailSuppressionTypeDef,
     BumperOutputTypeDef,
     BumperTypeDef,
     CdnConfigurationOutputTypeDef,
     CdnConfigurationTypeDef,
-    LogConfigurationForChannelOutputTypeDef,
+    LogConfigurationForChannelTypeDef,
     ClipRangeOutputTypeDef,
     ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
-    ConfigureLogsForChannelResponseOutputTypeDef,
+    ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
-    ConfigureLogsForPlaybackConfigurationResponseOutputTypeDef,
+    ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     HttpPackageConfigurationTypeDef,
     HttpPackageConfigurationOutputTypeDef,
     PrefetchRetrievalTypeDef,
     PrefetchRetrievalOutputTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     DefaultSegmentDeliveryConfigurationOutputTypeDef,
     HttpConfigurationOutputTypeDef,
     SegmentDeliveryConfigurationOutputTypeDef,
     DashConfigurationForPutTypeDef,
-    DashConfigurationOutputTypeDef,
+    DashConfigurationTypeDef,
     DashPlaylistSettingsOutputTypeDef,
     DashPlaylistSettingsTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteLiveSourceRequestRequestTypeDef,
     DeletePlaybackConfigurationRequestRequestTypeDef,
     DeletePrefetchScheduleRequestRequestTypeDef,
@@ -419,21 +419,21 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeLiveSourceRequestRequestTypeDef,
     DescribeProgramRequestRequestTypeDef,
     DescribeSourceLocationRequestRequestTypeDef,
     DescribeVodSourceRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
-    GetChannelPolicyResponseOutputTypeDef,
+    GetChannelPolicyResponseTypeDef,
     GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     GetChannelScheduleRequestRequestTypeDef,
     GetPlaybackConfigurationRequestRequestTypeDef,
-    HlsConfigurationOutputTypeDef,
+    HlsConfigurationTypeDef,
     LivePreRollConfigurationOutputTypeDef,
-    LogConfigurationOutputTypeDef,
+    LogConfigurationTypeDef,
     GetPrefetchScheduleRequestRequestTypeDef,
     HlsPlaylistSettingsOutputTypeDef,
     HlsPlaylistSettingsTypeDef,
     ListAlertsRequestListAlertsPaginateTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
@@ -442,88 +442,88 @@
     ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef,
     ListPlaybackConfigurationsRequestRequestTypeDef,
     ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     ListPrefetchSchedulesRequestRequestTypeDef,
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListSourceLocationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     ListVodSourcesRequestRequestTypeDef,
     LivePreRollConfigurationTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    ScheduleAdBreakOutputTypeDef,
+    ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorOutputTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProgramTransitionTypeDef,
     AccessConfigurationOutputTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesOutputTypeDef,
     ManifestProcessingRulesTypeDef,
-    ListAlertsResponseOutputTypeDef,
+    ListAlertsResponseTypeDef,
     PrefetchConsumptionOutputTypeDef,
     PrefetchConsumptionTypeDef,
     CreateLiveSourceRequestRequestTypeDef,
     CreateVodSourceRequestRequestTypeDef,
     UpdateLiveSourceRequestRequestTypeDef,
     UpdateVodSourceRequestRequestTypeDef,
-    CreateLiveSourceResponseOutputTypeDef,
-    CreateVodSourceResponseOutputTypeDef,
-    DescribeLiveSourceResponseOutputTypeDef,
-    DescribeVodSourceResponseOutputTypeDef,
-    LiveSourceOutputTypeDef,
-    UpdateLiveSourceResponseOutputTypeDef,
-    UpdateVodSourceResponseOutputTypeDef,
-    VodSourceOutputTypeDef,
-    ResponseOutputItemOutputTypeDef,
+    CreateLiveSourceResponseTypeDef,
+    CreateVodSourceResponseTypeDef,
+    DescribeLiveSourceResponseTypeDef,
+    DescribeVodSourceResponseTypeDef,
+    LiveSourceTypeDef,
+    UpdateLiveSourceResponseTypeDef,
+    UpdateVodSourceResponseTypeDef,
+    VodSourceTypeDef,
+    ResponseOutputItemTypeDef,
     RequestOutputItemTypeDef,
-    ScheduleEntryOutputTypeDef,
+    ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageOutputTypeDef,
     TimeSignalMessageTypeDef,
     UpdateProgramScheduleConfigurationTypeDef,
-    CreateSourceLocationResponseOutputTypeDef,
-    DescribeSourceLocationResponseOutputTypeDef,
-    SourceLocationOutputTypeDef,
-    UpdateSourceLocationResponseOutputTypeDef,
+    CreateSourceLocationResponseTypeDef,
+    DescribeSourceLocationResponseTypeDef,
+    SourceLocationTypeDef,
+    UpdateSourceLocationResponseTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
-    GetPlaybackConfigurationResponseOutputTypeDef,
-    PlaybackConfigurationOutputTypeDef,
-    PutPlaybackConfigurationResponseOutputTypeDef,
+    GetPlaybackConfigurationResponseTypeDef,
+    PlaybackConfigurationTypeDef,
+    PutPlaybackConfigurationResponseTypeDef,
     PutPlaybackConfigurationRequestRequestTypeDef,
-    CreatePrefetchScheduleResponseOutputTypeDef,
-    GetPrefetchScheduleResponseOutputTypeDef,
-    PrefetchScheduleOutputTypeDef,
+    CreatePrefetchScheduleResponseTypeDef,
+    GetPrefetchScheduleResponseTypeDef,
+    PrefetchScheduleTypeDef,
     CreatePrefetchScheduleRequestRequestTypeDef,
-    ListLiveSourcesResponseOutputTypeDef,
-    ListVodSourcesResponseOutputTypeDef,
-    ChannelOutputTypeDef,
-    CreateChannelResponseOutputTypeDef,
-    DescribeChannelResponseOutputTypeDef,
-    UpdateChannelResponseOutputTypeDef,
+    ListLiveSourcesResponseTypeDef,
+    ListVodSourcesResponseTypeDef,
+    ChannelTypeDef,
+    CreateChannelResponseTypeDef,
+    DescribeChannelResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    GetChannelScheduleResponseOutputTypeDef,
+    GetChannelScheduleResponseTypeDef,
     AdBreakOutputTypeDef,
     AdBreakTypeDef,
-    ListSourceLocationsResponseOutputTypeDef,
-    ListPlaybackConfigurationsResponseOutputTypeDef,
-    ListPrefetchSchedulesResponseOutputTypeDef,
-    ListChannelsResponseOutputTypeDef,
-    CreateProgramResponseOutputTypeDef,
-    DescribeProgramResponseOutputTypeDef,
-    UpdateProgramResponseOutputTypeDef,
+    ListSourceLocationsResponseTypeDef,
+    ListPlaybackConfigurationsResponseTypeDef,
+    ListPrefetchSchedulesResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    CreateProgramResponseTypeDef,
+    DescribeProgramResponseTypeDef,
+    UpdateProgramResponseTypeDef,
     CreateProgramRequestRequestTypeDef,
     UpdateProgramRequestRequestTypeDef,
 )
 
 
 def get_structure() -> SecretsManagerAccessTokenConfigurationOutputTypeDef:
     return {...}
```

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/mypy_boto3_mediatailor.egg-info/SOURCES.txt` & `mypy-boto3-mediatailor-1.28.3.post2/mypy_boto3_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.28.3.post1/setup.py` & `mypy-boto3-mediatailor-1.28.3.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediatailor",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MediaTailor 1.28.3 service generated with mypy-boto3-builder"
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

