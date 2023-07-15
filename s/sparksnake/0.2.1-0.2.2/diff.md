# Comparing `tmp/sparksnake-0.2.1.tar.gz` & `tmp/sparksnake-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparksnake-0.2.1.tar", last modified: Fri Jul 14 12:37:36 2023, max compression
+gzip compressed data, was "sparksnake-0.2.2.tar", last modified: Sat Jul 15 19:17:03 2023, max compression
```

## Comparing `sparksnake-0.2.1.tar` & `sparksnake-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 12:37:24.000000 sparksnake-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-14 12:37:36.159620 sparksnake-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-14 12:37:24.000000 sparksnake-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:37:36.159620 sparksnake-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-14 12:37:25.000000 sparksnake-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31988 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake/tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/tester/dataframes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:37:35.000000 sparksnake-0.2.1/sparksnake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/helpers/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_glue_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_manager_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_tester_dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_utils_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.537160 sparksnake-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 19:16:50.000000 sparksnake-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-15 19:17:03.537160 sparksnake-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-15 19:16:50.000000 sparksnake-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 19:17:03.537160 sparksnake-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-15 19:16:51.000000 sparksnake-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.533160 sparksnake-0.2.2/sparksnake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31988 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39061 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.533160 sparksnake-0.2.2/sparksnake/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/tester/dataframes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.533160 sparksnake-0.2.2/sparksnake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-15 19:16:51.000000 sparksnake-0.2.2/sparksnake/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.533160 sparksnake-0.2.2/sparksnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-15 19:17:03.000000 sparksnake-0.2.2/sparksnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-15 19:17:03.000000 sparksnake-0.2.2/sparksnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 19:17:03.000000 sparksnake-0.2.2/sparksnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 19:17:03.000000 sparksnake-0.2.2/sparksnake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 19:17:03.000000 sparksnake-0.2.2/sparksnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 19:17:03.000000 sparksnake-0.2.2/sparksnake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.533160 sparksnake-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:17:03.537160 sparksnake-0.2.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/helpers/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/test_glue_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/test_manager_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20229 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/test_tester_dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-15 19:16:51.000000 sparksnake-0.2.2/tests/test_utils_log.py
```

### Comparing `sparksnake-0.2.1/LICENSE` & `sparksnake-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/PKG-INFO` & `sparksnake-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.2.1
+Version: 0.2.2
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sparksnake-0.2.1/README.md` & `sparksnake-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/setup.py` & `sparksnake-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Reading README.md for project description
 with open("README.md", "r", encoding='utf-8') as f:
     __long_description__ = f.read()
 
 # Setting up package information
 setup(
     name='sparksnake',
-    version='0.2.1',
+    version='0.2.2',
     author='Thiago Panini',
     author_email='panini.development@gmail.com',
     packages=find_packages(),
     install_requires=[
         "pyspark",
         "Faker"
     ],
```

### Comparing `sparksnake-0.2.1/sparksnake/glue.py` & `sparksnake-0.2.2/sparksnake/glue.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/sparksnake/manager.py` & `sparksnake-0.2.2/sparksnake/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -839,28 +839,36 @@
 
         # Getting a list with keys of all inner dicts from sql pipeline list
         inner_pipe_keys = [list(pipe.keys()) for pipe in spark_sql_pipeline]
 
         # Checking if the required arguments are in all inner dict keys
         for inner_key in inner_pipe_keys:
             if not all(key in inner_key for key in required_keys):
-                raise ValueError("The sql_pipeline argument doesn't have the "
-                                 "required keys for all its elements. Check "
-                                 "if all inner dictionaries on the "
-                                 "spark_sql_pipeline list have at least the "
-                                 "'step' and the 'query' keys")
+                raise ValueError("Invalid value for spark_sql_pipeline "
+                                 "argument. Please, check if all inner "
+                                 "dictionaries have the 'step' and the "
+                                 "'query' required keys defined accordingly. "
+                                 "The main reason of this validation is "
+                                 "that without the 'step' key, the method "
+                                 "won't be able to sort and set the execution "
+                                 "order. Without the 'query' key, the method "
+                                 "won't be able to run any SparkSQL query")
 
         # Checking if all step keys are integers
         step_types_validation = list(set(
             [isinstance(pipe["step"], int) for pipe in spark_sql_pipeline]
         ))[0]
         if not step_types_validation:
-            raise ValueError("The steps in the sql_pipeline argument must be "
-                             "integers. Check if all the 'step' keys in the "
-                             "inner dictionaries are integers.")
+            raise ValueError("Invalid value for spark_sql_pipeline "
+                             "argument. Please check if all inner "
+                             "dictionaries have the 'step' key defined as "
+                             "integer values. If any 'step' key for a given "
+                             "step is defined with a non integer number, the "
+                             "method won't be able to sort the steps and set "
+                             "the execution order accordingly")
 
         # Going to the method: sorting the steps in an ascending order
         sorted_spark_sql_pipeline = sorted(
             spark_sql_pipeline,
             key=lambda x: x["step"]
         )
```

### Comparing `sparksnake-0.2.1/sparksnake/tester/dataframes.py` & `sparksnake-0.2.2/sparksnake/tester/dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,27 +257,21 @@
                 fake_row.append(faker.boolean())
             elif dtype == "date":
                 fake_row.append(faker.date_this_year())
             elif dtype == "timestamp":
                 fake_row.append(faker.date_time_this_year())
             elif dtype == "array":
                 # Extracting inner array data type
-                inner_array_dtype = field.dataType.json()\
-                    .split("elementType")[-1]\
-                    .split(",")[0]\
-                    .split(":")[-1]\
-                    .replace('"', "")\
-                    .strip()\
-                    .lower()
+                inner_array_dtype = field.dataType.jsonValue()["elementType"]
 
                 # Generating fake data according to array inner type
                 if inner_array_dtype == "string":
                     array_fake_data = faker.word()
                 elif inner_array_dtype in ("int", "integer", "bigint", "long"):
-                    array_fake_data = fake_row.append(randrange(-10000, 10000))
+                    array_fake_data = randrange(-10000, 10000)
 
                 # Transforming fake data into a list and appending to the row
                 fake_row.append([array_fake_data])
 
         # Appending the row to the data list
         fake_data_list.append(fake_row)
```

### Comparing `sparksnake-0.2.1/sparksnake/utils/log.py` & `sparksnake-0.2.2/sparksnake/utils/log.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/sparksnake.egg-info/PKG-INFO` & `sparksnake-0.2.2/sparksnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.2.1
+Version: 0.2.2
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sparksnake-0.2.1/sparksnake.egg-info/SOURCES.txt` & `sparksnake-0.2.2/sparksnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/tests/conftest.py` & `sparksnake-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/tests/helpers/user_inputs.py` & `sparksnake-0.2.2/tests/helpers/user_inputs.py`

 * *Files 24% similar despite different names*

```diff
@@ -82,14 +82,24 @@
         "Type": "date",
         "nullable": True
     },
     {
         "Name": "timestamp_field",
         "Type": "timestamp",
         "nullable": False
+    },
+    {
+        "Name": "array_string_field",
+        "Type": "array<string>",
+        "nullable": True
+    },
+    {
+        "Name": "array_int_field",
+        "Type": "array<int>",
+        "nullable": True
     }
 ]
 
 # A fake dictionary with multiple info about DataFrames to be created
 FAKE_DATAFRAMES_DEFINITION = {
     "tbl_with_fake_data": {
         "name": "tbl_with_fake_data",
@@ -146,7 +156,91 @@
         ],
         "data": [
             (1, "foo"),
             (2, "bar")
         ]
     },
 }
