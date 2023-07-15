# Comparing `tmp/longalpha_utils-0.61.tar.gz` & `tmp/longalpha_utils-0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.61.tar", last modified: Sun Jun 11 17:05:51 2023, max compression
+gzip compressed data, was "longalpha_utils-0.62.tar", last modified: Sat Jul 15 15:22:05 2023, max compression
```

## Comparing `longalpha_utils-0.61.tar` & `longalpha_utils-0.62.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:05:51.171100 longalpha_utils-0.61/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 17:05:51.171100 longalpha_utils-0.61/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:05:51.167100 longalpha_utils-0.61/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 17:05:41.000000 longalpha_utils-0.61/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 17:05:41.000000 longalpha_utils-0.61/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 17:05:41.000000 longalpha_utils-0.61/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-11 17:05:41.000000 longalpha_utils-0.61/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-11 17:05:41.000000 longalpha_utils-0.61/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-11 17:05:41.000000 longalpha_utils-0.61/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 17:05:51.171100 longalpha_utils-0.61/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 17:05:51.000000 longalpha_utils-0.61/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-11 17:05:51.000000 longalpha_utils-0.61/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 17:05:51.000000 longalpha_utils-0.61/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-11 17:05:51.000000 longalpha_utils-0.61/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 17:05:51.000000 longalpha_utils-0.61/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 17:05:51.171100 longalpha_utils-0.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-11 17:05:41.000000 longalpha_utils-0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:22:05.362236 longalpha_utils-0.62/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 15:22:05.362236 longalpha_utils-0.62/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:22:05.358236 longalpha_utils-0.62/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-15 15:21:54.000000 longalpha_utils-0.62/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:22:05.362236 longalpha_utils-0.62/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 15:22:05.000000 longalpha_utils-0.62/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:22:05.362236 longalpha_utils-0.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-15 15:21:54.000000 longalpha_utils-0.62/setup.py
```

### Comparing `longalpha_utils-0.61/longalpha_utils/messenger.py` & `longalpha_utils-0.62/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.61/longalpha_utils/transfers.py` & `longalpha_utils-0.62/longalpha_utils/transfers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+import concurrent.futures
 import os
 import tempfile
-from io import BytesIO
+from datetime import date, timedelta
 from typing import List, Optional, Dict, Any, Union
+
+import minio
 import pandas as pd
 from minio import Minio
+from minio.error import S3Error
 from pyspark.conf import SparkConf
 from pyspark.sql import SparkSession, DataFrame
-from sqlalchemy import Engine
-from sqlalchemy import create_engine
-from sqlalchemy import text
-from minio.error import S3Error
-from datetime import date, timedelta
 from pyspark.sql.utils import AnalysisException
-from longalpha_utils.utils import multi_union_by_name, get_s3_path
 from tqdm import tqdm
