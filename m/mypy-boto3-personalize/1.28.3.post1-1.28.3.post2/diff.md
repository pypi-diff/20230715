# Comparing `tmp/mypy-boto3-personalize-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-personalize-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:35 2023, max compression
```

## Comparing `mypy-boto3-personalize-1.28.3.post1.tar` & `mypy-boto3-personalize-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.999730 mypy-boto3-personalize-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-14 16:18:02.995730 mypy-boto3-personalize-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23266 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.983729 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52241 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52151 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-14 16:16:54.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66438 2023-07-14 16:16:56.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66405 2023-07-14 16:16:55.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:53.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:02.995730 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 16:18:02.000000 mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:02.999730 mypy-boto3-personalize-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-14 16:16:52.000000 mypy-boto3-personalize-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.238399 mypy-boto3-personalize-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24479 2023-07-15 06:38:35.238399 mypy-boto3-personalize-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22972 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.234399 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51525 2023-07-15 06:37:26.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51435 2023-07-15 06:37:26.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-15 06:37:26.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-15 06:37:26.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-07-15 06:37:26.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-15 06:37:26.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67247 2023-07-15 06:37:29.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67214 2023-07-15 06:37:27.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.238399 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24479 2023-07-15 06:38:35.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-15 06:38:35.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:35.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 06:38:35.000000 mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:35.238399 mypy-boto3-personalize-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-15 06:37:25.000000 mypy-boto3-personalize-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/LICENSE` & `mypy-boto3-personalize-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3.post1/PKG-INFO` & `mypy-boto3-personalize-1.28.3.post2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-personalize
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.7
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 personalize type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,59 +357,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize.type_defs import (
-    AlgorithmImageOutputTypeDef,
+    AlgorithmImageTypeDef,
     AutoMLConfigOutputTypeDef,
     AutoMLConfigTypeDef,
-    AutoMLResultOutputTypeDef,
+    AutoMLResultTypeDef,
+    BatchInferenceJobConfigOutputTypeDef,
     BatchInferenceJobConfigTypeDef,
+    S3DataConfigOutputTypeDef,
     S3DataConfigTypeDef,
-    BatchInferenceJobSummaryOutputTypeDef,
-    BatchSegmentJobSummaryOutputTypeDef,
+    BatchInferenceJobSummaryTypeDef,
+    BatchSegmentJobSummaryTypeDef,
     CampaignConfigOutputTypeDef,
     CampaignConfigTypeDef,
-    CampaignSummaryOutputTypeDef,
+    CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeOutputTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeOutputTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    CreateBatchInferenceJobResponseOutputTypeDef,
-    CreateBatchSegmentJobResponseOutputTypeDef,
-    CreateCampaignResponseOutputTypeDef,
-    CreateDatasetExportJobResponseOutputTypeDef,
-    CreateDatasetGroupResponseOutputTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
     DataSourceTypeDef,
-    CreateDatasetImportJobResponseOutputTypeDef,
-    CreateDatasetResponseOutputTypeDef,
-    CreateEventTrackerResponseOutputTypeDef,
-    CreateFilterResponseOutputTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
     MetricAttributeTypeDef,
-    CreateMetricAttributionResponseOutputTypeDef,
-    CreateRecommenderResponseOutputTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseOutputTypeDef,
-    CreateSolutionResponseOutputTypeDef,
-    CreateSolutionVersionResponseOutputTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DataSourceOutputTypeDef,
-    DatasetExportJobSummaryOutputTypeDef,
-    DatasetGroupOutputTypeDef,
-    DatasetGroupSummaryOutputTypeDef,
-    DatasetImportJobSummaryOutputTypeDef,
-    DatasetUpdateSummaryOutputTypeDef,
-    DatasetSchemaOutputTypeDef,
-    DatasetSchemaSummaryOutputTypeDef,
-    DatasetSummaryOutputTypeDef,
-    DefaultCategoricalHyperParameterRangeOutputTypeDef,
-    DefaultContinuousHyperParameterRangeOutputTypeDef,
-    DefaultIntegerHyperParameterRangeOutputTypeDef,
+    DatasetExportJobSummaryTypeDef,
+    DatasetGroupSummaryTypeDef,
+    DatasetGroupTypeDef,
+    DatasetImportJobSummaryTypeDef,
+    DatasetSchemaSummaryTypeDef,
+    DatasetSchemaTypeDef,
+    DatasetSummaryTypeDef,
+    DatasetUpdateSummaryTypeDef,
+    DefaultCategoricalHyperParameterRangeTypeDef,
+    DefaultContinuousHyperParameterRangeTypeDef,
+    DefaultIntegerHyperParameterRangeTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteMetricAttributionRequestRequestTypeDef,
     DeleteRecommenderRequestRequestTypeDef,
@@ -452,31 +422,31 @@
     DescribeBatchSegmentJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DescribeDatasetExportJobRequestRequestTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeEventTrackerRequestRequestTypeDef,
-    EventTrackerOutputTypeDef,
+    EventTrackerTypeDef,
     DescribeFeatureTransformationRequestRequestTypeDef,
-    FeatureTransformationOutputTypeDef,
+    FeatureTransformationTypeDef,
     DescribeFilterRequestRequestTypeDef,
-    FilterOutputTypeDef,
+    FilterTypeDef,
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
-    RecipeOutputTypeDef,
+    RecipeTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventTrackerSummaryOutputTypeDef,
-    FilterSummaryOutputTypeDef,
+    EventTrackerSummaryTypeDef,
+    FilterSummaryTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
-    GetSolutionMetricsResponseOutputTypeDef,
+    GetSolutionMetricsResponseTypeDef,
     HPOObjectiveOutputTypeDef,
     HPOResourceConfigOutputTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
     IntegerHyperParameterRangeOutputTypeDef,
     IntegerHyperParameterRangeTypeDef,
     ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
@@ -498,128 +468,134 @@
     ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
     MetricAttributeOutputTypeDef,
     ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
-    MetricAttributionSummaryOutputTypeDef,
+    MetricAttributionSummaryTypeDef,
     ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    RecipeSummaryOutputTypeDef,
+    RecipeSummaryTypeDef,
     ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
-    SolutionVersionSummaryOutputTypeDef,
+    SolutionVersionSummaryTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
-    SolutionSummaryOutputTypeDef,
+    SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagOutputTypeDef,
     OptimizationObjectiveOutputTypeDef,
     OptimizationObjectiveTypeDef,
     PaginatorConfigTypeDef,
     TrainingDataConfigOutputTypeDef,
     TrainingDataConfigTypeDef,
     ResponseMetadataTypeDef,
-    TunedHPOParamsOutputTypeDef,
+    TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
-    StartRecommenderResponseOutputTypeDef,
+    StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
-    StopRecommenderResponseOutputTypeDef,
+    StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCampaignResponseOutputTypeDef,
+    UpdateCampaignResponseTypeDef,
     UpdateDatasetRequestRequestTypeDef,
-    UpdateDatasetResponseOutputTypeDef,
-    UpdateMetricAttributionResponseOutputTypeDef,
-    UpdateRecommenderResponseOutputTypeDef,
+    UpdateDatasetResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
+    BatchInferenceJobInputOutputTypeDef,
+    BatchSegmentJobInputOutputTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    CampaignUpdateSummaryOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    CampaignUpdateSummaryTypeDef,
     UpdateCampaignRequestRequestTypeDef,
-    ListCampaignsResponseOutputTypeDef,
+    ListCampaignsResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
-    DatasetImportJobOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    DescribeDatasetGroupResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    DatasetOutputTypeDef,
-    DescribeSchemaResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    DefaultHyperParameterRangesOutputTypeDef,
-    DescribeEventTrackerResponseOutputTypeDef,
-    DescribeFeatureTransformationResponseOutputTypeDef,
-    DescribeFilterResponseOutputTypeDef,
-    DescribeRecipeResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
+    DatasetImportJobTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    DatasetTypeDef,
+    DefaultHyperParameterRangesTypeDef,
+    DescribeEventTrackerResponseTypeDef,
+    DescribeFeatureTransformationResponseTypeDef,
+    DescribeFilterResponseTypeDef,
+    DescribeRecipeResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
     HyperParameterRangesOutputTypeDef,
     HyperParameterRangesTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RecommenderConfigOutputTypeDef,
     RecommenderConfigTypeDef,
+    BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
-    DescribeBatchInferenceJobResponseOutputTypeDef,
+    BatchSegmentJobTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
-    DescribeBatchSegmentJobResponseOutputTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
-    DescribeDatasetExportJobResponseOutputTypeDef,
+    DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
-    DescribeMetricAttributionResponseOutputTypeDef,
+    MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
-    CampaignOutputTypeDef,
-    DescribeDatasetImportJobResponseOutputTypeDef,
-    DescribeDatasetResponseOutputTypeDef,
-    AlgorithmOutputTypeDef,
+    CampaignTypeDef,
+    DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
+    AlgorithmTypeDef,
     HPOConfigOutputTypeDef,
     HPOConfigTypeDef,
-    RecommenderSummaryOutputTypeDef,
-    RecommenderUpdateSummaryOutputTypeDef,
+    RecommenderSummaryTypeDef,
+    RecommenderUpdateSummaryTypeDef,
     CreateRecommenderRequestRequestTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
-    DescribeCampaignResponseOutputTypeDef,
-    DescribeAlgorithmResponseOutputTypeDef,
+    DescribeBatchInferenceJobResponseTypeDef,
+    DescribeBatchSegmentJobResponseTypeDef,
+    DescribeDatasetExportJobResponseTypeDef,
+    DescribeMetricAttributionResponseTypeDef,
+    DescribeCampaignResponseTypeDef,
+    DescribeAlgorithmResponseTypeDef,
     SolutionConfigOutputTypeDef,
     SolutionConfigTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    RecommenderOutputTypeDef,
-    SolutionOutputTypeDef,
-    SolutionVersionOutputTypeDef,
+    ListRecommendersResponseTypeDef,
+    RecommenderTypeDef,
+    SolutionTypeDef,
+    SolutionVersionTypeDef,
     CreateSolutionRequestRequestTypeDef,
-    DescribeRecommenderResponseOutputTypeDef,
-    DescribeSolutionResponseOutputTypeDef,
-    DescribeSolutionVersionResponseOutputTypeDef,
+    DescribeRecommenderResponseTypeDef,
+    DescribeSolutionResponseTypeDef,
+    DescribeSolutionVersionResponseTypeDef,
 )
 
 
-def get_structure() -> AlgorithmImageOutputTypeDef:
+def get_structure() -> AlgorithmImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/README.md` & `mypy-boto3-personalize-1.28.3.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-personalize
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 personalize type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,59 +389,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize.type_defs import (
-    AlgorithmImageOutputTypeDef,
+    AlgorithmImageTypeDef,
     AutoMLConfigOutputTypeDef,
     AutoMLConfigTypeDef,
-    AutoMLResultOutputTypeDef,
+    AutoMLResultTypeDef,
+    BatchInferenceJobConfigOutputTypeDef,
     BatchInferenceJobConfigTypeDef,
+    S3DataConfigOutputTypeDef,
     S3DataConfigTypeDef,
-    BatchInferenceJobSummaryOutputTypeDef,
-    BatchSegmentJobSummaryOutputTypeDef,
+    BatchInferenceJobSummaryTypeDef,
+    BatchSegmentJobSummaryTypeDef,
     CampaignConfigOutputTypeDef,
     CampaignConfigTypeDef,
-    CampaignSummaryOutputTypeDef,
+    CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeOutputTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeOutputTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    CreateBatchInferenceJobResponseOutputTypeDef,
-    CreateBatchSegmentJobResponseOutputTypeDef,
-    CreateCampaignResponseOutputTypeDef,
-    CreateDatasetExportJobResponseOutputTypeDef,
-    CreateDatasetGroupResponseOutputTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
     DataSourceTypeDef,
-    CreateDatasetImportJobResponseOutputTypeDef,
-    CreateDatasetResponseOutputTypeDef,
-    CreateEventTrackerResponseOutputTypeDef,
-    CreateFilterResponseOutputTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
     MetricAttributeTypeDef,
-    CreateMetricAttributionResponseOutputTypeDef,
-    CreateRecommenderResponseOutputTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseOutputTypeDef,
-    CreateSolutionResponseOutputTypeDef,
-    CreateSolutionVersionResponseOutputTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DataSourceOutputTypeDef,
-    DatasetExportJobSummaryOutputTypeDef,
-    DatasetGroupOutputTypeDef,
-    DatasetGroupSummaryOutputTypeDef,
-    DatasetImportJobSummaryOutputTypeDef,
-    DatasetUpdateSummaryOutputTypeDef,
-    DatasetSchemaOutputTypeDef,
-    DatasetSchemaSummaryOutputTypeDef,
-    DatasetSummaryOutputTypeDef,
-    DefaultCategoricalHyperParameterRangeOutputTypeDef,
-    DefaultContinuousHyperParameterRangeOutputTypeDef,
-    DefaultIntegerHyperParameterRangeOutputTypeDef,
+    DatasetExportJobSummaryTypeDef,
+    DatasetGroupSummaryTypeDef,
+    DatasetGroupTypeDef,
+    DatasetImportJobSummaryTypeDef,
+    DatasetSchemaSummaryTypeDef,
+    DatasetSchemaTypeDef,
+    DatasetSummaryTypeDef,
+    DatasetUpdateSummaryTypeDef,
+    DefaultCategoricalHyperParameterRangeTypeDef,
+    DefaultContinuousHyperParameterRangeTypeDef,
+    DefaultIntegerHyperParameterRangeTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteMetricAttributionRequestRequestTypeDef,
     DeleteRecommenderRequestRequestTypeDef,
@@ -420,31 +454,31 @@
     DescribeBatchSegmentJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DescribeDatasetExportJobRequestRequestTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeEventTrackerRequestRequestTypeDef,
-    EventTrackerOutputTypeDef,
+    EventTrackerTypeDef,
     DescribeFeatureTransformationRequestRequestTypeDef,
-    FeatureTransformationOutputTypeDef,
+    FeatureTransformationTypeDef,
     DescribeFilterRequestRequestTypeDef,
-    FilterOutputTypeDef,
+    FilterTypeDef,
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
-    RecipeOutputTypeDef,
+    RecipeTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventTrackerSummaryOutputTypeDef,
-    FilterSummaryOutputTypeDef,
+    EventTrackerSummaryTypeDef,
+    FilterSummaryTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
-    GetSolutionMetricsResponseOutputTypeDef,
+    GetSolutionMetricsResponseTypeDef,
     HPOObjectiveOutputTypeDef,
     HPOResourceConfigOutputTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
     IntegerHyperParameterRangeOutputTypeDef,
     IntegerHyperParameterRangeTypeDef,
     ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
@@ -466,128 +500,134 @@
     ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
     MetricAttributeOutputTypeDef,
     ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
-    MetricAttributionSummaryOutputTypeDef,
+    MetricAttributionSummaryTypeDef,
     ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    RecipeSummaryOutputTypeDef,
+    RecipeSummaryTypeDef,
     ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
-    SolutionVersionSummaryOutputTypeDef,
+    SolutionVersionSummaryTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
-    SolutionSummaryOutputTypeDef,
+    SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagOutputTypeDef,
     OptimizationObjectiveOutputTypeDef,
     OptimizationObjectiveTypeDef,
     PaginatorConfigTypeDef,
     TrainingDataConfigOutputTypeDef,
     TrainingDataConfigTypeDef,
     ResponseMetadataTypeDef,
-    TunedHPOParamsOutputTypeDef,
+    TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
-    StartRecommenderResponseOutputTypeDef,
+    StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
-    StopRecommenderResponseOutputTypeDef,
+    StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCampaignResponseOutputTypeDef,
+    UpdateCampaignResponseTypeDef,
     UpdateDatasetRequestRequestTypeDef,
-    UpdateDatasetResponseOutputTypeDef,
-    UpdateMetricAttributionResponseOutputTypeDef,
-    UpdateRecommenderResponseOutputTypeDef,
+    UpdateDatasetResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
+    BatchInferenceJobInputOutputTypeDef,
+    BatchSegmentJobInputOutputTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    CampaignUpdateSummaryOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    CampaignUpdateSummaryTypeDef,
     UpdateCampaignRequestRequestTypeDef,
-    ListCampaignsResponseOutputTypeDef,
+    ListCampaignsResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
-    DatasetImportJobOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    DescribeDatasetGroupResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    DatasetOutputTypeDef,
-    DescribeSchemaResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    DefaultHyperParameterRangesOutputTypeDef,
-    DescribeEventTrackerResponseOutputTypeDef,
-    DescribeFeatureTransformationResponseOutputTypeDef,
-    DescribeFilterResponseOutputTypeDef,
-    DescribeRecipeResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
+    DatasetImportJobTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    DatasetTypeDef,
+    DefaultHyperParameterRangesTypeDef,
+    DescribeEventTrackerResponseTypeDef,
+    DescribeFeatureTransformationResponseTypeDef,
+    DescribeFilterResponseTypeDef,
+    DescribeRecipeResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
     HyperParameterRangesOutputTypeDef,
     HyperParameterRangesTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RecommenderConfigOutputTypeDef,
     RecommenderConfigTypeDef,
+    BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
-    DescribeBatchInferenceJobResponseOutputTypeDef,
+    BatchSegmentJobTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
-    DescribeBatchSegmentJobResponseOutputTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
-    DescribeDatasetExportJobResponseOutputTypeDef,
+    DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
-    DescribeMetricAttributionResponseOutputTypeDef,
+    MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
-    CampaignOutputTypeDef,
-    DescribeDatasetImportJobResponseOutputTypeDef,
-    DescribeDatasetResponseOutputTypeDef,
-    AlgorithmOutputTypeDef,
+    CampaignTypeDef,
+    DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
+    AlgorithmTypeDef,
     HPOConfigOutputTypeDef,
     HPOConfigTypeDef,
-    RecommenderSummaryOutputTypeDef,
-    RecommenderUpdateSummaryOutputTypeDef,
+    RecommenderSummaryTypeDef,
+    RecommenderUpdateSummaryTypeDef,
     CreateRecommenderRequestRequestTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
-    DescribeCampaignResponseOutputTypeDef,
-    DescribeAlgorithmResponseOutputTypeDef,
+    DescribeBatchInferenceJobResponseTypeDef,
+    DescribeBatchSegmentJobResponseTypeDef,
+    DescribeDatasetExportJobResponseTypeDef,
+    DescribeMetricAttributionResponseTypeDef,
+    DescribeCampaignResponseTypeDef,
+    DescribeAlgorithmResponseTypeDef,
     SolutionConfigOutputTypeDef,
     SolutionConfigTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    RecommenderOutputTypeDef,
-    SolutionOutputTypeDef,
-    SolutionVersionOutputTypeDef,
+    ListRecommendersResponseTypeDef,
+    RecommenderTypeDef,
+    SolutionTypeDef,
+    SolutionVersionTypeDef,
     CreateSolutionRequestRequestTypeDef,
-    DescribeRecommenderResponseOutputTypeDef,
-    DescribeSolutionResponseOutputTypeDef,
-    DescribeSolutionVersionResponseOutputTypeDef,
+    DescribeRecommenderResponseTypeDef,
+    DescribeSolutionResponseTypeDef,
+    DescribeSolutionVersionResponseTypeDef,
 )
 
 
