# Comparing `tmp/irisml-tasks-azure-computervision-0.0.1.tar.gz` & `tmp/irisml-tasks-azure-computervision-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azure-computervision-0.0.1.tar", last modified: Sat Jul  8 06:33:17 2023, max compression
+gzip compressed data, was "irisml-tasks-azure-computervision-0.0.3.tar", last modified: Fri Jul 14 23:23:38 2023, max compression
```

## Comparing `irisml-tasks-azure-computervision-0.0.1.tar` & `irisml-tasks-azure-computervision-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/
--rw-r--r--   0 shono     (1000) shono     (1000)     1141 2023-07-08 06:20:37.000000 irisml-tasks-azure-computervision-0.0.1/LICENSE
--rw-r--r--   0 shono     (1000) shono     (1000)     1815 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)     1497 2023-07-08 06:22:12.000000 irisml-tasks-azure-computervision-0.0.1/README.md
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/irisml/
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/irisml/tasks/
--rw-r--r--   0 shono     (1000) shono     (1000)     1538 2023-07-08 06:20:37.000000 irisml-tasks-azure-computervision-0.0.1/irisml/tasks/create_azure_computervision_caption_model.py
--rw-r--r--   0 shono     (1000) shono     (1000)     3944 2023-07-08 06:26:18.000000 irisml-tasks-azure-computervision-0.0.1/irisml/tasks/create_azure_computervision_classification_model.py
--rw-r--r--   0 shono     (1000) shono     (1000)     1652 2023-07-08 06:26:06.000000 irisml-tasks-azure-computervision-0.0.1/irisml/tasks/create_azure_computervision_ocr_model.py
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/
--rw-r--r--   0 shono     (1000) shono     (1000)     1815 2023-07-08 06:33:17.000000 irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)      558 2023-07-08 06:33:17.000000 irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        1 2023-07-08 06:33:17.000000 irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       35 2023-07-08 06:33:17.000000 irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/requires.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        7 2023-07-08 06:33:17.000000 irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/top_level.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       81 2023-07-08 06:20:37.000000 irisml-tasks-azure-computervision-0.0.1/pyproject.toml
--rw-r--r--   0 shono     (1000) shono     (1000)      549 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/setup.cfg
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-07-08 06:33:17.730721 irisml-tasks-azure-computervision-0.0.1/test/
--rw-r--r--   0 shono     (1000) shono     (1000)      771 2023-07-08 06:20:37.000000 irisml-tasks-azure-computervision-0.0.1/test/test_create_azure_computervision_caption_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.020494 irisml-tasks-azure-computervision-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-14 23:23:38.020494 irisml-tasks-azure-computervision-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.012493 irisml-tasks-azure-computervision-0.0.3/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.016493 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.016493 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 23:23:38.020494 irisml-tasks-azure-computervision-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.016493 irisml-tasks-azure-computervision-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_train_azure_computervision_custom_model.py
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/LICENSE` & `irisml-tasks-azure-computervision-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.1/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.1
+Version: 0.0.3
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/README.md` & `irisml-tasks-azure-computervision-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.1/irisml/tasks/create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.1/irisml/tasks/create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_classification_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     class Outputs:
         model: torch.nn.Module
 
     def execute(self, inputs):
         if not self.config.endpoint.startswith('https://'):
             raise ValueError('endpoint must start with https://')
 
-        model = AzureComputervisionCaptionModel(self.config.endpoint, self.config.api_key)
+        model = AzureComputervisionClassificationModel(self.config.endpoint, self.config.api_key)
         return self.Outputs(model=model)
 
     def dry_run(self, inputs):
         return self.execute(inputs)
 
 
 def _should_retry(exception):
@@ -60,32 +60,34 @@
     def __init__(self, endpoint, api_key):
         super().__init__()
         self._endpoint = endpoint
         self._api_key = api_key
         self._url = self.get_url(endpoint)
 
     def forward(self, inputs) -> typing.List[str]:
-        texts = []
+        responses = []
         for image in inputs:
             image_bytes = self._get_image_bytes(image)
+            response = None
             try:
                 response = self._request(image_bytes)
             except Exception:
                 logger.exception("Failed to request to Azure Computer Vision API")
-                response = ''
-            logger.info(f"Genrated text: {repr(response)}")
-            texts.append(response)
-        return texts
+            responses.append(response)
+        return self.collate_result(responses)
 
     def get_url(self, endpoint):
         raise NotImplementedError
 
     def parse_response(self, response_body):
         raise NotImplementedError
 