+
+# A SparkSQL pipeline list to run_spark_sql_pipeline method
+FAKE_SPARK_SQL_PIPELINE = [
+    {
+        "step": 1,
+        "query": """
+            SELECT
+                idx,
+                2 * idx AS double_idx,
+                category
+
+            FROM tbl_with_predefined_data
+        """
+    },
+    {
+        "step": 2,
+        "query": """
+            SELECT
+                idx,
+                double_idx,
+                2 * double_idx AS quadruple_idx,
+                category
+
+            FROM step_1
+        """,
+        "create_temp_view": True,
+        "temp_view_name": "final_table"
+    }
+]
+
+
+# A SparkSQL pipeline list to test expections in run_spark_sql_pipeline method
+FAKE_SPARK_SQL_PIPELINE_WITH_STEP_ERRORS = [
+    {
+        "step": "not-an-integer",
+        "query": """
+            SELECT
+                idx,
+                2 * idx AS double_idx,
+                category
+
+            FROM tbl_with_predefined_data
+        """
+    },
+    {
+        "step": 2,
+        "query": """
+            SELECT
+                idx,
+                double_idx,
+                2 * double_idx AS quadruple_idx,
+                category
+
+            FROM step_1
+        """
+    }
+]
+
+# A SparkSQL pipeline list to test expections in run_spark_sql_pipeline method
+FAKE_SPARK_SQL_PIPELINE_WITH_MISSING_KEYS = [
+    {
+        # Missing the 'step' required key
+        "query": """
+            SELECT
+                idx,
+                2 * idx AS double_idx,
+                category
+
+            FROM tbl_with_predefined_data
+        """
+    },
+    {
+        "step": 2,
+        "query": """
+            SELECT
+                idx,
+                double_idx,
+                2 * double_idx AS quadruple_idx,
+                category
+
+            FROM step_1
+        """
+    }
+]
```

### Comparing `sparksnake-0.2.1/tests/test_glue_module.py` & `sparksnake-0.2.2/tests/test_glue_module.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.1/tests/test_manager_module.py` & `sparksnake-0.2.2/tests/test_manager_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,17 +7,31 @@
 
 ___
 """
 
 # Importing libraries
 import pytest
 
-from pyspark.sql.functions import expr
-from pyspark.sql.types import StringType, DateType, TimestampType
 from pyspark.sql.utils import AnalysisException
+from pyspark.sql.functions import expr
+from pyspark.sql.types import (
+    StringType,
+    DateType,
+    TimestampType
+)
+from pyspark.sql import (
+    DataFrame,
+    SparkSession
+)
+
+from tests.helpers.user_inputs import (
+    FAKE_SPARK_SQL_PIPELINE,
+    FAKE_SPARK_SQL_PIPELINE_WITH_STEP_ERRORS,
+    FAKE_SPARK_SQL_PIPELINE_WITH_MISSING_KEYS
+)
 
 from sparksnake.manager import SparkETLManager
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.constructor
 def test_error_on_initializing_class_with_invalid_mode():
@@ -47,19 +61,19 @@
     with pytest.raises(TypeError):
         _ = SparkETLManager(mode="glue")
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.date_transform
 def test_casting_date_column_with_date_transform_method(
-    df_fake,
-    spark_manager_default,
-    date_col="date_string_field",
-    date_col_type="date",
-    date_format="yyyy-MM-dd"
+    df_fake: DataFrame,
+    spark_manager_default: SparkETLManager,
+    date_col: str = "date_string_field",
+    date_col_type: str = "date",
+    date_format: str = "yyyy-MM-dd"
 ):
     """
     G: Given that an user has a string column in a DataFrame that has date
     information and they need to cast it to date
     W: When the date_transform method is called with the following parameters:
         - date_col="name-of-the-string-column"
         - date_col_type="date"