-import minio
+
+from longalpha_utils.utils import multi_union_by_name, get_s3_path
 
 
 def init_spark(
     spark_executor_memory: str = "30g",
     spark_driver_memory: str = "90g",
     s3_endpoint: Optional[str] = None,
     s3_access_key: Optional[str] = None,
@@ -118,15 +117,22 @@
             object_name: object name in the minio bucket
 
         Returns:
 
         """
         self.minio_client.fput_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
-    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str,  to_pickle: bool, index=False,) -> None:
+    def put(
+        self,
+        dataframe: pd.DataFrame,
+        bucket_name: str,
+        object_name: str,
+        to_pickle: bool,
+        index=False,
+    ) -> None:
         """
         put a pandas frame to parquet in s3
 
         Args:
             dataframe: a pandas dataframe
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
@@ -217,14 +223,15 @@
 
         """
         objects = self.minio_client.list_objects(bucket_name, prefix, recursive=True)
 
         for obj in objects:
             self.minio_client.remove_object(bucket_name, obj.object_name)
 
+
 #
 # def get_s3_data_spark(
 #     spark: SparkSession,
 #     start_date: date,
 #     end_date: date,
 #     bucket: str,
 #     prefix: str,
@@ -367,15 +374,15 @@
 #     if engine is None:
 #         engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
 #     query = text(sql)
 #     return pd.read_sql(sql=query, con=engine.connect(), **kwargs)
 
 
 class S3DataReader:
-    def __init__(self, start_date, end_date, s3_bucket: str, s3_prefix: str, show_missing_date: bool =True) -> None:
+    def __init__(self, start_date, end_date, s3_bucket: str, s3_prefix: str, show_missing_date: bool = True) -> None:
         """
         read pyspark data (in folder of snappy file) and pandas data (in pickle file) from s3
         Args:
             start_date: start date to get options data for
             end_date: end date to get options data for
             s3_bucket: s3 bucket name
             s3_prefix: prefix in the s3 bucket
@@ -408,28 +415,30 @@
             day:  date to get data for
             show_missing_date:  whether to print out missing dates
 
         Returns: pyspark dataframe for the day or None if the data does not exist
 
         """
         try:
-            return spark.read.parquet(get_s3_path(s3_bucket, s3_prefix, day))
+            df = spark.read.parquet(get_s3_path(s3_bucket, s3_prefix, day))
+            return df
         except AnalysisException:
             if show_missing_date:
                 print(f"Data for {day} does not exist.")
             else:
                 pass
 
     @staticmethod
     def get_pandas_data_one_day(
         mw: MinioWrapper, s3_bucket, s3_prefix, day: date, show_missing_date: bool = True
     ) -> Union[DataFrame, None]:
         try:
             object_name = os.path.join(s3_prefix, f"{day}.pkl")
-            return mw.get(bucket_name=s3_bucket, object_name=object_name, from_pickle=True)
+            df = mw.get(bucket_name=s3_bucket, object_name=object_name, from_pickle=True)
+            return df
         except minio.error.S3Error:
             if show_missing_date:
                 print(f"Data for {day} does not exist.")
             else:
                 pass
 
     def get_spark_data(self, spark: SparkSession) -> Union[DataFrame, None]:
@@ -439,48 +448,68 @@
         Args:
             spark: spark session
 
         Returns: a spark dataframe if data exists, None otherwise
 
         """
 
-        dfs = []
-        for day in tqdm(self._get_data_rage(self.start_date, self.end_date)):
-            df = self.get_spark_data_one_day(
+        def get_data(day):
+            return self.get_spark_data_one_day(
                 spark=spark,
                 s3_bucket=self.s3_bucket,
                 s3_prefix=self.s3_prefix,
                 day=day,
                 show_missing_date=self.show_missing_date,
             )
-            if df is not None:
-                dfs.append(df)
+
+        days = self._get_data_rage(self.start_date, self.end_date)
+        with concurrent.futures.ThreadPoolExecutor(max_workers=os.cpu_count()) as executor:
+            dfs = list(tqdm(executor.map(get_data, days), total=len(days)))
+        dfs = [df for df in dfs if df is not None]
         if len(dfs) == 0:
             return None
         return multi_union_by_name(dfs)
 
     def get_pandas_data(self, mw: MinioWrapper) -> Union[pd.DataFrame, None]:
         """
         Get padnas data in pickle files from s3 for a given date range
         Args:
             mw: minio wrapper
 
         Returns: a pandas dataframe if data exists, None otherwise
 
         """
 
-        dfs = []
-        for day in tqdm(self._get_data_rage(self.start_date, self.end_date)):
-            df = self.get_pandas_data_one_day(
+        def get_data(day):
+            return self.get_pandas_data_one_day(
                 mw=mw,
                 s3_bucket=self.s3_bucket,
                 s3_prefix=self.s3_prefix,
                 day=day,
                 show_missing_date=self.show_missing_date,
             )
-            if df is not None:
-                dfs.append(df)
 
+        days = self._get_data_rage(self.start_date, self.end_date)
+        with concurrent.futures.ThreadPoolExecutor(max_workers=os.cpu_count()) as executor:
+            dfs = list(tqdm(executor.map(get_data, days), total=len(days)))
+        dfs = [df for df in dfs if df is not None]
         if len(dfs) == 0:
             return None
         return pd.concat(dfs, axis=0, join="outer", ignore_index=False)
 
+
+if __name__ == "__main__":
+    from dotenv import load_dotenv
+
+    load_dotenv()
+    minio_endpoint = os.environ["MINIO_API"]
+    access_key = os.environ["MINIO_ACCESS_KEY"]
+    secret_key = os.environ["MINIO_SECRET_KEY"]
+    spark = init_spark(s3_endpoint=minio_endpoint, s3_access_key=access_key, s3_secret_key=secret_key)
+
+    options = S3DataReader(
+        start_date=date(2007, 1, 1),
+        end_date=date(2022, 12, 31),
+        s3_bucket="dev",
+        s3_prefix="raw_data/orats_options",
+        show_missing_date=False,
+    ).get_spark_data(spark=spark)
```

### Comparing `longalpha_utils-0.61/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.62/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.61/longalpha_utils/utils.py` & `longalpha_utils-0.62/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.61/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.62/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.61/setup.py` & `longalpha_utils-0.62/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.61",
+    version="0.62",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