+    def collate_result(self, batch):
+        return [b if b else '' for b in batch]
+
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), retry=tenacity.retry_if_exception(_should_retry))
     def _request(self, image_bytes):
         headers = {'Ocp-Apim-Subscription-Key': self._api_key, 'Content-Type': 'image/png'}
         response = None
         try:
             response = requests.post(self._url, headers=headers, data=image_bytes)
             response.raise_for_status()
@@ -105,13 +107,13 @@
             with io.BytesIO() as f:
                 image.save(f, format='PNG')
                 return f.getvalue()
 
         raise TypeError(f"image must be PIL.Image.Image or torch.Tensor, but got {type(image)}")
 
 
-class AzureComputervisionCaptionModel(AzureComputerVisionModel):
+class AzureComputervisionClassificationModel(AzureComputerVisionModel):
     def get_url(self, endpoint):
         return urllib.parse.urljoin(endpoint, '/computervision/imageanalysis:analyze?api-version=2023-04-01-preview&features=tags')
 
     def parse_response(self, response_body):
         return [t['name'] for t in response_body['tagsResult']['values']]
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/irisml/tasks/create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_ocr_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,35 +20,30 @@
     """
     VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Config:
         endpoint: str
         api_key: str
-        delimiter: str = '\n'
 
     @dataclasses.dataclass
     class Outputs:
         model: torch.nn.Module
 
     def execute(self, inputs):
         if not self.config.endpoint.startswith('https://'):
             raise ValueError('endpoint must start with https://')
 
-        model = AzureComputervisionOcrModel(self.config.endpoint, self.config.api_key, self.config.delimiter)
+        model = AzureComputervisionOcrModel(self.config.endpoint, self.config.api_key)
         return self.Outputs(model=model)
 
     def dry_run(self, inputs):
         return self.execute(inputs)
 
 
 class AzureComputervisionOcrModel(AzureComputerVisionModel):
-    def __init__(self, endpoint, api_key, delimiter):
-        super().__init__(endpoint, api_key)
-        self._delimiter = delimiter
-
     def get_url(self, endpoint):
         return urllib.parse.urljoin(endpoint, '/computervision/imageanalysis:analyze?api-version=2023-04-01-preview&features=read')
 
     def parse_response(self, response_body):
         # TODO: Should we use words/spans?
         return response_body['readResult']['content']
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.1
+Version: 0.0.3
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/irisml_tasks_azure_computervision.egg-info/SOURCES.txt` & `irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 irisml/tasks/create_azure_computervision_caption_model.py
 irisml/tasks/create_azure_computervision_classification_model.py
+irisml/tasks/create_azure_computervision_custom_model.py
 irisml/tasks/create_azure_computervision_ocr_model.py
+irisml/tasks/delete_azure_computervision_custom_model.py
+irisml/tasks/train_azure_computervision_custom_model.py
 irisml_tasks_azure_computervision.egg-info/PKG-INFO
 irisml_tasks_azure_computervision.egg-info/SOURCES.txt
 irisml_tasks_azure_computervision.egg-info/dependency_links.txt
 irisml_tasks_azure_computervision.egg-info/requires.txt
 irisml_tasks_azure_computervision.egg-info/top_level.txt
-test/test_create_azure_computervision_caption_model.py
+test/test_create_azure_computervision_caption_model.py
+test/test_create_azure_computervision_classification_model.py
+test/test_create_azure_computervision_custom_model.py
+test/test_create_azure_computervision_ocr_model.py
+test/test_delete_azure_computervision_custom_model.py
+test/test_train_azure_computervision_custom_model.py
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/setup.cfg` & `irisml-tasks-azure-computervision-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [metadata]
 name = irisml-tasks-azure-computervision
-version = 0.0.1
+version = 0.0.3
 url = https://github.com/microsoft/irisml-tasks-azure-computervision
 description = Azure Computer Vision API tasks for IrisML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
 
 [options]
 packages = find_namespace:
 python_requires = >= 3.8
 install_requires = 
 	irisml
 	Pillow
+	requests
 	tenacity
 	torchvision
 
 [options.packages.find]
 include = 
 	irisml.tasks
```

### Comparing `irisml-tasks-azure-computervision-0.0.1/test/test_create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