@@ -94,19 +108,19 @@
     assert dtype_pre_casting == StringType()
     assert dtype_pos_casting == DateType()
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.date_transform
 def test_casting_timestamp_column_with_date_transform_method(
-    df_fake,
-    spark_manager_default,
-    date_col="timestamp_string_field",
-    date_col_type="timestamp",
-    date_format="yyyy-MM-dd HH:mm:ss"
+    df_fake: DataFrame,
+    spark_manager_default: SparkETLManager,
+    date_col: str = "timestamp_string_field",
+    date_col_type: str = "timestamp",
+    date_format: str = "yyyy-MM-dd HH:mm:ss"
 ):
     """
     G: Given that an user has a string column in a DataFrame that has timestamp
     information and they need to cast it to timestamp
     W: When the date_transform method is called with the following parameters:
         - date_col="name-of-the-string-column"
         - date_col_type="timestamp"
@@ -141,19 +155,19 @@
     assert dtype_pre_casting == StringType()
     assert dtype_pos_casting == TimestampType()
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.date_transform
 def test_error_on_casting_date_column_with_invalid_date_col_type(
-    df_fake,
-    spark_manager_default,
-    date_col="date_field",
-    date_col_type="invalid_type",
-    date_format="yyyy-MM-dd"
+    df_fake: DataFrame,
+    spark_manager_default: SparkETLManager,
+    date_col: str = "date_field",
+    date_col_type: str = "invalid_type",
+    date_format: str = "yyyy-MM-dd"
 ):
     """
     G: Given that an user has a string column in a DataFrame that has date
     information and they need to cast it to date
     W: When the date_transform method is called with an invalid date_col_type
     attribute (e.g. something different from "date" or "timestamp")
     T: Then an ValueError must be raised
