# Comparing `tmp/labelbase-0.1.1.tar.gz` & `tmp/labelbase-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelbase-0.1.1.tar", last modified: Mon Jul 10 18:47:49 2023, max compression
+gzip compressed data, was "labelbase-0.1.2.tar", last modified: Fri Jul 14 22:14:44 2023, max compression
```

## Comparing `labelbase-0.1.1.tar` & `labelbase-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 18:47:40.000000 labelbase-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-10 18:47:49.533362 labelbase-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-10 18:47:40.000000 labelbase-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/labelbase/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26686 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/labelbase/converters/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/converters/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    26427 2023-07-10 18:47:40.000000 labelbase-0.1.1/labelbase/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:47:49.533362 labelbase-0.1.1/labelbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 18:47:49.000000 labelbase-0.1.1/labelbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:47:49.533362 labelbase-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-10 18:47:40.000000 labelbase-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 22:14:33.000000 labelbase-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 22:14:44.608208 labelbase-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 22:14:33.000000 labelbase-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/labelbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/labelbase/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/converters/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26163 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/labelbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:14:44.608208 labelbase-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 22:14:33.000000 labelbase-0.1.2/setup.py
```

### Comparing `labelbase-0.1.1/LICENSE` & `labelbase-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.1/PKG-INFO` & `labelbase-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.1
+Version: 0.1.2
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.1/labelbase/annotate.py` & `labelbase-0.1.2/labelbase/annotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                                         - "url" treats annotation input values as URLs uploads them directly
                                         - "array" converts the annotation input values into png bytes
                                         - "png" uploads png bytes directly
         divider                 :   Optional (str) - String delimiter for name paths        
     Returns
         NDJSON representation of an annotation
     """
+    
     annotation_type = ontology_index[top_level_name]["type"]
     if ontology_index['project_type'] == str(lb.MediaType.Geospatial_Tile):
         annotation_type = 'geo_' + annotation_type
 
     ndjson = {
         "uuid" : str(uuid.uuid4())
     }  
@@ -379,15 +380,14 @@
                     annotation_value = [png, "null"]
             if "classifications" in obj.keys():
                 if len(obj['classifications']) > 0:
                     return_paths = get_leaf_paths(
                         classifications=obj["classifications"], 
                         divider=divider
                     )
-                    print(return_paths)
                 else:
                     return_paths = []
             else:
                 return_paths = []
             flat_label[column_name].append([annotation_value, return_paths])
     if classifications:
         leaf_paths = get_leaf_paths(
```

### Comparing `labelbase-0.1.1/labelbase/connector.py` & `labelbase-0.1.2/labelbase/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,21 @@
                     raise ValueError(f"Invalid value in attachment column name {column_name} - must be `attachment{divider}` followed by one of the following: |{accepted_attachment_types}| followed by `{divider}column_name`")
                 x["attachment_index"][column_name] = attachment_type.upper()
             # Annotation columns --> annotation///annotation_type///top_level_class_name   
             elif input_type.lower() == "annotation":
                 annotation_type, top_level_class_name = column_name.split(divider)[1:]
                 if annotation_type.lower() not in accepted_annotation_types:
                     raise ValueError(f"Invalid value in annotation column name {column_name} - must be `annotation{divider}` followed by one of the following: |{accepted_annotation_types}| followed by `{divider}top_level_feature_name`")
-                x["annotation_index"][column_name] = top_level_class_name.lower()                    
+                x["annotation_index"][column_name] = top_level_class_name                  
             # Prediction columns --> prediction///annotation_type///top_level_class_name
             elif input_type.lower() == "prediction":
                 annotation_type, top_level_class_name = column_name.split(divider)[1:]
-                if column_type.lower() not in accepted_annotation_types:
+                if annotation_type.lower() not in accepted_annotation_types:
                     raise ValueError(f"Invalid value in prediction column name {column_name} - must be `prediction{divider}` followed by one of the following: |{accepted_annotation_types}| followed by `{divider}top_level_feature_name`")                    
-                x["prediction_index"][column_name] = top_level_class_name.lower()    
+                x["prediction_index"][column_name] = top_level_class_name   
             else:
                 continue
         else:
             # Confirm id column
             if column_name in cols:
                 x[f"{column_name}_col"] = column_name                    
             else:
```

### Comparing `labelbase-0.1.1/labelbase/converters/coco.py` & `labelbase-0.1.2/labelbase/converters/coco.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.1/labelbase/dataset.py` & `labelbase-0.1.2/labelbase/dataset.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.1/labelbase/downloader.py` & `labelbase-0.1.2/labelbase/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,34 +79,37 @@
                         flat_label["consensus_score"] = nested_label['performance_details']['consensus_score']
                 if include_performance:
                     flat_label["created_by"] = nested_label['label_details']['created_by']
                     flat_label["seconds_to_create"] = nested_label['performance_details']['seconds_to_create']
                     flat_label["seconds_to_review"] = nested_label['performance_details']['seconds_to_review']
                     flat_label["seconds_to_label"] = nested_label['performance_details']['seconds_to_create'] - nested_label['performance_details']['seconds_to_review']
                     for metadata in label['metadata_fields']:
-                        print(metadata)
-                        metadata_type = metadata_schema_to_type[metadata['schema_id']]
-                        print(metadata_schema_to_name_key.keys())
-                        print(metadata_schema_to_name_key['clhb4bzr602du072a4erfdyiu'])
                         try:
                             if metadata['value'] in metadata_schema_to_name_key.keys():
                                 name_path = metadata_schema_to_name_key[metadata['value']].split(divider)
                                 field_name = name_path[0]
                                 metadata_value = name_path[1]
+                                metadata_type = metadata_schema_to_type[metadata['value']]
                             else:
                                 field_name = metadata['schema_name']
+                                for key in metadata_schema_to_name_key.keys():
+                                    if metadata_schema_to_name_key[key] == field_name:
+                                        metadata_type = metadata_schema_to_type[key]
                                 if type(metadata['value']) == list:
                                     values = []
                                     for value in metadata['value']:
                                         values.append(value['schema_name'])
                                     metadata_value = values
                                 else:
                                     metadata_value = metadata['value']
                         except:
                             field_name = metadata['schema_name']
+                            for key in metadata_schema_to_name_key.keys():
+                                if metadata_schema_to_name_key[key] == field_name:
+                                    metadata_type = metadata_schema_to_type[key]
                             if type(metadata['value']) == list:
                                 values = []
                                 for value in metadata['value']:
                                     values.append(value['schema_name'])
                                 metadata_value = values
                             else:
                                 metadata_value = metadata['value']
```

### Comparing `labelbase-0.1.1/labelbase/masks.py` & `labelbase-0.1.2/labelbase/masks.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from labelbox import Client as labelboxClient
 
 def get_mask_from_url(url, headers, max_retries=5, n=0):
     try:
         if n >= max_retries:
             return
         r = requests.get(url, headers=headers).content
-        return np.array(Image.open(BytesIO(r)))[:,:,:3]
+        if '/index/' in url:
+            mask = np.array(Image.open(BytesIO(r)))[:,:]
+        else:
+            mask = np.array(Image.open(BytesIO(r)))[:,:,:3]
+        return mask
     except:
         return get_mask_from_url(url, headers, max_retries, n=n+1)
 
 def mask_to_bytes(client:labelboxClient, input:str, datarow_id:str, method:str="url", color=[255,255,255], output:str="png"):
     """ Given a mask input, returns a png bytearray of said mask
     Args:
         client      :   Required       - Labelbox client
