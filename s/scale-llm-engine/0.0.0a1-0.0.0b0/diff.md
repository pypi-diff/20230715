# Comparing `tmp/scale_llm_engine-0.0.0a1.tar.gz` & `tmp/scale_llm_engine-0.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0a1.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b0.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0a1.tar` & `scale_llm_engine-0.0.0b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1006 2023-07-15 10:44:42.384939 scale_llm_engine-0.0.0a1/README.md
--rw-r--r--   0        0        0     1060 2023-07-15 11:09:01.252314 scale_llm_engine-0.0.0a1/llmengine/__init__.py
--rw-r--r--   0        0        0     5709 2023-07-15 11:07:38.608065 scale_llm_engine-0.0.0a1/llmengine/api_engine.py
--rw-r--r--   0        0        0    17835 2023-07-15 10:44:42.386135 scale_llm_engine-0.0.0a1/llmengine/client.py
--rw-r--r--   0        0        0     7962 2023-07-15 10:44:42.387518 scale_llm_engine-0.0.0a1/llmengine/completion.py
--rw-r--r--   0        0        0     8154 2023-07-15 11:07:38.609074 scale_llm_engine-0.0.0a1/llmengine/data_types.py
--rw-r--r--   0        0        0     1523 2023-07-15 11:07:38.609814 scale_llm_engine-0.0.0a1/llmengine/errors.py
--rw-r--r--   0        0        0     4254 2023-07-15 10:44:42.389752 scale_llm_engine-0.0.0a1/llmengine/fine_tuning.py
--rw-r--r--   0        0        0     2069 2023-07-15 10:44:42.390031 scale_llm_engine-0.0.0a1/llmengine/model.py
--rw-r--r--   0        0        0      808 2023-07-15 11:09:01.245956 scale_llm_engine-0.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1006 2023-07-15 16:31:10.656012 scale_llm_engine-0.0.0b0/README.md
+-rw-r--r--   0        0        0     1059 2023-07-15 17:24:52.423107 scale_llm_engine-0.0.0b0/llmengine/__init__.py
+-rw-r--r--   0        0        0     5746 2023-07-15 17:24:30.933268 scale_llm_engine-0.0.0b0/llmengine/api_engine.py
+-rw-r--r--   0        0        0    17835 2023-07-15 16:31:10.659325 scale_llm_engine-0.0.0b0/llmengine/client.py
+-rw-r--r--   0        0        0     7962 2023-07-15 16:31:10.659701 scale_llm_engine-0.0.0b0/llmengine/completion.py
+-rw-r--r--   0        0        0     8154 2023-07-15 17:24:30.934470 scale_llm_engine-0.0.0b0/llmengine/data_types.py
+-rw-r--r--   0        0        0     1639 2023-07-15 17:24:30.935531 scale_llm_engine-0.0.0b0/llmengine/errors.py
+-rw-r--r--   0        0        0     4254 2023-07-15 16:31:10.660754 scale_llm_engine-0.0.0b0/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0     2069 2023-07-15 16:31:10.661087 scale_llm_engine-0.0.0b0/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-15 17:24:52.427224 scale_llm_engine-0.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b0/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0a1/README.md` & `scale_llm_engine-0.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0a1/llmengine/__init__.py` & `scale_llm_engine-0.0.0b0/llmengine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.alpha1"
+__version__ = "0.0.0.beta0"
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneJobResponse,
     CompletionOutput,
     CompletionStreamOutput,
     CompletionStreamV1Response,