@@ -169,19 +183,19 @@
             cast_string_to_date=True
         )
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.date_transform
 def test_error_on_casting_date_column_with_invalid_column_name(
-    df_fake,
-    spark_manager_default,
-    date_col="invalid_column_name",
-    date_col_type="date",
-    date_format="yyyy-MM-dd HH:mm:ss"
+    df_fake: DataFrame,
+    spark_manager_default: SparkETLManager,
+    date_col: str = "invalid_column_name",
+    date_col_type: str = "date",
+    date_format: str = "yyyy-MM-dd HH:mm:ss"
 ):
     """
     G: Given that an user has a string column in a DataFrame that has date
     information and they need to cast it to date
     W: When the date_transform method is called with a column name that
     doesn't exist on DataFrame
     T: Then an AnalysisException must be raised
@@ -197,17 +211,17 @@
             cast_string_to_date=True
         )
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.date_transform
 def test_correct_col_name_after_extracting_year_info_from_date(
-    spark_manager_default,
-    df_fake,
-    date_col="date_field"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    date_col: str = "date_field"
 ):
     """
     G: Given that an user wants to add a new column to an existing DataFrame
        with year information based on a date column
     W: When the date_transform() method is executed with kwarg year=True
     T: Then there might be a new DataFrame column named "year_{date_col}"
        where {date_col} is the name of the target date column used to get the
@@ -222,17 +236,17 @@
     )
 
     assert f"year_{date_col}" in df_fake_year.schema.fieldNames()
 
 
 @pytest.mark.date_transform
 def test_correct_col_value_after_extracting_year_info_from_date(
-    spark_manager_default,
-    df_fake,
-    date_col="date_field"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    date_col: str = "date_field"
 ):
     """
     G: Given that an user wants to add a new column to an existing DataFrame
        with year information based on a date column
     W: When the date_transform() method is executed with kwarg year=True
     T: Then the new year_{date_col} field must have the expected year
        information extracted from {date_col}
@@ -253,17 +267,17 @@
 
     assert current_value == expected_value
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.date_transform
 def test_correct_col_names_after_extracting_all_date_information(
-    spark_manager_default,
-    df_fake,
-    date_col="date_field"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    date_col: str = "date_field"
 ):
     """
     G: Given that an user wants to add a new column to an existing DataFrame
        with all possible date information based on a date column
     W: When the date_transform() method is executed with kwargs year=True,
        quarter=True, month=True, dayofmonth=True, dayofweek=True,
        dayofyear=True, weekofyear=True
