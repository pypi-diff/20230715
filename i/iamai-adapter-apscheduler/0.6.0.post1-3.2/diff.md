# Comparing `tmp/iamai_adapter_apscheduler-0.6.0.post1.tar.gz` & `tmp/iamai_adapter_apscheduler-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_apscheduler-0.6.0.post1.tar", max compression
+gzip compressed data, was "iamai_adapter_apscheduler-3.2.tar", max compression
```

## Comparing `iamai_adapter_apscheduler-0.6.0.post1.tar` & `iamai_adapter_apscheduler-3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/README.md
--rw-r--r--   0        0        0     4675 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/__init__.py
--rw-r--r--   0        0        0      377 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/config.py
--rw-r--r--   0        0        0      932 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/event.py
--rw-r--r--   0        0        0     1337 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/pyproject.toml
--rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 iamai_adapter_apscheduler-0.6.0.post1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-14 12:11:24.507443 iamai_adapter_apscheduler-3.2/README.md
+-rw-r--r--   0        0        0     4675 2023-07-14 12:11:24.511443 iamai_adapter_apscheduler-3.2/iamai/adapter/apscheduler/__init__.py
+-rw-r--r--   0        0        0      377 2023-07-14 12:11:24.511443 iamai_adapter_apscheduler-3.2/iamai/adapter/apscheduler/config.py
+-rw-r--r--   0        0        0      932 2023-07-14 12:11:24.511443 iamai_adapter_apscheduler-3.2/iamai/adapter/apscheduler/event.py
+-rw-r--r--   0        0        0     1336 2023-07-14 12:11:24.511443 iamai_adapter_apscheduler-3.2/pyproject.toml
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 iamai_adapter_apscheduler-3.2/PKG-INFO
```

### Comparing `iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/__init__.py` & `iamai_adapter_apscheduler-3.2/iamai/adapter/apscheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/event.py` & `iamai_adapter_apscheduler-3.2/iamai/adapter/apscheduler/event.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_apscheduler-0.6.0.post1/pyproject.toml` & `iamai_adapter_apscheduler-3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "iamai-adapter-apscheduler"
-version = "0.6.0.post1"
+version = "3.2"
 description = "APScheduler adapter for iamai."
-authors = ["简律纯 <admin@jyunko.cn>"]
-license = "MIT"
+authors = ["简律纯 <i@jyunko.cn>"]
+license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
 keywords = ["bot", "chatbot", "scheduling", "apscheduler"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -20,15 +20,15 @@
     "Topic :: Communications :: Chat",
 ]
 packages = [{ include = "iamai" }]
 exclude = ["iamai/__init__.py", "iamai/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-iamai = "^3.14"
+iamai = "^3.2"
 apscheduler = "^3.7"
 
 [tool.poetry.dev-dependencies]
 iamai = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `iamai_adapter_apscheduler-0.6.0.post1/PKG-INFO` & `iamai_adapter_apscheduler-3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-apscheduler
-Version: 0.6.0.post1
+Version: 3.2
 Summary: APScheduler adapter for iamai.
 Home-page: https://retrofor.space/
-License: MIT
+License: GPL-3.0 License
 Keywords: bot,chatbot,scheduling,apscheduler
 Author: 简律纯
-Author-email: admin@jyunko.cn
+Author-email: i@jyunko.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
 Requires-Dist: apscheduler (>=3.7,<4.0)
-Requires-Dist: iamai (>=3.14,<4.0)
+Requires-Dist: iamai (>=3.2,<4.0)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
```