```

### Comparing `scale_llm_engine-0.0.0a1/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b0/llmengine/api_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,47 +43,47 @@
     def get(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.get(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             timeout=timeout,
             headers={"x-api-key": api_key},
         )
-        payload = response.json()
         if response.status_code != 200:
-            raise parse_error(response.status_code, payload)
+            raise parse_error(response.status_code, response.content)
+        payload = response.json()
         return payload
 
     @classmethod
     def put(
         cls, resource_name: str, data: Optional[Dict[str, Any]], timeout: int
     ) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.put(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
             timeout=timeout,
             headers={"x-api-key": api_key},
         )
-        payload = response.json()
         if response.status_code != 200:
-            raise parse_error(response.status_code, payload)
+            raise parse_error(response.status_code, response.content)
+        payload = response.json()
         return payload
 
     @classmethod
     def post_sync(cls, resource_name: str, data: Dict[str, Any], timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.post(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
             timeout=timeout,
             headers={"x-api-key": api_key},
         )
-        payload = response.json()
         if response.status_code != 200:
-            raise parse_error(response.status_code, payload)
+            raise parse_error(response.status_code, response.content)
+        payload = response.json()
         return payload
 
     @classmethod
     def post_stream(
         cls, resource_name: str, data: Dict[str, Any], timeout: int
     ) -> Iterator[Dict[str, Any]]:
         api_key = get_api_key()
@@ -91,15 +91,15 @@
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
             timeout=timeout,
             headers={"x-api-key": api_key},
             stream=True,
         )
         if response.status_code != 200:
-            raise parse_error(response.status_code, response.json())
+            raise parse_error(response.status_code, response.content)
         for byte_payload in response.iter_lines():
             # Skip line
             if byte_payload == b"\n":
                 continue
 
             payload = byte_payload.decode("utf-8")
 
@@ -120,33 +120,32 @@
         api_key = get_api_key()
         async with ClientSession(
             timeout=ClientTimeout(timeout), headers={"x-api-key": api_key}
         ) as session:
             async with session.post(
                 os.path.join(LLM_ENGINE_BASE_PATH, resource_name), json=data
             ) as resp:
-                payload = await resp.json()
-
                 if resp.status != 200:
-                    raise parse_error(resp.status, payload)
+                    raise parse_error(resp.status, await resp.read())
+                payload = await resp.json()
                 return payload
 
     @classmethod
     async def apost_stream(
         cls, resource_name: str, data: Dict[str, Any], timeout: int
     ) -> AsyncIterable[Dict[str, Any]]:
         api_key = get_api_key()
         async with ClientSession(
             timeout=ClientTimeout(timeout), headers={"x-api-key": api_key}
         ) as session:
             async with session.post(
                 os.path.join(LLM_ENGINE_BASE_PATH, resource_name), json=data
             ) as resp:
                 if resp.status != 200:
-                    raise parse_error(resp.status, await resp.json())
+                    raise parse_error(resp.status, await resp.read())
                 async for byte_payload in resp.content:
                     # Skip line
                     if byte_payload == b"\n":
                         continue
 
                     payload = byte_payload.decode("utf-8")
```

### Comparing `scale_llm_engine-0.0.0a1/llmengine/client.py` & `scale_llm_engine-0.0.0b0/llmengine/client.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0a1/llmengine/completion.py` & `scale_llm_engine-0.0.0b0/llmengine/completion.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0a1/llmengine/data_types.py` & `scale_llm_engine-0.0.0b0/llmengine/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 class CompletionSyncV1Request(BaseModel):
     """
     Request object for a synchronous prompt completion task.
     """
 
     prompts: List[str] = Field(..., min_items=1)
     max_new_tokens: int = Field(..., gt=0)
-    temperature: float = Field(..., ge=0.0)
+    temperature: float = Field(..., gt=0.0)
 
 
 class CompletionOutput(BaseModel):
     text: str
     """Text"""
 
     num_prompt_tokens: Optional[int]
@@ -215,15 +215,15 @@
 class CompletionStreamV1Request(BaseModel):
     """
     Request object for a stream prompt completion task.
     """
 
     prompt: str = Field(..., min_length=1)
     max_new_tokens: int = Field(..., gt=0)
-    temperature: float = Field(..., ge=0.0)
+    temperature: float = Field(..., gt=0.0)
 
 
 class CompletionStreamOutput(BaseModel):
     text: str
     """Text"""
 
     finished: bool
```

### Comparing `scale_llm_engine-0.0.0a1/llmengine/errors.py` & `scale_llm_engine-0.0.0b0/llmengine/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Dict
 
 
 # LLM Engine Errors
 class ValidationError(Exception):
     def __init__(self, message: str):
         super().__init__(message)
@@ -30,30 +31,34 @@
 
 # Unknown error
 class UnknownError(Exception):
     def __init__(self, message: str):
         super().__init__(message)
 
 
-def parse_error(status_code: int, payload: Dict[str, str]) -> Exception:
+def parse_error(status_code: int, content: bytes) -> Exception:
     """
-    Parse error given an HTTP status code and a json payload
+    Parse error given an HTTP status code and a bytes payload
 
     Args:
         status_code (`int`):
             HTTP status code
-        payload (`Dict[str, str]`):
-            Json payload
+        content (`bytes`):
+            payload
 
     Returns:
         Exception: parsed exception
 
     """
     # Try to parse a LLM Engine error
-    message = payload["detail"]
+    try:
+        payload = json.loads(content)
+        message = payload["detail"]
+    except json.JSONDecodeError:
+        message = content.decode("utf-8")
 
     # Try to parse a APIInference error
     if status_code == 400:
         return BadRequestError(message)
     if status_code == 401:
         return UnauthorizedError(message)
     if status_code == 404:
```

### Comparing `scale_llm_engine-0.0.0a1/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b0/llmengine/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0a1/llmengine/model.py` & `scale_llm_engine-0.0.0b0/llmengine/model.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0a1/pyproject.toml` & `scale_llm_engine-0.0.0b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.alpha1"
+version = "0.0.0.beta0"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0a1/PKG-INFO` & `scale_llm_engine-0.0.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0a1
+Version: 0.0.0b0
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

