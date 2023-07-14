# Comparing `tmp/labelspark-0.7.32.tar.gz` & `tmp/labelspark-0.7.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelspark-0.7.32.tar", last modified: Tue Jul 11 21:54:23 2023, max compression
+gzip compressed data, was "labelspark-0.7.33.tar", last modified: Fri Jul 14 22:18:30 2023, max compression
```

## Comparing `labelspark-0.7.32.tar` & `labelspark-0.7.33.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:54:23.230970 labelspark-0.7.32/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 21:54:14.000000 labelspark-0.7.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-11 21:54:23.230970 labelspark-0.7.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-11 21:54:14.000000 labelspark-0.7.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:54:23.230970 labelspark-0.7.32/labelspark/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/add_json_answers_to_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/bronze_to_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)    33989 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/create_labelbox_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/dataframe_schema_enrichment.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/dictionary_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/flatten_bronze_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/get_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/get_videoframe_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/is_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/jsonToDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/spark_schema_to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/update_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-07-11 21:54:14.000000 labelspark-0.7.32/labelspark/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:54:23.230970 labelspark-0.7.32/labelspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 21:54:23.000000 labelspark-0.7.32/labelspark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:54:23.230970 labelspark-0.7.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-11 21:54:14.000000 labelspark-0.7.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:18:30.242192 labelspark-0.7.33/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 22:18:16.000000 labelspark-0.7.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-14 22:18:30.242192 labelspark-0.7.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-14 22:18:16.000000 labelspark-0.7.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:18:30.238192 labelspark-0.7.33/labelspark/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/add_json_answers_to_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/bronze_to_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/create_labelbox_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/dataframe_schema_enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/dictionary_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/flatten_bronze_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/get_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/get_videoframe_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/is_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/jsonToDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/spark_schema_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/update_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-07-14 22:18:16.000000 labelspark-0.7.33/labelspark/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:18:30.242192 labelspark-0.7.33/labelspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-14 22:18:30.000000 labelspark-0.7.33/labelspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 22:18:30.000000 labelspark-0.7.33/labelspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:18:30.000000 labelspark-0.7.33/labelspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 22:18:30.000000 labelspark-0.7.33/labelspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 22:18:30.000000 labelspark-0.7.33/labelspark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:18:30.242192 labelspark-0.7.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-14 22:18:16.000000 labelspark-0.7.33/setup.py
```

### Comparing `labelspark-0.7.32/LICENSE` & `labelspark-0.7.33/LICENSE`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/PKG-INFO` & `labelspark-0.7.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.32
+Version: 0.7.33
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `labelspark-0.7.32/README.md` & `labelspark-0.7.33/README.md`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/__init__.py` & `labelspark-0.7.33/labelspark/__init__.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/add_json_answers_to_dictionary.py` & `labelspark-0.7.33/labelspark/add_json_answers_to_dictionary.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/api_key.py` & `labelspark-0.7.33/labelspark/api_key.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/bronze_to_silver.py` & `labelspark-0.7.33/labelspark/bronze_to_silver.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/client.py` & `labelspark-0.7.33/labelspark/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,23 @@
             mask_method=mask_method, verbose=verbose, divider=divider
         )
 
         for label in flattened_labels_dict:
             for key in label.keys():
                 if divider in key:
                     label[key] = json.dumps(label[key])
+                elif label[key] == None:
+                    label[key] = ""
 
-    
-        df = spark.createDataFrame(sc.parallelize(flattened_labels_dict))
+        columns = set().union(*(d.keys() for d in flattened_labels_dict))
+        struct_fields = []
+        for column in columns:
+            struct_fields.append(pyspark.sql.types.StructField(column, pyspark.sql.types.StringType(), True))
+        schema = pyspark.sql.types.StructType(struct_fields)
+        df = spark.createDataFrame(data=flattened_labels_dict, schema=schema)
         
         if verbose:
             print(f"Success: DataFrame generated")
         
         return df        
     
     def export_to_delta_table(self, project, 
@@ -124,16 +130,20 @@
         for label in flattened_labels_dict:
             for key in label.keys():
                 if divider in key:
                     label[key] = json.dumps(label[key])
                 elif label[key] == None:
                     label[key] = ""
 
-        
-        df = spark.createDataFrame(sc.parallelize(flattened_labels_dict))
+        columns = set().union(*(d.keys() for d in flattened_labels_dict))
+        struct_fields = []
+        for column in columns:
+            struct_fields.append(pyspark.sql.types.StructField(column, pyspark.sql.types.StringType(), True))
+        schema = pyspark.sql.types.StructType(struct_fields)
+        df = spark.createDataFrame(data=flattened_labels_dict, schema=schema)
         df.write.format("delta").mode(write_mode).save(table_path)
         
         if verbose:
             print(f"Success: Table saved to {table_path}")
         
         return df
     
@@ -249,55 +259,44 @@
             row_data_col=x["row_data_col"], global_key_col=x["global_key_col"], external_id_col=x["external_id_col"], 
             dataset_id_col=x["dataset_id_col"], dataset_id=dataset_id, 
             project_id_col=x["project_id_col"], project_id=project_id,
             metadata_index=x["metadata_index"], attachment_index=x["attachment_index"], 
             annotation_index=x["annotation_index"],
             upload_method=upload_method, mask_method=mask_method, divider=divider, verbose=verbose
         )    
-                
+
         # Upload your data rows to Labelbox - update upload_dict if global keys are modified during upload
         data_row_upload_results, upload_dict = batch_create_data_rows(
             client=self.lb_client, upload_dict=upload_dict, 
             skip_duplicates=skip_duplicates, divider=divider, verbose=verbose
         )
         
         # Bath to project attempt
         if actions['batch']: 
             try:
-                # Create a dictionary where {key=global_key : value=data_row_id}
-                global_keys_list = []
-                for dataset_id in upload_dict.keys():
-                    for global_key in upload_dict[dataset_id].keys():
-                        global_keys_list.append(global_key)
-                global_key_to_data_row_id = create_global_key_to_data_row_id_dict(
-                    client=self.lb_client, global_keys=global_keys_list
-                )     
-                # Create batch dictionary where {key=project_id : value=[data_row_ids]}   
-                project_id_to_batch_dict = {}                
-                for dataset_id in upload_dict:
-                    for global_key in upload_dict[dataset_id].keys():                    
-                        project_id = upload_dict[dataset_id][global_key]["project_id"]
-                        if project_id:
-                            if project_id not in project_id_to_batch_dict.keys():
-                                project_id_to_batch_dict[project_id] = []
-                            project_id_to_batch_dict[project_id].append(global_key_to_data_row_id[global_key])
                 # Labelbase command to batch data rows to projects
                 batch_to_project_results = batch_rows_to_project(
-                    client=self.lb_client, project_id_to_batch_dict=project_id_to_batch_dict, 
+                    client=self.lb_client, upload_dict=upload_dict, 
                     priority=priority, verbose=verbose
                 )
             except Exception as e:
                 actions['annotate'] = False
                 batch_to_project_results = e
         else:
             batch_to_project_results = []                
         
         # Annotation upload attempt
         if actions['annotate']:
             try:               
+                global_keys_list = []
+                for global_key in upload_dict.keys():
+                    global_keys_list.append(global_key)
+                global_key_to_data_row_id = create_global_key_to_data_row_id_dict(
+                    client=self.lb_client, global_keys=global_keys_list
+                )   
                 # Create batch dictionary where {key=project_id : value=[data_row_ids]}
                 project_id_to_upload_dict = {}
                 for dataset_id in upload_dict.keys():
                     for global_key in upload_dict[dataset_id].keys():
                         project_id = upload_dict[dataset_id][global_key]["project_id"]
                         annotations = []
                         annotations_no_data_row_id = upload_dict[dataset_id][global_key]["annotations"]
```