@@ -295,19 +309,19 @@
 
     assert all(d in new_field_names for d in expected_field_names)
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.agg_data
 def test_correct_col_names_after_aggregating_data_with_all_possible_functions(
-    spark_manager_default,
-    df_fake,
-    spark_session,
-    agg_col="integer_field",
-    group_by="boolean_field"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    spark_session: SparkSession,
+    agg_col: str = "integer_field",
+    group_by: str = "boolean_field"
 ):
     """
     G: Given that an user wants to aggregate data from a DataFrame
     W: When the agg_data() method is called to aggregate data using all
        possible functions available on method
     T: Then there might new columns with named matching the pattern
        {function}_{agg_col} where {function} is the aggreaget function flag
@@ -336,19 +350,19 @@
 
     assert all(c in df_agg.schema.fieldNames() for c in expected_columns)
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.agg_data
 def test_columns_on_groupby_list_are_part_of_schema_after_aggregating_data(
-    spark_manager_default,
-    df_fake,
-    spark_session,
-    agg_col="integer_field",
-    group_by=["string_field", "boolean_field"]
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    spark_session: SparkSession,
+    agg_col: str = "integer_field",
+    group_by: list = ["string_field", "boolean_field"]
 ):
     """
     G: Given that an user wants to aggregate data from a DataFrame
     W: When the agg_data() method is called to aggregate data using a list of
        columns on group_by argument and any agg function
     T: Then the group_by list must be on the returned DataFrame schema
     """
@@ -365,19 +379,19 @@
     # Checking if group_by list are in schema
     assert all(c in df_agg.schema.fieldNames() for c in group_by)
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.agg_data
 def test_aggregating_data_with_sum_function_returns_expected_value(
-    spark_manager_default,
-    df_fake,
-    spark_session,
-    agg_col="integer_field",
-    group_by="boolean_field"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    spark_session: SparkSession,
+    agg_col: str = "integer_field",
+    group_by: str = "boolean_field"
 ):
     """
     G: Given that an user wants to aggregate data from a DataFrame
     W: When the agg_data() method is called to aggregate data with sum
     T: Then sum_{agg_col} column value must match the expected
     """
 
@@ -403,19 +417,19 @@
 
     assert agg_result == expected_result
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.agg_data
 def test_error_on_calling_agg_data_method_with_invalid_agg_col_reference(
-    spark_manager_default,
-    df_fake,
-    spark_session,
-    agg_col="invalid_col",
-    group_by="boolean_field"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    spark_session: SparkSession,
+    agg_col: str = "invalid_col",
+    group_by: str = "boolean_field"
 ):
     """
     G: Given that an user wants to aggregate data from a DataFrame
     W: When the agg_data() method is called with a column reference for
        agg_col argument that doesn't exist on the target DataFrame
     T: Then a AnalysisException error must be raised
     """
@@ -429,19 +443,19 @@
             group_by=group_by
         )
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.agg_data
 def test_error_on_calling_agg_data_method_with_invalid_group_by_reference(
-    spark_manager_default,
-    df_fake,
-    spark_session,
-    agg_col="integer_field",
-    group_by="invalid_col"
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    spark_session: SparkSession,
+    agg_col: str = "integer_field",
+    group_by: str = "invalid_col"
 ):
     """
     G: Given that an user wants to aggregate data from a DataFrame
     W: When the agg_data() method is called with a column reference for
        group_by argument that doesn't exist on the target DataFrame
     T: Then a AnalysisException error must be raised
     """
@@ -455,18 +469,18 @@
             group_by=group_by
         )
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.add_partition_column
 def test_correct_col_name_after_adding_partition_with_add_partition_method(
-    spark_manager_default,
-    df_fake,
-    partition_name="execution_date",
-    partition_value=0
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    partition_name: str = "execution_date",
+    partition_value: int = 0
 ):
     """
     G: Given that an user wants to add a new partition column to a DataFrame
     W: When the add_partition_column() method is called
     T: Then the partition column name must exists on the returned DataFrame
     """
 
@@ -479,18 +493,18 @@
 
     assert partition_name in df_fake_partitioned.schema.fieldNames()
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.add_partition_column
 def test_correct_col_value_after_adding_partition_with_add_partition_method(
-    spark_manager_default,
-    df_fake,
-    partition_name="execution_date",
-    partition_value=0
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    partition_name: str = "execution_date",
+    partition_value: int = 0
 ):
     """
     G: Given that an user wants to add a new partition column to a DataFrame
     W: When the add_partition_column() method is called
     T: Then the partition column value must match the partition_value argument
     """
 
@@ -503,18 +517,18 @@
 
     assert df_fake_partitioned.select(partition_name).take(1)[0][0] == 0
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.add_partition_column
 def test_error_on_calling_add_partition_method_with_invalid_partition_name(
-    spark_manager_default,
-    df_fake,
-    partition_name=0,
-    partition_value=0
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame,
+    partition_name: int = 0,
+    partition_value: int = 0
 ):
     """
     G: Given that an user wants to add a new partition column to a DataFrame
     W: When the add_partition_column() method is called with an invalid value
        for partition_name argument (e.g. an integer number instead of a string
        column name reference)
     T: Then an Exception must be raised
@@ -528,16 +542,16 @@
             partition_value=partition_value
         )
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.repartition_dataframe
 def test_decreasing_dataframe_partitions_with_repartition_method(
-    spark_manager_default,
-    df_fake
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame
 ):
     """
     G: Given that an user wants to decrease the number of partitions in a
        Spark DataFrame
     W: When the repartition_dataframe() method is called with a number of
        desired partitions on num_partition arg that is LESS THAN the current
        number of DataFrame partitions
@@ -556,16 +570,16 @@
 
     assert df_repartitioned.rdd.getNumPartitions() == partitions_to_set
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.repartition_dataframe
 def test_increasing_dataframe_partitions_with_repartition_method(
-    spark_manager_default,
-    df_fake
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame
 ):
     """
     G: Given that an user wants to increase the number of partitions in a
        Spark DataFrame
     W: When the repartition_dataframe() method is called with a number of
        desired partitions on num_partition arg that is MORE THAN the current
        number of DataFrame partitions