@@ -50,22 +54,27 @@
     elif len(color) == 3:
         np_color = color
     else:
         raise ValueError(f"The specified color of your segmentation mask must either be a number (for 2D masks) or an RGB code (for 3D masks) - {color}")
     # Return either a numpy array or a png byte string
     if output == "array":
         return np_mask
+    
     else:
+        if '/index/' in input:
+            mask = lb_types.MaskData.from_2D_arr(arr=np_mask)
+        else:
+            mask = lb_types.MaskData(arr=np_mask)
         mask_label = lb_types.Label(
             data=lb_types.ImageData(uid=datarow_id),
             annotations=[
                 lb_types.ObjectAnnotation(
                     name="", 
                     value=lb_types.Mask(
-                        mask=lb_types.MaskData(arr=np_mask), 
+                        mask=mask,
                         color=np_color
                     )
                 )
             ]
         )
         # Convert back into ndjson
         mask_png = list(NDJsonConverter.serialize([mask_label]))[0]["mask"]["png"]
```

### Comparing `labelbase-0.1.1/labelbase/metadata.py` & `labelbase-0.1.2/labelbase/metadata.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.1/labelbase/models.py` & `labelbase-0.1.2/labelbase/models.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.1/labelbase/ontology.py` & `labelbase-0.1.2/labelbase/ontology.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.1/labelbase/uploader.py` & `labelbase-0.1.2/labelbase/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from labelbox import Client as labelboxClient
 from labelbox import Dataset as labelboxDataset
 from labelbox import Project as labelboxProject
 import uuid
