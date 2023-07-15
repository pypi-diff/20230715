# Comparing `tmp/chatdocs-0.2.4.tar.gz` & `tmp/chatdocs-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.2.4.tar", last modified: Sat Jun 10 21:49:34 2023, max compression
+gzip compressed data, was "chatdocs-0.2.5.tar", last modified: Sat Jul 15 19:53:53 2023, max compression
```

## Comparing `chatdocs-0.2.4.tar` & `chatdocs-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-10 21:49:34.126123 chatdocs-0.2.4/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6766 2023-06-10 21:30:46.000000 chatdocs-0.2.4/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.4/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.4/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5675 2023-06-10 08:41:19.000000 chatdocs-0.2.4/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.4/chatdocs/chains.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-06-07 13:32:32.000000 chatdocs-0.2.4/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.4/chatdocs/config.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/chatdocs/data/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      697 2023-06-10 21:23:28.000000 chatdocs-0.2.4/chatdocs/data/chatdocs.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4297 2023-06-10 21:28:38.000000 chatdocs-0.2.4/chatdocs/data/index.html
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.4/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.4/chatdocs/embeddings.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.4/chatdocs/llms.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.4/chatdocs/main.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1693 2023-06-04 19:41:17.000000 chatdocs-0.2.4/chatdocs/ui.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.4/chatdocs/utils.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.4/chatdocs/vectorstores.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-10 21:49:34.126123 chatdocs-0.2.4/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      445 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-10 21:49:34.000000 chatdocs-0.2.4/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-10 21:49:34.126123 chatdocs-0.2.4/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2247 2023-06-10 21:43:44.000000 chatdocs-0.2.4/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-07-15 19:53:53.120638 chatdocs-0.2.5/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-07-15 19:53:53.120638 chatdocs-0.2.5/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6766 2023-06-10 21:30:46.000000 chatdocs-0.2.5/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-07-15 19:53:53.100638 chatdocs-0.2.5/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.5/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.5/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5675 2023-06-10 08:41:19.000000 chatdocs-0.2.5/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      554 2023-06-04 12:15:53.000000 chatdocs-0.2.5/chatdocs/chains.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1376 2023-07-15 19:25:16.000000 chatdocs-0.2.5/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.5/chatdocs/config.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-07-15 19:53:53.120638 chatdocs-0.2.5/chatdocs/data/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      725 2023-07-15 17:57:43.000000 chatdocs-0.2.5/chatdocs/data/chatdocs.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4417 2023-07-15 19:34:15.000000 chatdocs-0.2.5/chatdocs/data/index.html
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-07 19:32:55.000000 chatdocs-0.2.5/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.5/chatdocs/embeddings.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2668 2023-06-07 19:29:24.000000 chatdocs-0.2.5/chatdocs/llms.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1259 2023-06-04 11:04:07.000000 chatdocs-0.2.5/chatdocs/main.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2062 2023-07-15 19:28:40.000000 chatdocs-0.2.5/chatdocs/ui.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      219 2023-06-07 13:30:29.000000 chatdocs-0.2.5/chatdocs/utils.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.5/chatdocs/vectorstores.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-07-15 19:53:53.110638 chatdocs-0.2.5/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     9830 2023-07-15 19:53:52.000000 chatdocs-0.2.5/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      544 2023-07-15 19:53:53.000000 chatdocs-0.2.5/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-07-15 19:53:52.000000 chatdocs-0.2.5/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-07-15 19:53:52.000000 chatdocs-0.2.5/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-07-15 19:53:52.000000 chatdocs-0.2.5/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      446 2023-07-15 19:53:52.000000 chatdocs-0.2.5/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-07-15 19:53:52.000000 chatdocs-0.2.5/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-07-15 19:53:53.120638 chatdocs-0.2.5/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2248 2023-07-15 19:41:41.000000 chatdocs-0.2.5/setup.py
```

### Comparing `chatdocs-0.2.4/PKG-INFO` & `chatdocs-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.4
+Version: 0.2.5
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
```

### Comparing `chatdocs-0.2.4/README.md` & `chatdocs-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/add.py` & `chatdocs-0.2.5/chatdocs/add.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/chains.py` & `chatdocs-0.2.5/chatdocs/chains.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/chat.py` & `chatdocs-0.2.5/chatdocs/chat.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/config.py` & `chatdocs-0.2.5/chatdocs/config.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/data/chatdocs.yml` & `chatdocs-0.2.5/chatdocs/data/chatdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,17 @@
   model: TheBloke/Wizard-Vicuna-7B-Uncensored-GPTQ
   model_file: Wizard-Vicuna-7B-Uncensored-GPTQ-4bit-128g.no-act-order.safetensors
   pipeline_kwargs:
     max_new_tokens: 256
 
 download: false
 
+host: localhost
 port: 5000
+auth: false
 
 chroma:
   persist_directory: db
   chroma_db_impl: duckdb+parquet
   anonymized_telemetry: false
 
 retriever:
```

### Comparing `chatdocs-0.2.4/chatdocs/data/index.html` & `chatdocs-0.2.5/chatdocs/data/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 <title>ChatDocs</title>
 
 <script>
+  const auth = new URLSearchParams(window.location.search).get('auth');
   const ws = new WebSocket(`ws://${location.host}/ws`);
 
   ws.addEventListener('message', (event) => {
     data = JSON.parse(event.data);
     onReceive(data);
   });
 
   const send = (req) => {
+    if (auth) {
+      req['auth'] = auth;
+    }
     req = JSON.stringify(req);
     ws.send(req);
   };
 
   const el = (tag) => document.createElement(tag);
 
   const onReceive = (res) => {
```

### Comparing `chatdocs-0.2.4/chatdocs/llms.py` & `chatdocs-0.2.5/chatdocs/llms.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/main.py` & `chatdocs-0.2.5/chatdocs/main.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs/vectorstores.py` & `chatdocs-0.2.5/chatdocs/vectorstores.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/chatdocs.egg-info/PKG-INFO` & `chatdocs-0.2.5/chatdocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.2.4
+Version: 0.2.5
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
```

### Comparing `chatdocs-0.2.4/chatdocs.egg-info/SOURCES.txt` & `chatdocs-0.2.5/chatdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatdocs-0.2.4/setup.py` & `chatdocs-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.2.4",
+    version="0.2.5",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
@@ -20,15 +20,15 @@
     entry_points={
         "console_scripts": [
             f"{name} = {name}.main:app",
         ],
     },
     install_requires=[
         "chromadb>=0.3.0,<0.4.0",
-        "ctransformers>=0.2.5,<0.3.0",
+        "ctransformers>=0.2.12,<0.3.0",
         "deepmerge>=1.1.0,<2.0.0",
         "InstructorEmbedding>=1.0.1,<2.0.0",
         "langchain>=0.0.181",
         "pyyaml>=6.0",
         "quart>=0.18.3,<0.19.0",
         "sentence-transformers>=2.2.2,<3.0.0",
         "tqdm>=4.64.1,<5.0.0",
```

