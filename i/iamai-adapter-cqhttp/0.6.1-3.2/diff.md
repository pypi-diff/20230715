# Comparing `tmp/iamai_adapter_cqhttp-0.6.1.tar.gz` & `tmp/iamai_adapter_cqhttp-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_cqhttp-0.6.1.tar", max compression
+gzip compressed data, was "iamai_adapter_cqhttp-3.2.tar", max compression
```

## Comparing `iamai_adapter_cqhttp-0.6.1.tar` & `iamai_adapter_cqhttp-3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/README.md
--rw-r--r--   0        0        0     7995 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0      899 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/config.py
--rw-r--r--   0        0        0    14033 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      656 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7475 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     1313 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 iamai_adapter_cqhttp-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/README.md
+-rw-r--r--   0        0        0     7995 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/config.py
+-rw-r--r--   0        0        0    14025 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/event.py
+-rw-r--r--   0        0        0      656 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/exceptions.py
+-rw-r--r--   0        0        0     7475 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/message.py
+-rw-r--r--   0        0        0     1321 2023-07-14 12:11:24.511443 iamai_adapter_cqhttp-3.2/pyproject.toml
+-rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 iamai_adapter_cqhttp-3.2/PKG-INFO
```

### Comparing `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/__init__.py` & `iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/config.py` & `iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/event.py` & `iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pydantic import Field, BaseModel
 
 from iamai.event import Event
 
 from .message import CQHTTPMessage
 
 if TYPE_CHECKING:
+    from . import CQHTTPAdapter
     from .message import T_CQMSG
-    from . import CQHTTPAdapter  # noqa
 
 T_CQHTTPEvent = TypeVar("T_CQHTTPEvent", bound="CQHTTPEvent")
 
 
 class Sender(BaseModel):
     user_id: Optional[int]
     nickname: Optional[str]
```

### Comparing `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/exceptions.py` & `iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/message.py` & `iamai_adapter_cqhttp-3.2/iamai/adapter/cqhttp/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.1/pyproject.toml` & `iamai_adapter_cqhttp-3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "iamai-adapter-cqhttp"
-version = "0.6.1"
-description = "OneBot(CQHTTP) adapter for iamai."
-authors = ["简律纯 <admin@jyunko.cn>"]
-license = "MIT"
+version = "3.2"
+description = "OneBot(go-cqhttp) adapter for iamai."
+authors = ["简律纯 <i@jyunko.cn>"]
+license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
 keywords = ["bot", "chatbot", "qq", "qqbot", "cqhttp", "coolq"]
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

### Comparing `iamai_adapter_cqhttp-0.6.1/PKG-INFO` & `iamai_adapter_cqhttp-3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-cqhttp
-Version: 0.6.1
-Summary: OneBot(CQHTTP) adapter for iamai.
+Version: 3.2
+Summary: OneBot(go-cqhttp) adapter for iamai.
 Home-page: https://retrofor.space/
-License: MIT
+License: GPL-3.0 License
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
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
```

