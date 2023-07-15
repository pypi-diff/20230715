# Comparing `tmp/deepllm-0.6.1.tar.gz` & `tmp/deepllm-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-0.6.1.tar", last modified: Sat Jul  8 02:03:01 2023, max compression
+gzip compressed data, was "deepllm-0.6.2.tar", last modified: Sat Jul 15 03:55:11 2023, max compression
```

## Comparing `deepllm-0.6.1.tar` & `deepllm-0.6.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.618979 deepllm-0.6.1/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.6.1/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4266 2023-07-08 02:03:01.618681 deepllm-0.6.1/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     3981 2023-07-07 22:49:34.000000 deepllm-0.6.1/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.606563 deepllm-0.6.1/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-08 01:27:50.000000 deepllm-0.6.1/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     1322 2023-07-08 00:50:25.000000 deepllm-0.6.1/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.610050 deepllm-0.6.1/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.6.1/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     1303 2023-07-08 01:34:30.000000 deepllm-0.6.1/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.6.1/deepllm/apps/app.sh
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.1/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       47 2023-07-07 23:04:29.000000 deepllm-0.6.1/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.6.1/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.611837 deepllm-0.6.1/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.6.1/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.6.1/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.6.1/deepllm/demos/demo.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.1/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.6.1/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.6.1/deepllm/demos/wikifetch.py
--rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.6.1/deepllm/embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.6.1/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.6.1/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.614198 deepllm-0.6.1/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.6.1/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.6.1/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.1/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.6.1/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.6.1/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.6.1/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.6.1/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 05:21:46.000000 deepllm-0.6.1/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.6.1/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     6880 2023-07-06 02:50:36.000000 deepllm-0.6.1/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.6.1/deepllm/refiners.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.618210 deepllm-0.6.1/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.6.1/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.6.1/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.6.1/deepllm/tests/test_all.sh
--rw-r--r--   0 tarau      (503) staff       (20)      735 2023-07-08 01:55:34.000000 deepllm-0.6.1/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.6.1/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.6.1/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.6.1/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.6.1/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.6.1/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.6.1/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.6.1/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.6.1/deepllm/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 02:03:01.608451 deepllm-0.6.1/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4266 2023-07-08 02:03:01.000000 deepllm-0.6.1/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-08 02:03:01.000000 deepllm-0.6.1/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-08 02:03:01.000000 deepllm-0.6.1/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-08 02:03:01.000000 deepllm-0.6.1/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-08 02:03:01.000000 deepllm-0.6.1/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-08 02:03:01.000000 deepllm-0.6.1/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-08 02:03:01.619102 deepllm-0.6.1/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.6.1/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.977902 deepllm-0.6.2/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.6.2/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4266 2023-07-15 03:55:11.977485 deepllm-0.6.2/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     3981 2023-07-07 22:49:34.000000 deepllm-0.6.2/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.958030 deepllm-0.6.2/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-15 03:54:23.000000 deepllm-0.6.2/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1357 2023-07-15 03:33:52.000000 deepllm-0.6.2/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.962435 deepllm-0.6.2/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-0.6.2/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     1898 2023-07-15 03:31:05.000000 deepllm-0.6.2/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.6.2/deepllm/apps/app.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.2/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       47 2023-07-07 23:04:29.000000 deepllm-0.6.2/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.6.2/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.965855 deepllm-0.6.2/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-0.6.2/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.6.2/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2109 2023-07-12 22:37:40.000000 deepllm-0.6.2/deepllm/demos/demo.py
+-rw-r--r--   0 tarau      (503) staff       (20)       74 2023-07-12 22:36:18.000000 deepllm-0.6.2/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.6.2/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1920 2023-07-08 21:41:31.000000 deepllm-0.6.2/deepllm/demos/viz.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.6.2/deepllm/demos/wikifetch.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.6.2/deepllm/embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.6.2/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.6.2/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.969802 deepllm-0.6.2/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.6.2/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.6.2/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.2/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.6.2/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.6.2/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.6.2/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.6.2/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 05:21:46.000000 deepllm-0.6.2/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6116 2023-07-10 01:11:15.000000 deepllm-0.6.2/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     8313 2023-07-15 03:51:16.000000 deepllm-0.6.2/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.6.2/deepllm/refiners.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.976525 deepllm-0.6.2/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-0.6.2/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.6.2/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      507 2023-07-08 20:37:00.000000 deepllm-0.6.2/deepllm/tests/test_all.py
+-rw-r--r--   0 tarau      (503) staff       (20)      735 2023-07-08 01:55:34.000000 deepllm-0.6.2/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.6.2/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.6.2/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.6.2/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.6.2/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.6.2/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.6.2/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-0.6.2/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.6.2/deepllm/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-15 03:55:11.960184 deepllm-0.6.2/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4266 2023-07-15 03:55:11.000000 deepllm-0.6.2/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1277 2023-07-15 03:55:11.000000 deepllm-0.6.2/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-15 03:55:11.000000 deepllm-0.6.2/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-15 03:55:11.000000 deepllm-0.6.2/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-15 03:55:11.000000 deepllm-0.6.2/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-15 03:55:11.000000 deepllm-0.6.2/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-15 03:55:11.978041 deepllm-0.6.2/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.6.2/setup.py
```

### Comparing `deepllm-0.6.1/LICENSE` & `deepllm-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/PKG-INFO` & `deepllm-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.6.1
+Version: 0.6.2
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-0.6.1/README.md` & `deepllm-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/api.py` & `deepllm-0.6.2/deepllm/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from .prompters import *
 from .params import *