@@ -584,16 +598,16 @@
 
     assert df_repartitioned.rdd.getNumPartitions() == partitions_to_set
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.repartition_dataframe
 def test_trying_to_repartition_dataframe_with_current_number_of_partitions(
-    spark_manager_default,
-    df_fake
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame
 ):
     """
     G: Given that an user wants to change the number of partitions in a
        Spark DataFrame
     W: When the repartition_dataframe() method is called with a number of
        desired partitions on num_partition arg that is EQUAL to the current
        number of DataFrame partitions
@@ -613,16 +627,16 @@
 
     assert df_repartitioned.rdd.getNumPartitions() == partitions_to_set
 
 
 @pytest.mark.spark_manager_default
 @pytest.mark.repartition_dataframe
 def test_trying_to_repartition_dataframe_with_negative_number_of_partitions(
-    spark_manager_default,
-    df_fake
+    spark_manager_default: SparkETLManager,
+    df_fake: DataFrame
 ):
     """
     G: Given that an user wants to change the number of partitions in a
        Spark DataFrame
     W: When the repartition_dataframe() method is called with a negative
        number of desired partitions on num_partition argument
     T: Then no operation should be done and the same DataFrame must be
@@ -636,7 +650,119 @@
     # Calling the repartition method
     df_repartitioned = spark_manager_default.repartition_dataframe(
         df=df_fake,
         num_partitions=partitions_to_set
     )
 
     assert df_repartitioned.rdd.getNumPartitions() == current_partitions
