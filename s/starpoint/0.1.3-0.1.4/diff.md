# Comparing `tmp/starpoint-0.1.3.tar.gz` & `tmp/starpoint-0.1.4.tar.gz`

## Comparing `starpoint-0.1.3.tar` & `starpoint-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.1.3/dev-requirements.txt
--rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.1.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.3/starpoint/__init__.py
--rw-r--r--   0        0        0    20425 2020-02-02 00:00:00.000000 starpoint-0.1.3/starpoint/db.py
--rw-r--r--   0        0        0    26784 2020-02-02 00:00:00.000000 starpoint-0.1.3/tests/test_db.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.3/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.3/LICENSE
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.1.3/README.md
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starpoint-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.1.4/dev-requirements.txt
+-rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.1.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.4/starpoint/__init__.py
+-rw-r--r--   0        0        0    20438 2020-02-02 00:00:00.000000 starpoint-0.1.4/starpoint/db.py
+-rw-r--r--   0        0        0    26788 2020-02-02 00:00:00.000000 starpoint-0.1.4/tests/test_db.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.4/LICENSE
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.1.4/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 starpoint-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.1.4/PKG-INFO
```

### Comparing `starpoint-0.1.3/dev-requirements.txt` & `starpoint-0.1.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.3/requirements.txt` & `starpoint-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.3/starpoint/db.py` & `starpoint-0.1.4/starpoint/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     _check_host_health(trimmed_hostname)
 
     return trimmed_hostname
 
 
 def _check_collection_identifier_collision(
-    collection_id: Optional[UUID] = None, collection_name: Optional[str] = None
+    collection_id: Optional[str] = None, collection_name: Optional[str] = None
 ):
     if collection_id is None and collection_name is None:
         raise ValueError(NO_COLLECTION_VALUE_ERROR)
     elif collection_id and collection_name:
         raise ValueError(MULTI_COLLECTION_VALUE_ERROR)
 
 
@@ -91,15 +91,15 @@
             host = WRITER_URL
 
         self.host = _set_and_validate_host(host)
         self.api_key = api_key
 
     def delete(
         self,
-        documents: List[UUID],
+        documents: List[str],
         collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         # TODO: filter through documents to make sure values are what we expect them to be
@@ -109,15 +109,15 @@
             collection_name="collection_name_example",
             documents=["uuid-uuid-uuid"]
             ],
         )
         """
 
         request_data = dict(
-            collection_id=str(collection_id),
+            collection_id=collection_id,
             collection_name=collection_name,
             documents=[str(document) for document in documents],
         )
         try:
             response = requests.delete(
                 url=f"{self.host}{DOCUMENTS_PATH}",
                 json=request_data,
@@ -137,15 +137,15 @@
             )
             return {}
         return response.json()
 
     def insert(
         self,
         documents: List[Dict[Any, Any]],
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         # TODO: filter through documents to make sure values are what we expect them to be
         """