-def get_structure() -> AlgorithmImageOutputTypeDef:
+def get_structure() -> AlgorithmImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.py` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__init__.pyi` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/__main__.py` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.28.3\nVersion:         1.28.3.post1\nBuilder"
-        " version: 7.14.7\nDocs:           "
+        "Type annotations for boto3.Personalize 1.28.3\nVersion:         1.28.3.post2\nBuilder"
+        " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
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

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.py` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,77 +40,77 @@
 from .type_defs import (
     BatchInferenceJobConfigTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     CampaignConfigTypeDef,
-    CreateBatchInferenceJobResponseOutputTypeDef,
-    CreateBatchSegmentJobResponseOutputTypeDef,
-    CreateCampaignResponseOutputTypeDef,
-    CreateDatasetExportJobResponseOutputTypeDef,
-    CreateDatasetGroupResponseOutputTypeDef,
-    CreateDatasetImportJobResponseOutputTypeDef,
-    CreateDatasetResponseOutputTypeDef,
-    CreateEventTrackerResponseOutputTypeDef,
-    CreateFilterResponseOutputTypeDef,
-    CreateMetricAttributionResponseOutputTypeDef,
-    CreateRecommenderResponseOutputTypeDef,
-    CreateSchemaResponseOutputTypeDef,
-    CreateSolutionResponseOutputTypeDef,
-    CreateSolutionVersionResponseOutputTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DatasetExportJobOutputTypeDef,
     DataSourceTypeDef,
-    DescribeAlgorithmResponseOutputTypeDef,
-    DescribeBatchInferenceJobResponseOutputTypeDef,
-    DescribeBatchSegmentJobResponseOutputTypeDef,
-    DescribeCampaignResponseOutputTypeDef,
-    DescribeDatasetExportJobResponseOutputTypeDef,
-    DescribeDatasetGroupResponseOutputTypeDef,
-    DescribeDatasetImportJobResponseOutputTypeDef,
-    DescribeDatasetResponseOutputTypeDef,
-    DescribeEventTrackerResponseOutputTypeDef,
-    DescribeFeatureTransformationResponseOutputTypeDef,
-    DescribeFilterResponseOutputTypeDef,
-    DescribeMetricAttributionResponseOutputTypeDef,
-    DescribeRecipeResponseOutputTypeDef,
-    DescribeRecommenderResponseOutputTypeDef,
-    DescribeSchemaResponseOutputTypeDef,
-    DescribeSolutionResponseOutputTypeDef,
-    DescribeSolutionVersionResponseOutputTypeDef,
+    DescribeAlgorithmResponseTypeDef,
+    DescribeBatchInferenceJobResponseTypeDef,
+    DescribeBatchSegmentJobResponseTypeDef,
+    DescribeCampaignResponseTypeDef,
+    DescribeDatasetExportJobResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
+    DescribeEventTrackerResponseTypeDef,
+    DescribeFeatureTransformationResponseTypeDef,
+    DescribeFilterResponseTypeDef,
+    DescribeMetricAttributionResponseTypeDef,
+    DescribeRecipeResponseTypeDef,
+    DescribeRecommenderResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    DescribeSolutionResponseTypeDef,
+    DescribeSolutionVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseOutputTypeDef,
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    ListCampaignsResponseOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    GetSolutionMetricsResponseTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    ListCampaignsResponseTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListRecommendersResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
     RecommenderConfigTypeDef,
     SolutionConfigTypeDef,
-    StartRecommenderResponseOutputTypeDef,
-    StopRecommenderResponseOutputTypeDef,
+    StartRecommenderResponseTypeDef,
+    StopRecommenderResponseTypeDef,
     TagTypeDef,
-    UpdateCampaignResponseOutputTypeDef,
-    UpdateDatasetResponseOutputTypeDef,
-    UpdateMetricAttributionResponseOutputTypeDef,
-    UpdateRecommenderResponseOutputTypeDef,
+    UpdateCampaignResponseTypeDef,
+    UpdateDatasetResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -179,15 +179,15 @@
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchInferenceJobResponseOutputTypeDef:
+    ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Creates a batch inference job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_inference_job)
         """
 
@@ -198,15 +198,15 @@
         solutionVersionArn: str,
         jobInput: BatchSegmentJobInputTypeDef,
         jobOutput: BatchSegmentJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchSegmentJobResponseOutputTypeDef:
+    ) -> CreateBatchSegmentJobResponseTypeDef:
         """
         Creates a batch segment job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_segment_job)
         """
 
@@ -214,15 +214,15 @@
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateCampaignResponseOutputTypeDef:
+    ) -> CreateCampaignResponseTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
 
@@ -230,15 +230,15 @@
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetResponseOutputTypeDef:
+    ) -> CreateDatasetResponseTypeDef:
         """
         Creates an empty dataset and adds it to the specified dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset)
         """
 
@@ -247,15 +247,15 @@
         *,
         jobName: str,
         datasetArn: str,
         roleArn: str,
         jobOutput: DatasetExportJobOutputTypeDef,
         ingestionMode: IngestionModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetExportJobResponseOutputTypeDef:
+    ) -> CreateDatasetExportJobResponseTypeDef:
         """
         Creates a job that exports data from your dataset to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_export_job)
         """
 
@@ -263,15 +263,15 @@
         self,
         *,
         name: str,
         roleArn: str = ...,
         kmsKeyArn: str = ...,
         domain: DomainType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetGroupResponseOutputTypeDef:
+    ) -> CreateDatasetGroupResponseTypeDef:
         """
         Creates an empty dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_group)
         """
 
@@ -281,26 +281,26 @@
         jobName: str,
         datasetArn: str,
         dataSource: DataSourceTypeDef,
         roleArn: str,
         tags: Sequence[TagTypeDef] = ...,
         importMode: ImportModeType = ...,
         publishAttributionMetricsToS3: bool = ...
-    ) -> CreateDatasetImportJobResponseOutputTypeDef:
+    ) -> CreateDatasetImportJobResponseTypeDef:
         """
         Creates a job that imports training data from your data source (an Amazon S3
         bucket) to an Amazon Personalize dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_import_job)
         """
 
     def create_event_tracker(
         self, *, name: str, datasetGroupArn: str, tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventTrackerResponseOutputTypeDef:
+    ) -> CreateEventTrackerResponseTypeDef:
         """
         Creates an event tracker that you use when adding event data to a specified
         dataset group using the
         [PutEvents](https://docs.aws.amazon.com/personalize/latest/dg/API_UBS_PutEvents.html)_
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_event_tracker)
@@ -310,30 +310,30 @@
     def create_filter(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         filterExpression: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateFilterResponseOutputTypeDef:
+    ) -> CreateFilterResponseTypeDef:
         """
         Creates a recommendation filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_filter)
         """
 
     def create_metric_attribution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         metrics: Sequence[MetricAttributeTypeDef],
         metricsOutputConfig: MetricAttributionOutputTypeDef
-    ) -> CreateMetricAttributionResponseOutputTypeDef:
+    ) -> CreateMetricAttributionResponseTypeDef:
         """
         Creates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_metric_attribution)
         """
 
@@ -341,26 +341,26 @@
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
         recommenderConfig: RecommenderConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRecommenderResponseOutputTypeDef:
+    ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_recommender)
         """
 
     def create_schema(
         self, *, name: str, schema: str, domain: DomainType = ...
-    ) -> CreateSchemaResponseOutputTypeDef:
+    ) -> CreateSchemaResponseTypeDef:
         """
         Creates an Amazon Personalize schema from the specified schema string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_schema)
         """
 
@@ -371,30 +371,30 @@
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionResponseOutputTypeDef:
+    ) -> CreateSolutionResponseTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
         """
 
     def create_solution_version(
         self,
         *,
         solutionArn: str,
         name: str = ...,
         trainingMode: TrainingModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionVersionResponseOutputTypeDef:
+    ) -> CreateSolutionVersionResponseTypeDef:
         """
         Trains or retrains an active solution in a Custom dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution_version)
         """
 
@@ -468,171 +468,169 @@
         """
         Deletes all versions of a solution and the `Solution` object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#delete_solution)
         """
 
-    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseOutputTypeDef:
+    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseTypeDef:
         """
         Describes the given algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_algorithm)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_algorithm)
         """
 
     def describe_batch_inference_job(
         self, *, batchInferenceJobArn: str
-    ) -> DescribeBatchInferenceJobResponseOutputTypeDef:
+    ) -> DescribeBatchInferenceJobResponseTypeDef:
         """
         Gets the properties of a batch inference job including name, Amazon Resource
         Name (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate the recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_inference_job)
         """
 
     def describe_batch_segment_job(
         self, *, batchSegmentJobArn: str
-    ) -> DescribeBatchSegmentJobResponseOutputTypeDef:
+    ) -> DescribeBatchSegmentJobResponseTypeDef:
         """
         Gets the properties of a batch segment job including name, Amazon Resource Name
         (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate segments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_segment_job)
         """
 
-    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseOutputTypeDef:
+    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseTypeDef:
         """
         Describes the given campaign, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_campaign)
         """
 
-    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseOutputTypeDef:
+    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Describes the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset)
         """
 
     def describe_dataset_export_job(
         self, *, datasetExportJobArn: str
-    ) -> DescribeDatasetExportJobResponseOutputTypeDef:
+    ) -> DescribeDatasetExportJobResponseTypeDef:
         """
         Describes the dataset export job created by
         [CreateDatasetExportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetExportJob.html)_,
         including the export job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_export_job)
         """
 
     def describe_dataset_group(
         self, *, datasetGroupArn: str
-    ) -> DescribeDatasetGroupResponseOutputTypeDef:
+    ) -> DescribeDatasetGroupResponseTypeDef:
         """
         Describes the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_group)
         """
 
     def describe_dataset_import_job(
         self, *, datasetImportJobArn: str
-    ) -> DescribeDatasetImportJobResponseOutputTypeDef:
+    ) -> DescribeDatasetImportJobResponseTypeDef:
         """
         Describes the dataset import job created by
         [CreateDatasetImportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetImportJob.html)_,
         including the import job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_import_job)
         """
 
     def describe_event_tracker(
         self, *, eventTrackerArn: str
-    ) -> DescribeEventTrackerResponseOutputTypeDef:
+    ) -> DescribeEventTrackerResponseTypeDef:
         """
         Describes an event tracker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_event_tracker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_event_tracker)
         """
 
     def describe_feature_transformation(
         self, *, featureTransformationArn: str
-    ) -> DescribeFeatureTransformationResponseOutputTypeDef:
+    ) -> DescribeFeatureTransformationResponseTypeDef:
         """
         Describes the given feature transformation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_feature_transformation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_feature_transformation)
         """
 
-    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseOutputTypeDef:
+    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseTypeDef:
         """
         Describes a filter's properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_filter)
         """
 
     def describe_metric_attribution(
         self, *, metricAttributionArn: str
-    ) -> DescribeMetricAttributionResponseOutputTypeDef:
+    ) -> DescribeMetricAttributionResponseTypeDef:
         """
         Describes a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_metric_attribution)
         """
 
-    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseOutputTypeDef:
+    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseTypeDef:
         """
         Describes a recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recipe)
         """
 
-    def describe_recommender(
-        self, *, recommenderArn: str
-    ) -> DescribeRecommenderResponseOutputTypeDef:
+    def describe_recommender(self, *, recommenderArn: str) -> DescribeRecommenderResponseTypeDef:
         """
         Describes the given recommender, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recommender)
         """
 
-    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseOutputTypeDef:
+    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseTypeDef:
         """
         Describes a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_schema)
         """
 
-    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseOutputTypeDef:
+    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseTypeDef:
         """
         Describes a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution)
         """
 
     def describe_solution_version(
         self, *, solutionVersionArn: str
-    ) -> DescribeSolutionVersionResponseOutputTypeDef:
+    ) -> DescribeSolutionVersionResponseTypeDef:
         """
         Describes a specific version of a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution_version)
         """
 
@@ -646,211 +644,207 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#generate_presigned_url)
         """
 
-    def get_solution_metrics(
-        self, *, solutionVersionArn: str
-    ) -> GetSolutionMetricsResponseOutputTypeDef:
+    def get_solution_metrics(self, *, solutionVersionArn: str) -> GetSolutionMetricsResponseTypeDef:
         """
         Gets the metrics for the specified solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.get_solution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#get_solution_metrics)
         """
 
     def list_batch_inference_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchInferenceJobsResponseOutputTypeDef:
+    ) -> ListBatchInferenceJobsResponseTypeDef:
         """
         Gets a list of the batch inference jobs that have been performed off of a
         solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_inference_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_inference_jobs)
         """
 
     def list_batch_segment_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchSegmentJobsResponseOutputTypeDef:
+    ) -> ListBatchSegmentJobsResponseTypeDef:
         """
         Gets a list of the batch segment jobs that have been performed off of a solution
         version that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_segment_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_segment_jobs)
         """
 
     def list_campaigns(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListCampaignsResponseOutputTypeDef:
+    ) -> ListCampaignsResponseTypeDef:
         """
         Returns a list of campaigns that use the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_campaigns)
         """
 
     def list_dataset_export_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetExportJobsResponseOutputTypeDef:
+    ) -> ListDatasetExportJobsResponseTypeDef:
         """
         Returns a list of dataset export jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_export_jobs)
         """
 
     def list_dataset_groups(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetGroupsResponseOutputTypeDef:
+    ) -> ListDatasetGroupsResponseTypeDef:
         """
         Returns a list of dataset groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_groups)
         """
 
     def list_dataset_import_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetImportJobsResponseOutputTypeDef:
+    ) -> ListDatasetImportJobsResponseTypeDef:
         """
         Returns a list of dataset import jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_import_jobs)
         """
 
     def list_datasets(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetsResponseOutputTypeDef:
+    ) -> ListDatasetsResponseTypeDef:
         """
         Returns the list of datasets contained in the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_datasets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_datasets)
         """
 
     def list_event_trackers(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListEventTrackersResponseOutputTypeDef:
+    ) -> ListEventTrackersResponseTypeDef:
         """
         Returns the list of event trackers associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_event_trackers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_event_trackers)
         """
 
     def list_filters(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListFiltersResponseOutputTypeDef:
+    ) -> ListFiltersResponseTypeDef:
         """
         Lists all filters that belong to a given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_filters)
         """
 
     def list_metric_attribution_metrics(
         self, *, metricAttributionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionMetricsResponseOutputTypeDef:
+    ) -> ListMetricAttributionMetricsResponseTypeDef:
         """
         Lists the metrics for the metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attribution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attribution_metrics)
         """
 
     def list_metric_attributions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionsResponseOutputTypeDef:
+    ) -> ListMetricAttributionsResponseTypeDef:
         """
         Lists metric attributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attributions)
         """
 
     def list_recipes(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         domain: DomainType = ...
-    ) -> ListRecipesResponseOutputTypeDef:
+    ) -> ListRecipesResponseTypeDef:
         """
         Returns a list of available recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recipes)
         """
 
     def list_recommenders(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListRecommendersResponseOutputTypeDef:
+    ) -> ListRecommendersResponseTypeDef:
         """
         Returns a list of recommenders in a given Domain dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recommenders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recommenders)
         """
 
     def list_schemas(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListSchemasResponseOutputTypeDef:
+    ) -> ListSchemasResponseTypeDef:
         """
         Returns the list of schemas associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_schemas)
         """
 
     def list_solution_versions(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionVersionsResponseOutputTypeDef:
+    ) -> ListSolutionVersionsResponseTypeDef:
         """
         Returns a list of solution versions for the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solution_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solution_versions)
         """
 
     def list_solutions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionsResponseOutputTypeDef:
+    ) -> ListSolutionsResponseTypeDef:
         """
         Returns a list of solutions that use the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
 
-    def list_tags_for_resource(
-        self, *, resourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_tags_for_resource)
         """
 
-    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseOutputTypeDef:
+    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseTypeDef:
         """
         Starts a recommender that is INACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.start_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#start_recommender)
         """
 
-    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseOutputTypeDef:
+    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseTypeDef:
         """
         Stops a recommender that is ACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#stop_recommender)
         """
 
@@ -885,51 +879,49 @@
     def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...
-    ) -> UpdateCampaignResponseOutputTypeDef:
+    ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
 
-    def update_dataset(
-        self, *, datasetArn: str, schemaArn: str
-    ) -> UpdateDatasetResponseOutputTypeDef:
+    def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
         """
         Update a dataset to replace its schema with a new or existing one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_dataset)
         """
 
     def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