+
+
+@pytest.mark.spark_manager_default
+@pytest.mark.run_spark_sql_pipeline
+def test_run_spark_sql_pipeline_method_returns_a_spark_dataframe_object(
+    spark_manager_default: SparkETLManager,
+    dataframes_dict: dict,
+    spark_sql_pipeline: list = FAKE_SPARK_SQL_PIPELINE
+):
+    """
+    G: Given that users want to run SparkSQL queries in sequence
+    W: When the method run_spark_sql_pipeline() is called with a predefined
+       list of steps to be executed
+    T: Then the object returned by the method must be a Spark DataFrame
+    """
+
+    # Creating a Spark temp view for a given fake DataFrame
+    df_sample = dataframes_dict["df_with_predefined_data"]
+    df_sample.createOrReplaceTempView("tbl_with_predefined_data")
+
+    # Calling the method
+    df_final_step = spark_manager_default.run_spark_sql_pipeline(
+        spark_session=spark_manager_default.spark,
+        spark_sql_pipeline=spark_sql_pipeline
+    )
+
+    assert isinstance(df_final_step, DataFrame)
+
+
+@pytest.mark.spark_manager_default
+@pytest.mark.run_spark_sql_pipeline
+def test_run_spark_sql_pipeline_method_returns_a_dataframe_with_expected_cols(
+    spark_manager_default: SparkETLManager,
+    dataframes_dict: dict,
+    spark_sql_pipeline: list = FAKE_SPARK_SQL_PIPELINE
+):
+    """
+    G: Given that users want to run SparkSQL queries in sequence
+    W: When the method run_spark_sql_pipeline() is called with a predefined
+       list of steps to be executed
+    T: Then the final DataFrame returned must have a set of expected columns,
+       proving that the steps of the pipeline were succesfully executed
+    """
+
+    # Creating a Spark temp view for a given fake DataFrame
+    df_sample = dataframes_dict["df_with_predefined_data"]
+    df_sample.createOrReplaceTempView("tbl_with_predefined_data")
+
+    # Calling the method
+    df_final_step = spark_manager_default.run_spark_sql_pipeline(
+        spark_session=spark_manager_default.spark,
+        spark_sql_pipeline=spark_sql_pipeline
+    )
+
+    # Defining a list of expected columns for final step of the pipeline
+    expected_columns = ["idx", "double_idx", "quadruple_idx", "category"]
+
+    assert df_final_step.columns == expected_columns
+
+
+@pytest.mark.spark_manager_default
+@pytest.mark.run_spark_sql_pipeline
+def test_error_when_trying_to_execute_sql_pipeline_with_invalid_step_key_value(
+    spark_manager_default: SparkETLManager,
+    dataframes_dict: dict,
+    spark_sql_pipeline: list = FAKE_SPARK_SQL_PIPELINE_WITH_STEP_ERRORS
+):
+    """
+    G: Given that users want to run SparkSQL queries in sequence
+    W: When the method run_spark_sql_pipeline() is called with a predefined
+       list of steps to be executed but with the 'step' key incorrectly defined
+       (i.e. not an integer number)
+    T: Then a ValueError exception must be raised
+    """
+
+    # Creating a Spark temp view for a given fake DataFrame
+    df_sample = dataframes_dict["df_with_predefined_data"]
+    df_sample.createOrReplaceTempView("tbl_with_predefined_data")
+
+    # Calling the method
+    with pytest.raises(ValueError):
+        _ = spark_manager_default.run_spark_sql_pipeline(
+            spark_session=spark_manager_default.spark,
+            spark_sql_pipeline=spark_sql_pipeline
+        )
+
+
+@pytest.mark.spark_manager_default
+@pytest.mark.run_spark_sql_pipeline
+def test_error_when_trying_to_execute_sql_pipeline_without_required_keys(
+    spark_manager_default: SparkETLManager,
+    dataframes_dict: dict,
+    spark_sql_pipeline: list = FAKE_SPARK_SQL_PIPELINE_WITH_MISSING_KEYS
+):
+    """
+    G: Given that users want to run SparkSQL queries in sequence
+    W: When the method run_spark_sql_pipeline() is called with a predefined
+       list of steps to be executed but missing some of required keys ('step'
+       or 'query' keys)
+    T: Then a ValueError exception must be raised
+    """
+
+    # Creating a Spark temp view for a given fake DataFrame
+    df_sample = dataframes_dict["df_with_predefined_data"]
+    df_sample.createOrReplaceTempView("tbl_with_predefined_data")
+
+    # Calling the method
+    with pytest.raises(ValueError):
+        _ = spark_manager_default.run_spark_sql_pipeline(
+            spark_session=spark_manager_default.spark,
+            spark_sql_pipeline=spark_sql_pipeline
+        )
```

### Comparing `sparksnake-0.2.1/tests/test_tester_dataframes.py` & `sparksnake-0.2.2/tests/test_tester_dataframes.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,39 @@
 """
 
 # Importing libraries
 import pytest
 from decimal import Decimal
 from datetime import date, datetime
 
-from sparksnake.tester.dataframes import parse_string_to_spark_dtype,\
-    compare_schemas, generate_fake_dataframe
+from sparksnake.tester.dataframes import (
+    parse_string_to_spark_dtype,
+    compare_schemas,
+    generate_fake_dataframe
+)
 
-from tests.helpers.user_inputs import FAKE_SCHEMA_INFO,\
+from tests.helpers.user_inputs import (
+    FAKE_SCHEMA_INFO,
     FAKE_DATAFRAMES_DEFINITION
+)
 
-from pyspark.sql.types import StringType, IntegerType, LongType, DecimalType,\
-    FloatType, DoubleType, BooleanType, DateType, TimestampType, StructType
 from pyspark.sql import DataFrame
+from pyspark.sql.types import (
+    StringType,
+    IntegerType,
+    LongType,
+    DecimalType,
+    FloatType,
+    DoubleType,
+    BooleanType,
+    DateType,
+    TimestampType,
+    StructType,
+    ArrayType
+)
 
 
 @pytest.mark.tester
 @pytest.mark.dataframes
 @pytest.mark.parse_string_to_spark_dtype
 def test_string_reference_correctly_parsed_as_spark_string_dype_object():
     """
@@ -186,14 +202,78 @@
 
     assert parse_string_to_spark_dtype("timestamp") == TimestampType
 
 
 @pytest.mark.tester
 @pytest.mark.dataframes
 @pytest.mark.parse_string_to_spark_dtype