-import math
 
 def create_global_key_to_label_id_dict(client:labelboxClient, project_id:str, global_keys:list):
     """ Creates a dictionary where { key=global_key : value=label_id } by exporting labels from a project
     Args:
         client          :   Required (labelbox.client.Client) - Labelbox Client object    
         project_id      :   Required (str) - Labelbox Project ID
         global_keys     :   Required (list(str)) - List of global key strings
@@ -167,15 +166,15 @@
                     print(f'Success: Upload batch number {batch_number} successful')  
     if verbose:
         print(f'Upload complete - all data rows uploaded')
     return e, upload_dict
 
 def batch_rows_to_project(
     client:labelboxClient, upload_dict:dict, priority:int=5, 
-    batch_name:str=str(uuid.uuid4()), batch_size:int=1000, verbose:bool=False):
+    batch_name:str=str(uuid.uuid4()), batch_size:int=10000, verbose:bool=False):
     """ Takes a large amount of data row IDs and creates subsets of batches to send to a project
     
     upload_dict must be in the following format:
     {
         global_key : {
             "project_id" : "" -- Labelbox Project ID to batch data rows to
         },
@@ -266,21 +265,15 @@
     else:
         return f"No annotation upload attempted - import method must be wither 'mal' or 'import' - received value {how}"
     # Dictionary where { key=project_id : value= { data_row_id : annotations_list } }
     project_id_to_upload_dict = {}
     for gk in upload_dict:
         project_id = upload_dict[gk]["project_id"]
         data_row_id = global_key_to_data_row_id[gk]
-        annotations_dict = upload_dict[gk]["annotations"]
-        annotations = []
-        for annotation in annotations_dict:
-            for key in annotation.keys():
-                print(type(annotation[key]))
-                print(annotation[key])
-                annotations.append(annotation[key])
+        annotations = upload_dict[gk]["annotations"]
         annotations_with_data_row_id = []
         for annotation in annotations:
             if "dataRow" in annotation.keys():
                 annotations_with_data_row_id.append(annotation)
             else:
                 x = annotation
                 x["dataRow"] = {"id" : data_row_id}
@@ -303,15 +296,14 @@
             upload = []
             for drid in data_row_ids:
                 upload.extend(data_row_id_to_upload[drid])
             batch_number += 1
             if verbose:
                 print(f"Batch #{batch_number}: {len(upload)} annotations for {len(data_row_ids)} data rows")
             # Upload annotations
-            print(upload)
             import_request = upload_protocol.create_from_objects(client, project_id, f"{import_name}-{batch_number}", upload)
             errors = import_request.errors
             if errors:
                 if verbose:
                     print(f'Error: upload batch number {batch_number} unsuccessful')
                 e = errors
                 break
@@ -350,14 +342,15 @@
         model_run_to_global_keys = {}
         for gk in upload_dict:
             model_run_id = upload_dict[gk]["model_run_id"]
             if model_run_id not in model_run_to_global_keys.keys():
                 model_run_to_global_keys[model_run_id] = []
             model_run_to_global_keys[model_run_id].append(gk)
         # For each model_run, batch data rows in groups of batch_size
+        batch_number = 0
         for model_run_id in model_run_to_global_keys:
             model_run = client.get_model_run(model_run_id)
             global_keys = model_run_to_global_keys[model_run_id]
             for i in range(0, len(global_keys), batch_size):
                 batch_number += 1
                 subset = global_keys[i:] if i+batch_size >= len(global_keys) else global_keys[i:i+batch_size]
                 model_run.upsert_data_rows(global_keys=subset)
```

### Comparing `labelbase-0.1.1/labelbase.egg-info/PKG-INFO` & `labelbase-0.1.2/labelbase.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.1
+Version: 0.1.2
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.1/setup.py` & `labelbase-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
       name='labelbase',
-      version='0.1.01',
+      version='0.1.02',
       author='Labelbox',
       author_email='raphael@labelbox.com',
       description='Labelbox Helper Library',      
       packages=setuptools.find_packages(),
       url="https://labelbox.com",
       long_description=long_description,
       long_description_content_type="text/markdown",
```