-from .recursors import AndOrExplorer
+from .recursors import AndOrExplorer, show_clauses, show_model
 from .refiners import Advisor, Rater, TruthRater, AbstractMaker
 
+
 def run_recursor(initiator=None, prompter=None, lim=None):
     assert None not in (prompter, initiator, lim)
     recursor = AndOrExplorer(initiator=initiator, prompter=prompter, lim=lim)
     yield from recursor.run()
 
+
 def run_advisor(initiator=None, prompter=None, lim=None):
     assert None not in (prompter, initiator, lim)
     recursor = Advisor(initiator=initiator, prompter=prompter, lim=lim)
     yield from recursor.run()
 
+
 def run_rater(initiator=None, prompter=None, lim=None, threshold=None):
     assert None not in (prompter, initiator, lim, threshold)
     recursor = Rater(initiator=initiator, prompter=prompter, lim=lim, threshold=threshold)
     yield from recursor.run()
 
+
 def run_truth_rater(initiator=None, prompter=None, truth_file=None, threshold=None, lim=None):
     assert None not in (initiator, prompter, truth_file, threshold, lim)
     rater = TruthRater(initiator=initiator, prompter=prompter, truth_file=truth_file, threshold=threshold, lim=lim)
     yield from rater.run()
 
-def run_abstract_maker(topic=None,keywords=None):
+
+def run_abstract_maker(topic=None, keywords=None):
     assert None not in (topic, keywords)
-    recursor = AbstractMaker(topic=topic,keywords=keywords)
+    recursor = AbstractMaker(topic=topic, keywords=keywords)
     return recursor.run()
+
+
```

### Comparing `deepllm-0.6.1/deepllm/configurator.py` & `deepllm-0.6.2/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/demos/demo.py` & `deepllm-0.6.2/deepllm/demos/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     test_truth_rater(prompter=sci_prompter, goal='Unification algorithm', truth_file='logic_programming',
                      threshold=0.10, lim=1)
     test_truth_rater(prompter=sci_prompter, goal='Teaching computational thinking with Prolog',
                      truth_file='computational_thinking', threshold=0.50, lim=2)
     test_truth_rater(prompter=sci_prompter, goal='Artificial general intelligence',
                      truth_file='artificial_general_intelligence', threshold=0.50, lim=2)
 
-    return
-
     test_rater(prompter=causal_prompter, goal='The Fermi paradox', threshold=0.60, lim=2)
 
     test_rater(prompter=conseq_prompter, goal='P = NP', threshold=0.50, lim=3)
 
     test_advisor(prompter=recommendation_prompter, goal='The Godfather', lim=2)
     test_rater(prompter=recommendation_prompter, goal='The Godfather', threshold=0.20, lim=2)