### Comparing `labelspark-0.7.32/labelspark/connector.py` & `labelspark-0.7.33/labelspark/connector.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/create_dataset.py` & `labelspark-0.7.33/labelspark/create_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/create_labelbox_dataset.py` & `labelspark-0.7.33/labelspark/create_labelbox_dataset.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/dataframe_schema_enrichment.py` & `labelspark-0.7.33/labelspark/dataframe_schema_enrichment.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/flatten_bronze_table.py` & `labelspark-0.7.33/labelspark/flatten_bronze_table.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/get_annotations.py` & `labelspark-0.7.33/labelspark/get_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/get_videoframe_annotations.py` & `labelspark-0.7.33/labelspark/get_videoframe_annotations.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/spark_schema_to_string.py` & `labelspark-0.7.33/labelspark/spark_schema_to_string.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/update_metadata.py` & `labelspark-0.7.33/labelspark/update_metadata.py`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/labelspark/uploader.py` & `labelspark-0.7.33/labelspark/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         extra_client                :   Ignore this value - necessary for other labelbase integrations                
     Returns:
         - global_key_to_upload_dict - Dictionary in the above format
     """     
     # Check that global key column is entirely unique values
     table_length = get_table_length(table=table, extra_client=extra_client)
     if verbose:
-        print(f'Creating upload list - {table_length} rows in Pandas DataFrame')
+        print(f'Creating upload list - {table_length} rows in Spark DataFrame')
     unique_global_key_count = len(get_unique_values(table=table, col=global_key_col, extra_client=extra_client))
     if table_length != unique_global_key_count:
         print(f"Warning: Your global key column is not unique - upload will resume, only uploading 1 data row per unique global key")      
 
     # Create your column of upload dict values using UDFs
     uploads_table = create_uploads_column(
         client=client, table=table, row_data_col=row_data_col, global_key_col=global_key_col, external_id_col=external_id_col, 
@@ -160,25 +160,22 @@
 
     table = table.withColumn(
       'uploads', data_rows_udf(
           row_data_col, global_key_col, external_id_col, lit(metadata_name_key_to_schema_bytes),
           lit(project_id_col), project_input, lit(project_id), lit(dataset_id_col), dataset_input, lit(dataset_id)
       )
     )
-    print(table.collect()[0])
     # Run a UDF to add attachments, if applicable  
     if attachment_index:
-        print(attachment_index)
         attachments_udf = udf(create_attachments, upload_schema)  # Create a UDF
         for attachment_column_name in attachment_index: # Run this UDF for each attachment column in the attachment index
             attachment_type = attachment_index[attachment_column_name]
             table = table.withColumn('uploads', attachments_udf('uploads', lit(attachment_type), attachment_column_name))        
     # Run a UDF to add metadata, if applicable
     if metadata_index:
-        print(metadata_index)
         metadata_udf = udf(create_metadata, upload_schema) # Create a UDF
         for metadata_field_name in metadata_index: # Run this UDF for each metadata field name in the metadata index
             metadata_type = metadata_index[metadata_field_name]
             metadata_column_name = f"metadata{divider}{metadata_type}{divider}{metadata_field_name}"
             table = table.withColumn(
                 'uploads', metadata_udf(
                     'uploads', lit(metadata_field_name), metadata_column_name, lit(metadata_type), lit(metadata_name_key_to_schema_bytes), lit(divider)
@@ -240,27 +237,25 @@
     return uploads_col  
 
 def create_annotations(uploads_col, top_level_feature_name, annotations, mask_method, annotation_type, project_id_to_ontology_index_bytes, divider):
     """ Function to-be-wrapped in a UDF that adds attachments to your upload dict
     """  
     project_id_to_ontology_index = json.loads(project_id_to_ontology_index_bytes)
     ontology_index = project_id_to_ontology_index[uploads_col["project_id"]]
-    print(annotations)
     if annotations is not None:
         annotation_list = []
         ndjsons = create_ndjsons(
                     top_level_name=top_level_feature_name,
                     annotation_inputs=annotations,
                     ontology_index=ontology_index,
                     mask_method=mask_method,
                     divider=divider    
                 )
         for ndjson in ndjsons:
             annotation_list.append({annotation_type:json.dumps(ndjson)})
-        print(annotation_list)
         uploads_col["annotations"].extend(
             annotation_list
         )
     return uploads_col
 
 
 def process_upload(x):
```

### Comparing `labelspark-0.7.32/labelspark.egg-info/PKG-INFO` & `labelspark-0.7.33/labelspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelspark
-Version: 0.7.32
+Version: 0.7.33
 Summary: Labelbox Connector for Databricks
 Home-page: https://github.com/Labelbox/LabelSpark.git
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `labelspark-0.7.32/labelspark.egg-info/SOURCES.txt` & `labelspark-0.7.33/labelspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labelspark-0.7.32/setup.py` & `labelspark-0.7.33/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelspark',
-    version='0.7.32',
+    version='0.7.33',
     author='Labelbox',
     author_email="raphael@labelbox.com",      
     packages=find_packages(),
     url='https://github.com/Labelbox/LabelSpark.git',
     description='Labelbox Connector for Databricks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

