# Comparing `tmp/llm-toys-0.0.1.tar.gz` & `tmp/llm-toys-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-toys-0.0.1.tar", last modified: Sat Jul  8 11:02:14 2023, max compression
+gzip compressed data, was "llm-toys-0.0.4.tar", last modified: Sat Jul 15 13:48:48 2023, max compression
```

## Comparing `llm-toys-0.0.1.tar` & `llm-toys-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-08 11:02:14.097064 llm-toys-0.0.1/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1072 2023-07-08 10:26:30.000000 llm-toys-0.0.1/LICENCE
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      478 2023-07-08 11:02:14.097064 llm-toys-0.0.1/PKG-INFO
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       96 2023-07-08 10:53:40.000000 llm-toys-0.0.1/README.md
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-08 11:02:14.097064 llm-toys-0.0.1/llm_toys/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       22 2023-07-08 10:22:21.000000 llm-toys-0.0.1/llm_toys/__init__.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-08 11:02:14.097064 llm-toys-0.0.1/llm_toys.egg-info/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      478 2023-07-08 11:02:14.000000 llm-toys-0.0.1/llm_toys.egg-info/PKG-INFO
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      221 2023-07-08 11:02:14.000000 llm-toys-0.0.1/llm_toys.egg-info/SOURCES.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        1 2023-07-08 11:02:14.000000 llm-toys-0.0.1/llm_toys.egg-info/dependency_links.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       21 2023-07-08 11:02:14.000000 llm-toys-0.0.1/llm_toys.egg-info/requires.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        9 2023-07-08 11:02:14.000000 llm-toys-0.0.1/llm_toys.egg-info/top_level.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       89 2023-07-08 10:52:46.000000 llm-toys-0.0.1/pyproject.toml
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       38 2023-07-08 11:02:14.097064 llm-toys-0.0.1/setup.cfg
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1482 2023-07-08 11:02:08.000000 llm-toys-0.0.1/setup.py
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

### Comparing `llm-toys-0.0.1/setup.py` & `llm-toys-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,16 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def parse_requirements(file_name: str) -> List[str]:
-    with open(file_name, "r") as f:
-        return [
-            require.strip()
-            for require in f
-            if require.strip() and not require.startswith("#")
-        ]
+    with open("/home/tarnished/Developer/llm-toys/" + file_name, "r") as f:
+        return [require.strip() for require in f if require.strip() and not require.startswith("#")]
 
 
 def read(*parts):
     with codecs.open(os.path.join(here, *parts), "r") as fp:
         return fp.read()
 
 
@@ -41,14 +37,12 @@
     packages=find_packages(),
     version=find_version("llm_toys", "__init__.py"),
     author="Kumar Utsav",
     author_email="krum.utsav@gmail.com",
     description="Production-ready small LLMs fine-tuned for diverse tasks, all without an OpenAI key.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=parse_requirements(
-        "/home/tarnished/Developer/llm-toys/requirements.txt"
-    ),
+    install_requires=parse_requirements("requirements.txt"),
     url="https://github.com/kuutsav/llm-toys",
     license="https://opensource.org/license/mit/",
     python_requires=">=3.9.0",
 )
```

