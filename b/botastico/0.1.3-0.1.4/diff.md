# Comparing `tmp/botastico-0.1.3.tar.gz` & `tmp/botastico-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botastico-0.1.3.tar", max compression
+gzip compressed data, was "botastico-0.1.4.tar", max compression
```

## Comparing `botastico-0.1.3.tar` & `botastico-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1077 2023-07-14 06:40:48.122486 botastico-0.1.3/LICENSE
--rw-r--r--   0        0        0     2203 2023-07-14 06:36:20.539247 botastico-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.3/botastico/__init__.py
--rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.3/botastico/langchain.py
--rw-r--r--   0        0        0      524 2023-07-14 06:47:28.619441 botastico-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 botastico-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-14 06:40:48.122486 botastico-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2298 2023-07-15 06:05:55.272558 botastico-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.4/botastico/__init__.py
+-rw-r--r--   0        0        0     5720 2023-07-15 05:21:00.183824 botastico-0.1.4/botastico/langchain.py
+-rw-r--r--   0        0        0      870 2023-07-15 06:20:24.896251 botastico-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 botastico-0.1.4/PKG-INFO
```

### Comparing `botastico-0.1.3/LICENSE` & `botastico-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `botastico-0.1.3/README.md` & `botastico-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Botastico python SDK
 
+[![PyPI version](https://badge.fury.io/py/botastico.svg)](https://badge.fury.io/py/botastico)
+
 ## Introduction
 
 This is the official python SDK for Botastico, a sophisticated conversational AI service. The SDK enables developers to easily integrate Botastico's powerful conversational capabilities into their applications, products, or services.
 
 This SDK is designed to interact with the Botastico API, offering an easy and user-friendly way to send and receive messages, manage conversations, and much more. Whether you're building a chatbot, a virtual assistant, or any other kind of conversational application, this SDK will simplify your work and increase your productivity.
 
 ## Current Version
```

### Comparing `botastico-0.1.3/botastico/langchain.py` & `botastico-0.1.4/botastico/langchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
         headers, params = self._prepare_request(messages, **kwargs)
 
         response = requests.post(
-            f"{self.base_url}/v1/agents/{self.botastico_agent_id}/interaction",
+            f"{self.base_url}/v1/agents/{self.botastico_agent_id}/interactions",
             headers=headers,
             data=json.dumps(params),
             timeout=self.request_timeout,
         )
 
         if response.status_code == 200:
             resp_json = response.json()
@@ -117,15 +117,15 @@
         **kwargs: Any,
     ) -> ChatResult:
         headers, params = self._prepare_request(messages, **kwargs)
 
         # Use aiohttp to make the request
         async with ClientSession() as session:
             async with session.post(
-                f"{self.base_url}/v1/agents/{self.botastico_agent_id}/interaction",
+                f"{self.base_url}/v1/agents/{self.botastico_agent_id}/interactions",
                 json=params,
                 headers=headers,
             ) as resp:
                 # Check for HTTP errors
                 resp.raise_for_status()
 
                 # Parse the JSON response
```

### Comparing `botastico-0.1.3/PKG-INFO` & `botastico-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: botastico
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK for using the botasti.co chat API
 Home-page: https://github.com/botastico/botastico-python
 Author: Andres Kull
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: langchain (>=0.0.231,<0.0.232)
+Requires-Dist: python-semantic-release (>=7.34.6,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Botastico python SDK
 
+[![PyPI version](https://badge.fury.io/py/botastico.svg)](https://badge.fury.io/py/botastico)
+
 ## Introduction
 
 This is the official python SDK for Botastico, a sophisticated conversational AI service. The SDK enables developers to easily integrate Botastico's powerful conversational capabilities into their applications, products, or services.
 
 This SDK is designed to interact with the Botastico API, offering an easy and user-friendly way to send and receive messages, manage conversations, and much more. Whether you're building a chatbot, a virtual assistant, or any other kind of conversational application, this SDK will simplify your work and increase your productivity.
 
 ## Current Version
```

