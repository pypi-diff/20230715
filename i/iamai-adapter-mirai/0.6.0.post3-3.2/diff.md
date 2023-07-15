# Comparing `tmp/iamai_adapter_mirai-0.6.0.post3.tar.gz` & `tmp/iamai_adapter_mirai-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_mirai-0.6.0.post3.tar", max compression
+gzip compressed data, was "iamai_adapter_mirai-3.2.tar", max compression
```

## Comparing `iamai_adapter_mirai-0.6.0.post3.tar` & `iamai_adapter_mirai-3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/LICENSE
--rw-r--r--   0        0        0      242 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/README.md
--rw-r--r--   0        0        0     9055 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/config.py
--rw-r--r--   0        0        0      562 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/__init__.py
--rw-r--r--   0        0        0      822 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/base.py
--rw-r--r--   0        0        0     1042 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/mate.py
--rw-r--r--   0        0        0     3650 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/message.py
--rw-r--r--   0        0        0     5492 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/notice.py
--rw-r--r--   0        0        0     4264 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/request.py
--rw-r--r--   0        0        0      644 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/exceptions.py
--rw-r--r--   0        0        0     4419 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/message.py
--rw-r--r--   0        0        0     1300 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/pyproject.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 iamai_adapter_mirai-0.6.0.post3/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/LICENSE
+-rw-r--r--   0        0        0      242 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/README.md
+-rw-r--r--   0        0        0     9055 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/config.py
+-rw-r--r--   0        0        0      562 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/base.py
+-rw-r--r--   0        0        0     1042 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/mate.py
+-rw-r--r--   0        0        0     3650 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/message.py
+-rw-r--r--   0        0        0     5492 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/notice.py
+-rw-r--r--   0        0        0     4264 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/request.py
+-rw-r--r--   0        0        0      644 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/exceptions.py
+-rw-r--r--   0        0        0     4419 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/iamai/adapter/mirai/message.py
+-rw-r--r--   0        0        0     1299 2023-07-14 12:11:24.511443 iamai_adapter_mirai-3.2/pyproject.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 iamai_adapter_mirai-3.2/PKG-INFO
```

### Comparing `iamai_adapter_mirai-0.6.0.post3/LICENSE` & `iamai_adapter_mirai-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/__init__.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/config.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/__init__.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/base.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/base.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/mate.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/mate.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/message.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/notice.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/notice.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/request.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/event/request.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/exceptions.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/message.py` & `iamai_adapter_mirai-3.2/iamai/adapter/mirai/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post3/pyproject.toml` & `iamai_adapter_mirai-3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "iamai-adapter-mirai"
-version = "0.6.0.post3"
+version = "3.2"
 description = "Mirai adapter for iamai."
-authors = ["简律纯 <admin@jyunko.cn>"]
-license = "MIT"
+authors = ["简律纯 <i@jyunko.cn>"]
+license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
 keywords = ["bot", "chatbot", "qq", "qqbot", "mirai"]
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
 
 [tool.poetry.dev-dependencies]
 iamai = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `iamai_adapter_mirai-0.6.0.post3/PKG-INFO` & `iamai_adapter_mirai-3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-mirai
-Version: 0.6.0.post3
+Version: 3.2
 Summary: Mirai adapter for iamai.
 Home-page: https://retrofor.space/
-License: MIT
+License: GPL-3.0 License
 Keywords: bot,chatbot,qq,qqbot,mirai
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
-Requires-Dist: iamai (>=3.14,<4.0)
+Requires-Dist: iamai (>=3.2,<4.0)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.iamai.dev/"><img src="https://raw.githubusercontent.com/retrofor/iamai/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: iamai-adapter-mirai Version: 0.6.0.post3 Summary:
-Mirai adapter for iamai. Home-page: https://retrofor.space/ License: MIT
+Metadata-Version: 2.1 Name: iamai-adapter-mirai Version: 3.2 Summary: Mirai
+adapter for iamai. Home-page: https://retrofor.space/ License: GPL-3.0 License
 Keywords: bot,chatbot,qq,qqbot,mirai Author: ç®å¾çº¯ Author-email:
-admin@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3
-- Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot
-Framework Classifier: Framework :: Robot Framework :: Library Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Topic :: Communications :: Chat Requires-Dist: iamai
-(>=3.14,<4.0) Project-URL: Documentation, https://iamai.retrofor.space/
-Project-URL: Repository, https://github.com/retrofor/iamai Description-Content-
-Type: text/markdown
+i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3 -
+Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
+Approved :: MIT License Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2,<4.0) Project-URL:
+Documentation, https://iamai.retrofor.space/ Project-URL: Repository, https://
+github.com/retrofor/iamai Description-Content-Type: text/markdown
              [logo] # iamai-Adapter-CQHTTP **Mirai åè®®éé**
```