```

### Comparing `deepllm-0.6.1/deepllm/demos/wikifetch.py` & `deepllm-0.6.2/deepllm/demos/wikifetch.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/embedders.py` & `deepllm-0.6.2/deepllm/embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/horn_prover.py` & `deepllm-0.6.2/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/interactors.py` & `deepllm-0.6.2/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/local_llms/local_runs.py` & `deepllm-0.6.2/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/local_llms/test_vicuna.py` & `deepllm-0.6.2/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/params.py` & `deepllm-0.6.2/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/prompters.py` & `deepllm-0.6.2/deepllm/prompters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 goal_prompter = dict(
-    name='planner',
+    name='task_planner',
     and_p="""The plan so far is: "$context".
      In this context my goal is "$g." 
      Advise me how to achieve "$g", step by step, while ensuring each step is consistent with each other.
      Itemize your answer, one sentence per line.""",
     or_p="""The plan so far is: "$context".
     In this context my goal is "$g." 
     Suggest 2-3 mutually exclusive alternative ways to achieve "$g".
```

### Comparing `deepllm-0.6.1/deepllm/recursors.py` & `deepllm-0.6.2/deepllm/recursors.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,25 +92,14 @@
         and_context = to_context((g, trace), self.initiator)
         for h in hs:
             if h == g or in_stack(h, trace): continue
             bs = self.unf.ask_and(h, and_context)  # invent their bodies
             if h in bs: continue
             yield h, bs
 
-    # begin overrides
-    def resume(self):
-        self.unf.resume()
-
-    def persist(self):
-        self.unf.persist()
-
-    def appraise(self, g, _trace):
-        # return g[0] in "CILKPE" # just to test it trims model
-        return True
-
     def costs(self):
         return self.unf.costs()
 
     # end overrides
 
     def solve(self):
 
@@ -134,42 +123,73 @@
                     for b in bs:
                         yield from step(b, trace, d + 1)
                 if self.strict and len(hs) > 1: self.clauses['false'].append(hs)
 
         for gs in step(self.initiator, (), 0):
             yield list(reversed(to_list(gs)))
 
-        for fact in self.facts: self.clauses[fact].append([])
-
         self.persist()
 
-        pro_name = f'{self.OUT}{self.name}_{self.pname}_{self.lim}'
-
-        to_prolog(self.clauses, pro_name)
-
+        for fact in self.facts: self.clauses[fact].append([])
         css = [(h, bs) for (h, bss) in self.clauses.items() for bs in bss]
+        self.logic_model = qprove(css, goal=self.initiator)
+        self.trim_clauses()
+        self.save_results()
 
-        # css=list(self.clauses.items())
+    def save_results(self):
+        pro_name = f'{self.OUT}{self.name}_{self.pname}_{self.lim}'
+        mo_name = pro_name + "_model"
 
-        self.logic_model = qprove(css, goal=self.initiator)
+        to_prolog(self.clauses, pro_name)
 
         if self.logic_model is None:
+            self.logic_model = []
             tprint('\nNO MODEL ENTAILING:', self.initiator)
         else:
             tprint('\nMODEL:', len(self.logic_model), 'facts', '\n')
             for fact in self.logic_model: tprint(fact)
-            save_model(self.initiator, self.logic_model, pro_name + "_model")
+        save_model(self.initiator, self.logic_model, mo_name)
 
     def run(self):
         for r in self.solve():
             yield 'TRACE', r
-        yield 'CLAUSES',dict(self.clauses)
+        yield 'CLAUSES', dict(self.clauses)
         yield 'MODEL', self.logic_model
         yield 'COSTS', self.costs()
 
+    # -------- begin overrides -------------
+
+    def resume(self):
+        self.unf.resume()
+
+    def persist(self):
+        self.unf.persist()
+
+    def appraise(self, g, _trace):
+        """
+        to be overriden by refiners
+        """
+        return True
+
+    def trim_clauses(self):
+        """
+        to be overriden : only atoms in the model
+        will be kept - no action here as they all are
+        """
+        pass
+        clauses = defaultdict(list)
+        if self.logic_model is not None:
+            model = set(self.logic_model)
+            clauses = defaultdict(list)
+            for (h, bss) in self.clauses.items():
+                for bs in bss:
+                    ok = all(b in model for b in bs)
+                    if ok: clauses[h].append(bs)
+        self.clauses = clauses
+
 
 def run_explorer(goal=None, prompter=None, lim=None):
     assert None not in (prompter, goal, lim)
     r = AndOrExplorer(initiator=goal, prompter=prompter, lim=lim)
     seen = dict()
     for a in r.solve():
         print('\nTRACE:')
@@ -191,27 +211,62 @@
     return True
 
 
 def quote(x):
     return "'" + x + "'"
 
 
-def save_model(goal, facts, fname, suf='.pl'):
+def show_clauses(clauses):
+    buf = []
+
+    def p(x):
+        buf.append(x)
+
+    for h, bss in clauses.items():
+        if bss == []:
+            p(f"'{h}'.\n")
+            break
+
+        for i, bs in enumerate(bss):
+            if i == 0:
+                end = ":-" if bs else "."
+                p(f"'{h}'{end}\n")
+
+            for j, b in enumerate(bs):
+                b = f"'{b}'"
+                if j + 1 == len(bs):
+                    print('!!!!',b)
+                    b = b + ("." if i + 1 == len(bss) else ";")
+                else:
+                    b = b + ","
+                p("    " + b + "\n")
+
+    return "".join(buf)
+
+
+def show_model(facts):
+    buf = []
+    for fact in facts:
+        buf.append(f"'{fact}'.")
+    return "\n".join(buf)
+
+
+def save_model(goal, facts, fname, suf='.pro'):
     path = fname + suf
     ensure_path(path)
     with open(path, 'w') as f:
         print(f'% MODEL: {len(facts)} facts', file=f)
         for fact in facts:
             line = quote(fact) + "."
             if fact == goal: line = line + "%" + (10 * " ") + "<==== initiator !"
             print(line, file=f)
 
 
-def to_prolog(clauses, fname, neck=":-"):
-    suf = '.nat' if neck == ":" else ".pl"
+def to_prolog(clauses, fname, neck=":-", suf='.pro'):
+    suf = '.nat' if neck == ":" else suf
 
     path = fname + suf
     ensure_path(path)
     with open(path, 'w') as f:
         print('% CLAUSES:', file=f)
         for h, bss in clauses.items():
             for bs in bss:
```

### Comparing `deepllm-0.6.1/deepllm/refiners.py` & `deepllm-0.6.2/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/tests/test_api.py` & `deepllm-0.6.2/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/tests/test_recursors.py` & `deepllm-0.6.2/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm/tests/test_refiners.py` & `deepllm-0.6.2/deepllm/tests/test_refiners.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     r = Rater(initiator=goal, prompter=prompter, threshold=threshold, lim=lim)
 
     for a in r.solve():
         print('\nTRACE:')
         for x in a:
             print(x)
         print()
-
+    print('MODEL:',len(r.logic_model))
     c = r.costs()
     print('COSTS in $:', c)
     return True
 
 
 def test_advisor(prompter=None, goal=None, lim=None):
     assert None not in (goal, prompter, lim)
@@ -78,12 +78,12 @@
     print('Cost: $', writer.agent.dollar_cost())
     return True
 
 def test_refiners():
     assert test_abstract_maker1()
     # assert test_abstract_maker2()
     assert test_advisor(prompter=sci_prompter, goal='Low power circuit design',lim=1)
-    assert test_rater(prompter=causal_prompter, goal='The Fermi paradox', threshold=0.50, lim=1)
+    assert test_rater(prompter=causal_prompter, goal='The Fermi paradox', threshold=0.60, lim=1)
 
 
 if __name__ == "__main__":
     test_refiners()
```

### Comparing `deepllm-0.6.1/deepllm/tools.py` & `deepllm-0.6.2/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.6.1/deepllm.egg-info/PKG-INFO` & `deepllm-0.6.2/deepllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.6.1
+Version: 0.6.2
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-0.6.1/deepllm.egg-info/SOURCES.txt` & `deepllm-0.6.2/deepllm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 deepllm/apps/install.sh
 deepllm/apps/requirements.txt
 deepllm/demos/README.md
 deepllm/demos/__init__.py
 deepllm/demos/demo.py
 deepllm/demos/install.sh
 deepllm/demos/requirements.txt
+deepllm/demos/viz.py
 deepllm/demos/wikifetch.py
 deepllm/local_llms/README.md
 deepllm/local_llms/__init__.py
 deepllm/local_llms/install.sh
 deepllm/local_llms/local_runs.py
 deepllm/local_llms/requirements.txt
 deepllm/local_llms/server.sh
 deepllm/local_llms/test_vicuna.py
 deepllm/tests/README.md
 deepllm/tests/__init__.py
-deepllm/tests/test_all.sh
+deepllm/tests/test_all.py
 deepllm/tests/test_api.py
 deepllm/tests/test_configurator.py
 deepllm/tests/test_embedders.py
 deepllm/tests/test_horn_prover.py
 deepllm/tests/test_interactors.py
 deepllm/tests/test_params.py
 deepllm/tests/test_recursors.py
```

### Comparing `deepllm-0.6.1/setup.py` & `deepllm-0.6.2/setup.py`

 * *Files identical despite different names*