@@ -187,38 +187,38 @@
             return {}
         return response.json()
 
     def column_insert(
         self,
         embeddings: List[float],
         document_metadatas: List[Dict[Any, Any]],
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         if len(embeddings) != len(document_metadatas):
             LOGGER.warning(EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING)
 
-        document = [
+        documents = [
             {
                 "embedding": embedding,
                 "metadata": document_metadata,
             }
             for embedding, document_metadata in zip(embeddings, document_metadatas)
         ]
 
-        self.insert(
-            document=document,
+        return self.insert(
+            documents=documents,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
     def update(
         self,
         documents: List[Dict[Any, Any]],
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         # TODO: filter through documents to make sure values are what we expect them to be
         """
@@ -294,15 +294,15 @@
             LOGGER.error(
                 f"Request failed with status code {response.status_code} "
                 f"and the following message:\n{response.text}"
             )
             return {}
         return response.json()
 
-    def delete_collection(self, collection_id: UUID) -> Dict[Any, Any]:
+    def delete_collection(self, collection_id: str) -> Dict[Any, Any]:
         """
         dict(
             collection_id="collection_id_example",
         )
         """
 
         request_data = dict(
@@ -339,15 +339,15 @@
 
         self.host = _set_and_validate_host(host)
         self.api_key = api_key
 
     def query(
         self,
         sql: Optional[str] = None,
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
         query_embedding: Optional[List[float]] = None,
         params: Optional[List[Any]] = None,
     ) -> Dict[Any, Any]:
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
@@ -387,17 +387,17 @@
                 f"and the following message:\n{response.text}"
             )
             return {}
         return response.json()
 
     def infer_schema(
         self,
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
-    ) -> Dict[any, any]:
+    ) -> Dict[Any, Any]:
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         """
         dict(
             collection_id="collection_id_example",
             collection_name="collection_name_example",
@@ -439,80 +439,80 @@
         self.reader = Reader(api_key=api_key, host=reader_host)
 
         # Consider a wrapper around openai once this class gets bloated
         self.openai = None
 
     def delete(
         self,
-        documents: List[UUID],
-        collection_id: Optional[UUID] = None,
+        documents: List[str],
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         return self.writer.delete(
             documents=documents,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
     def insert(
         self,
         documents: List[Dict[Any, Any]],
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         return self.writer.insert(
             documents=documents,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
     def column_insert(
         self,
         embeddings: List[float],
         document_metadatas: List[Dict[Any, Any]],
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         return self.writer.column_insert(
             embeddings=embeddings,
             document_metadatas=document_metadatas,
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
     def query(
         self,
         sql: Optional[str] = None,
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
         query_embedding: Optional[List[float]] = None,
         params: Optional[List[Any]] = None,
     ) -> Dict[Any, Any]:
         return self.reader.query(
             sql=sql,
             collection_id=collection_id,
             collection_name=collection_name,
             query_embedding=query_embedding,
             params=params,
         )
 
     def infer_schema(
         self,
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         return self.reader.infer_schema(
             collection_id=collection_id,
             collection_name=collection_name,
         )
 
     def update(
         self,
         documents: List[Dict[Any, Any]],
-        collection_id: Optional[UUID] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
         return self.writer.update(
             documents=documents,
             collection_id=collection_id,
             collection_name=collection_name,
         )
@@ -521,15 +521,15 @@
         self, collection_name: str, dimensionality: int
     ) -> Dict[Any, Any]:
         return self.writer.create_collection(
             collection_name=collection_name,
             dimensionality=dimensionality,
         )
 
-    def delete_collection(self, collection_id: UUID) -> Dict[Any, Any]:
+    def delete_collection(self, collection_id: str) -> Dict[Any, Any]:
         return self.writer.delete_collection(
             collection_id=collection_id,
         )
 
     """
     OpenAI convenience wrappers
     """
@@ -558,20 +558,20 @@
         except ValueError as e:
             self.openai = None
             raise e
 
     def build_and_insert_embeddings_from_openai(
         self,
         model: str,
-        input_data: Union[str, Iterable],
-        document_metadatas: Optional[List[Dict]] = None,
-        collection_id: Optional[UUID] = None,
+        input_data: Union[str, Iterable[Any]],
+        document_metadatas: Optional[List[Dict[Any, Any]]] = None,
+        collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
         openai_user: Optional[str] = None,
-    ) -> Dict:
+    ) -> Dict[Any, Any]:
         if self.openai is None:
             raise RuntimeError(
                 "OpenAI instance has not been initialized. Please initialize it using "
                 "Client.init_openai()"
             )
 
         _check_collection_identifier_collision(collection_id, collection_name)
```

### Comparing `starpoint-0.1.3/tests/test_db.py` & `starpoint-0.1.4/tests/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     ]
 
     writer.column_insert(
         embeddings=test_embeddings, document_metadatas=test_document_metadatas
     )
 
     insert_mock.assert_called_once_with(
-        document=expected_insert_document,
+        documents=expected_insert_document,
         collection_id=None,
         collection_name=None,
     )
 
 
 @patch("starpoint.db.Writer.insert")
 def test_writer_column_insert_collection_id_collection_name_passed_through(
@@ -321,15 +321,15 @@
         embeddings=test_embeddings,
         document_metadatas=test_document_metadatas,
         collection_id=expected_collection_id,
         collection_name=expected_collection_name,
     )
 
     insert_mock.assert_called_once_with(
-        document=expected_insert_document,
+        documents=expected_insert_document,
         collection_id=expected_collection_id,
         collection_name=expected_collection_name,
     )
 
 
 @patch("starpoint.db.Writer.insert")
 def test_writer_column_insert_shorter_metadatas_length(
@@ -351,15 +351,15 @@
         embeddings=test_embeddings, document_metadatas=test_document_metadatas
     )
 
     logger_mock.warning.assert_called_once_with(
         db.EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING
     )
     insert_mock.assert_called_once_with(
-        document=expected_insert_document,
+        documents=expected_insert_document,
         collection_id=None,
         collection_name=None,
     )
 
 
 @patch("starpoint.db.Writer.insert")
 def test_writer_column_insert_shorter_embeddings_length(
@@ -381,15 +381,15 @@
         embeddings=test_embeddings, document_metadatas=test_document_metadatas
     )
 
     logger_mock.warning.assert_called_once_with(
         db.EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING
     )
     insert_mock.assert_called_once_with(
-        document=expected_insert_document,
+        documents=expected_insert_document,
         collection_id=None,
         collection_name=None,
     )
 
 
 @patch("starpoint.db._check_collection_identifier_collision")
 @patch("starpoint.db.requests")
```

### Comparing `starpoint-0.1.3/LICENSE` & `starpoint-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.3/README.md` & `starpoint-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.3/pyproject.toml` & `starpoint-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "starpoint"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "pointable", email = "package-maintainers@pointable.ai" }]
 description = "SDK for Starpoint DB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
-dependencies = [
-  "openai~=0.27",
-  "requests~=2.28",
-  "validators~=0.20",
-]
+dependencies = ["openai~=0.27", "requests~=2.28", "validators~=0.20"]
 
 [project.optional-dependencies]
-dev = [
-  "pip-tools~=6.14",
-  "pre-commit~=3.3",
-  "pytest-cov~=4.1",
-  "pytest~=7.3",
-]
+dev = ["pip-tools~=6.14", "pre-commit~=3.3", "pytest-cov~=4.1", "pytest~=7.3"]
 
 [project.urls]
 "Homepage" = "https://github.com/starpoint-ai/sdk"
 "Bug Tracker" = "https://github.com/starpoint-ai/sdk/issues"
```

### Comparing `starpoint-0.1.3/PKG-INFO` & `starpoint-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starpoint
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK for Starpoint DB
 Project-URL: Homepage, https://github.com/starpoint-ai/sdk
 Project-URL: Bug Tracker, https://github.com/starpoint-ai/sdk/issues
 Author-email: pointable <package-maintainers@pointable.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

