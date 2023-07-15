# Comparing `tmp/iamai_adapter_dingtalk-3.2.tar.gz` & `tmp/iamai_adapter_dingtalk-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_dingtalk-3.2.tar", max compression
+gzip compressed data, was "iamai_adapter_dingtalk-3.2.1.tar", max compression
```

## Comparing `iamai_adapter_dingtalk-3.2.tar` & `iamai_adapter_dingtalk-3.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/README.md
--rw-r--r--   0        0        0     5440 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/__init__.py
--rw-r--r--   0        0        0      590 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/config.py
--rw-r--r--   0        0        0     2363 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/event.py
--rw-r--r--   0        0        0      387 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/exceptions.py
--rw-r--r--   0        0        0     3200 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/message.py
--rw-r--r--   0        0        0     1292 2023-07-14 12:11:24.511443 iamai_adapter_dingtalk-3.2/pyproject.toml
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 iamai_adapter_dingtalk-3.2/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/README.md
+-rw-r--r--   0        0        0     5440 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/config.py
+-rw-r--r--   0        0        0     2363 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/event.py
+-rw-r--r--   0        0        0      387 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/exceptions.py
+-rw-r--r--   0        0        0     3200 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/message.py
+-rw-r--r--   0        0        0     1294 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 iamai_adapter_dingtalk-3.2.1/PKG-INFO
```

### Comparing `iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/__init__.py` & `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/config.py` & `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/event.py` & `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/event.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-3.2/iamai/adapter/dingtalk/message.py` & `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-3.2/pyproject.toml` & `iamai_adapter_dingtalk-3.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-dingtalk"
-version = "3.2"
+version = "3.2.1"
 description = "DingTalk adapter for iamai."
 authors = ["简律纯 <i@jyunko.cn>"]
 license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