-    ) -> UpdateMetricAttributionResponseOutputTypeDef:
+    ) -> UpdateMetricAttributionResponseTypeDef:
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_metric_attribution)
         """
 
     def update_recommender(
         self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
-    ) -> UpdateRecommenderResponseOutputTypeDef:
+    ) -> UpdateRecommenderResponseTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_recommender)
         """
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/client.pyi` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -40,77 +40,77 @@
 from .type_defs import (
     BatchInferenceJobConfigTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     CampaignConfigTypeDef,
-    CreateBatchInferenceJobResponseOutputTypeDef,
-    CreateBatchSegmentJobResponseOutputTypeDef,
-    CreateCampaignResponseOutputTypeDef,
-    CreateDatasetExportJobResponseOutputTypeDef,
-    CreateDatasetGroupResponseOutputTypeDef,
-    CreateDatasetImportJobResponseOutputTypeDef,
-    CreateDatasetResponseOutputTypeDef,
-    CreateEventTrackerResponseOutputTypeDef,
-    CreateFilterResponseOutputTypeDef,
-    CreateMetricAttributionResponseOutputTypeDef,
-    CreateRecommenderResponseOutputTypeDef,
-    CreateSchemaResponseOutputTypeDef,
-    CreateSolutionResponseOutputTypeDef,
-    CreateSolutionVersionResponseOutputTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DatasetExportJobOutputTypeDef,
     DataSourceTypeDef,
-    DescribeAlgorithmResponseOutputTypeDef,
-    DescribeBatchInferenceJobResponseOutputTypeDef,
-    DescribeBatchSegmentJobResponseOutputTypeDef,
-    DescribeCampaignResponseOutputTypeDef,
-    DescribeDatasetExportJobResponseOutputTypeDef,
-    DescribeDatasetGroupResponseOutputTypeDef,
-    DescribeDatasetImportJobResponseOutputTypeDef,
-    DescribeDatasetResponseOutputTypeDef,
-    DescribeEventTrackerResponseOutputTypeDef,
-    DescribeFeatureTransformationResponseOutputTypeDef,
-    DescribeFilterResponseOutputTypeDef,
-    DescribeMetricAttributionResponseOutputTypeDef,
-    DescribeRecipeResponseOutputTypeDef,
-    DescribeRecommenderResponseOutputTypeDef,
-    DescribeSchemaResponseOutputTypeDef,
-    DescribeSolutionResponseOutputTypeDef,
-    DescribeSolutionVersionResponseOutputTypeDef,
+    DescribeAlgorithmResponseTypeDef,
+    DescribeBatchInferenceJobResponseTypeDef,
+    DescribeBatchSegmentJobResponseTypeDef,
+    DescribeCampaignResponseTypeDef,
+    DescribeDatasetExportJobResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
+    DescribeEventTrackerResponseTypeDef,
+    DescribeFeatureTransformationResponseTypeDef,
+    DescribeFilterResponseTypeDef,
+    DescribeMetricAttributionResponseTypeDef,
+    DescribeRecipeResponseTypeDef,
+    DescribeRecommenderResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    DescribeSolutionResponseTypeDef,
+    DescribeSolutionVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetSolutionMetricsResponseOutputTypeDef,
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    ListCampaignsResponseOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    GetSolutionMetricsResponseTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    ListCampaignsResponseTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListRecommendersResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
     RecommenderConfigTypeDef,
     SolutionConfigTypeDef,
-    StartRecommenderResponseOutputTypeDef,
-    StopRecommenderResponseOutputTypeDef,
+    StartRecommenderResponseTypeDef,
+    StopRecommenderResponseTypeDef,
     TagTypeDef,
-    UpdateCampaignResponseOutputTypeDef,
-    UpdateDatasetResponseOutputTypeDef,
-    UpdateMetricAttributionResponseOutputTypeDef,
-    UpdateRecommenderResponseOutputTypeDef,
+    UpdateCampaignResponseTypeDef,
+    UpdateDatasetResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -172,15 +172,15 @@
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchInferenceJobResponseOutputTypeDef:
+    ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Creates a batch inference job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_inference_job)
         """
     def create_batch_segment_job(
@@ -190,45 +190,45 @@
         solutionVersionArn: str,
         jobInput: BatchSegmentJobInputTypeDef,
         jobOutput: BatchSegmentJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateBatchSegmentJobResponseOutputTypeDef:
+    ) -> CreateBatchSegmentJobResponseTypeDef:
         """
         Creates a batch segment job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_batch_segment_job)
         """
     def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateCampaignResponseOutputTypeDef:
+    ) -> CreateCampaignResponseTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
     def create_dataset(
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetResponseOutputTypeDef:
+    ) -> CreateDatasetResponseTypeDef:
         """
         Creates an empty dataset and adds it to the specified dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset)
         """
     def create_dataset_export_job(
@@ -236,30 +236,30 @@
         *,
         jobName: str,
         datasetArn: str,
         roleArn: str,
         jobOutput: DatasetExportJobOutputTypeDef,
         ingestionMode: IngestionModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetExportJobResponseOutputTypeDef:
+    ) -> CreateDatasetExportJobResponseTypeDef:
         """
         Creates a job that exports data from your dataset to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_export_job)
         """
     def create_dataset_group(
         self,
         *,
         name: str,
         roleArn: str = ...,
         kmsKeyArn: str = ...,
         domain: DomainType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDatasetGroupResponseOutputTypeDef:
+    ) -> CreateDatasetGroupResponseTypeDef:
         """
         Creates an empty dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_group)
         """
     def create_dataset_import_job(
@@ -268,25 +268,25 @@
         jobName: str,
         datasetArn: str,
         dataSource: DataSourceTypeDef,
         roleArn: str,
         tags: Sequence[TagTypeDef] = ...,
         importMode: ImportModeType = ...,
         publishAttributionMetricsToS3: bool = ...
-    ) -> CreateDatasetImportJobResponseOutputTypeDef:
+    ) -> CreateDatasetImportJobResponseTypeDef:
         """
         Creates a job that imports training data from your data source (an Amazon S3
         bucket) to an Amazon Personalize dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_dataset_import_job)
         """
     def create_event_tracker(
         self, *, name: str, datasetGroupArn: str, tags: Sequence[TagTypeDef] = ...
-    ) -> CreateEventTrackerResponseOutputTypeDef:
+    ) -> CreateEventTrackerResponseTypeDef:
         """
         Creates an event tracker that you use when adding event data to a specified
         dataset group using the
         [PutEvents](https://docs.aws.amazon.com/personalize/latest/dg/API_UBS_PutEvents.html)_
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_event_tracker)
@@ -295,54 +295,54 @@
     def create_filter(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         filterExpression: str,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateFilterResponseOutputTypeDef:
+    ) -> CreateFilterResponseTypeDef:
         """
         Creates a recommendation filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_filter)
         """
     def create_metric_attribution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         metrics: Sequence[MetricAttributeTypeDef],
         metricsOutputConfig: MetricAttributionOutputTypeDef
-    ) -> CreateMetricAttributionResponseOutputTypeDef:
+    ) -> CreateMetricAttributionResponseTypeDef:
         """
         Creates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_metric_attribution)
         """
     def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
         recommenderConfig: RecommenderConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRecommenderResponseOutputTypeDef:
+    ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_recommender)
         """
     def create_schema(
         self, *, name: str, schema: str, domain: DomainType = ...
-    ) -> CreateSchemaResponseOutputTypeDef:
+    ) -> CreateSchemaResponseTypeDef:
         """
         Creates an Amazon Personalize schema from the specified schema string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_schema)
         """
     def create_solution(
@@ -352,29 +352,29 @@
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionResponseOutputTypeDef:
+    ) -> CreateSolutionResponseTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
         """
     def create_solution_version(
         self,
         *,
         solutionArn: str,
         name: str = ...,
         trainingMode: TrainingModeType = ...,
         tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSolutionVersionResponseOutputTypeDef:
+    ) -> CreateSolutionVersionResponseTypeDef:
         """
         Trains or retrains an active solution in a Custom dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution_version)
         """
     def delete_campaign(self, *, campaignArn: str) -> EmptyResponseMetadataTypeDef:
@@ -438,155 +438,153 @@
     def delete_solution(self, *, solutionArn: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes all versions of a solution and the `Solution` object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#delete_solution)
         """
-    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseOutputTypeDef:
+    def describe_algorithm(self, *, algorithmArn: str) -> DescribeAlgorithmResponseTypeDef:
         """
         Describes the given algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_algorithm)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_algorithm)
         """
     def describe_batch_inference_job(
         self, *, batchInferenceJobArn: str
-    ) -> DescribeBatchInferenceJobResponseOutputTypeDef:
+    ) -> DescribeBatchInferenceJobResponseTypeDef:
         """
         Gets the properties of a batch inference job including name, Amazon Resource
         Name (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate the recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_inference_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_inference_job)
         """
     def describe_batch_segment_job(
         self, *, batchSegmentJobArn: str
-    ) -> DescribeBatchSegmentJobResponseOutputTypeDef:
+    ) -> DescribeBatchSegmentJobResponseTypeDef:
         """
         Gets the properties of a batch segment job including name, Amazon Resource Name
         (ARN), status, input and output configurations, and the ARN of the solution
         version used to generate segments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_segment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_batch_segment_job)
         """
-    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseOutputTypeDef:
+    def describe_campaign(self, *, campaignArn: str) -> DescribeCampaignResponseTypeDef:
         """
         Describes the given campaign, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_campaign)
         """
-    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseOutputTypeDef:
+    def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Describes the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset)
         """
     def describe_dataset_export_job(
         self, *, datasetExportJobArn: str
-    ) -> DescribeDatasetExportJobResponseOutputTypeDef:
+    ) -> DescribeDatasetExportJobResponseTypeDef:
         """
         Describes the dataset export job created by
         [CreateDatasetExportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetExportJob.html)_,
         including the export job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_export_job)
         """
     def describe_dataset_group(
         self, *, datasetGroupArn: str
-    ) -> DescribeDatasetGroupResponseOutputTypeDef:
+    ) -> DescribeDatasetGroupResponseTypeDef:
         """
         Describes the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_group)
         """
     def describe_dataset_import_job(
         self, *, datasetImportJobArn: str
-    ) -> DescribeDatasetImportJobResponseOutputTypeDef:
+    ) -> DescribeDatasetImportJobResponseTypeDef:
         """
         Describes the dataset import job created by
         [CreateDatasetImportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetImportJob.html)_,
         including the import job status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset_import_job)
         """
     def describe_event_tracker(
         self, *, eventTrackerArn: str
-    ) -> DescribeEventTrackerResponseOutputTypeDef:
+    ) -> DescribeEventTrackerResponseTypeDef:
         """
         Describes an event tracker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_event_tracker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_event_tracker)
         """
     def describe_feature_transformation(
         self, *, featureTransformationArn: str
-    ) -> DescribeFeatureTransformationResponseOutputTypeDef:
+    ) -> DescribeFeatureTransformationResponseTypeDef:
         """
         Describes the given feature transformation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_feature_transformation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_feature_transformation)
         """
-    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseOutputTypeDef:
+    def describe_filter(self, *, filterArn: str) -> DescribeFilterResponseTypeDef:
         """
         Describes a filter's properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_filter)
         """
     def describe_metric_attribution(
         self, *, metricAttributionArn: str
-    ) -> DescribeMetricAttributionResponseOutputTypeDef:
+    ) -> DescribeMetricAttributionResponseTypeDef:
         """
         Describes a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_metric_attribution)
         """
-    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseOutputTypeDef:
+    def describe_recipe(self, *, recipeArn: str) -> DescribeRecipeResponseTypeDef:
         """
         Describes a recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recipe)
         """
-    def describe_recommender(
-        self, *, recommenderArn: str
-    ) -> DescribeRecommenderResponseOutputTypeDef:
+    def describe_recommender(self, *, recommenderArn: str) -> DescribeRecommenderResponseTypeDef:
         """
         Describes the given recommender, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_recommender)
         """
-    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseOutputTypeDef:
+    def describe_schema(self, *, schemaArn: str) -> DescribeSchemaResponseTypeDef:
         """
         Describes a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_schema)
         """
-    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseOutputTypeDef:
+    def describe_solution(self, *, solutionArn: str) -> DescribeSolutionResponseTypeDef:
         """
         Describes a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution)
         """
     def describe_solution_version(
         self, *, solutionVersionArn: str
-    ) -> DescribeSolutionVersionResponseOutputTypeDef:
+    ) -> DescribeSolutionVersionResponseTypeDef:
         """
         Describes a specific version of a solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_solution_version)
         """
     def generate_presigned_url(
@@ -598,192 +596,188 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#generate_presigned_url)
         """
-    def get_solution_metrics(
-        self, *, solutionVersionArn: str
-    ) -> GetSolutionMetricsResponseOutputTypeDef:
+    def get_solution_metrics(self, *, solutionVersionArn: str) -> GetSolutionMetricsResponseTypeDef:
         """
         Gets the metrics for the specified solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.get_solution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#get_solution_metrics)
         """
     def list_batch_inference_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchInferenceJobsResponseOutputTypeDef:
+    ) -> ListBatchInferenceJobsResponseTypeDef:
         """
         Gets a list of the batch inference jobs that have been performed off of a
         solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_inference_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_inference_jobs)
         """
     def list_batch_segment_jobs(
         self, *, solutionVersionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListBatchSegmentJobsResponseOutputTypeDef:
+    ) -> ListBatchSegmentJobsResponseTypeDef:
         """
         Gets a list of the batch segment jobs that have been performed off of a solution
         version that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_segment_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_batch_segment_jobs)
         """
     def list_campaigns(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListCampaignsResponseOutputTypeDef:
+    ) -> ListCampaignsResponseTypeDef:
         """
         Returns a list of campaigns that use the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_campaigns)
         """
     def list_dataset_export_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetExportJobsResponseOutputTypeDef:
+    ) -> ListDatasetExportJobsResponseTypeDef:
         """
         Returns a list of dataset export jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_export_jobs)
         """
     def list_dataset_groups(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetGroupsResponseOutputTypeDef:
+    ) -> ListDatasetGroupsResponseTypeDef:
         """
         Returns a list of dataset groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_groups)
         """
     def list_dataset_import_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetImportJobsResponseOutputTypeDef:
+    ) -> ListDatasetImportJobsResponseTypeDef:
         """
         Returns a list of dataset import jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_dataset_import_jobs)
         """
     def list_datasets(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListDatasetsResponseOutputTypeDef:
+    ) -> ListDatasetsResponseTypeDef:
         """
         Returns the list of datasets contained in the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_datasets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_datasets)
         """
     def list_event_trackers(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListEventTrackersResponseOutputTypeDef:
+    ) -> ListEventTrackersResponseTypeDef:
         """
         Returns the list of event trackers associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_event_trackers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_event_trackers)
         """
     def list_filters(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListFiltersResponseOutputTypeDef:
+    ) -> ListFiltersResponseTypeDef:
         """
         Lists all filters that belong to a given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_filters)
         """
     def list_metric_attribution_metrics(
         self, *, metricAttributionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionMetricsResponseOutputTypeDef:
+    ) -> ListMetricAttributionMetricsResponseTypeDef:
         """
         Lists the metrics for the metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attribution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attribution_metrics)
         """
     def list_metric_attributions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListMetricAttributionsResponseOutputTypeDef:
+    ) -> ListMetricAttributionsResponseTypeDef:
         """
         Lists metric attributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_metric_attributions)
         """
     def list_recipes(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         domain: DomainType = ...
-    ) -> ListRecipesResponseOutputTypeDef:
+    ) -> ListRecipesResponseTypeDef:
         """
         Returns a list of available recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recipes)
         """
     def list_recommenders(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListRecommendersResponseOutputTypeDef:
+    ) -> ListRecommendersResponseTypeDef:
         """
         Returns a list of recommenders in a given Domain dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recommenders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_recommenders)
         """
     def list_schemas(
         self, *, nextToken: str = ..., maxResults: int = ...
-    ) -> ListSchemasResponseOutputTypeDef:
+    ) -> ListSchemasResponseTypeDef:
         """
         Returns the list of schemas associated with the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_schemas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_schemas)
         """
     def list_solution_versions(
         self, *, solutionArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionVersionsResponseOutputTypeDef:
+    ) -> ListSolutionVersionsResponseTypeDef:
         """
         Returns a list of solution versions for the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solution_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solution_versions)
         """
     def list_solutions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
-    ) -> ListSolutionsResponseOutputTypeDef:
+    ) -> ListSolutionsResponseTypeDef:
         """
         Returns a list of solutions that use the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
-    def list_tags_for_resource(
-        self, *, resourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_tags_for_resource)
         """
-    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseOutputTypeDef:
+    def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseTypeDef:
         """
         Starts a recommender that is INACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.start_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#start_recommender)
         """
-    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseOutputTypeDef:
+    def stop_recommender(self, *, recommenderArn: str) -> StopRecommenderResponseTypeDef:
         """
         Stops a recommender that is ACTIVE.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#stop_recommender)
         """
     def stop_solution_version_creation(
@@ -814,48 +808,46 @@
     def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...
-    ) -> UpdateCampaignResponseOutputTypeDef:
+    ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
-    def update_dataset(
-        self, *, datasetArn: str, schemaArn: str
-    ) -> UpdateDatasetResponseOutputTypeDef:
+    def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
         """
         Update a dataset to replace its schema with a new or existing one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_dataset)
         """
     def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
-    ) -> UpdateMetricAttributionResponseOutputTypeDef:
+    ) -> UpdateMetricAttributionResponseTypeDef:
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_metric_attribution)
         """
     def update_recommender(
         self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
-    ) -> UpdateRecommenderResponseOutputTypeDef:
+    ) -> UpdateRecommenderResponseTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_recommender)
         """
     @overload
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.py` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/literals.pyi` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.py` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DomainType
 from .type_defs import (
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    ListCampaignsResponseOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    ListCampaignsResponseTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListRecommendersResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -115,165 +115,165 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchInferenceJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListBatchInferenceJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
         """
 
 
 class ListBatchSegmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchSegmentJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListBatchSegmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
         """
 
 
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListCampaignsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
         """
 
 
 class ListDatasetExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetExportJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
         """
 
 
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
         """
 
 
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetImportJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
         """
 
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
         """
 
 
 class ListEventTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEventTrackersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEventTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
         """
 
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListFiltersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
         """
 
 
 class ListMetricAttributionMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
     """
 
     def paginate(
         self, *, metricAttributionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionMetricsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
         """
 
 
 class ListMetricAttributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
         """
 
 
 class ListRecipesPaginator(Paginator):
@@ -284,72 +284,72 @@
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecipesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecipespaginator)
         """
 
 
 class ListRecommendersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecommendersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRecommendersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSchemasResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
         """
 
 
 class ListSolutionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionVersionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSolutionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
         """
 
 
 class ListSolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSolutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
         """
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/paginator.pyi` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DomainType
 from .type_defs import (
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    ListCampaignsResponseOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    ListCampaignsResponseTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListRecommendersResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -111,155 +111,155 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchInferenceJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListBatchInferenceJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchinferencejobspaginator)
         """
 
 class ListBatchSegmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
     """
 
     def paginate(
         self, *, solutionVersionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBatchSegmentJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListBatchSegmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listbatchsegmentjobspaginator)
         """
 
 class ListCampaignsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListCampaignsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listcampaignspaginator)
         """
 
 class ListDatasetExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetExportJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetexportjobspaginator)
         """
 
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetgroupspaginator)
         """
 
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self, *, datasetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetImportJobsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetimportjobspaginator)
         """
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDatasetsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listdatasetspaginator)
         """
 
 class ListEventTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEventTrackersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEventTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listeventtrackerspaginator)
         """
 
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListFiltersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listfilterspaginator)
         """
 
 class ListMetricAttributionMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
     """
 
     def paginate(
         self, *, metricAttributionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionMetricsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributionMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionmetricspaginator)
         """
 
 class ListMetricAttributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMetricAttributionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMetricAttributionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListMetricAttributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listmetricattributionspaginator)
         """
 
 class ListRecipesPaginator(Paginator):
     """
@@ -269,68 +269,68 @@
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecipesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecipespaginator)
         """
 
 class ListRecommendersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRecommendersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRecommendersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSchemasResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listschemaspaginator)
         """
 
 class ListSolutionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
     """
 
     def paginate(
         self, *, solutionArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionVersionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSolutionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionversionspaginator)
         """
 
 class ListSolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSolutionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSolutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listsolutionspaginator)
         """
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.py` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for personalize service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize.type_defs import AlgorithmImageOutputTypeDef
+    from mypy_boto3_personalize.type_defs import AlgorithmImageTypeDef
 
-    data: AlgorithmImageOutputTypeDef = {...}
+    data: AlgorithmImageTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -30,59 +30,61 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AlgorithmImageOutputTypeDef",
+    "AlgorithmImageTypeDef",
     "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
-    "AutoMLResultOutputTypeDef",
+    "AutoMLResultTypeDef",
+    "BatchInferenceJobConfigOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
+    "S3DataConfigOutputTypeDef",
     "S3DataConfigTypeDef",
-    "BatchInferenceJobSummaryOutputTypeDef",
-    "BatchSegmentJobSummaryOutputTypeDef",
+    "BatchInferenceJobSummaryTypeDef",
+    "BatchSegmentJobSummaryTypeDef",
     "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
-    "CampaignSummaryOutputTypeDef",
+    "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeOutputTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
-    "CreateBatchInferenceJobResponseOutputTypeDef",
-    "CreateBatchSegmentJobResponseOutputTypeDef",
-    "CreateCampaignResponseOutputTypeDef",
-    "CreateDatasetExportJobResponseOutputTypeDef",
-    "CreateDatasetGroupResponseOutputTypeDef",
+    "CreateBatchInferenceJobResponseTypeDef",
+    "CreateBatchSegmentJobResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDatasetExportJobResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
     "DataSourceTypeDef",
-    "CreateDatasetImportJobResponseOutputTypeDef",
-    "CreateDatasetResponseOutputTypeDef",
-    "CreateEventTrackerResponseOutputTypeDef",
-    "CreateFilterResponseOutputTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateEventTrackerResponseTypeDef",
+    "CreateFilterResponseTypeDef",
     "MetricAttributeTypeDef",
-    "CreateMetricAttributionResponseOutputTypeDef",
-    "CreateRecommenderResponseOutputTypeDef",
+    "CreateMetricAttributionResponseTypeDef",
+    "CreateRecommenderResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseOutputTypeDef",
-    "CreateSolutionResponseOutputTypeDef",
-    "CreateSolutionVersionResponseOutputTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "CreateSolutionResponseTypeDef",
+    "CreateSolutionVersionResponseTypeDef",
     "DataSourceOutputTypeDef",
-    "DatasetExportJobSummaryOutputTypeDef",
-    "DatasetGroupOutputTypeDef",
-    "DatasetGroupSummaryOutputTypeDef",
-    "DatasetImportJobSummaryOutputTypeDef",
-    "DatasetUpdateSummaryOutputTypeDef",
-    "DatasetSchemaOutputTypeDef",
-    "DatasetSchemaSummaryOutputTypeDef",
-    "DatasetSummaryOutputTypeDef",
-    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
-    "DefaultContinuousHyperParameterRangeOutputTypeDef",
-    "DefaultIntegerHyperParameterRangeOutputTypeDef",
+    "DatasetExportJobSummaryTypeDef",
+    "DatasetGroupSummaryTypeDef",
+    "DatasetGroupTypeDef",
+    "DatasetImportJobSummaryTypeDef",
+    "DatasetSchemaSummaryTypeDef",
+    "DatasetSchemaTypeDef",
+    "DatasetSummaryTypeDef",
+    "DatasetUpdateSummaryTypeDef",
+    "DefaultCategoricalHyperParameterRangeTypeDef",
+    "DefaultContinuousHyperParameterRangeTypeDef",
+    "DefaultIntegerHyperParameterRangeTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteMetricAttributionRequestRequestTypeDef",
     "DeleteRecommenderRequestRequestTypeDef",
@@ -93,31 +95,31 @@
     "DescribeBatchSegmentJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DescribeDatasetExportJobRequestRequestTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeEventTrackerRequestRequestTypeDef",
-    "EventTrackerOutputTypeDef",
+    "EventTrackerTypeDef",
     "DescribeFeatureTransformationRequestRequestTypeDef",
-    "FeatureTransformationOutputTypeDef",
+    "FeatureTransformationTypeDef",
     "DescribeFilterRequestRequestTypeDef",
-    "FilterOutputTypeDef",
+    "FilterTypeDef",
     "DescribeMetricAttributionRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
-    "RecipeOutputTypeDef",
+    "RecipeTypeDef",
     "DescribeRecommenderRequestRequestTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
     "DescribeSolutionRequestRequestTypeDef",
     "DescribeSolutionVersionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "EventTrackerSummaryOutputTypeDef",
-    "FilterSummaryOutputTypeDef",
+    "EventTrackerSummaryTypeDef",
+    "FilterSummaryTypeDef",
     "GetSolutionMetricsRequestRequestTypeDef",
-    "GetSolutionMetricsResponseOutputTypeDef",
+    "GetSolutionMetricsResponseTypeDef",
     "HPOObjectiveOutputTypeDef",
     "HPOResourceConfigOutputTypeDef",
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
     "IntegerHyperParameterRangeOutputTypeDef",
     "IntegerHyperParameterRangeTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
@@ -139,128 +141,134 @@
     "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
     "MetricAttributeOutputTypeDef",
     "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     "ListMetricAttributionsRequestRequestTypeDef",
-    "MetricAttributionSummaryOutputTypeDef",
+    "MetricAttributionSummaryTypeDef",
     "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
-    "RecipeSummaryOutputTypeDef",
+    "RecipeSummaryTypeDef",
     "ListRecommendersRequestListRecommendersPaginateTypeDef",
     "ListRecommendersRequestRequestTypeDef",
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
-    "SolutionVersionSummaryOutputTypeDef",
+    "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListSolutionsRequestRequestTypeDef",
-    "SolutionSummaryOutputTypeDef",
+    "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagOutputTypeDef",
     "OptimizationObjectiveOutputTypeDef",
     "OptimizationObjectiveTypeDef",
     "PaginatorConfigTypeDef",
     "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "ResponseMetadataTypeDef",
-    "TunedHPOParamsOutputTypeDef",
+    "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
-    "StartRecommenderResponseOutputTypeDef",
+    "StartRecommenderResponseTypeDef",
     "StopRecommenderRequestRequestTypeDef",
-    "StopRecommenderResponseOutputTypeDef",
+    "StopRecommenderResponseTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCampaignResponseOutputTypeDef",
+    "UpdateCampaignResponseTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
-    "UpdateDatasetResponseOutputTypeDef",
-    "UpdateMetricAttributionResponseOutputTypeDef",
-    "UpdateRecommenderResponseOutputTypeDef",
+    "UpdateDatasetResponseTypeDef",
+    "UpdateMetricAttributionResponseTypeDef",
+    "UpdateRecommenderResponseTypeDef",
+    "BatchInferenceJobInputOutputTypeDef",
+    "BatchSegmentJobInputOutputTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
-    "ListBatchInferenceJobsResponseOutputTypeDef",
-    "ListBatchSegmentJobsResponseOutputTypeDef",
-    "CampaignUpdateSummaryOutputTypeDef",
+    "ListBatchInferenceJobsResponseTypeDef",
+    "ListBatchSegmentJobsResponseTypeDef",
+    "CampaignUpdateSummaryTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
-    "ListCampaignsResponseOutputTypeDef",
+    "ListCampaignsResponseTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
-    "DatasetImportJobOutputTypeDef",
-    "ListDatasetExportJobsResponseOutputTypeDef",
-    "DescribeDatasetGroupResponseOutputTypeDef",
-    "ListDatasetGroupsResponseOutputTypeDef",
-    "ListDatasetImportJobsResponseOutputTypeDef",
-    "DatasetOutputTypeDef",
-    "DescribeSchemaResponseOutputTypeDef",
-    "ListSchemasResponseOutputTypeDef",
-    "ListDatasetsResponseOutputTypeDef",
-    "DefaultHyperParameterRangesOutputTypeDef",
-    "DescribeEventTrackerResponseOutputTypeDef",
-    "DescribeFeatureTransformationResponseOutputTypeDef",
-    "DescribeFilterResponseOutputTypeDef",
-    "DescribeRecipeResponseOutputTypeDef",
-    "ListEventTrackersResponseOutputTypeDef",
-    "ListFiltersResponseOutputTypeDef",
+    "DatasetImportJobTypeDef",
+    "ListDatasetExportJobsResponseTypeDef",
+    "ListDatasetGroupsResponseTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
+    "ListDatasetImportJobsResponseTypeDef",
+    "ListSchemasResponseTypeDef",
+    "DescribeSchemaResponseTypeDef",
+    "ListDatasetsResponseTypeDef",
+    "DatasetTypeDef",
+    "DefaultHyperParameterRangesTypeDef",
+    "DescribeEventTrackerResponseTypeDef",
+    "DescribeFeatureTransformationResponseTypeDef",
+    "DescribeFilterResponseTypeDef",
+    "DescribeRecipeResponseTypeDef",
+    "ListEventTrackersResponseTypeDef",
+    "ListFiltersResponseTypeDef",
     "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
-    "ListMetricAttributionMetricsResponseOutputTypeDef",
-    "ListMetricAttributionsResponseOutputTypeDef",
-    "ListRecipesResponseOutputTypeDef",
-    "ListSolutionVersionsResponseOutputTypeDef",
-    "ListSolutionsResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "ListMetricAttributionMetricsResponseTypeDef",
+    "ListMetricAttributionsResponseTypeDef",
+    "ListRecipesResponseTypeDef",
+    "ListSolutionVersionsResponseTypeDef",
+    "ListSolutionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
+    "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
-    "DescribeBatchInferenceJobResponseOutputTypeDef",
+    "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
-    "DescribeBatchSegmentJobResponseOutputTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
-    "DescribeDatasetExportJobResponseOutputTypeDef",
+    "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
-    "DescribeMetricAttributionResponseOutputTypeDef",
+    "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
-    "CampaignOutputTypeDef",
-    "DescribeDatasetImportJobResponseOutputTypeDef",
-    "DescribeDatasetResponseOutputTypeDef",
-    "AlgorithmOutputTypeDef",
+    "CampaignTypeDef",
+    "DescribeDatasetImportJobResponseTypeDef",
+    "DescribeDatasetResponseTypeDef",
+    "AlgorithmTypeDef",
     "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
-    "RecommenderSummaryOutputTypeDef",
-    "RecommenderUpdateSummaryOutputTypeDef",
+    "RecommenderSummaryTypeDef",
+    "RecommenderUpdateSummaryTypeDef",
     "CreateRecommenderRequestRequestTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
-    "DescribeCampaignResponseOutputTypeDef",
-    "DescribeAlgorithmResponseOutputTypeDef",
+    "DescribeBatchInferenceJobResponseTypeDef",
+    "DescribeBatchSegmentJobResponseTypeDef",
+    "DescribeDatasetExportJobResponseTypeDef",
+    "DescribeMetricAttributionResponseTypeDef",
+    "DescribeCampaignResponseTypeDef",
+    "DescribeAlgorithmResponseTypeDef",
     "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
-    "ListRecommendersResponseOutputTypeDef",
-    "RecommenderOutputTypeDef",
-    "SolutionOutputTypeDef",
-    "SolutionVersionOutputTypeDef",
+    "ListRecommendersResponseTypeDef",
+    "RecommenderTypeDef",
+    "SolutionTypeDef",
+    "SolutionVersionTypeDef",
     "CreateSolutionRequestRequestTypeDef",
-    "DescribeRecommenderResponseOutputTypeDef",
-    "DescribeSolutionResponseOutputTypeDef",
-    "DescribeSolutionVersionResponseOutputTypeDef",
+    "DescribeRecommenderResponseTypeDef",
+    "DescribeSolutionResponseTypeDef",
+    "DescribeSolutionVersionResponseTypeDef",
 )
 
