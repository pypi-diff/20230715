# Comparing `tmp/llm-toys-0.0.2.tar.gz` & `tmp/llm-toys-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-toys-0.0.2.tar", last modified: Sat Jul 15 13:54:36 2023, max compression
+gzip compressed data, was "llm-toys-0.0.4.tar", last modified: Sat Jul 15 13:48:48 2023, max compression
```

## Comparing `llm-toys-0.0.2.tar` & `llm-toys-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:54:36.159119 llm-toys-0.0.2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      760 2023-07-15 13:54:36.159119 llm-toys-0.0.2/PKG-INFO
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      400 2023-07-14 12:54:54.000000 llm-toys-0.0.2/README.md
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:54:36.159119 llm-toys-0.0.2/llm_toys/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      512 2023-07-15 13:54:13.000000 llm-toys-0.0.2/llm_toys/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1030 2023-07-15 07:24:40.000000 llm-toys-0.0.2/llm_toys/config.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      579 2023-07-14 12:41:16.000000 llm-toys-0.0.2/llm_toys/prompts.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:54:36.159119 llm-toys-0.0.2/llm_toys/tasks/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      116 2023-07-15 06:08:47.000000 llm-toys-0.0.2/llm_toys/tasks/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2637 2023-07-15 06:20:23.000000 llm-toys-0.0.2/llm_toys/tasks/paraphrase.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3768 2023-07-15 07:24:40.000000 llm-toys-0.0.2/llm_toys/tasks/predict.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2649 2023-07-15 05:21:51.000000 llm-toys-0.0.2/llm_toys/tasks/tone_change.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8306 2023-07-14 12:32:07.000000 llm-toys-0.0.2/llm_toys/train.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2363 2023-07-14 13:03:24.000000 llm-toys-0.0.2/llm_toys/utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:54:36.159119 llm-toys-0.0.2/llm_toys.egg-info/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      760 2023-07-15 13:54:36.000000 llm-toys-0.0.2/llm_toys.egg-info/PKG-INFO
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      400 2023-07-15 13:54:36.000000 llm-toys-0.0.2/llm_toys.egg-info/SOURCES.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        1 2023-07-15 13:54:36.000000 llm-toys-0.0.2/llm_toys.egg-info/dependency_links.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1438 2023-07-15 13:54:36.000000 llm-toys-0.0.2/llm_toys.egg-info/requires.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        9 2023-07-15 13:54:36.000000 llm-toys-0.0.2/llm_toys.egg-info/top_level.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       89 2023-07-15 06:02:36.000000 llm-toys-0.0.2/pyproject.toml
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       38 2023-07-15 13:54:36.159119 llm-toys-0.0.2/setup.cfg
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1427 2023-07-15 07:35:58.000000 llm-toys-0.0.2/setup.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:48:48.600420 llm-toys-0.0.4/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      760 2023-07-15 13:48:48.600420 llm-toys-0.0.4/PKG-INFO
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      400 2023-07-14 12:54:54.000000 llm-toys-0.0.4/README.md
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:48:48.600420 llm-toys-0.0.4/llm_toys/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      494 2023-07-15 13:43:22.000000 llm-toys-0.0.4/llm_toys/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1030 2023-07-15 07:24:40.000000 llm-toys-0.0.4/llm_toys/config.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      579 2023-07-14 12:41:16.000000 llm-toys-0.0.4/llm_toys/prompts.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:48:48.600420 llm-toys-0.0.4/llm_toys/tasks/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      116 2023-07-15 06:08:47.000000 llm-toys-0.0.4/llm_toys/tasks/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2637 2023-07-15 06:20:23.000000 llm-toys-0.0.4/llm_toys/tasks/paraphrase.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3768 2023-07-15 07:24:40.000000 llm-toys-0.0.4/llm_toys/tasks/predict.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2649 2023-07-15 05:21:51.000000 llm-toys-0.0.4/llm_toys/tasks/tone_change.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8306 2023-07-14 12:32:07.000000 llm-toys-0.0.4/llm_toys/train.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2363 2023-07-14 13:03:24.000000 llm-toys-0.0.4/llm_toys/utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 13:48:48.600420 llm-toys-0.0.4/llm_toys.egg-info/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      760 2023-07-15 13:48:48.000000 llm-toys-0.0.4/llm_toys.egg-info/PKG-INFO
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      400 2023-07-15 13:48:48.000000 llm-toys-0.0.4/llm_toys.egg-info/SOURCES.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        1 2023-07-15 13:48:48.000000 llm-toys-0.0.4/llm_toys.egg-info/dependency_links.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1438 2023-07-15 13:48:48.000000 llm-toys-0.0.4/llm_toys.egg-info/requires.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        9 2023-07-15 13:48:48.000000 llm-toys-0.0.4/llm_toys.egg-info/top_level.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       89 2023-07-15 06:02:36.000000 llm-toys-0.0.4/pyproject.toml
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       38 2023-07-15 13:48:48.600420 llm-toys-0.0.4/setup.cfg
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1427 2023-07-15 07:35:58.000000 llm-toys-0.0.4/setup.py
```

### Comparing `llm-toys-0.0.2/PKG-INFO` & `llm-toys-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-toys
-Version: 0.0.2
+Version: 0.0.4
 Summary: Production-ready small LLMs fine-tuned for diverse tasks, all without an OpenAI key.
 Home-page: https://github.com/kuutsav/llm-toys
 Author: Kumar Utsav
 Author-email: krum.utsav@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `llm-toys-0.0.2/llm_toys/config.py` & `llm-toys-0.0.4/llm_toys/config.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys/prompts.py` & `llm-toys-0.0.4/llm_toys/prompts.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys/tasks/paraphrase.py` & `llm-toys-0.0.4/llm_toys/tasks/paraphrase.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys/tasks/predict.py` & `llm-toys-0.0.4/llm_toys/tasks/predict.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys/tasks/tone_change.py` & `llm-toys-0.0.4/llm_toys/tasks/tone_change.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys/train.py` & `llm-toys-0.0.4/llm_toys/train.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys/utils.py` & `llm-toys-0.0.4/llm_toys/utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/llm_toys.egg-info/PKG-INFO` & `llm-toys-0.0.4/llm_toys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-toys
-Version: 0.0.2
+Version: 0.0.4
 Summary: Production-ready small LLMs fine-tuned for diverse tasks, all without an OpenAI key.
 Home-page: https://github.com/kuutsav/llm-toys
 Author: Kumar Utsav
 Author-email: krum.utsav@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `llm-toys-0.0.2/llm_toys.egg-info/requires.txt` & `llm-toys-0.0.4/llm_toys.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `llm-toys-0.0.2/setup.py` & `llm-toys-0.0.4/setup.py`

 * *Files identical despite different names*