+def test_array_str_reference_correctly_parsed_as_spark_timestamp_dype_object():
+    """
+    G: Given that users want to get a valid Spark dtype object based on a
+       python string reference
+    W: When the function parse_string_to_spark_dtype() is called with dtype
+       argument equals to "array<string>"
+    T: Then the return must be a ArrayType(StringType()) object
+    """
+
+    dtype = parse_string_to_spark_dtype(dtype="array<string>")
+    assert dtype == ArrayType(StringType())
+
+
+@pytest.mark.tester
+@pytest.mark.dataframes
+@pytest.mark.parse_string_to_spark_dtype
+def test_array_int_reference_correctly_parsed_as_spark_timestamp_dype_object():
+    """
+    G: Given that users want to get a valid Spark dtype object based on a
+       python string reference
+    W: When the function parse_string_to_spark_dtype() is called with dtype
+       argument equals to "array<int>"
+    T: Then the return must be a ArrayType(IntegerType()) object
+    """
+
+    dtype = parse_string_to_spark_dtype(dtype="array<int>")
+    assert dtype == ArrayType(IntegerType())
+
+
+@pytest.mark.tester
+@pytest.mark.dataframes
+@pytest.mark.parse_string_to_spark_dtype
+def test_error_on_try_to_parse_an_array_type_with_a_not_supported_inner_type():
+    """
+    G: Given that users want to get a valid Spark dtype object based on a
+       python string reference
+    W: When the function parse_string_to_spark_dtype() is called with dtype
+       argument equals to "array<foo>"
+    T: Then a TypeError must be raised
+    """
+
+    with pytest.raises(TypeError):
+        _ = parse_string_to_spark_dtype(dtype="array<foo>")
+
+
+@pytest.mark.tester
+@pytest.mark.dataframes
+@pytest.mark.parse_string_to_spark_dtype
+def test_error_on_try_to_parse_an_array_type_with_an_invalid_string_type_ref():
+    """
+    G: Given that users want to get a valid Spark dtype object based on a
+       python string reference
+    W: When the function parse_string_to_spark_dtype() is called with dtype
+       argument equals to "array(string)"
+    T: Then a TypeError must be raised
+    """
+
+    with pytest.raises(TypeError):
+        _ = parse_string_to_spark_dtype(dtype="array(string)")
+
+
+@pytest.mark.tester
+@pytest.mark.dataframes
+@pytest.mark.parse_string_to_spark_dtype
 def test_error_when_trying_to_parse_an_invalid_string_to_spark_dtype():
     """
     G: Given that users want to get a valid Spark dtype object based on a
        python string reference
     W: When the function parse_string_to_spark_dtype() is called with dtype
        argument assuming a string reference that is not parseable as a valid
        Spark dtype (i.e. "foo")
@@ -255,18 +335,26 @@
     """
 
     # Extracting the field names of the user predefined attributes list
     expected_dtypes = [
         parse_string_to_spark_dtype(f["Type"]) for f in FAKE_SCHEMA_INFO
     ]
 
+    # Considering a special condition with array data types
+    expected_dtypes_prep = [
+        dtype() if dtype.typeName() != "array" else dtype
+        for dtype in expected_dtypes
+    ]
+
     # Extracting the data types on the returned schema
-    schema_dtypes = [type(field.dataType) for field in fake_schema]
+    schema_dtypes = [
+        field.dataType for field in fake_schema
+    ]
 
-    assert schema_dtypes == expected_dtypes
+    assert schema_dtypes == expected_dtypes_prep
 
 
 @pytest.mark.tester
 @pytest.mark.dataframes
 @pytest.mark.generate_fake_data_from_schema
 def test_function_generate_fake_data_from_schema_returns_a_list(fake_data):
     """
@@ -330,17 +418,19 @@
     # Extracting data types of the generated fake data
     fake_data_types = [[type(element) for element in row] for row in fake_data]
 
     # Getting a sample row to compare
     row_data_types = fake_data_types[0]
 
     # Creating an expected list of data types
-    expec_types = [str, int, int, Decimal, float, float, bool, date, datetime]
+    expected_python_types = [
+        str, int, int, Decimal, float, float, bool, date, datetime, list, list
+    ]
 
-    assert row_data_types == expec_types
+    assert row_data_types == expected_python_types
 
 
 @pytest.mark.tester
 @pytest.mark.dataframes
 @pytest.mark.generate_fake_dataframe
 def test_function_generate_fake_dataframe_returns_a_spark_dataframe_object(
     df_fake
```

### Comparing `sparksnake-0.2.1/tests/test_utils_log.py` & `sparksnake-0.2.2/tests/test_utils_log.py`

 * *Files identical despite different names*