-AlgorithmImageOutputTypeDef = TypedDict(
-    "AlgorithmImageOutputTypeDef",
+AlgorithmImageTypeDef = TypedDict(
+    "AlgorithmImageTypeDef",
     {
         "name": str,
         "dockerURI": str,
     },
 )
 
 AutoMLConfigOutputTypeDef = TypedDict(
@@ -276,29 +284,44 @@
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
 )
 
-AutoMLResultOutputTypeDef = TypedDict(
-    "AutoMLResultOutputTypeDef",
+AutoMLResultTypeDef = TypedDict(
+    "AutoMLResultTypeDef",
     {
         "bestRecipeArn": str,
     },
 )
 
+BatchInferenceJobConfigOutputTypeDef = TypedDict(
+    "BatchInferenceJobConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": Dict[str, str],
+    },
+)
+
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
 
+S3DataConfigOutputTypeDef = TypedDict(
+    "S3DataConfigOutputTypeDef",
+    {
+        "path": str,
+        "kmsKeyArn": str,
+    },
+)
+
 _RequiredS3DataConfigTypeDef = TypedDict(
     "_RequiredS3DataConfigTypeDef",
     {
         "path": str,
     },
 )
 _OptionalS3DataConfigTypeDef = TypedDict(
@@ -310,29 +333,29 @@
 )
 
 
 class S3DataConfigTypeDef(_RequiredS3DataConfigTypeDef, _OptionalS3DataConfigTypeDef):
     pass
 
 
-BatchInferenceJobSummaryOutputTypeDef = TypedDict(
-    "BatchInferenceJobSummaryOutputTypeDef",
+BatchInferenceJobSummaryTypeDef = TypedDict(
+    "BatchInferenceJobSummaryTypeDef",
     {
         "batchInferenceJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
 )
 
-BatchSegmentJobSummaryOutputTypeDef = TypedDict(
-    "BatchSegmentJobSummaryOutputTypeDef",
+BatchSegmentJobSummaryTypeDef = TypedDict(
+    "BatchSegmentJobSummaryTypeDef",
     {
         "batchSegmentJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -351,16 +374,16 @@
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
 
-CampaignSummaryOutputTypeDef = TypedDict(
-    "CampaignSummaryOutputTypeDef",
+CampaignSummaryTypeDef = TypedDict(
+    "CampaignSummaryTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -407,48 +430,48 @@
     "TagTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
     },
 )
 
-CreateBatchInferenceJobResponseOutputTypeDef = TypedDict(
-    "CreateBatchInferenceJobResponseOutputTypeDef",
+CreateBatchInferenceJobResponseTypeDef = TypedDict(
+    "CreateBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBatchSegmentJobResponseOutputTypeDef = TypedDict(
-    "CreateBatchSegmentJobResponseOutputTypeDef",
+CreateBatchSegmentJobResponseTypeDef = TypedDict(
+    "CreateBatchSegmentJobResponseTypeDef",
     {
         "batchSegmentJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCampaignResponseOutputTypeDef = TypedDict(
-    "CreateCampaignResponseOutputTypeDef",
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetExportJobResponseOutputTypeDef = TypedDict(
-    "CreateDatasetExportJobResponseOutputTypeDef",
+CreateDatasetExportJobResponseTypeDef = TypedDict(
+    "CreateDatasetExportJobResponseTypeDef",
     {
         "datasetExportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetGroupResponseOutputTypeDef = TypedDict(
-    "CreateDatasetGroupResponseOutputTypeDef",
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
     {
         "datasetGroupArn": str,
         "domain": DomainType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -456,41 +479,41 @@
     "DataSourceTypeDef",
     {
         "dataLocation": str,
     },
     total=False,
 )
 
-CreateDatasetImportJobResponseOutputTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseOutputTypeDef",
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
     {
         "datasetImportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetResponseOutputTypeDef = TypedDict(
-    "CreateDatasetResponseOutputTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEventTrackerResponseOutputTypeDef = TypedDict(
-    "CreateEventTrackerResponseOutputTypeDef",
+CreateEventTrackerResponseTypeDef = TypedDict(
+    "CreateEventTrackerResponseTypeDef",
     {
         "eventTrackerArn": str,
         "trackingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFilterResponseOutputTypeDef = TypedDict(
-    "CreateFilterResponseOutputTypeDef",
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
     {
         "filterArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricAttributeTypeDef = TypedDict(
@@ -498,24 +521,24 @@
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
-CreateMetricAttributionResponseOutputTypeDef = TypedDict(
-    "CreateMetricAttributionResponseOutputTypeDef",
+CreateMetricAttributionResponseTypeDef = TypedDict(
+    "CreateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRecommenderResponseOutputTypeDef = TypedDict(
-    "CreateRecommenderResponseOutputTypeDef",
+CreateRecommenderResponseTypeDef = TypedDict(
+    "CreateRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
@@ -536,165 +559,165 @@
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
 
-CreateSchemaResponseOutputTypeDef = TypedDict(
-    "CreateSchemaResponseOutputTypeDef",
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
     {
         "schemaArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionResponseOutputTypeDef = TypedDict(
-    "CreateSolutionResponseOutputTypeDef",
+CreateSolutionResponseTypeDef = TypedDict(
+    "CreateSolutionResponseTypeDef",
     {
         "solutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionVersionResponseOutputTypeDef = TypedDict(
-    "CreateSolutionVersionResponseOutputTypeDef",
+CreateSolutionVersionResponseTypeDef = TypedDict(
+    "CreateSolutionVersionResponseTypeDef",
     {
         "solutionVersionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSourceOutputTypeDef = TypedDict(
     "DataSourceOutputTypeDef",
     {
         "dataLocation": str,
     },
 )
 
-DatasetExportJobSummaryOutputTypeDef = TypedDict(
-    "DatasetExportJobSummaryOutputTypeDef",
+DatasetExportJobSummaryTypeDef = TypedDict(
+    "DatasetExportJobSummaryTypeDef",
     {
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
 )
 
-DatasetGroupOutputTypeDef = TypedDict(
-    "DatasetGroupOutputTypeDef",
+DatasetGroupSummaryTypeDef = TypedDict(
+    "DatasetGroupSummaryTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
-        "roleArn": str,
-        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetGroupSummaryOutputTypeDef = TypedDict(
-    "DatasetGroupSummaryOutputTypeDef",
+DatasetGroupTypeDef = TypedDict(
+    "DatasetGroupTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
+        "roleArn": str,
+        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetImportJobSummaryOutputTypeDef = TypedDict(
-    "DatasetImportJobSummaryOutputTypeDef",
+DatasetImportJobSummaryTypeDef = TypedDict(
+    "DatasetImportJobSummaryTypeDef",
     {
         "datasetImportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
     },
 )
 
-DatasetUpdateSummaryOutputTypeDef = TypedDict(
-    "DatasetUpdateSummaryOutputTypeDef",
+DatasetSchemaSummaryTypeDef = TypedDict(
+    "DatasetSchemaSummaryTypeDef",
     {
+        "name": str,
         "schemaArn": str,
-        "status": str,
-        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
+        "domain": DomainType,
     },
 )
 
-DatasetSchemaOutputTypeDef = TypedDict(
-    "DatasetSchemaOutputTypeDef",
+DatasetSchemaTypeDef = TypedDict(
+    "DatasetSchemaTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "schema": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
 )
 
-DatasetSchemaSummaryOutputTypeDef = TypedDict(
-    "DatasetSchemaSummaryOutputTypeDef",
+DatasetSummaryTypeDef = TypedDict(
+    "DatasetSummaryTypeDef",
     {
         "name": str,
-        "schemaArn": str,
+        "datasetArn": str,
+        "datasetType": str,
+        "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "domain": DomainType,
     },
 )
 
-DatasetSummaryOutputTypeDef = TypedDict(
-    "DatasetSummaryOutputTypeDef",
+DatasetUpdateSummaryTypeDef = TypedDict(
+    "DatasetUpdateSummaryTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetType": str,
+        "schemaArn": str,
         "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-DefaultCategoricalHyperParameterRangeOutputTypeDef = TypedDict(
-    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
+DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
+    "DefaultCategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": List[str],
         "isTunable": bool,
     },
 )
 
-DefaultContinuousHyperParameterRangeOutputTypeDef = TypedDict(
-    "DefaultContinuousHyperParameterRangeOutputTypeDef",
+DefaultContinuousHyperParameterRangeTypeDef = TypedDict(
+    "DefaultContinuousHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
         "isTunable": bool,
     },
 )
 
-DefaultIntegerHyperParameterRangeOutputTypeDef = TypedDict(
-    "DefaultIntegerHyperParameterRangeOutputTypeDef",
+DefaultIntegerHyperParameterRangeTypeDef = TypedDict(
+    "DefaultIntegerHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
         "isTunable": bool,
     },
 )
@@ -821,16 +844,16 @@
 DescribeEventTrackerRequestRequestTypeDef = TypedDict(
     "DescribeEventTrackerRequestRequestTypeDef",
     {
         "eventTrackerArn": str,
     },
 )
 
-EventTrackerOutputTypeDef = TypedDict(
-    "EventTrackerOutputTypeDef",
+EventTrackerTypeDef = TypedDict(
+    "EventTrackerTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "accountId": str,
         "trackingId": str,
         "datasetGroupArn": str,
         "status": str,
@@ -842,16 +865,16 @@
 DescribeFeatureTransformationRequestRequestTypeDef = TypedDict(
     "DescribeFeatureTransformationRequestRequestTypeDef",
     {
         "featureTransformationArn": str,
     },
 )
 
-FeatureTransformationOutputTypeDef = TypedDict(
-    "FeatureTransformationOutputTypeDef",
+FeatureTransformationTypeDef = TypedDict(
+    "FeatureTransformationTypeDef",
     {
         "name": str,
         "featureTransformationArn": str,
         "defaultParameters": Dict[str, str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
@@ -861,16 +884,16 @@
 DescribeFilterRequestRequestTypeDef = TypedDict(
     "DescribeFilterRequestRequestTypeDef",
     {
         "filterArn": str,
     },
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -889,16 +912,16 @@
 DescribeRecipeRequestRequestTypeDef = TypedDict(
     "DescribeRecipeRequestRequestTypeDef",
     {
         "recipeArn": str,
     },
 )
 
-RecipeOutputTypeDef = TypedDict(
-    "RecipeOutputTypeDef",
+RecipeTypeDef = TypedDict(
+    "RecipeTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "algorithmArn": str,
         "featureTransformationArn": str,
         "status": str,
         "description": str,
@@ -939,27 +962,27 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EventTrackerSummaryOutputTypeDef = TypedDict(
-    "EventTrackerSummaryOutputTypeDef",
+EventTrackerSummaryTypeDef = TypedDict(
+    "EventTrackerSummaryTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-FilterSummaryOutputTypeDef = TypedDict(
-    "FilterSummaryOutputTypeDef",
+FilterSummaryTypeDef = TypedDict(
+    "FilterSummaryTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -970,16 +993,16 @@
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
-GetSolutionMetricsResponseOutputTypeDef = TypedDict(
-    "GetSolutionMetricsResponseOutputTypeDef",
+GetSolutionMetricsResponseTypeDef = TypedDict(
+    "GetSolutionMetricsResponseTypeDef",
     {
         "solutionVersionArn": str,
         "metrics": Dict[str, float],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1250,16 +1273,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-MetricAttributionSummaryOutputTypeDef = TypedDict(
-    "MetricAttributionSummaryOutputTypeDef",
+MetricAttributionSummaryTypeDef = TypedDict(
+    "MetricAttributionSummaryTypeDef",
     {
         "name": str,
         "metricAttributionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -1283,16 +1306,16 @@
         "nextToken": str,
         "maxResults": int,
         "domain": DomainType,
     },
     total=False,
 )
 
-RecipeSummaryOutputTypeDef = TypedDict(
-    "RecipeSummaryOutputTypeDef",
+RecipeSummaryTypeDef = TypedDict(
+    "RecipeSummaryTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
@@ -1350,16 +1373,16 @@
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionVersionSummaryOutputTypeDef = TypedDict(
-    "SolutionVersionSummaryOutputTypeDef",
+SolutionVersionSummaryTypeDef = TypedDict(
+    "SolutionVersionSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
@@ -1380,16 +1403,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionSummaryOutputTypeDef = TypedDict(
-    "SolutionSummaryOutputTypeDef",
+SolutionSummaryTypeDef = TypedDict(
+    "SolutionSummaryTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recipeArn": str,
@@ -1460,45 +1483,45 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TunedHPOParamsOutputTypeDef = TypedDict(
-    "TunedHPOParamsOutputTypeDef",
+TunedHPOParamsTypeDef = TypedDict(
+    "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
 )
 
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StartRecommenderResponseOutputTypeDef = TypedDict(
-    "StartRecommenderResponseOutputTypeDef",
+StartRecommenderResponseTypeDef = TypedDict(
+    "StartRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRecommenderRequestRequestTypeDef = TypedDict(
     "StopRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StopRecommenderResponseOutputTypeDef = TypedDict(
-    "StopRecommenderResponseOutputTypeDef",
+StopRecommenderResponseTypeDef = TypedDict(
+    "StopRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopSolutionVersionCreationRequestRequestTypeDef = TypedDict(
@@ -1512,54 +1535,68 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateCampaignResponseOutputTypeDef = TypedDict(
-    "UpdateCampaignResponseOutputTypeDef",
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDatasetRequestRequestTypeDef = TypedDict(
     "UpdateDatasetRequestRequestTypeDef",
     {
         "datasetArn": str,
         "schemaArn": str,
     },
 )
 
-UpdateDatasetResponseOutputTypeDef = TypedDict(
-    "UpdateDatasetResponseOutputTypeDef",
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateMetricAttributionResponseOutputTypeDef = TypedDict(
-    "UpdateMetricAttributionResponseOutputTypeDef",
+UpdateMetricAttributionResponseTypeDef = TypedDict(
+    "UpdateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRecommenderResponseOutputTypeDef = TypedDict(
-    "UpdateRecommenderResponseOutputTypeDef",
+UpdateRecommenderResponseTypeDef = TypedDict(
+    "UpdateRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchInferenceJobInputOutputTypeDef = TypedDict(
+    "BatchInferenceJobInputOutputTypeDef",
+    {
+        "s3DataSource": S3DataConfigOutputTypeDef,
+    },
+)
+
+BatchSegmentJobInputOutputTypeDef = TypedDict(
+    "BatchSegmentJobInputOutputTypeDef",
+    {
+        "s3DataSource": S3DataConfigOutputTypeDef,
+    },
+)
+
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 
@@ -1608,34 +1645,34 @@
 
 class MetricAttributionOutputTypeDef(
     _RequiredMetricAttributionOutputTypeDef, _OptionalMetricAttributionOutputTypeDef
 ):
     pass
 
 
-ListBatchInferenceJobsResponseOutputTypeDef = TypedDict(
-    "ListBatchInferenceJobsResponseOutputTypeDef",
+ListBatchInferenceJobsResponseTypeDef = TypedDict(
+    "ListBatchInferenceJobsResponseTypeDef",
     {
-        "batchInferenceJobs": List[BatchInferenceJobSummaryOutputTypeDef],
+        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBatchSegmentJobsResponseOutputTypeDef = TypedDict(
-    "ListBatchSegmentJobsResponseOutputTypeDef",
+ListBatchSegmentJobsResponseTypeDef = TypedDict(
+    "ListBatchSegmentJobsResponseTypeDef",
     {
-        "batchSegmentJobs": List[BatchSegmentJobSummaryOutputTypeDef],
+        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CampaignUpdateSummaryOutputTypeDef = TypedDict(
-    "CampaignUpdateSummaryOutputTypeDef",
+CampaignUpdateSummaryTypeDef = TypedDict(
+    "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
@@ -1662,18 +1699,18 @@
 
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
 
-ListCampaignsResponseOutputTypeDef = TypedDict(
-    "ListCampaignsResponseOutputTypeDef",
+ListCampaignsResponseTypeDef = TypedDict(
+    "ListCampaignsResponseTypeDef",
     {
-        "campaigns": List[CampaignSummaryOutputTypeDef],
+        "campaigns": List[CampaignSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
@@ -1849,16 +1886,16 @@
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
 
-DatasetImportJobOutputTypeDef = TypedDict(
-    "DatasetImportJobOutputTypeDef",
+DatasetImportJobTypeDef = TypedDict(
+    "DatasetImportJobTypeDef",
     {
         "jobName": str,
         "datasetImportJobArn": str,
         "datasetArn": str,
         "dataSource": DataSourceOutputTypeDef,
         "roleArn": str,
         "status": str,
@@ -1866,144 +1903,144 @@
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
 )
 
-ListDatasetExportJobsResponseOutputTypeDef = TypedDict(
-    "ListDatasetExportJobsResponseOutputTypeDef",
+ListDatasetExportJobsResponseTypeDef = TypedDict(
+    "ListDatasetExportJobsResponseTypeDef",
     {
-        "datasetExportJobs": List[DatasetExportJobSummaryOutputTypeDef],
+        "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetGroupResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseOutputTypeDef",
+ListDatasetGroupsResponseTypeDef = TypedDict(
+    "ListDatasetGroupsResponseTypeDef",
     {
-        "datasetGroup": DatasetGroupOutputTypeDef,
+        "datasetGroups": List[DatasetGroupSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetGroupsResponseOutputTypeDef = TypedDict(
-    "ListDatasetGroupsResponseOutputTypeDef",
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
     {
-        "datasetGroups": List[DatasetGroupSummaryOutputTypeDef],
-        "nextToken": str,
+        "datasetGroup": DatasetGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetImportJobsResponseOutputTypeDef = TypedDict(
-    "ListDatasetImportJobsResponseOutputTypeDef",
+ListDatasetImportJobsResponseTypeDef = TypedDict(
+    "ListDatasetImportJobsResponseTypeDef",
     {
-        "datasetImportJobs": List[DatasetImportJobSummaryOutputTypeDef],
+        "datasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetOutputTypeDef = TypedDict(
-    "DatasetOutputTypeDef",
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
-        "schemaArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "latestDatasetUpdate": DatasetUpdateSummaryOutputTypeDef,
+        "schemas": List[DatasetSchemaSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSchemaResponseOutputTypeDef = TypedDict(
-    "DescribeSchemaResponseOutputTypeDef",
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
     {
-        "schema": DatasetSchemaOutputTypeDef,
+        "schema": DatasetSchemaTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSchemasResponseOutputTypeDef = TypedDict(
-    "ListSchemasResponseOutputTypeDef",
+ListDatasetsResponseTypeDef = TypedDict(
+    "ListDatasetsResponseTypeDef",
     {
-        "schemas": List[DatasetSchemaSummaryOutputTypeDef],
+        "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetsResponseOutputTypeDef = TypedDict(
-    "ListDatasetsResponseOutputTypeDef",
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
     {
-        "datasets": List[DatasetSummaryOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
     },
 )
 
-DefaultHyperParameterRangesOutputTypeDef = TypedDict(
-    "DefaultHyperParameterRangesOutputTypeDef",
+DefaultHyperParameterRangesTypeDef = TypedDict(
+    "DefaultHyperParameterRangesTypeDef",
     {
-        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeOutputTypeDef],
-        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeOutputTypeDef],
-        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeOutputTypeDef],
+        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
+        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
+        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeTypeDef],
     },
 )
 
-DescribeEventTrackerResponseOutputTypeDef = TypedDict(
-    "DescribeEventTrackerResponseOutputTypeDef",
+DescribeEventTrackerResponseTypeDef = TypedDict(
+    "DescribeEventTrackerResponseTypeDef",
     {
-        "eventTracker": EventTrackerOutputTypeDef,
+        "eventTracker": EventTrackerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFeatureTransformationResponseOutputTypeDef = TypedDict(
-    "DescribeFeatureTransformationResponseOutputTypeDef",
+DescribeFeatureTransformationResponseTypeDef = TypedDict(
+    "DescribeFeatureTransformationResponseTypeDef",
     {
-        "featureTransformation": FeatureTransformationOutputTypeDef,
+        "featureTransformation": FeatureTransformationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFilterResponseOutputTypeDef = TypedDict(
-    "DescribeFilterResponseOutputTypeDef",
+DescribeFilterResponseTypeDef = TypedDict(
+    "DescribeFilterResponseTypeDef",
     {
-        "filter": FilterOutputTypeDef,
+        "filter": FilterTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecipeResponseOutputTypeDef = TypedDict(
-    "DescribeRecipeResponseOutputTypeDef",
+DescribeRecipeResponseTypeDef = TypedDict(
+    "DescribeRecipeResponseTypeDef",
     {
-        "recipe": RecipeOutputTypeDef,
+        "recipe": RecipeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEventTrackersResponseOutputTypeDef = TypedDict(
-    "ListEventTrackersResponseOutputTypeDef",
+ListEventTrackersResponseTypeDef = TypedDict(
+    "ListEventTrackersResponseTypeDef",
     {
-        "eventTrackers": List[EventTrackerSummaryOutputTypeDef],
+        "eventTrackers": List[EventTrackerSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListFiltersResponseOutputTypeDef = TypedDict(
-    "ListFiltersResponseOutputTypeDef",
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
     {
-        "Filters": List[FilterSummaryOutputTypeDef],
+        "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HyperParameterRangesOutputTypeDef = TypedDict(
     "HyperParameterRangesOutputTypeDef",
@@ -2020,61 +2057,61 @@
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMetricAttributionMetricsResponseOutputTypeDef = TypedDict(
-    "ListMetricAttributionMetricsResponseOutputTypeDef",
+ListMetricAttributionMetricsResponseTypeDef = TypedDict(
+    "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMetricAttributionsResponseOutputTypeDef = TypedDict(
-    "ListMetricAttributionsResponseOutputTypeDef",
+ListMetricAttributionsResponseTypeDef = TypedDict(
+    "ListMetricAttributionsResponseTypeDef",
     {
-        "metricAttributions": List[MetricAttributionSummaryOutputTypeDef],
+        "metricAttributions": List[MetricAttributionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRecipesResponseOutputTypeDef = TypedDict(
-    "ListRecipesResponseOutputTypeDef",
+ListRecipesResponseTypeDef = TypedDict(
+    "ListRecipesResponseTypeDef",
     {
-        "recipes": List[RecipeSummaryOutputTypeDef],
+        "recipes": List[RecipeSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionVersionsResponseOutputTypeDef = TypedDict(
-    "ListSolutionVersionsResponseOutputTypeDef",
+ListSolutionVersionsResponseTypeDef = TypedDict(
+    "ListSolutionVersionsResponseTypeDef",
     {
-        "solutionVersions": List[SolutionVersionSummaryOutputTypeDef],
+        "solutionVersions": List[SolutionVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionsResponseOutputTypeDef = TypedDict(
-    "ListSolutionsResponseOutputTypeDef",
+ListSolutionsResponseTypeDef = TypedDict(
+    "ListSolutionsResponseTypeDef",
     {
-        "solutions": List[SolutionSummaryOutputTypeDef],
+        "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommenderConfigOutputTypeDef = TypedDict(
@@ -2092,14 +2129,33 @@
         "itemExplorationConfig": Mapping[str, str],
         "minRecommendationRequestsPerSecond": int,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
+BatchInferenceJobTypeDef = TypedDict(
+    "BatchInferenceJobTypeDef",
+    {
+        "jobName": str,
+        "batchInferenceJobArn": str,
+        "filterArn": str,
+        "failureReason": str,
+        "solutionVersionArn": str,
+        "numResults": int,
+        "jobInput": BatchInferenceJobInputOutputTypeDef,
+        "jobOutput": BatchInferenceJobOutputTypeDef,
+        "batchInferenceJobConfig": BatchInferenceJobConfigOutputTypeDef,
+        "roleArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+    },
+)
+
 _RequiredCreateBatchInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchInferenceJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
         "jobInput": BatchInferenceJobInputTypeDef,
         "jobOutput": BatchInferenceJobOutputTypeDef,
@@ -2121,19 +2177,29 @@
 class CreateBatchInferenceJobRequestRequestTypeDef(
     _RequiredCreateBatchInferenceJobRequestRequestTypeDef,
     _OptionalCreateBatchInferenceJobRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeBatchInferenceJobResponseOutputTypeDef = TypedDict(
-    "DescribeBatchInferenceJobResponseOutputTypeDef",
+BatchSegmentJobTypeDef = TypedDict(
+    "BatchSegmentJobTypeDef",
     {
-        "batchInferenceJob": BatchInferenceJobOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jobName": str,
+        "batchSegmentJobArn": str,
+        "filterArn": str,
+        "failureReason": str,
+        "solutionVersionArn": str,
+        "numResults": int,
+        "jobInput": BatchSegmentJobInputOutputTypeDef,
+        "jobOutput": BatchSegmentJobOutputTypeDef,
+        "roleArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
     },
 )
 
 _RequiredCreateBatchSegmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchSegmentJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -2157,22 +2223,14 @@
 class CreateBatchSegmentJobRequestRequestTypeDef(
     _RequiredCreateBatchSegmentJobRequestRequestTypeDef,
     _OptionalCreateBatchSegmentJobRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeBatchSegmentJobResponseOutputTypeDef = TypedDict(
-    "DescribeBatchSegmentJobResponseOutputTypeDef",
-    {
-        "batchSegmentJob": BatchSegmentJobOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDatasetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetExportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "roleArn": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
@@ -2191,91 +2249,105 @@
 class CreateDatasetExportJobRequestRequestTypeDef(
     _RequiredCreateDatasetExportJobRequestRequestTypeDef,
     _OptionalCreateDatasetExportJobRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeDatasetExportJobResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetExportJobResponseOutputTypeDef",
+DatasetExportJobTypeDef = TypedDict(
+    "DatasetExportJobTypeDef",
     {
-        "datasetExportJob": DatasetExportJobOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jobName": str,
+        "datasetExportJobArn": str,
+        "datasetArn": str,
+        "ingestionMode": IngestionModeType,
+        "roleArn": str,
+        "status": str,
+        "jobOutput": DatasetExportJobOutputTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "failureReason": str,
     },
 )
 
 CreateMetricAttributionRequestRequestTypeDef = TypedDict(
     "CreateMetricAttributionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "metrics": Sequence[MetricAttributeTypeDef],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
     },
 )
 
-DescribeMetricAttributionResponseOutputTypeDef = TypedDict(
-    "DescribeMetricAttributionResponseOutputTypeDef",
+MetricAttributionTypeDef = TypedDict(
+    "MetricAttributionTypeDef",
     {
-        "metricAttribution": MetricAttributionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "metricAttributionArn": str,
+        "datasetGroupArn": str,
+        "metricsOutputConfig": MetricAttributionOutputTypeDef,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "failureReason": str,
     },
 )
 
 UpdateMetricAttributionRequestRequestTypeDef = TypedDict(
     "UpdateMetricAttributionRequestRequestTypeDef",
     {
         "addMetrics": Sequence[MetricAttributeTypeDef],
         "removeMetrics": Sequence[str],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
         "metricAttributionArn": str,
     },
     total=False,
 )
 
-CampaignOutputTypeDef = TypedDict(
-    "CampaignOutputTypeDef",
+CampaignTypeDef = TypedDict(
+    "CampaignTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestCampaignUpdate": CampaignUpdateSummaryOutputTypeDef,
+        "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
     },
 )
 
-DescribeDatasetImportJobResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetImportJobResponseOutputTypeDef",
+DescribeDatasetImportJobResponseTypeDef = TypedDict(
+    "DescribeDatasetImportJobResponseTypeDef",
     {
-        "datasetImportJob": DatasetImportJobOutputTypeDef,
+        "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetResponseOutputTypeDef",
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
     {
-        "dataset": DatasetOutputTypeDef,
+        "dataset": DatasetTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AlgorithmOutputTypeDef = TypedDict(
-    "AlgorithmOutputTypeDef",
+AlgorithmTypeDef = TypedDict(
+    "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
-        "algorithmImage": AlgorithmImageOutputTypeDef,
+        "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
-        "defaultHyperParameterRanges": DefaultHyperParameterRangesOutputTypeDef,
+        "defaultHyperParameterRanges": DefaultHyperParameterRangesTypeDef,
         "defaultResourceConfig": Dict[str, str],
         "trainingInputMode": str,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
@@ -2295,30 +2367,30 @@
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
         "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
-RecommenderSummaryOutputTypeDef = TypedDict(
-    "RecommenderSummaryOutputTypeDef",
+RecommenderSummaryTypeDef = TypedDict(
+    "RecommenderSummaryTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
         "recommenderConfig": RecommenderConfigOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-RecommenderUpdateSummaryOutputTypeDef = TypedDict(
-    "RecommenderUpdateSummaryOutputTypeDef",
+RecommenderUpdateSummaryTypeDef = TypedDict(
+    "RecommenderUpdateSummaryTypeDef",
     {
         "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
@@ -2352,26 +2424,58 @@
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
 
-DescribeCampaignResponseOutputTypeDef = TypedDict(
-    "DescribeCampaignResponseOutputTypeDef",
+DescribeBatchInferenceJobResponseTypeDef = TypedDict(
+    "DescribeBatchInferenceJobResponseTypeDef",
+    {
+        "batchInferenceJob": BatchInferenceJobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBatchSegmentJobResponseTypeDef = TypedDict(
+    "DescribeBatchSegmentJobResponseTypeDef",
+    {
+        "batchSegmentJob": BatchSegmentJobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeDatasetExportJobResponseTypeDef = TypedDict(
+    "DescribeDatasetExportJobResponseTypeDef",
+    {
+        "datasetExportJob": DatasetExportJobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeMetricAttributionResponseTypeDef = TypedDict(
+    "DescribeMetricAttributionResponseTypeDef",
+    {
+        "metricAttribution": MetricAttributionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeCampaignResponseTypeDef = TypedDict(
+    "DescribeCampaignResponseTypeDef",
     {
-        "campaign": CampaignOutputTypeDef,
+        "campaign": CampaignTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAlgorithmResponseOutputTypeDef = TypedDict(
-    "DescribeAlgorithmResponseOutputTypeDef",
+DescribeAlgorithmResponseTypeDef = TypedDict(
+    "DescribeAlgorithmResponseTypeDef",
     {
-        "algorithm": AlgorithmOutputTypeDef,
+        "algorithm": AlgorithmTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SolutionConfigOutputTypeDef = TypedDict(
     "SolutionConfigOutputTypeDef",
     {
@@ -2395,74 +2499,74 @@
         "autoMLConfig": AutoMLConfigTypeDef,
         "optimizationObjective": OptimizationObjectiveTypeDef,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
-ListRecommendersResponseOutputTypeDef = TypedDict(
-    "ListRecommendersResponseOutputTypeDef",
+ListRecommendersResponseTypeDef = TypedDict(
+    "ListRecommendersResponseTypeDef",
     {
-        "recommenders": List[RecommenderSummaryOutputTypeDef],
+        "recommenders": List[RecommenderSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommenderOutputTypeDef = TypedDict(
-    "RecommenderOutputTypeDef",
+RecommenderTypeDef = TypedDict(
+    "RecommenderTypeDef",
     {
         "recommenderArn": str,
         "datasetGroupArn": str,
         "name": str,
         "recipeArn": str,
         "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
-        "latestRecommenderUpdate": RecommenderUpdateSummaryOutputTypeDef,
+        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
         "modelMetrics": Dict[str, float],
     },
 )
 
-SolutionOutputTypeDef = TypedDict(
-    "SolutionOutputTypeDef",
+SolutionTypeDef = TypedDict(
+    "SolutionTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "datasetGroupArn": str,
         "eventType": str,
         "solutionConfig": SolutionConfigOutputTypeDef,
-        "autoMLResult": AutoMLResultOutputTypeDef,
+        "autoMLResult": AutoMLResultTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestSolutionVersion": SolutionVersionSummaryOutputTypeDef,
+        "latestSolutionVersion": SolutionVersionSummaryTypeDef,
     },
 )
 
-SolutionVersionOutputTypeDef = TypedDict(
-    "SolutionVersionOutputTypeDef",
+SolutionVersionTypeDef = TypedDict(
+    "SolutionVersionTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "eventType": str,
         "datasetGroupArn": str,
         "solutionConfig": SolutionConfigOutputTypeDef,
         "trainingHours": float,
         "trainingMode": TrainingModeType,
-        "tunedHPOParams": TunedHPOParamsOutputTypeDef,
+        "tunedHPOParams": TunedHPOParamsTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
@@ -2489,30 +2593,30 @@
 
 class CreateSolutionRequestRequestTypeDef(
     _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
 ):
     pass
 
 
-DescribeRecommenderResponseOutputTypeDef = TypedDict(
-    "DescribeRecommenderResponseOutputTypeDef",
+DescribeRecommenderResponseTypeDef = TypedDict(
+    "DescribeRecommenderResponseTypeDef",
     {
-        "recommender": RecommenderOutputTypeDef,
+        "recommender": RecommenderTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionResponseOutputTypeDef = TypedDict(
-    "DescribeSolutionResponseOutputTypeDef",
+DescribeSolutionResponseTypeDef = TypedDict(
+    "DescribeSolutionResponseTypeDef",
     {
-        "solution": SolutionOutputTypeDef,
+        "solution": SolutionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionVersionResponseOutputTypeDef = TypedDict(
-    "DescribeSolutionVersionResponseOutputTypeDef",
+DescribeSolutionVersionResponseTypeDef = TypedDict(
+    "DescribeSolutionVersionResponseTypeDef",
     {
-        "solutionVersion": SolutionVersionOutputTypeDef,
+        "solutionVersion": SolutionVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize/type_defs.pyi` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for personalize service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize.type_defs import AlgorithmImageOutputTypeDef
+    from mypy_boto3_personalize.type_defs import AlgorithmImageTypeDef
 
-    data: AlgorithmImageOutputTypeDef = {...}
+    data: AlgorithmImageTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -29,59 +29,61 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AlgorithmImageOutputTypeDef",
+    "AlgorithmImageTypeDef",
     "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
-    "AutoMLResultOutputTypeDef",
+    "AutoMLResultTypeDef",
+    "BatchInferenceJobConfigOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
+    "S3DataConfigOutputTypeDef",
     "S3DataConfigTypeDef",
-    "BatchInferenceJobSummaryOutputTypeDef",
-    "BatchSegmentJobSummaryOutputTypeDef",
+    "BatchInferenceJobSummaryTypeDef",
+    "BatchSegmentJobSummaryTypeDef",
     "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
-    "CampaignSummaryOutputTypeDef",
+    "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeOutputTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
-    "CreateBatchInferenceJobResponseOutputTypeDef",
-    "CreateBatchSegmentJobResponseOutputTypeDef",
-    "CreateCampaignResponseOutputTypeDef",
-    "CreateDatasetExportJobResponseOutputTypeDef",
-    "CreateDatasetGroupResponseOutputTypeDef",
+    "CreateBatchInferenceJobResponseTypeDef",
+    "CreateBatchSegmentJobResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDatasetExportJobResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
     "DataSourceTypeDef",
-    "CreateDatasetImportJobResponseOutputTypeDef",
-    "CreateDatasetResponseOutputTypeDef",
-    "CreateEventTrackerResponseOutputTypeDef",
-    "CreateFilterResponseOutputTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateEventTrackerResponseTypeDef",
+    "CreateFilterResponseTypeDef",
     "MetricAttributeTypeDef",
-    "CreateMetricAttributionResponseOutputTypeDef",
-    "CreateRecommenderResponseOutputTypeDef",
+    "CreateMetricAttributionResponseTypeDef",
+    "CreateRecommenderResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseOutputTypeDef",
-    "CreateSolutionResponseOutputTypeDef",
-    "CreateSolutionVersionResponseOutputTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "CreateSolutionResponseTypeDef",
+    "CreateSolutionVersionResponseTypeDef",
     "DataSourceOutputTypeDef",
-    "DatasetExportJobSummaryOutputTypeDef",
-    "DatasetGroupOutputTypeDef",
-    "DatasetGroupSummaryOutputTypeDef",
-    "DatasetImportJobSummaryOutputTypeDef",
-    "DatasetUpdateSummaryOutputTypeDef",
-    "DatasetSchemaOutputTypeDef",
-    "DatasetSchemaSummaryOutputTypeDef",
-    "DatasetSummaryOutputTypeDef",
-    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
-    "DefaultContinuousHyperParameterRangeOutputTypeDef",
-    "DefaultIntegerHyperParameterRangeOutputTypeDef",
+    "DatasetExportJobSummaryTypeDef",
+    "DatasetGroupSummaryTypeDef",
+    "DatasetGroupTypeDef",
+    "DatasetImportJobSummaryTypeDef",
+    "DatasetSchemaSummaryTypeDef",
+    "DatasetSchemaTypeDef",
+    "DatasetSummaryTypeDef",
+    "DatasetUpdateSummaryTypeDef",
+    "DefaultCategoricalHyperParameterRangeTypeDef",
+    "DefaultContinuousHyperParameterRangeTypeDef",
+    "DefaultIntegerHyperParameterRangeTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteMetricAttributionRequestRequestTypeDef",
     "DeleteRecommenderRequestRequestTypeDef",
@@ -92,31 +94,31 @@
     "DescribeBatchSegmentJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DescribeDatasetExportJobRequestRequestTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeEventTrackerRequestRequestTypeDef",
-    "EventTrackerOutputTypeDef",
+    "EventTrackerTypeDef",
     "DescribeFeatureTransformationRequestRequestTypeDef",
-    "FeatureTransformationOutputTypeDef",
+    "FeatureTransformationTypeDef",
     "DescribeFilterRequestRequestTypeDef",
-    "FilterOutputTypeDef",
+    "FilterTypeDef",
     "DescribeMetricAttributionRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
-    "RecipeOutputTypeDef",
+    "RecipeTypeDef",
     "DescribeRecommenderRequestRequestTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
     "DescribeSolutionRequestRequestTypeDef",
     "DescribeSolutionVersionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "EventTrackerSummaryOutputTypeDef",
-    "FilterSummaryOutputTypeDef",
+    "EventTrackerSummaryTypeDef",
+    "FilterSummaryTypeDef",
     "GetSolutionMetricsRequestRequestTypeDef",
-    "GetSolutionMetricsResponseOutputTypeDef",
+    "GetSolutionMetricsResponseTypeDef",
     "HPOObjectiveOutputTypeDef",
     "HPOResourceConfigOutputTypeDef",
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
     "IntegerHyperParameterRangeOutputTypeDef",
     "IntegerHyperParameterRangeTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
@@ -138,128 +140,134 @@
     "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
     "MetricAttributeOutputTypeDef",
     "ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef",
     "ListMetricAttributionsRequestRequestTypeDef",
-    "MetricAttributionSummaryOutputTypeDef",
+    "MetricAttributionSummaryTypeDef",
     "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
-    "RecipeSummaryOutputTypeDef",
+    "RecipeSummaryTypeDef",
     "ListRecommendersRequestListRecommendersPaginateTypeDef",
     "ListRecommendersRequestRequestTypeDef",
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
-    "SolutionVersionSummaryOutputTypeDef",
+    "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListSolutionsRequestRequestTypeDef",
-    "SolutionSummaryOutputTypeDef",
+    "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagOutputTypeDef",
     "OptimizationObjectiveOutputTypeDef",
     "OptimizationObjectiveTypeDef",
     "PaginatorConfigTypeDef",
     "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "ResponseMetadataTypeDef",
-    "TunedHPOParamsOutputTypeDef",
+    "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
-    "StartRecommenderResponseOutputTypeDef",
+    "StartRecommenderResponseTypeDef",
     "StopRecommenderRequestRequestTypeDef",
-    "StopRecommenderResponseOutputTypeDef",
+    "StopRecommenderResponseTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateCampaignResponseOutputTypeDef",
+    "UpdateCampaignResponseTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
-    "UpdateDatasetResponseOutputTypeDef",
-    "UpdateMetricAttributionResponseOutputTypeDef",
-    "UpdateRecommenderResponseOutputTypeDef",
+    "UpdateDatasetResponseTypeDef",
+    "UpdateMetricAttributionResponseTypeDef",
+    "UpdateRecommenderResponseTypeDef",
+    "BatchInferenceJobInputOutputTypeDef",
+    "BatchSegmentJobInputOutputTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
-    "ListBatchInferenceJobsResponseOutputTypeDef",
-    "ListBatchSegmentJobsResponseOutputTypeDef",
-    "CampaignUpdateSummaryOutputTypeDef",
+    "ListBatchInferenceJobsResponseTypeDef",
+    "ListBatchSegmentJobsResponseTypeDef",
+    "CampaignUpdateSummaryTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
-    "ListCampaignsResponseOutputTypeDef",
+    "ListCampaignsResponseTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
-    "DatasetImportJobOutputTypeDef",
-    "ListDatasetExportJobsResponseOutputTypeDef",
-    "DescribeDatasetGroupResponseOutputTypeDef",
-    "ListDatasetGroupsResponseOutputTypeDef",
-    "ListDatasetImportJobsResponseOutputTypeDef",
-    "DatasetOutputTypeDef",
-    "DescribeSchemaResponseOutputTypeDef",
-    "ListSchemasResponseOutputTypeDef",
-    "ListDatasetsResponseOutputTypeDef",
-    "DefaultHyperParameterRangesOutputTypeDef",
-    "DescribeEventTrackerResponseOutputTypeDef",
-    "DescribeFeatureTransformationResponseOutputTypeDef",
-    "DescribeFilterResponseOutputTypeDef",
-    "DescribeRecipeResponseOutputTypeDef",
-    "ListEventTrackersResponseOutputTypeDef",
-    "ListFiltersResponseOutputTypeDef",
+    "DatasetImportJobTypeDef",
+    "ListDatasetExportJobsResponseTypeDef",
+    "ListDatasetGroupsResponseTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
+    "ListDatasetImportJobsResponseTypeDef",
+    "ListSchemasResponseTypeDef",
+    "DescribeSchemaResponseTypeDef",
+    "ListDatasetsResponseTypeDef",
+    "DatasetTypeDef",
+    "DefaultHyperParameterRangesTypeDef",
+    "DescribeEventTrackerResponseTypeDef",
+    "DescribeFeatureTransformationResponseTypeDef",
+    "DescribeFilterResponseTypeDef",
+    "DescribeRecipeResponseTypeDef",
+    "ListEventTrackersResponseTypeDef",
+    "ListFiltersResponseTypeDef",
     "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
-    "ListMetricAttributionMetricsResponseOutputTypeDef",
-    "ListMetricAttributionsResponseOutputTypeDef",
-    "ListRecipesResponseOutputTypeDef",
-    "ListSolutionVersionsResponseOutputTypeDef",
-    "ListSolutionsResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
+    "ListMetricAttributionMetricsResponseTypeDef",
+    "ListMetricAttributionsResponseTypeDef",
+    "ListRecipesResponseTypeDef",
+    "ListSolutionVersionsResponseTypeDef",
+    "ListSolutionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
+    "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
-    "DescribeBatchInferenceJobResponseOutputTypeDef",
+    "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
-    "DescribeBatchSegmentJobResponseOutputTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
-    "DescribeDatasetExportJobResponseOutputTypeDef",
+    "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
-    "DescribeMetricAttributionResponseOutputTypeDef",
+    "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
-    "CampaignOutputTypeDef",
-    "DescribeDatasetImportJobResponseOutputTypeDef",
-    "DescribeDatasetResponseOutputTypeDef",
-    "AlgorithmOutputTypeDef",
+    "CampaignTypeDef",
+    "DescribeDatasetImportJobResponseTypeDef",
+    "DescribeDatasetResponseTypeDef",
+    "AlgorithmTypeDef",
     "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
-    "RecommenderSummaryOutputTypeDef",
-    "RecommenderUpdateSummaryOutputTypeDef",
+    "RecommenderSummaryTypeDef",
+    "RecommenderUpdateSummaryTypeDef",
     "CreateRecommenderRequestRequestTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
-    "DescribeCampaignResponseOutputTypeDef",
-    "DescribeAlgorithmResponseOutputTypeDef",
+    "DescribeBatchInferenceJobResponseTypeDef",
+    "DescribeBatchSegmentJobResponseTypeDef",
+    "DescribeDatasetExportJobResponseTypeDef",
+    "DescribeMetricAttributionResponseTypeDef",
+    "DescribeCampaignResponseTypeDef",
+    "DescribeAlgorithmResponseTypeDef",
     "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
-    "ListRecommendersResponseOutputTypeDef",
-    "RecommenderOutputTypeDef",
-    "SolutionOutputTypeDef",
-    "SolutionVersionOutputTypeDef",
+    "ListRecommendersResponseTypeDef",
+    "RecommenderTypeDef",
+    "SolutionTypeDef",
+    "SolutionVersionTypeDef",
     "CreateSolutionRequestRequestTypeDef",
-    "DescribeRecommenderResponseOutputTypeDef",
-    "DescribeSolutionResponseOutputTypeDef",
-    "DescribeSolutionVersionResponseOutputTypeDef",
+    "DescribeRecommenderResponseTypeDef",
+    "DescribeSolutionResponseTypeDef",
+    "DescribeSolutionVersionResponseTypeDef",
 )
 
-AlgorithmImageOutputTypeDef = TypedDict(
-    "AlgorithmImageOutputTypeDef",
+AlgorithmImageTypeDef = TypedDict(
+    "AlgorithmImageTypeDef",
     {
         "name": str,
         "dockerURI": str,
     },
 )
 
 AutoMLConfigOutputTypeDef = TypedDict(
@@ -275,29 +283,44 @@
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
 )
 
-AutoMLResultOutputTypeDef = TypedDict(
-    "AutoMLResultOutputTypeDef",
+AutoMLResultTypeDef = TypedDict(
+    "AutoMLResultTypeDef",
     {
         "bestRecipeArn": str,
     },
 )
 
+BatchInferenceJobConfigOutputTypeDef = TypedDict(
+    "BatchInferenceJobConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": Dict[str, str],
+    },
+)
+
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
 
+S3DataConfigOutputTypeDef = TypedDict(
+    "S3DataConfigOutputTypeDef",
+    {
+        "path": str,
+        "kmsKeyArn": str,
+    },
+)
+
 _RequiredS3DataConfigTypeDef = TypedDict(
     "_RequiredS3DataConfigTypeDef",
     {
         "path": str,
     },
 )
 _OptionalS3DataConfigTypeDef = TypedDict(
@@ -307,29 +330,29 @@
     },
     total=False,
 )
 
 class S3DataConfigTypeDef(_RequiredS3DataConfigTypeDef, _OptionalS3DataConfigTypeDef):
     pass
 
-BatchInferenceJobSummaryOutputTypeDef = TypedDict(
-    "BatchInferenceJobSummaryOutputTypeDef",
+BatchInferenceJobSummaryTypeDef = TypedDict(
+    "BatchInferenceJobSummaryTypeDef",
     {
         "batchInferenceJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
 )
 
-BatchSegmentJobSummaryOutputTypeDef = TypedDict(
-    "BatchSegmentJobSummaryOutputTypeDef",
+BatchSegmentJobSummaryTypeDef = TypedDict(
+    "BatchSegmentJobSummaryTypeDef",
     {
         "batchSegmentJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -348,16 +371,16 @@
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
 
-CampaignSummaryOutputTypeDef = TypedDict(
-    "CampaignSummaryOutputTypeDef",
+CampaignSummaryTypeDef = TypedDict(
+    "CampaignSummaryTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -404,48 +427,48 @@
     "TagTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
     },
 )
 
-CreateBatchInferenceJobResponseOutputTypeDef = TypedDict(
-    "CreateBatchInferenceJobResponseOutputTypeDef",
+CreateBatchInferenceJobResponseTypeDef = TypedDict(
+    "CreateBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBatchSegmentJobResponseOutputTypeDef = TypedDict(
-    "CreateBatchSegmentJobResponseOutputTypeDef",
+CreateBatchSegmentJobResponseTypeDef = TypedDict(
+    "CreateBatchSegmentJobResponseTypeDef",
     {
         "batchSegmentJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCampaignResponseOutputTypeDef = TypedDict(
-    "CreateCampaignResponseOutputTypeDef",
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetExportJobResponseOutputTypeDef = TypedDict(
-    "CreateDatasetExportJobResponseOutputTypeDef",
+CreateDatasetExportJobResponseTypeDef = TypedDict(
+    "CreateDatasetExportJobResponseTypeDef",
     {
         "datasetExportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetGroupResponseOutputTypeDef = TypedDict(
-    "CreateDatasetGroupResponseOutputTypeDef",
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
     {
         "datasetGroupArn": str,
         "domain": DomainType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -453,41 +476,41 @@
     "DataSourceTypeDef",
     {
         "dataLocation": str,
     },
     total=False,
 )
 
-CreateDatasetImportJobResponseOutputTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseOutputTypeDef",
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
     {
         "datasetImportJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDatasetResponseOutputTypeDef = TypedDict(
-    "CreateDatasetResponseOutputTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEventTrackerResponseOutputTypeDef = TypedDict(
-    "CreateEventTrackerResponseOutputTypeDef",
+CreateEventTrackerResponseTypeDef = TypedDict(
+    "CreateEventTrackerResponseTypeDef",
     {
         "eventTrackerArn": str,
         "trackingId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFilterResponseOutputTypeDef = TypedDict(
-    "CreateFilterResponseOutputTypeDef",
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
     {
         "filterArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricAttributeTypeDef = TypedDict(
@@ -495,24 +518,24 @@
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
-CreateMetricAttributionResponseOutputTypeDef = TypedDict(
-    "CreateMetricAttributionResponseOutputTypeDef",
+CreateMetricAttributionResponseTypeDef = TypedDict(
+    "CreateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRecommenderResponseOutputTypeDef = TypedDict(
-    "CreateRecommenderResponseOutputTypeDef",
+CreateRecommenderResponseTypeDef = TypedDict(
+    "CreateRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
@@ -531,165 +554,165 @@
 )
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
-CreateSchemaResponseOutputTypeDef = TypedDict(
-    "CreateSchemaResponseOutputTypeDef",
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
     {
         "schemaArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionResponseOutputTypeDef = TypedDict(
-    "CreateSolutionResponseOutputTypeDef",
+CreateSolutionResponseTypeDef = TypedDict(
+    "CreateSolutionResponseTypeDef",
     {
         "solutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSolutionVersionResponseOutputTypeDef = TypedDict(
-    "CreateSolutionVersionResponseOutputTypeDef",
+CreateSolutionVersionResponseTypeDef = TypedDict(
+    "CreateSolutionVersionResponseTypeDef",
     {
         "solutionVersionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSourceOutputTypeDef = TypedDict(
     "DataSourceOutputTypeDef",
     {
         "dataLocation": str,
     },
 )
 
-DatasetExportJobSummaryOutputTypeDef = TypedDict(
-    "DatasetExportJobSummaryOutputTypeDef",
+DatasetExportJobSummaryTypeDef = TypedDict(
+    "DatasetExportJobSummaryTypeDef",
     {
         "datasetExportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
 )
 
-DatasetGroupOutputTypeDef = TypedDict(
-    "DatasetGroupOutputTypeDef",
+DatasetGroupSummaryTypeDef = TypedDict(
+    "DatasetGroupSummaryTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
-        "roleArn": str,
-        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetGroupSummaryOutputTypeDef = TypedDict(
-    "DatasetGroupSummaryOutputTypeDef",
+DatasetGroupTypeDef = TypedDict(
+    "DatasetGroupTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "status": str,
+        "roleArn": str,
+        "kmsKeyArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "domain": DomainType,
     },
 )
 
-DatasetImportJobSummaryOutputTypeDef = TypedDict(
-    "DatasetImportJobSummaryOutputTypeDef",
+DatasetImportJobSummaryTypeDef = TypedDict(
+    "DatasetImportJobSummaryTypeDef",
     {
         "datasetImportJobArn": str,
         "jobName": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
     },
 )
 
-DatasetUpdateSummaryOutputTypeDef = TypedDict(
-    "DatasetUpdateSummaryOutputTypeDef",
+DatasetSchemaSummaryTypeDef = TypedDict(
+    "DatasetSchemaSummaryTypeDef",
     {
+        "name": str,
         "schemaArn": str,
-        "status": str,
-        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
+        "domain": DomainType,
     },
 )
 
-DatasetSchemaOutputTypeDef = TypedDict(
-    "DatasetSchemaOutputTypeDef",
+DatasetSchemaTypeDef = TypedDict(
+    "DatasetSchemaTypeDef",
     {
         "name": str,
         "schemaArn": str,
         "schema": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
     },
 )
 
-DatasetSchemaSummaryOutputTypeDef = TypedDict(
-    "DatasetSchemaSummaryOutputTypeDef",
+DatasetSummaryTypeDef = TypedDict(
+    "DatasetSummaryTypeDef",
     {
         "name": str,
-        "schemaArn": str,
+        "datasetArn": str,
+        "datasetType": str,
+        "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "domain": DomainType,
     },
 )
 
-DatasetSummaryOutputTypeDef = TypedDict(
-    "DatasetSummaryOutputTypeDef",
+DatasetUpdateSummaryTypeDef = TypedDict(
+    "DatasetUpdateSummaryTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetType": str,
+        "schemaArn": str,
         "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-DefaultCategoricalHyperParameterRangeOutputTypeDef = TypedDict(
-    "DefaultCategoricalHyperParameterRangeOutputTypeDef",
+DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
+    "DefaultCategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": List[str],
         "isTunable": bool,
     },
 )
 
-DefaultContinuousHyperParameterRangeOutputTypeDef = TypedDict(
-    "DefaultContinuousHyperParameterRangeOutputTypeDef",
+DefaultContinuousHyperParameterRangeTypeDef = TypedDict(
+    "DefaultContinuousHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": float,
         "maxValue": float,
         "isTunable": bool,
     },
 )
 
-DefaultIntegerHyperParameterRangeOutputTypeDef = TypedDict(
-    "DefaultIntegerHyperParameterRangeOutputTypeDef",
+DefaultIntegerHyperParameterRangeTypeDef = TypedDict(
+    "DefaultIntegerHyperParameterRangeTypeDef",
     {
         "name": str,
         "minValue": int,
         "maxValue": int,
         "isTunable": bool,
     },
 )
@@ -816,16 +839,16 @@
 DescribeEventTrackerRequestRequestTypeDef = TypedDict(
     "DescribeEventTrackerRequestRequestTypeDef",
     {
         "eventTrackerArn": str,
     },
 )
 
-EventTrackerOutputTypeDef = TypedDict(
-    "EventTrackerOutputTypeDef",
+EventTrackerTypeDef = TypedDict(
+    "EventTrackerTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "accountId": str,
         "trackingId": str,
         "datasetGroupArn": str,
         "status": str,
@@ -837,16 +860,16 @@
 DescribeFeatureTransformationRequestRequestTypeDef = TypedDict(
     "DescribeFeatureTransformationRequestRequestTypeDef",
     {
         "featureTransformationArn": str,
     },
 )
 
-FeatureTransformationOutputTypeDef = TypedDict(
-    "FeatureTransformationOutputTypeDef",
+FeatureTransformationTypeDef = TypedDict(
+    "FeatureTransformationTypeDef",
     {
         "name": str,
         "featureTransformationArn": str,
         "defaultParameters": Dict[str, str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
@@ -856,16 +879,16 @@
 DescribeFilterRequestRequestTypeDef = TypedDict(
     "DescribeFilterRequestRequestTypeDef",
     {
         "filterArn": str,
     },
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -884,16 +907,16 @@
 DescribeRecipeRequestRequestTypeDef = TypedDict(
     "DescribeRecipeRequestRequestTypeDef",
     {
         "recipeArn": str,
     },
 )
 
-RecipeOutputTypeDef = TypedDict(
-    "RecipeOutputTypeDef",
+RecipeTypeDef = TypedDict(
+    "RecipeTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "algorithmArn": str,
         "featureTransformationArn": str,
         "status": str,
         "description": str,
@@ -934,27 +957,27 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EventTrackerSummaryOutputTypeDef = TypedDict(
-    "EventTrackerSummaryOutputTypeDef",
+EventTrackerSummaryTypeDef = TypedDict(
+    "EventTrackerSummaryTypeDef",
     {
         "name": str,
         "eventTrackerArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-FilterSummaryOutputTypeDef = TypedDict(
-    "FilterSummaryOutputTypeDef",
+FilterSummaryTypeDef = TypedDict(
+    "FilterSummaryTypeDef",
     {
         "name": str,
         "filterArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "datasetGroupArn": str,
         "failureReason": str,
@@ -965,16 +988,16 @@
 GetSolutionMetricsRequestRequestTypeDef = TypedDict(
     "GetSolutionMetricsRequestRequestTypeDef",
     {
         "solutionVersionArn": str,
     },
 )
 
-GetSolutionMetricsResponseOutputTypeDef = TypedDict(
-    "GetSolutionMetricsResponseOutputTypeDef",
+GetSolutionMetricsResponseTypeDef = TypedDict(
+    "GetSolutionMetricsResponseTypeDef",
     {
         "solutionVersionArn": str,
         "metrics": Dict[str, float],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1245,16 +1268,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-MetricAttributionSummaryOutputTypeDef = TypedDict(
-    "MetricAttributionSummaryOutputTypeDef",
+MetricAttributionSummaryTypeDef = TypedDict(
+    "MetricAttributionSummaryTypeDef",
     {
         "name": str,
         "metricAttributionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
@@ -1278,16 +1301,16 @@
         "nextToken": str,
         "maxResults": int,
         "domain": DomainType,
     },
     total=False,
 )
 
-RecipeSummaryOutputTypeDef = TypedDict(
-    "RecipeSummaryOutputTypeDef",
+RecipeSummaryTypeDef = TypedDict(
+    "RecipeSummaryTypeDef",
     {
         "name": str,
         "recipeArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "domain": DomainType,
@@ -1345,16 +1368,16 @@
         "solutionArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionVersionSummaryOutputTypeDef = TypedDict(
-    "SolutionVersionSummaryOutputTypeDef",
+SolutionVersionSummaryTypeDef = TypedDict(
+    "SolutionVersionSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
@@ -1375,16 +1398,16 @@
         "datasetGroupArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SolutionSummaryOutputTypeDef = TypedDict(
-    "SolutionSummaryOutputTypeDef",
+SolutionSummaryTypeDef = TypedDict(
+    "SolutionSummaryTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recipeArn": str,
@@ -1455,45 +1478,45 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TunedHPOParamsOutputTypeDef = TypedDict(
-    "TunedHPOParamsOutputTypeDef",
+TunedHPOParamsTypeDef = TypedDict(
+    "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
 )
 
 StartRecommenderRequestRequestTypeDef = TypedDict(
     "StartRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StartRecommenderResponseOutputTypeDef = TypedDict(
-    "StartRecommenderResponseOutputTypeDef",
+StartRecommenderResponseTypeDef = TypedDict(
+    "StartRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRecommenderRequestRequestTypeDef = TypedDict(
     "StopRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
     },
 )
 
-StopRecommenderResponseOutputTypeDef = TypedDict(
-    "StopRecommenderResponseOutputTypeDef",
+StopRecommenderResponseTypeDef = TypedDict(
+    "StopRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopSolutionVersionCreationRequestRequestTypeDef = TypedDict(
@@ -1507,54 +1530,68 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateCampaignResponseOutputTypeDef = TypedDict(
-    "UpdateCampaignResponseOutputTypeDef",
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDatasetRequestRequestTypeDef = TypedDict(
     "UpdateDatasetRequestRequestTypeDef",
     {
         "datasetArn": str,
         "schemaArn": str,
     },
 )
 
-UpdateDatasetResponseOutputTypeDef = TypedDict(
-    "UpdateDatasetResponseOutputTypeDef",
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
     {
         "datasetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateMetricAttributionResponseOutputTypeDef = TypedDict(
-    "UpdateMetricAttributionResponseOutputTypeDef",
+UpdateMetricAttributionResponseTypeDef = TypedDict(
+    "UpdateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRecommenderResponseOutputTypeDef = TypedDict(
-    "UpdateRecommenderResponseOutputTypeDef",
+UpdateRecommenderResponseTypeDef = TypedDict(
+    "UpdateRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchInferenceJobInputOutputTypeDef = TypedDict(
+    "BatchInferenceJobInputOutputTypeDef",
+    {
+        "s3DataSource": S3DataConfigOutputTypeDef,
+    },
+)
+
+BatchSegmentJobInputOutputTypeDef = TypedDict(
+    "BatchSegmentJobInputOutputTypeDef",
+    {
+        "s3DataSource": S3DataConfigOutputTypeDef,
+    },
+)
+
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 
@@ -1601,34 +1638,34 @@
 )
 
 class MetricAttributionOutputTypeDef(
     _RequiredMetricAttributionOutputTypeDef, _OptionalMetricAttributionOutputTypeDef
 ):
     pass
 
-ListBatchInferenceJobsResponseOutputTypeDef = TypedDict(
-    "ListBatchInferenceJobsResponseOutputTypeDef",
+ListBatchInferenceJobsResponseTypeDef = TypedDict(
+    "ListBatchInferenceJobsResponseTypeDef",
     {
-        "batchInferenceJobs": List[BatchInferenceJobSummaryOutputTypeDef],
+        "batchInferenceJobs": List[BatchInferenceJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBatchSegmentJobsResponseOutputTypeDef = TypedDict(
-    "ListBatchSegmentJobsResponseOutputTypeDef",
+ListBatchSegmentJobsResponseTypeDef = TypedDict(
+    "ListBatchSegmentJobsResponseTypeDef",
     {
-        "batchSegmentJobs": List[BatchSegmentJobSummaryOutputTypeDef],
+        "batchSegmentJobs": List[BatchSegmentJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CampaignUpdateSummaryOutputTypeDef = TypedDict(
-    "CampaignUpdateSummaryOutputTypeDef",
+CampaignUpdateSummaryTypeDef = TypedDict(
+    "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
@@ -1653,18 +1690,18 @@
 )
 
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
-ListCampaignsResponseOutputTypeDef = TypedDict(
-    "ListCampaignsResponseOutputTypeDef",
+ListCampaignsResponseTypeDef = TypedDict(
+    "ListCampaignsResponseTypeDef",
     {
-        "campaigns": List[CampaignSummaryOutputTypeDef],
+        "campaigns": List[CampaignSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
@@ -1826,16 +1863,16 @@
 
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
-DatasetImportJobOutputTypeDef = TypedDict(
-    "DatasetImportJobOutputTypeDef",
+DatasetImportJobTypeDef = TypedDict(
+    "DatasetImportJobTypeDef",
     {
         "jobName": str,
         "datasetImportJobArn": str,
         "datasetArn": str,
         "dataSource": DataSourceOutputTypeDef,
         "roleArn": str,
         "status": str,
@@ -1843,144 +1880,144 @@
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "importMode": ImportModeType,
         "publishAttributionMetricsToS3": bool,
     },
 )
 
-ListDatasetExportJobsResponseOutputTypeDef = TypedDict(
-    "ListDatasetExportJobsResponseOutputTypeDef",
+ListDatasetExportJobsResponseTypeDef = TypedDict(
+    "ListDatasetExportJobsResponseTypeDef",
     {
-        "datasetExportJobs": List[DatasetExportJobSummaryOutputTypeDef],
+        "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetGroupResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseOutputTypeDef",
+ListDatasetGroupsResponseTypeDef = TypedDict(
+    "ListDatasetGroupsResponseTypeDef",
     {
-        "datasetGroup": DatasetGroupOutputTypeDef,
+        "datasetGroups": List[DatasetGroupSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetGroupsResponseOutputTypeDef = TypedDict(
-    "ListDatasetGroupsResponseOutputTypeDef",
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
     {
-        "datasetGroups": List[DatasetGroupSummaryOutputTypeDef],
-        "nextToken": str,
+        "datasetGroup": DatasetGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetImportJobsResponseOutputTypeDef = TypedDict(
-    "ListDatasetImportJobsResponseOutputTypeDef",
+ListDatasetImportJobsResponseTypeDef = TypedDict(
+    "ListDatasetImportJobsResponseTypeDef",
     {
-        "datasetImportJobs": List[DatasetImportJobSummaryOutputTypeDef],
+        "datasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetOutputTypeDef = TypedDict(
-    "DatasetOutputTypeDef",
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
-        "schemaArn": str,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "latestDatasetUpdate": DatasetUpdateSummaryOutputTypeDef,
+        "schemas": List[DatasetSchemaSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSchemaResponseOutputTypeDef = TypedDict(
-    "DescribeSchemaResponseOutputTypeDef",
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
     {
-        "schema": DatasetSchemaOutputTypeDef,
+        "schema": DatasetSchemaTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSchemasResponseOutputTypeDef = TypedDict(
-    "ListSchemasResponseOutputTypeDef",
+ListDatasetsResponseTypeDef = TypedDict(
+    "ListDatasetsResponseTypeDef",
     {
-        "schemas": List[DatasetSchemaSummaryOutputTypeDef],
+        "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDatasetsResponseOutputTypeDef = TypedDict(
-    "ListDatasetsResponseOutputTypeDef",
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
     {
-        "datasets": List[DatasetSummaryOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
     },
 )
 
-DefaultHyperParameterRangesOutputTypeDef = TypedDict(
-    "DefaultHyperParameterRangesOutputTypeDef",
+DefaultHyperParameterRangesTypeDef = TypedDict(
+    "DefaultHyperParameterRangesTypeDef",
     {
-        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeOutputTypeDef],
-        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeOutputTypeDef],
-        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeOutputTypeDef],
+        "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
+        "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
+        "categoricalHyperParameterRanges": List[DefaultCategoricalHyperParameterRangeTypeDef],
     },
 )
 
-DescribeEventTrackerResponseOutputTypeDef = TypedDict(
-    "DescribeEventTrackerResponseOutputTypeDef",
+DescribeEventTrackerResponseTypeDef = TypedDict(
+    "DescribeEventTrackerResponseTypeDef",
     {
-        "eventTracker": EventTrackerOutputTypeDef,
+        "eventTracker": EventTrackerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFeatureTransformationResponseOutputTypeDef = TypedDict(
-    "DescribeFeatureTransformationResponseOutputTypeDef",
+DescribeFeatureTransformationResponseTypeDef = TypedDict(
+    "DescribeFeatureTransformationResponseTypeDef",
     {
-        "featureTransformation": FeatureTransformationOutputTypeDef,
+        "featureTransformation": FeatureTransformationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFilterResponseOutputTypeDef = TypedDict(
-    "DescribeFilterResponseOutputTypeDef",
+DescribeFilterResponseTypeDef = TypedDict(
+    "DescribeFilterResponseTypeDef",
     {
-        "filter": FilterOutputTypeDef,
+        "filter": FilterTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecipeResponseOutputTypeDef = TypedDict(
-    "DescribeRecipeResponseOutputTypeDef",
+DescribeRecipeResponseTypeDef = TypedDict(
+    "DescribeRecipeResponseTypeDef",
     {
-        "recipe": RecipeOutputTypeDef,
+        "recipe": RecipeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEventTrackersResponseOutputTypeDef = TypedDict(
-    "ListEventTrackersResponseOutputTypeDef",
+ListEventTrackersResponseTypeDef = TypedDict(
+    "ListEventTrackersResponseTypeDef",
     {
-        "eventTrackers": List[EventTrackerSummaryOutputTypeDef],
+        "eventTrackers": List[EventTrackerSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListFiltersResponseOutputTypeDef = TypedDict(
-    "ListFiltersResponseOutputTypeDef",
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
     {
-        "Filters": List[FilterSummaryOutputTypeDef],
+        "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HyperParameterRangesOutputTypeDef = TypedDict(
     "HyperParameterRangesOutputTypeDef",
@@ -1997,61 +2034,61 @@
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMetricAttributionMetricsResponseOutputTypeDef = TypedDict(
-    "ListMetricAttributionMetricsResponseOutputTypeDef",
+ListMetricAttributionMetricsResponseTypeDef = TypedDict(
+    "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMetricAttributionsResponseOutputTypeDef = TypedDict(
-    "ListMetricAttributionsResponseOutputTypeDef",
+ListMetricAttributionsResponseTypeDef = TypedDict(
+    "ListMetricAttributionsResponseTypeDef",
     {
-        "metricAttributions": List[MetricAttributionSummaryOutputTypeDef],
+        "metricAttributions": List[MetricAttributionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRecipesResponseOutputTypeDef = TypedDict(
-    "ListRecipesResponseOutputTypeDef",
+ListRecipesResponseTypeDef = TypedDict(
+    "ListRecipesResponseTypeDef",
     {
-        "recipes": List[RecipeSummaryOutputTypeDef],
+        "recipes": List[RecipeSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionVersionsResponseOutputTypeDef = TypedDict(
-    "ListSolutionVersionsResponseOutputTypeDef",
+ListSolutionVersionsResponseTypeDef = TypedDict(
+    "ListSolutionVersionsResponseTypeDef",
     {
-        "solutionVersions": List[SolutionVersionSummaryOutputTypeDef],
+        "solutionVersions": List[SolutionVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSolutionsResponseOutputTypeDef = TypedDict(
-    "ListSolutionsResponseOutputTypeDef",
+ListSolutionsResponseTypeDef = TypedDict(
+    "ListSolutionsResponseTypeDef",
     {
-        "solutions": List[SolutionSummaryOutputTypeDef],
+        "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommenderConfigOutputTypeDef = TypedDict(
@@ -2069,14 +2106,33 @@
         "itemExplorationConfig": Mapping[str, str],
         "minRecommendationRequestsPerSecond": int,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
+BatchInferenceJobTypeDef = TypedDict(
+    "BatchInferenceJobTypeDef",
+    {
+        "jobName": str,
+        "batchInferenceJobArn": str,
+        "filterArn": str,
+        "failureReason": str,
+        "solutionVersionArn": str,
+        "numResults": int,
+        "jobInput": BatchInferenceJobInputOutputTypeDef,
+        "jobOutput": BatchInferenceJobOutputTypeDef,
+        "batchInferenceJobConfig": BatchInferenceJobConfigOutputTypeDef,
+        "roleArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+    },
+)
+
 _RequiredCreateBatchInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchInferenceJobRequestRequestTypeDef",
     {
         "jobName": str,
         "solutionVersionArn": str,
         "jobInput": BatchInferenceJobInputTypeDef,
         "jobOutput": BatchInferenceJobOutputTypeDef,
@@ -2096,19 +2152,29 @@
 
 class CreateBatchInferenceJobRequestRequestTypeDef(
     _RequiredCreateBatchInferenceJobRequestRequestTypeDef,
     _OptionalCreateBatchInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-DescribeBatchInferenceJobResponseOutputTypeDef = TypedDict(
-    "DescribeBatchInferenceJobResponseOutputTypeDef",
+BatchSegmentJobTypeDef = TypedDict(
+    "BatchSegmentJobTypeDef",
     {
-        "batchInferenceJob": BatchInferenceJobOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jobName": str,
+        "batchSegmentJobArn": str,
+        "filterArn": str,
+        "failureReason": str,
+        "solutionVersionArn": str,
+        "numResults": int,
+        "jobInput": BatchSegmentJobInputOutputTypeDef,
+        "jobOutput": BatchSegmentJobOutputTypeDef,
+        "roleArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
     },
 )
 
 _RequiredCreateBatchSegmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchSegmentJobRequestRequestTypeDef",
     {
         "jobName": str,
@@ -2130,22 +2196,14 @@
 
 class CreateBatchSegmentJobRequestRequestTypeDef(
     _RequiredCreateBatchSegmentJobRequestRequestTypeDef,
     _OptionalCreateBatchSegmentJobRequestRequestTypeDef,
 ):
     pass
 
-DescribeBatchSegmentJobResponseOutputTypeDef = TypedDict(
-    "DescribeBatchSegmentJobResponseOutputTypeDef",
-    {
-        "batchSegmentJob": BatchSegmentJobOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDatasetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetExportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "roleArn": str,
         "jobOutput": DatasetExportJobOutputTypeDef,
@@ -2162,91 +2220,105 @@
 
 class CreateDatasetExportJobRequestRequestTypeDef(
     _RequiredCreateDatasetExportJobRequestRequestTypeDef,
     _OptionalCreateDatasetExportJobRequestRequestTypeDef,
 ):
     pass
 
-DescribeDatasetExportJobResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetExportJobResponseOutputTypeDef",
+DatasetExportJobTypeDef = TypedDict(
+    "DatasetExportJobTypeDef",
     {
-        "datasetExportJob": DatasetExportJobOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jobName": str,
+        "datasetExportJobArn": str,
+        "datasetArn": str,
+        "ingestionMode": IngestionModeType,
+        "roleArn": str,
+        "status": str,
+        "jobOutput": DatasetExportJobOutputTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "failureReason": str,
     },
 )
 
 CreateMetricAttributionRequestRequestTypeDef = TypedDict(
     "CreateMetricAttributionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "metrics": Sequence[MetricAttributeTypeDef],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
     },
 )
 
-DescribeMetricAttributionResponseOutputTypeDef = TypedDict(
-    "DescribeMetricAttributionResponseOutputTypeDef",
+MetricAttributionTypeDef = TypedDict(
+    "MetricAttributionTypeDef",
     {
-        "metricAttribution": MetricAttributionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "metricAttributionArn": str,
+        "datasetGroupArn": str,
+        "metricsOutputConfig": MetricAttributionOutputTypeDef,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "failureReason": str,
     },
 )
 
 UpdateMetricAttributionRequestRequestTypeDef = TypedDict(
     "UpdateMetricAttributionRequestRequestTypeDef",
     {
         "addMetrics": Sequence[MetricAttributeTypeDef],
         "removeMetrics": Sequence[str],
         "metricsOutputConfig": MetricAttributionOutputTypeDef,
         "metricAttributionArn": str,
     },
     total=False,
 )
 
-CampaignOutputTypeDef = TypedDict(
-    "CampaignOutputTypeDef",
+CampaignTypeDef = TypedDict(
+    "CampaignTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
         "campaignConfig": CampaignConfigOutputTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestCampaignUpdate": CampaignUpdateSummaryOutputTypeDef,
+        "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
     },
 )
 
-DescribeDatasetImportJobResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetImportJobResponseOutputTypeDef",
+DescribeDatasetImportJobResponseTypeDef = TypedDict(
+    "DescribeDatasetImportJobResponseTypeDef",
     {
-        "datasetImportJob": DatasetImportJobOutputTypeDef,
+        "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDatasetResponseOutputTypeDef = TypedDict(
-    "DescribeDatasetResponseOutputTypeDef",
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
     {
-        "dataset": DatasetOutputTypeDef,
+        "dataset": DatasetTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AlgorithmOutputTypeDef = TypedDict(
-    "AlgorithmOutputTypeDef",
+AlgorithmTypeDef = TypedDict(
+    "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
-        "algorithmImage": AlgorithmImageOutputTypeDef,
+        "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
-        "defaultHyperParameterRanges": DefaultHyperParameterRangesOutputTypeDef,
+        "defaultHyperParameterRanges": DefaultHyperParameterRangesTypeDef,
         "defaultResourceConfig": Dict[str, str],
         "trainingInputMode": str,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
@@ -2266,30 +2338,30 @@
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
         "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
-RecommenderSummaryOutputTypeDef = TypedDict(
-    "RecommenderSummaryOutputTypeDef",
+RecommenderSummaryTypeDef = TypedDict(
+    "RecommenderSummaryTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
         "recommenderConfig": RecommenderConfigOutputTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
-RecommenderUpdateSummaryOutputTypeDef = TypedDict(
-    "RecommenderUpdateSummaryOutputTypeDef",
+RecommenderUpdateSummaryTypeDef = TypedDict(
+    "RecommenderUpdateSummaryTypeDef",
     {
         "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
@@ -2321,26 +2393,58 @@
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
 
-DescribeCampaignResponseOutputTypeDef = TypedDict(
-    "DescribeCampaignResponseOutputTypeDef",
+DescribeBatchInferenceJobResponseTypeDef = TypedDict(
+    "DescribeBatchInferenceJobResponseTypeDef",
+    {
+        "batchInferenceJob": BatchInferenceJobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBatchSegmentJobResponseTypeDef = TypedDict(
+    "DescribeBatchSegmentJobResponseTypeDef",
+    {
+        "batchSegmentJob": BatchSegmentJobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeDatasetExportJobResponseTypeDef = TypedDict(
+    "DescribeDatasetExportJobResponseTypeDef",
+    {
+        "datasetExportJob": DatasetExportJobTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeMetricAttributionResponseTypeDef = TypedDict(
+    "DescribeMetricAttributionResponseTypeDef",
+    {
+        "metricAttribution": MetricAttributionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeCampaignResponseTypeDef = TypedDict(
+    "DescribeCampaignResponseTypeDef",
     {
-        "campaign": CampaignOutputTypeDef,
+        "campaign": CampaignTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAlgorithmResponseOutputTypeDef = TypedDict(
-    "DescribeAlgorithmResponseOutputTypeDef",
+DescribeAlgorithmResponseTypeDef = TypedDict(
+    "DescribeAlgorithmResponseTypeDef",
     {
-        "algorithm": AlgorithmOutputTypeDef,
+        "algorithm": AlgorithmTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SolutionConfigOutputTypeDef = TypedDict(
     "SolutionConfigOutputTypeDef",
     {
@@ -2364,74 +2468,74 @@
         "autoMLConfig": AutoMLConfigTypeDef,
         "optimizationObjective": OptimizationObjectiveTypeDef,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
     total=False,
 )
 
-ListRecommendersResponseOutputTypeDef = TypedDict(
-    "ListRecommendersResponseOutputTypeDef",
+ListRecommendersResponseTypeDef = TypedDict(
+    "ListRecommendersResponseTypeDef",
     {
-        "recommenders": List[RecommenderSummaryOutputTypeDef],
+        "recommenders": List[RecommenderSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecommenderOutputTypeDef = TypedDict(
-    "RecommenderOutputTypeDef",
+RecommenderTypeDef = TypedDict(
+    "RecommenderTypeDef",
     {
         "recommenderArn": str,
         "datasetGroupArn": str,
         "name": str,
         "recipeArn": str,
         "recommenderConfig": RecommenderConfigOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
-        "latestRecommenderUpdate": RecommenderUpdateSummaryOutputTypeDef,
+        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
         "modelMetrics": Dict[str, float],
     },
 )
 
-SolutionOutputTypeDef = TypedDict(
-    "SolutionOutputTypeDef",
+SolutionTypeDef = TypedDict(
+    "SolutionTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "datasetGroupArn": str,
         "eventType": str,
         "solutionConfig": SolutionConfigOutputTypeDef,
-        "autoMLResult": AutoMLResultOutputTypeDef,
+        "autoMLResult": AutoMLResultTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "latestSolutionVersion": SolutionVersionSummaryOutputTypeDef,
+        "latestSolutionVersion": SolutionVersionSummaryTypeDef,
     },
 )
 
-SolutionVersionOutputTypeDef = TypedDict(
-    "SolutionVersionOutputTypeDef",
+SolutionVersionTypeDef = TypedDict(
+    "SolutionVersionTypeDef",
     {
         "name": str,
         "solutionVersionArn": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "eventType": str,
         "datasetGroupArn": str,
         "solutionConfig": SolutionConfigOutputTypeDef,
         "trainingHours": float,
         "trainingMode": TrainingModeType,
-        "tunedHPOParams": TunedHPOParamsOutputTypeDef,
+        "tunedHPOParams": TunedHPOParamsTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
 )
 
@@ -2456,30 +2560,30 @@
 )
 
 class CreateSolutionRequestRequestTypeDef(
     _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
 ):
     pass
 
-DescribeRecommenderResponseOutputTypeDef = TypedDict(
-    "DescribeRecommenderResponseOutputTypeDef",
+DescribeRecommenderResponseTypeDef = TypedDict(
+    "DescribeRecommenderResponseTypeDef",
     {
-        "recommender": RecommenderOutputTypeDef,
+        "recommender": RecommenderTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionResponseOutputTypeDef = TypedDict(
-    "DescribeSolutionResponseOutputTypeDef",
+DescribeSolutionResponseTypeDef = TypedDict(
+    "DescribeSolutionResponseTypeDef",
     {
-        "solution": SolutionOutputTypeDef,
+        "solution": SolutionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSolutionVersionResponseOutputTypeDef = TypedDict(
-    "DescribeSolutionVersionResponseOutputTypeDef",
+DescribeSolutionVersionResponseTypeDef = TypedDict(
+    "DescribeSolutionVersionResponseTypeDef",
     {
-        "solutionVersion": SolutionVersionOutputTypeDef,
+        "solutionVersion": SolutionVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,59 +389,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize.type_defs import (
-    AlgorithmImageOutputTypeDef,
+    AlgorithmImageTypeDef,
     AutoMLConfigOutputTypeDef,
     AutoMLConfigTypeDef,
-    AutoMLResultOutputTypeDef,
+    AutoMLResultTypeDef,
+    BatchInferenceJobConfigOutputTypeDef,
     BatchInferenceJobConfigTypeDef,
+    S3DataConfigOutputTypeDef,
     S3DataConfigTypeDef,
-    BatchInferenceJobSummaryOutputTypeDef,
-    BatchSegmentJobSummaryOutputTypeDef,
+    BatchInferenceJobSummaryTypeDef,
+    BatchSegmentJobSummaryTypeDef,
     CampaignConfigOutputTypeDef,
     CampaignConfigTypeDef,
-    CampaignSummaryOutputTypeDef,
+    CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeOutputTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeOutputTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
-    CreateBatchInferenceJobResponseOutputTypeDef,
-    CreateBatchSegmentJobResponseOutputTypeDef,
-    CreateCampaignResponseOutputTypeDef,
-    CreateDatasetExportJobResponseOutputTypeDef,
-    CreateDatasetGroupResponseOutputTypeDef,
+    CreateBatchInferenceJobResponseTypeDef,
+    CreateBatchSegmentJobResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDatasetExportJobResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
     DataSourceTypeDef,
-    CreateDatasetImportJobResponseOutputTypeDef,
-    CreateDatasetResponseOutputTypeDef,
-    CreateEventTrackerResponseOutputTypeDef,
-    CreateFilterResponseOutputTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateEventTrackerResponseTypeDef,
+    CreateFilterResponseTypeDef,
     MetricAttributeTypeDef,
-    CreateMetricAttributionResponseOutputTypeDef,
-    CreateRecommenderResponseOutputTypeDef,
+    CreateMetricAttributionResponseTypeDef,
+    CreateRecommenderResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseOutputTypeDef,
-    CreateSolutionResponseOutputTypeDef,
-    CreateSolutionVersionResponseOutputTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateSolutionResponseTypeDef,
+    CreateSolutionVersionResponseTypeDef,
     DataSourceOutputTypeDef,
-    DatasetExportJobSummaryOutputTypeDef,
-    DatasetGroupOutputTypeDef,
-    DatasetGroupSummaryOutputTypeDef,
-    DatasetImportJobSummaryOutputTypeDef,
-    DatasetUpdateSummaryOutputTypeDef,
-    DatasetSchemaOutputTypeDef,
-    DatasetSchemaSummaryOutputTypeDef,
-    DatasetSummaryOutputTypeDef,
-    DefaultCategoricalHyperParameterRangeOutputTypeDef,
-    DefaultContinuousHyperParameterRangeOutputTypeDef,
-    DefaultIntegerHyperParameterRangeOutputTypeDef,
+    DatasetExportJobSummaryTypeDef,
+    DatasetGroupSummaryTypeDef,
+    DatasetGroupTypeDef,
+    DatasetImportJobSummaryTypeDef,
+    DatasetSchemaSummaryTypeDef,
+    DatasetSchemaTypeDef,
+    DatasetSummaryTypeDef,
+    DatasetUpdateSummaryTypeDef,
+    DefaultCategoricalHyperParameterRangeTypeDef,
+    DefaultContinuousHyperParameterRangeTypeDef,
+    DefaultIntegerHyperParameterRangeTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteEventTrackerRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteMetricAttributionRequestRequestTypeDef,
     DeleteRecommenderRequestRequestTypeDef,
@@ -452,31 +454,31 @@
     DescribeBatchSegmentJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DescribeDatasetExportJobRequestRequestTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeEventTrackerRequestRequestTypeDef,
-    EventTrackerOutputTypeDef,
+    EventTrackerTypeDef,
     DescribeFeatureTransformationRequestRequestTypeDef,
-    FeatureTransformationOutputTypeDef,
+    FeatureTransformationTypeDef,
     DescribeFilterRequestRequestTypeDef,
-    FilterOutputTypeDef,
+    FilterTypeDef,
     DescribeMetricAttributionRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
-    RecipeOutputTypeDef,
+    RecipeTypeDef,
     DescribeRecommenderRequestRequestTypeDef,
     DescribeSchemaRequestRequestTypeDef,
     DescribeSolutionRequestRequestTypeDef,
     DescribeSolutionVersionRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventTrackerSummaryOutputTypeDef,
-    FilterSummaryOutputTypeDef,
+    EventTrackerSummaryTypeDef,
+    FilterSummaryTypeDef,
     GetSolutionMetricsRequestRequestTypeDef,
-    GetSolutionMetricsResponseOutputTypeDef,
+    GetSolutionMetricsResponseTypeDef,
     HPOObjectiveOutputTypeDef,
     HPOResourceConfigOutputTypeDef,
     HPOObjectiveTypeDef,
     HPOResourceConfigTypeDef,
     IntegerHyperParameterRangeOutputTypeDef,
     IntegerHyperParameterRangeTypeDef,
     ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef,
@@ -498,128 +500,134 @@
     ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     ListMetricAttributionMetricsRequestListMetricAttributionMetricsPaginateTypeDef,
     ListMetricAttributionMetricsRequestRequestTypeDef,
     MetricAttributeOutputTypeDef,
     ListMetricAttributionsRequestListMetricAttributionsPaginateTypeDef,
     ListMetricAttributionsRequestRequestTypeDef,
-    MetricAttributionSummaryOutputTypeDef,
+    MetricAttributionSummaryTypeDef,
     ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    RecipeSummaryOutputTypeDef,
+    RecipeSummaryTypeDef,
     ListRecommendersRequestListRecommendersPaginateTypeDef,
     ListRecommendersRequestRequestTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
-    SolutionVersionSummaryOutputTypeDef,
+    SolutionVersionSummaryTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListSolutionsRequestRequestTypeDef,
-    SolutionSummaryOutputTypeDef,
+    SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagOutputTypeDef,
     OptimizationObjectiveOutputTypeDef,
     OptimizationObjectiveTypeDef,
     PaginatorConfigTypeDef,
     TrainingDataConfigOutputTypeDef,
     TrainingDataConfigTypeDef,
     ResponseMetadataTypeDef,
-    TunedHPOParamsOutputTypeDef,
+    TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
-    StartRecommenderResponseOutputTypeDef,
+    StartRecommenderResponseTypeDef,
     StopRecommenderRequestRequestTypeDef,
-    StopRecommenderResponseOutputTypeDef,
+    StopRecommenderResponseTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateCampaignResponseOutputTypeDef,
+    UpdateCampaignResponseTypeDef,
     UpdateDatasetRequestRequestTypeDef,
-    UpdateDatasetResponseOutputTypeDef,
-    UpdateMetricAttributionResponseOutputTypeDef,
-    UpdateRecommenderResponseOutputTypeDef,
+    UpdateDatasetResponseTypeDef,
+    UpdateMetricAttributionResponseTypeDef,
+    UpdateRecommenderResponseTypeDef,
+    BatchInferenceJobInputOutputTypeDef,
+    BatchSegmentJobInputOutputTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
     DatasetExportJobOutputTypeDef,
     MetricAttributionOutputTypeDef,
-    ListBatchInferenceJobsResponseOutputTypeDef,
-    ListBatchSegmentJobsResponseOutputTypeDef,
-    CampaignUpdateSummaryOutputTypeDef,
+    ListBatchInferenceJobsResponseTypeDef,
+    ListBatchSegmentJobsResponseTypeDef,
+    CampaignUpdateSummaryTypeDef,
     UpdateCampaignRequestRequestTypeDef,
-    ListCampaignsResponseOutputTypeDef,
+    ListCampaignsResponseTypeDef,
     CreateCampaignRequestRequestTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateEventTrackerRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateSolutionVersionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
-    DatasetImportJobOutputTypeDef,
-    ListDatasetExportJobsResponseOutputTypeDef,
-    DescribeDatasetGroupResponseOutputTypeDef,
-    ListDatasetGroupsResponseOutputTypeDef,
-    ListDatasetImportJobsResponseOutputTypeDef,
-    DatasetOutputTypeDef,
-    DescribeSchemaResponseOutputTypeDef,
-    ListSchemasResponseOutputTypeDef,
-    ListDatasetsResponseOutputTypeDef,
-    DefaultHyperParameterRangesOutputTypeDef,
-    DescribeEventTrackerResponseOutputTypeDef,
-    DescribeFeatureTransformationResponseOutputTypeDef,
-    DescribeFilterResponseOutputTypeDef,
-    DescribeRecipeResponseOutputTypeDef,
-    ListEventTrackersResponseOutputTypeDef,
-    ListFiltersResponseOutputTypeDef,
+    DatasetImportJobTypeDef,
+    ListDatasetExportJobsResponseTypeDef,
+    ListDatasetGroupsResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    ListDatasetImportJobsResponseTypeDef,
+    ListSchemasResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    ListDatasetsResponseTypeDef,
+    DatasetTypeDef,
+    DefaultHyperParameterRangesTypeDef,
+    DescribeEventTrackerResponseTypeDef,
+    DescribeFeatureTransformationResponseTypeDef,
+    DescribeFilterResponseTypeDef,
+    DescribeRecipeResponseTypeDef,
+    ListEventTrackersResponseTypeDef,
+    ListFiltersResponseTypeDef,
     HyperParameterRangesOutputTypeDef,
     HyperParameterRangesTypeDef,
-    ListMetricAttributionMetricsResponseOutputTypeDef,
-    ListMetricAttributionsResponseOutputTypeDef,
-    ListRecipesResponseOutputTypeDef,
-    ListSolutionVersionsResponseOutputTypeDef,
-    ListSolutionsResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
+    ListMetricAttributionMetricsResponseTypeDef,
+    ListMetricAttributionsResponseTypeDef,
+    ListRecipesResponseTypeDef,
+    ListSolutionVersionsResponseTypeDef,
+    ListSolutionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RecommenderConfigOutputTypeDef,
     RecommenderConfigTypeDef,
+    BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
-    DescribeBatchInferenceJobResponseOutputTypeDef,
+    BatchSegmentJobTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
-    DescribeBatchSegmentJobResponseOutputTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
-    DescribeDatasetExportJobResponseOutputTypeDef,
+    DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
-    DescribeMetricAttributionResponseOutputTypeDef,
+    MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
-    CampaignOutputTypeDef,
-    DescribeDatasetImportJobResponseOutputTypeDef,
-    DescribeDatasetResponseOutputTypeDef,
-    AlgorithmOutputTypeDef,
+    CampaignTypeDef,
+    DescribeDatasetImportJobResponseTypeDef,
+    DescribeDatasetResponseTypeDef,
+    AlgorithmTypeDef,
     HPOConfigOutputTypeDef,
     HPOConfigTypeDef,
-    RecommenderSummaryOutputTypeDef,
-    RecommenderUpdateSummaryOutputTypeDef,
+    RecommenderSummaryTypeDef,
+    RecommenderUpdateSummaryTypeDef,
     CreateRecommenderRequestRequestTypeDef,
     UpdateRecommenderRequestRequestTypeDef,
-    DescribeCampaignResponseOutputTypeDef,
-    DescribeAlgorithmResponseOutputTypeDef,
+    DescribeBatchInferenceJobResponseTypeDef,
+    DescribeBatchSegmentJobResponseTypeDef,
+    DescribeDatasetExportJobResponseTypeDef,
+    DescribeMetricAttributionResponseTypeDef,
+    DescribeCampaignResponseTypeDef,
+    DescribeAlgorithmResponseTypeDef,
     SolutionConfigOutputTypeDef,
     SolutionConfigTypeDef,
-    ListRecommendersResponseOutputTypeDef,
-    RecommenderOutputTypeDef,
-    SolutionOutputTypeDef,
-    SolutionVersionOutputTypeDef,
+    ListRecommendersResponseTypeDef,
+    RecommenderTypeDef,
+    SolutionTypeDef,
+    SolutionVersionTypeDef,
     CreateSolutionRequestRequestTypeDef,
-    DescribeRecommenderResponseOutputTypeDef,
-    DescribeSolutionResponseOutputTypeDef,
-    DescribeSolutionVersionResponseOutputTypeDef,
+    DescribeRecommenderResponseTypeDef,
+    DescribeSolutionResponseTypeDef,
+    DescribeSolutionVersionResponseTypeDef,
 )
 
 
-def get_structure() -> AlgorithmImageOutputTypeDef:
+def get_structure() -> AlgorithmImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-1.28.3.post1/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy-boto3-personalize-1.28.3.post2/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.28.3.post1/setup.py` & `mypy-boto3-personalize-1.28.3.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Personalize 1.28.3 service generated with mypy-boto3-builder"
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

