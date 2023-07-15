# Comparing `tmp/mbapy-0.1.4.1.tar.gz` & `tmp/mbapy-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.1.4.1.tar", last modified: Thu Jul 13 11:14:15 2023, max compression
+gzip compressed data, was "mbapy-0.1.4.2.tar", last modified: Sat Jul 15 16:58:44 2023, max compression
```

## Comparing `mbapy-0.1.4.1.tar` & `mbapy-0.1.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.068061 mbapy-0.1.4.1/
--rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.4.1/LICENSE
--rw-rw-rw-   0        0        0     3252 2023-07-13 11:14:15.067063 mbapy-0.1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2424 2023-07-12 14:06:22.000000 mbapy-0.1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.019053 mbapy-0.1.4.1/mbapy/
--rw-rw-rw-   0        0        0      862 2023-07-11 16:18:10.000000 mbapy-0.1.4.1/mbapy/__init__.py
--rw-rw-rw-   0        0        0      421 2023-07-13 11:13:59.000000 mbapy-0.1.4.1/mbapy/__version__.py
--rw-rw-rw-   0        0        0    12020 2023-07-11 14:33:25.000000 mbapy-0.1.4.1/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.046058 mbapy-0.1.4.1/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.4.1/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.048058 mbapy-0.1.4.1/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.050059 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.054063 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.4.1/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.4.1/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.4.1/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.057061 mbapy-0.1.4.1/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.4.1/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.4.1/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    10373 2023-07-10 14:50:19.000000 mbapy-0.1.4.1/mbapy/file.py
--rw-rw-rw-   0        0        0    16575 2023-07-12 13:05:45.000000 mbapy-0.1.4.1/mbapy/paper.py
--rw-rw-rw-   0        0        0    14968 2023-07-10 12:49:19.000000 mbapy-0.1.4.1/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.063062 mbapy-0.1.4.1/mbapy/stats/
--rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.4.1/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    12351 2023-07-10 12:49:19.000000 mbapy-0.1.4.1/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.4.1/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.4.1/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    12735 2023-07-10 12:49:19.000000 mbapy-0.1.4.1/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.064062 mbapy-0.1.4.1/mbapy/storage/
--rw-rw-rw-   0        0        0    86016 2023-07-06 15:23:54.000000 mbapy-0.1.4.1/mbapy/storage/stats.dll
--rw-rw-rw-   0        0        0    16243 2023-07-12 13:29:22.000000 mbapy-0.1.4.1/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.036065 mbapy-0.1.4.1/mbapy.egg-info/
--rw-rw-rw-   0        0        0     3252 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      432 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:14:15.068061 mbapy-0.1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     3092 2023-07-13 11:11:54.000000 mbapy-0.1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.066062 mbapy-0.1.4.1/test/
--rw-rw-rw-   0        0        0     1998 2023-07-12 13:19:31.000000 mbapy-0.1.4.1/test/test_base.py
--rw-rw-rw-   0        0        0     1740 2023-07-12 13:29:09.000000 mbapy-0.1.4.1/test/test_web.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.593464 mbapy-0.1.4.2/
+-rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     3438 2023-07-15 16:58:44.592465 mbapy-0.1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2610 2023-07-13 11:33:05.000000 mbapy-0.1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.520444 mbapy-0.1.4.2/mbapy/
+-rw-rw-rw-   0        0        0      840 2023-07-15 15:37:57.000000 mbapy-0.1.4.2/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-07-15 16:58:29.000000 mbapy-0.1.4.2/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    12516 2023-07-14 14:29:59.000000 mbapy-0.1.4.2/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.554452 mbapy-0.1.4.2/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.4.2/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.554452 mbapy-0.1.4.2/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.559453 mbapy-0.1.4.2/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.562454 mbapy-0.1.4.2/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.4.2/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.4.2/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.4.2/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.4.2/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.4.2/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.4.2/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.4.2/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.564456 mbapy-0.1.4.2/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.4.2/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.4.2/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.4.2/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    14747 2023-07-15 16:32:44.000000 mbapy-0.1.4.2/mbapy/file.py
+-rw-rw-rw-   0        0        0    21397 2023-07-15 16:38:50.000000 mbapy-0.1.4.2/mbapy/paper.py
+-rw-rw-rw-   0        0        0    15504 2023-07-13 13:04:47.000000 mbapy-0.1.4.2/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.569456 mbapy-0.1.4.2/mbapy/stats/
+-rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.4.2/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    12351 2023-07-10 12:49:19.000000 mbapy-0.1.4.2/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.4.2/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.4.2/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    12735 2023-07-10 12:49:19.000000 mbapy-0.1.4.2/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.587459 mbapy-0.1.4.2/mbapy/storage/
+-rw-rw-rw-   0        0        0    86016 2023-07-06 15:23:54.000000 mbapy-0.1.4.2/mbapy/storage/stats.dll
+-rw-rw-rw-   0        0        0    16985 2023-07-14 14:26:37.000000 mbapy-0.1.4.2/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.546450 mbapy-0.1.4.2/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     3438 2023-07-15 16:58:44.000000 mbapy-0.1.4.2/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2023-07-15 16:58:44.000000 mbapy-0.1.4.2/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:58:44.000000 mbapy-0.1.4.2/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      438 2023-07-15 16:58:44.000000 mbapy-0.1.4.2/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-15 16:58:44.000000 mbapy-0.1.4.2/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:58:44.593464 mbapy-0.1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3108 2023-07-15 16:57:54.000000 mbapy-0.1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:58:44.590462 mbapy-0.1.4.2/test/
+-rw-rw-rw-   0        0        0     1998 2023-07-12 13:19:31.000000 mbapy-0.1.4.2/test/test_base.py
+-rw-rw-rw-   0        0        0     1740 2023-07-12 13:29:09.000000 mbapy-0.1.4.2/test/test_web.py
```

### Comparing `mbapy-0.1.4.1/LICENSE` & `mbapy-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/PKG-INFO` & `mbapy-0.1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
@@ -22,42 +22,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
  * @LastEditors: BHM-Bob 2262029386@qq.com
- * @LastEditTime: 2023-07-12 22:06:01
+ * @LastEditTime: 2023-07-13 19:32:26
  * @Description: 
 -->
 # BA_PY
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
 
 ![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy)
  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
 
 
 ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY)
 
-some helpful python scripts. (Basic for All in Python)
-Mainly contains sci-plot, stats, web-crawler and deeplearing-torch.
+mbapy contains some helpful python scripts, which aims at goal of *Basic for All in Python*.
+Mainly contains sci-plot, stats, web-crawler, sci-paper utils and deeplearing-torch.
 
 ## get start
 
-### install 
-#### pypi 
+#### install 
 Now, mbapy only support pypi install:  
-`pip install mbapy`  
-For updating:  
-`pip install --upgrade mbapy`  
+```
+pip install mbapy
+```
+
+If you find the latest release version has installing problems, you can download this repo and try:
+```
+pip install .
+```
 
-### wiki
-[wiki](https://github.com/BHM-Bob/BA_PY/wiki)
+#### wiki
+mbapy has it's wiki as API document, you can find it in [wiki](https://github.com/BHM-Bob/BA_PY/wiki).
 
 # contain  
 ## mbapy python package  
 #### \_\_version\_\_  
 *some version info*
 #### base
```

### Comparing `mbapy-0.1.4.1/README.md` & `mbapy-0.1.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
  * @LastEditors: BHM-Bob 2262029386@qq.com
- * @LastEditTime: 2023-07-12 22:06:01
+ * @LastEditTime: 2023-07-13 19:32:26
  * @Description: 
 -->
 # BA_PY
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
 
 ![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy)
  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
 
 
 ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY)
 
-some helpful python scripts. (Basic for All in Python)
-Mainly contains sci-plot, stats, web-crawler and deeplearing-torch.
+mbapy contains some helpful python scripts, which aims at goal of *Basic for All in Python*.
+Mainly contains sci-plot, stats, web-crawler, sci-paper utils and deeplearing-torch.
 
 ## get start
 
-### install 
-#### pypi 
+#### install 
 Now, mbapy only support pypi install:  
-`pip install mbapy`  
-For updating:  
-`pip install --upgrade mbapy`  
+```
+pip install mbapy
+```
+
+If you find the latest release version has installing problems, you can download this repo and try:
+```
+pip install .
+```
 
-### wiki
-[wiki](https://github.com/BHM-Bob/BA_PY/wiki)
+#### wiki
+mbapy has it's wiki as API document, you can find it in [wiki](https://github.com/BHM-Bob/BA_PY/wiki).
 
 # contain  
 ## mbapy python package  
 #### \_\_version\_\_  
 *some version info*
 #### base
```

### Comparing `mbapy-0.1.4.1/mbapy/__init__.py` & `mbapy-0.1.4.2/mbapy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 22:16:49
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-10 16:59:12
+LastEditTime: 2023-07-15 23:37:57
 Description: some helpful python scripts in plot, stats and deeplearning
 '''
 from . import base, file, plot, web, stats
 from .__version__ import (
     __author__,
     __author_email__,
     __build__,
@@ -21,15 +21,14 @@
     import torch
     from mbapy import dl_torch as dl_torch
 except:
     pass
     # print('no torch module available')
     
 try:
-    import scihub_cn
     from . import paper
 except:
     pass
     # print('no scihub_cn module available')
 
 # def main():
 #     pass
```

### Comparing `mbapy-0.1.4.1/mbapy/base.py` & `mbapy-0.1.4.2/mbapy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-10-19 22:46:30
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-11 22:33:19
+LastEditTime: 2023-07-14 22:28:03
 Description: 
 '''
 import sys, os
 import time
 from functools import wraps
 from typing import List
 import ctypes
 import inspect
 import platform
 
 import numpy as np
 
-
+# TODO : add global var modification options support
 __NO_ERR__ = False
 _Params = {
-    'LAUNCH_WEB_SUB_THREAD':False,
 }
 
 def put_err(info:str, ret = None):
     """put err info, return ret"""
     if not __NO_ERR__:
         frame = inspect.currentframe().f_back
         caller_name = frame.f_code.co_name
@@ -188,14 +187,27 @@
     :param chr: The character to replace the ':' separator. Default value is ':'.
     :type chr: str
     :return: A string that represents the current time with a given separator replacing the standard colon separator.
     :rtype: str
     """
     return time.asctime(time.localtime()).replace(':', chr)
 
+def format_secs(sumSecs):
+    """
+    Formats a given number of seconds into hours, minutes, and seconds.
+
+    :param sumSecs: An integer representing the total number of seconds.
+    :return: A tuple containing three integers representing the number of hours,
+             minutes, and seconds respectively.
+    """
+    sumHs = int(sumSecs//3600)
+    sumMs = int((sumSecs-sumHs*3600)//60)
+    sumSs = int(sumSecs-sumHs*3600-sumMs*60)
+    return sumHs, sumMs, sumSs
+
 class MyArgs():
     def __init__(self, args:dict) -> None:
         self.args = dict()
         args = self.get_args(args)
     def get_args(self, args:dict, force_update = True, del_origin = False):
         for arg_name in list(args.keys()):
             if arg_name in self.args and not force_update:
```

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.1.4.2/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.1.4.2/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/bb.py` & `mbapy-0.1.4.2/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/data.py` & `mbapy-0.1.4.2/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/hyper_search.py` & `mbapy-0.1.4.2/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/loss.py` & `mbapy-0.1.4.2/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/m.py` & `mbapy-0.1.4.2/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/optim.py` & `mbapy-0.1.4.2/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/paper/bb.py` & `mbapy-0.1.4.2/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/dl_torch/utils.py` & `mbapy-0.1.4.2/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/file.py` & `mbapy-0.1.4.2/mbapy/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 19:09:54
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-10 22:50:19
+LastEditTime: 2023-07-16 00:32:44
 Description: 
 '''
 import chardet
 import json
 import os
 from typing import List, Dict
 
 import pandas as pd
+from tqdm import tqdm
 
 if __name__ == '__main__':
     # dev mode
-    from mbapy.base import put_err, parameter_checker, check_parameters_path
+    from mbapy.base import put_err, parameter_checker, check_parameters_path, get_default_for_bool, format_secs
 else:
     # release mode
-    from .base import put_err, parameter_checker, check_parameters_path
+    from .base import put_err, parameter_checker, check_parameters_path, get_default_for_bool, format_secs
 
 def replace_invalid_path_chr(path:str, valid_chrs:str = '_'):
     """
     Replaces any invalid characters in a given path with a specified valid character.
 
     Args:
         path (str): The path string to be checked for invalid characters.
@@ -31,30 +32,31 @@
         str: The path string with all invalid characters replaced by the valid character.
     """
     invalid_chrs = ':*?"<>|'
     for invalid_chr in invalid_chrs:
         path = path.replace(invalid_chr, '_')
     return path
 
-@parameter_checker(check_parameters_path, raise_err = False)
-def opts_file(path:str, mode:str = 'r', encoding:str = 'utf-8', way:str = 'str', data = None):
+def opts_file(path:str, mode:str = 'r', encoding:str = 'utf-8', way:str = 'str', data = None, **kwargs):
     """
     A function that reads or writes data to a file based on the provided options.
 
     Parameters:
         path (str): The path to the file.
         mode (str, optional): The mode in which the file should be opened. Defaults to 'r'.
         encoding (str, optional): The encoding of the file. Defaults to 'utf-8'.
         way (str, optional): The way in which the data should be read or written. Defaults to 'lines'.
         data (Any, optional): The data to be written to the file. Only applicable in write mode. Defaults to None.
 
     Returns:
         list or str or dict or None: The data read from the file, or None if the file was opened in write mode and no data was provided.
     """
-    with open(path, mode, encoding=encoding) as f:
+    if 'b' not in mode:
+        kwargs.update(encoding=encoding)
+    with open(path, mode, **kwargs) as f:
         if 'r' in mode:
             if way == 'lines':
                 return f.readlines()
             elif way == 'str':
                 return f.read()
             elif way == 'json':
                 return json.loads(f.read())
@@ -236,13 +238,110 @@
     if backend == 'PyPDF2':
         import PyPDF2
         with open(path, 'rb') as file:
             reader = PyPDF2.PdfReader(file)
             return '\n'.join([page.extract_text() for page in reader.pages])
     else:
         raise NotImplementedError
+    
+def get_cv2_video_attr(video, attr_name:str, ret_int:bool = True):
+    """
+    Get the value of a specific attribute from a cv2 video object.
+
+    Parameters:
+        - video: cv2 video object.
+        - attr_name (str): The name of the attribute to retrieve. for CAP_PROP_FRAME_WIDTH, just pass 'FRAME_WIDTH'.
+        - ret_int (bool, optional): Indicates whether to return the attribute value as an integer. Defaults to True.
+
+    Returns:
+        - The value of the specified attribute. If ret_int is True, the value is returned as an integer.
+          Otherwise, the value is returned as is.
+
+    Example:
+        >>> video = cv2.VideoCapture(0)
+        >>> frame_width = get_cv2_video_attr(video, 'FRAME_WIDTH')
+        >>> print(frame_width)
+        >>> # Output: 640
+    """
+    import cv2
+    if ret_int:
+        return int(video.get(getattr(cv2, 'CAP_PROP_'+attr_name)))
+    else:
+        return video.get(getattr(cv2, 'CAP_PROP_'+attr_name))
+    
+@parameter_checker(check_parameters_path)
+def extract_frame_to_img(video_path:str, img_type = 'jpg', return_frames = False, write_file = True, dir:str = None,
+                         sum_frame = -1, read_frame_interval = 0, img_size = [-1, -1], **kwargs):
+    """
+    Extract frames from a video and save them as images.
+
+    Parameters:
+    - video_path (str): The path to the video file.
+    - img_type (str): The type of image file to save (default: 'jpg').
+    - return_frames (bool): Whether to return the frames as a list (default: False).
+    - write_file (bool): Whether to save the frames as image files (default: True).
+    - dir (str): The directory to save the image files (default: None).
+    - sum_frame (int): The number of frames to extract (-1 means extract all frames, default: -1).
+    - read_frame_interval (int): The interval between frames to be read (default: 0).
+    - img_size (List[int]): The size of the output images (default: [-1, -1]).
+    - **kwargs: Additional keyword arguments.
+
+    Returns:
+    - frames (List[array]): The extracted frames as a list, if `return_frames` is True.
+    
+    Files:
+    - writes image files in dir, each image file name include frame time stamp in format HH-MM-SS.
+    """
+    import cv2
+    # Create the directory if it doesn't exist
+    if write_file:
+        if dir and not os.path.exists(dir):
+            os.makedirs(dir)
+        else:
+            dir = video_path[:video_path.rfind('.')]
+            if not os.path.exists(dir):
+                os.makedirs(dir)
+    # Open the video file
+    video = cv2.VideoCapture(video_path)
+    sum_frame = get_cv2_video_attr(video, 'FRAME_COUNT') if sum_frame == -1 else sum_frame
+    frame_size = [get_cv2_video_attr(video, 'FRAME_WIDTH'), get_cv2_video_attr(video, 'FRAME_HEIGHT')]
+    fps = get_cv2_video_attr(video, 'FPS')
+    img_size[0] = frame_size[0] if img_size[0] <= 0 else img_size[0]
+    img_size[1] = frame_size[1] if img_size[1] <= 0 else img_size[1]
+    is_img_size_changed = img_size[0] != frame_size[0] and img_size[1] != frame_size
+    # Read frames from the video
+    frame_idx, frames = 0, []
+    bar = tqdm(range(sum_frame), desc='extract frames')
+    while True:
+        success, frame = video.read()
+        if read_frame_interval == 0 or frame_idx % (read_frame_interval+1) == 0:
+            if not success:
+                break
+            if is_img_size_changed:
+                cv2.resize(frame, img_size)
+            if return_frames:
+                frames.append(frame)
+            # write frames to img file if needed
+            if write_file:
+                time = '-'.join(map(lambda x: str(x), format_secs(frame_idx / fps)))
+                img_name = f"frame_{time}.{img_type}"
+                img_path = os.path.join(dir, img_name) if dir else img_name
+                cv2.imwrite(img_path, frame)
+            # update progress bar
+            bar.update(read_frame_interval+1)
+        frame_idx += 1
+    # Release the video file
+    video.release()
+    # return frames lst
+    return frames
 
 if __name__ == '__main__':
     # dev code
-    pdf_path = r"./data_tmp/DiffBP Generative Diffusion of 3D Molecules for Target Protein Binding.pdf"
-    print(convert_pdf_to_txt(pdf_path))
+    
+    # extract pdf text
+    # pdf_path = r"./data_tmp/DiffBP Generative Diffusion of 3D Molecules for Target Protein Binding.pdf"
+    # print(convert_pdf_to_txt(pdf_path))
+    
+    # extract video frames
+    video_path = r"./data_tmp/extract_frames.mp4"
+    extract_frame_to_img(video_path, read_frame_interval=50)
```

### Comparing `mbapy-0.1.4.1/mbapy/paper.py` & `mbapy-0.1.4.2/mbapy/paper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 '''
 Date: 2023-07-07 20:51:46
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-12 00:17:56
+LastEditTime: 2023-07-16 00:38:50
 FilePath: \BA_PY\mbapy\paper.py
 Description: 
 '''
-import os, re
+import os, re, requests
 from typing import List, Dict
 
+from lxml import etree
 import rispy
-from scihub_cn.scihub import SciHub
 import PyPDF2
 
 if __name__ == '__main__':
     # dev mode
     from mbapy.base import *
     from mbapy.file import replace_invalid_path_chr, convert_pdf_to_txt, read_text, opts_file
     import mbapy.web as web
 else:
     # release mode
     from .base import *
     from .file import replace_invalid_path_chr, convert_pdf_to_txt, opts_file
     from . import web
 
-scihub = SciHub()
+
+session = requests.Session()
 
 @parameter_checker(check_parameters_path, raise_err = False)
 def parse_ris(ris_path:str, fill_none_doi:str = None):
     """
     Parses a RIS file and returns the contents as a list of dictionaries.
 
     Parameters:
         ris_path (str): The path to the RIS file.
         fill_none_doi (str, optional): The DOI value to fill in for missing entries. Defaults to None.
 
     Returns:
         list: A list of dictionaries containing the parsed contents of the RIS file.
     """
-    with open('./data_tmp/savedrecs.ris', 'r', encoding='utf-8') as bibliography_file:
+    with open(ris_path, 'r', encoding='utf-8') as bibliography_file:
         ris = rispy.load(bibliography_file)
         if fill_none_doi is not None:
             for r in ris:
                 if 'doi' not in r:
                     r['doi'] = fill_none_doi
         return ris
     
 @parameter_checker(check_parameters_len, raise_err = False)
-def search_by_baidu(query:str, limit:int = 1):
+def search_by_baidu(query:str, limit:int = 1, proxies = None):
     """
     This function is used to search for articles on Baidu Scholar using a given query.
     
     Parameters:
         query (str): The search query.
         limit (int, optional): The maximum number of articles to retrieve. Defaults to 1.
         
@@ -58,26 +59,24 @@
         list: A list of dictionaries containing information about the articles found.
             Each dictionary has the following keys:
             - title (str): The title of the article.
             - abstract (str): The abstract of the article.
             - keyword (list): A list of keywords associated with the article.
             - doi (str): The DOI (Digital Object Identifier) of the article.
     """
-    from lxml import etree
     def _get_a_search_page(query:str, page:int = 0):
-        res = scihub.sess.request(method='GET', url='https://xueshu.baidu.com/s',
-                                params={'wd': query, 'pn': page, 'filter': 'sc_type%3D%7B1%7D'},
-                                proxies=scihub.proxies)
+        res = session.request(method='GET', url='https://xueshu.baidu.com/s',
+                              params={'wd': query, 'pn': page, 'filter': 'sc_type%3D%7B1%7D'})
         s = etree.HTML(res.text)
         return s.xpath("//div[@class='sc_content']/h3/a/@href")
     
     def _parse_links(links:list):
         results = []
         for link in links:
-            res = scihub.sess.request(method='GET', url=link, proxies=scihub.proxies)
+            res = session.request(method='GET', url=link, proxies=proxies)
             s = etree.HTML(res.text)
             title = s.xpath("//div[@class='main-info']/h3/a/text()")
             if len(title) == 0:
                 title = s.xpath("//div[@class='main-info']/h3/span/text()")
             title = get_default_for_bool(title, [''])[0].strip()
             abstract = s.xpath("//p[@class='abstract']/text()")
             abstract = get_default_for_bool(abstract, [''])[0].strip()
@@ -93,98 +92,208 @@
         # 未登录的百度学术一页只显示10个结果
         page = 1
         while limit > 10:
             limit -= 10
             links += _get_a_search_page(query, page)[: (limit%10 if limit > 10 else limit)]
             page += 1
     return _parse_links(links)
+
+@parameter_checker(check_parameters_len, check_parameters_len, raise_err = False)
+def search_by_pubmed(query:str, email:str = None, limit:int = 1):
+    from Bio import Entrez
+    Entrez.email = email  # 设置邮箱地址
+    handle = Entrez.esearch(db='pubmed', term=query, retmax=limit)
+    record = Entrez.read(handle)
+    handle.close()
+    pubmed_ids = record['IdList']
+
+    results = []
+    for pubmed_id in pubmed_ids:
+        handle = Entrez.efetch(db='pubmed', id=pubmed_id, retmode='xml')
+        record = Entrez.read(handle)
+        handle.close()
+        
+        if len(record['PubmedArticle']) > 0:
+            article = record['PubmedArticle'][0]['MedlineCitation']['Article']
+            title = str(article['ArticleTitle'])
+            doi = str(article['ELocationID'][0]) if 'ELocationID' in article else ''
+            abstract = str(article['Abstract']['AbstractText']) if 'Abstract' in article else ''
+            journal = str(article['Journal']['Title']) if 'Journal' in article else ''
+            results.append({'title': title, 'abstract': abstract, 'doi': doi, 'journal': journal})
+
+    return results
+    
         
-def search(query:str, limit:int = 1, search_engine:str = 'publons'):
+def search(query:str, limit:int = 1, search_engine:str = 'baidu xueshu', email:str = None):
     """
     Search for a given query using a specified search engine and return the results.
 
     Parameters:
     - query (str): The query string to search for.
     - limit (int): The maximum number of results to return.
     - search_engine (str): The search engine to use. Default is 'baidu xueshu'.
          allows: 'baidu xueshu', 'science direct', 'publons', if not recognized, returns None
 
     Returns:
     - The search results as a list of dict, contain 'title', 'abstract', 'keyword' and 'doi'.
     """
     if search_engine == 'baidu xueshu':
         return search_by_baidu(query, limit)
+    elif search_engine == 'pubmed' and email is not None:
+        return search_by_pubmed(query, email, limit)
     elif search_engine == 'science direct':
-        if os.path.isfile(get_storage_path('science_direct_cookie.txt')):
-            cookie = opts_file(get_storage_path('science_direct_cookie.txt'))
-        else:
-            import browser_cookie3
-            cookie = browser_cookie3.load('https://www.sciencedirect.com/')
-            opts_file(get_storage_path('science_direct_cookie.txt'), 'w', encoding='utf-8', data = cookie)
-        return scihub.search_by_science_direct(query, cookie, limit)
+        raise NotImplementedError
+        # if os.path.isfile(get_storage_path('science_direct_cookie.txt')):
+        #     cookie = opts_file(get_storage_path('science_direct_cookie.txt'))
+        # else:
+        #     import browser_cookie3
+        #     cookie = browser_cookie3.load('https://www.sciencedirect.com/')
+        #     opts_file(get_storage_path('science_direct_cookie.txt'), 'w', encoding='utf-8', data = cookie)
     elif search_engine == 'publons':
-        return scihub.search_by_publons([query], limit)
+        raise NotImplementedError
+        # return scihub.search_by_publons([query], limit)
     else:
         return put_err(f'Unknown search engine: {search_engine}, returns None', None)
 
+def _get_available_scihub_urls(proxies = None):
+    '''
+    Finds available scihub urls via http://tool.yovisun.com/scihub/
+    '''
+    links = []
+    res = session.request(method='GET', url='http://tool.yovisun.com/scihub/', proxies=proxies)
+    results = etree.HTML(res.text).xpath('//tr[@class="item"]')
+    for result in results:
+        # 我真的服了这个'latin1'编码，都没见过，还是问的chatGPT。。。
+        status = result.xpath('.//td[@class="status"]/span[@class="label  label-success"]/text()')[0]
+        status = status.encode('latin1').decode('utf-8')
+        if status == '可用':
+            ssl_link = result.xpath('.//td[@class="domainssl"]/a/@href')[0]
+            links.append(ssl_link)
+    return links
+
+# avoid multiple requests
+available_scihub_urls = None
+def _update_available_scihub_urls():
+    global available_scihub_urls
+    available_scihub_urls = _get_available_scihub_urls() if available_scihub_urls is None else available_scihub_urls
+    return available_scihub_urls    
+
+def _download_from_scihub_webpage(webpage:requests.Response, proxies = None):
+    """
+    Downloads a file from the SciHub webpage.
+
+    Args:
+        webpage (requests.Response): The response object of the SciHub webpage.
+        proxies (dict, optional): The proxies to be used for the request. Defaults to None.
+
+    Returns:
+        dict: A dictionary containing the title, DOI, and the response object of the download request.
+    """
+    def _get_valid_download_link(link:str):
+        available_scihub_urls = _update_available_scihub_urls()
+        if not link.startswith('http:'):
+            if link.find('sci-hub') == -1:
+                link = (available_scihub_urls[0]+'/') + link
+            else:
+                link = 'http:' + link
+        return link
+            
+    results = etree.HTML(webpage.text)
+    title = results.xpath('//div[@id="citation"]/i/text()')[0]
+    doi = results.xpath('//div[@id="citation"]//following-sibling::text()')[0]
+    download_link = results.xpath('//div[@id="buttons"]/button[1]/@onclick')[0].split("'")[1]
+    valid_download_link = _get_valid_download_link(download_link)
+    res = session.request(method='GET', url=valid_download_link, proxies=proxies)
+    return {'title': title, 'doi': doi, 'res': res}
+
 @parameter_checker(check_parameters_bool, raise_err = False)
-def download_from_scihub_by_doi(doi):
-    try:
-        return scihub.fetch({'doi':doi})
-    except:
-        return put_err(f'Maybe DOI: {doi:s} does not exist. scihub fetch error', None)
+def download_from_scihub_by_doi(doi:str, proxies = None):
+    """
+    Downloads a file from the Sci-Hub database using the DOI.
+
+    Parameters:
+        doi (str): The DOI of the file to download.
+        proxies (dict): A dictionary of proxies to use for the request.
+
+    Returns:
+        a dictionary containing the title, DOI, and the response object of the download request.
+        if meets error, returns None.
+
+    Raises:
+        Exception: If the DOI does not exist or if there is an error fetching the file from Sci-Hub.
+    """
+    # try:
+    available_scihub_urls = _update_available_scihub_urls()
+    res = session.request(method='GET', url=available_scihub_urls[0]+'/'+doi, proxies=proxies)
+    return _download_from_scihub_webpage(res)
+    # except:
+    #     return put_err(f'Maybe DOI: {doi:s} does not exist. scihub fetch error', None)
             
 @parameter_checker(check_parameters_bool, raise_err = False)
-def download_from_scihub_by_title(title):
-    scihub_url = scihub._get_available_scihub_urls()[0]
-    res = scihub.sess.post(scihub_url, data = {'request': title}, proxies=scihub.proxies)
-    doi = web.get_between(res.text, "doi:", "&nbsp", find_tail_from_head=True)
-    # TODO : xpath do not work
-    # dl = s.xpath("//div[@id='buttons']/ul/li/a[@href='#']")
-    return download_from_scihub_by_doi(doi)
+def download_from_scihub_by_title(title, proxies = None):
+    """
+    Downloads a document from Scihub by title.
+
+    Parameters:
+        title (str): The title of the document to be downloaded.
+        proxies (dict, optional): A dictionary of proxies to be used for the HTTP request.
+
+    Returns:
+        a dictionary containing the title, DOI, and the response object of the download request.
+        if meets error, returns None.
+
+    Raises:
+        Exception: If the document with the given title does not exist on Scihub.
+    """
+    try:
+        available_scihub_urls = _update_available_scihub_urls()
+        res = session.post(available_scihub_urls[0], data = {'request': title}, proxies=proxies)
+        return _download_from_scihub_webpage(res)
+    except:
+        return put_err(f'Maybe TITLE: {title:s} does not exist. scihub fetch error', None)
             
-@parameter_checker(check_parameters_path, raise_err = False)
 def download_by_scihub(dir: str, doi: str = None, title:str = None,
                        file_full_name:str = None, use_title_as_name: bool = True,
                        valid_path_chr:str = '_'):
     """
     Download a paper from Sci-Hub using its DOI.
     if file_full_name is None, use the paper's title as the file name, if not, use the paper's DOI as the file name.
 
     Args:
-        doi (str): The DOI (Digital Object Identifier) of the paper.
         dir (str): The directory where the downloaded file will be saved.
+        doi (str): The DOI (Digital Object Identifier) of the paper.
         file_full_name (str, optional): The name of the downloaded file, include the file extension(.pdf). Defaults to None.
         use_title_as_name (bool, optional): Whether to use the paper's title as the file name. Defaults to True.
         valid_path_chr (str, optional): The character used to replace invalid characters in the file name. Defaults to '_'.
 
     Returns:
         dict or None: If successful, returns a dictionary containing information
             about the downloaded paper. If unsuccessful, returns None.
     """
+    # check dir exists, if not, create it
+    if not check_parameters_path(dir):
+        os.makedirs(dir)
     # check whether doi or title are specified
     if doi is None and title is None:
         return put_err('Either DOI or title must be specified, returns None', None)
     # download from Sci-Hub by DOI or title
     if doi:
-        res, paper_info = download_from_scihub_by_doi(doi)
+        result = download_from_scihub_by_doi(doi)
     else:
-        res, paper_info = download_from_scihub_by_title(title)
-    if type(res) == dict and 'err' in res:        
-        return put_err(res['err'])
-    if not res:
+        result = download_from_scihub_by_title(title)
+    if result is None:
         return None
     # get the file name, save the file
     if file_full_name is not None:
         file_name = file_full_name
     else:
-        file_name = ((title if title else paper_info.title) if use_title_as_name else doi) + '.pdf'
+        file_name = ((title if title else result['title']) if use_title_as_name else doi) + '.pdf'
     file_name = replace_invalid_path_chr(file_name, valid_path_chr)
-    scihub._save(res.content, os.path.join(dir, file_name))
-    return paper_info
+    opts_file(os.path.join(dir, file_name), 'wb', data = result['res'].content)
+    return result
     
 def _flatten_pdf_bookmarks(*bookmarks):
     """
         Parse a list of bookmarks and return a flattened list of all bookmarks.
 
         Args:
             *bookmarks (List[Any]): A variable number of bookmark lists.
@@ -363,27 +472,28 @@
     struction = {}
     for key in struct:
         struction[key] = ''
 
 if __name__ == '__main__':
     # dev code
     from mbapy.base import rand_choose
-    from mbapy.file import convert_pdf_to_txt
+    from mbapy.file import convert_pdf_to_txt, read_json
     
     # RIS parse
     ris = parse_ris('./data_tmp/savedrecs.ris', '')
     ris = rand_choose(ris)
     print(f'title: {ris["title"]}\ndoi: {ris["doi"]}')
     
     # search
-    search_result = search_by_baidu('linaclotide', 11)
+    # search_result = search_by_baidu('linaclotide', 11)
+    search_result = search_by_pubmed('linaclotide', read_json('./data_tmp/id.json')['edu_email'], 11)
     search_result2 = search(ris["title"])
     
     # download
     dl_result = download_by_scihub('./data_tmp/', title = search_result[0]['title'])
-    download_by_scihub(ris["doi"], './data_tmp/', file_full_name = f'{ris["title"]:s}.pdf')
+    download_by_scihub('./data_tmp/', '10.1097/j.pain.0000000000001905', ris["title"], file_full_name = f'{ris["title"]:s}.pdf')
     
     # extract section
     pdf_path = replace_invalid_path_chr("./data_tmp/{:s}.pdf".format(ris["title"]))
     sections = get_english_part_of_bookmarks(get_section_bookmarks(pdf_path))
     paper, section = convert_pdf_to_txt(pdf_path), rand_choose(sections, 0)
     print(sections, section, get_section_from_paper(paper, section, keys=sections))
```

### Comparing `mbapy-0.1.4.1/mbapy/plot.py` & `mbapy-0.1.4.2/mbapy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,38 +110,42 @@
                 pos[axis_idx].append(st_pos+this_hue_per/2)
                 st_pos += this_hue_per
     return xlabels, pos
 
 def plot_bar(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     stack bar plot with hue style\n
-    factors:[low_lever_factor, medium_lever_factor, ...] or just one
-    tags:[stack_low_y, stack_medium_y, ...] or just one
-    df:df from pro_bar_data or sort_df_factors
-        kwargs:
-    width = 0.4
-    bar_space = 0.2
-    xrotations = [0]*len(factors)
-    colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
-    hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
-    labels:None,
-    font_size:None, 
-    offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]
+    factors:[low_lever_factor, medium_lever_factor, ...] or just one\n
+    tags:[stack_low_y, stack_medium_y, ...] or just one\n
+    df:df from pro_bar_data or sort_df_factors\n
+    kwargs:
+        width = 0.4\n
+        bar_space = 0.2\n
+        xrotations = [0]*len(factors)\n
+        colors = plt.rcParams['axes.prop_cycle'].by_key()['color']\n
+        hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],\n
+        labels:None,\n
+        font_size:None, \n
+        offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]\n
+        err = None\n
+        err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k'}
     """
     ax1 = host_subplot(111, axes_class=axisartist.Axes)
     
     if len(tags) == 0:
         tags = list(df.columns)[len(factors):]
     args = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
                             'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
                             'hatchs':['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
                             'font_size':None,
                             'labels':None,
                             'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
-                            'edgecolor':'white'},
+                            'edgecolor':'white',
+                            'err':None,
+                            'err_kwargs':{'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k'}},
                             kwargs)
     args.xrotations.append(0)
     xlabels, pos = pro_hue_pos(factors, df, args.width, args.bar_space)
     bottom = kwargs['bottom'] if 'bottom' in kwargs else np.zeros(len(pos[0]))
     
     for yIdx, yName in enumerate(tags):
         if args.labels is not None:
@@ -152,14 +156,17 @@
                 edgecolor=args.edgecolor, color=args.colors[yIdx])
         bottom += df[yName]
     ax1.set_xlim(0, pos[0][-1]+args.bar_space+args.width/2)
     ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
     plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0])
     if args.font_size is not None:
         plt.setp(ax1.axis["bottom"].major_ticklabels, fontsize=args.font_size[0])
+    # err bar
+    if args.err is not None:        
+        plt.errorbar(pos[0], bottom, yerr=1.96 * args.err, **args.err_kwargs)
     
     axs = []
     for idx, sub_pos in enumerate(pos[1:]):
         axs.append(ax1.twiny())
         axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
         new_axisline = axs[-1].get_grid_helper().new_fixed_axis
         axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx]))
@@ -305,14 +312,17 @@
     df = pd.read_excel('./data/plot.xlsx', sheet_name='MWM')
     df['Animal Type'] = df['Animal Type'].astype('str')
     model = mst.multicomp_turkeyHSD({'Animal Type':[]}, 'Duration', df)
     result = mst.turkey_to_table(model)
     print(result)
     sub_df = get_df_data({'Animal Type':[]}, ['Duration'], df)
     sub_df = pro_bar_data(['Animal Type'], ['Duration'], sub_df)
+    # test err
+    plot_bar(['Animal Type'], ['Duration'], sub_df, err = sub_df['Duration_SE'])
+    plt.show()
     plot_turkey(sub_df['Duration'], sub_df['Duration_SE'], model)
     plt.show()
     
     df = pd.DataFrame({'Month': [5, 5, 6, 6, 7, 7, 8, 8, 9, 9],
                        'Ozone': [23.61538, 22.22445, 29.44444, 18.20790, 59.11538, 31.63584, 59.96154, 39.68121, 31.44828, 24.14182]})
     model = mst.multicomp_turkeyHSD({'Month':[]}, 'Ozone', df)
     result = mst.turkey_to_table(model)
```

### Comparing `mbapy-0.1.4.1/mbapy/stats/__init__.py` & `mbapy-0.1.4.2/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/stats/df.py` & `mbapy-0.1.4.2/mbapy/stats/df.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/stats/geography.py` & `mbapy-0.1.4.2/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/stats/reg.py` & `mbapy-0.1.4.2/mbapy/stats/reg.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/stats/test.py` & `mbapy-0.1.4.2/mbapy/stats/test.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/storage/stats.dll` & `mbapy-0.1.4.2/mbapy/storage/stats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/mbapy/web.py` & `mbapy-0.1.4.2/mbapy/web.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 import pandas as pd
 from bs4 import BeautifulSoup
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
-from . import base
-from mbapy.base import put_err
-from mbapy.file import save_json, read_json, save_excel, read_excel
+if __name__ == '__main__':
+    from mbapy import base as mb
+    from mbapy.file import save_json, read_json, save_excel, read_excel
+else:
+    from . import base as mb
+    from .file import save_json, read_json, save_excel, read_excel
 
 CHROMEDRIVERPATH = r"C:\Users\Administrator\AppData\Local\Google\Chrome\Application\chromedriver.exe"
 
 def get_url_page(url:str, coding = 'gbk'):
     """
     Given a url and a coding, this function returns the decoded content of the page.
     :param url: A string representing the URL to be visited.
@@ -123,17 +126,17 @@
     """
     headIdx = string.rfind(head) if headRFind else string.find(head)
     if find_tail_from_head:
         tailIdx = string[headIdx+len(head):].find(tail) + headIdx + len(head)
     else:
         tailIdx = string.rfind(tail) if tailRFind else string.find(tail)
     if headIdx == -1 or tailIdx == -1:
-        return put_err(f"{head if headIdx == -1 else tail:s} not found, return string", string)
+        return mb.put_err(f"{head if headIdx == -1 else tail:s} not found, return string", string)
     if headIdx == tailIdx:
-        return put_err(f"headIdx == tailIdx with head:{head:s} and string:{string:s}, return ''", '')
+        return mb.put_err(f"headIdx == tailIdx with head:{head:s} and string:{string:s}, return ''", '')
     idx1 = headIdx if ret_head else headIdx+len(head)
     idx2 = tailIdx+len(tail) if ret_tail else tailIdx
     return string[idx1:idx2]
 def get_between_re(string:str, head:str, tail:str,
                head_r:bool = False, tail_r:bool = True,
                 ret_head:bool = False, ret_tail:bool = False):
     """
@@ -159,15 +162,15 @@
     :type ret_tail: bool
     :return: The substring between `head` and `tail` in `string`.
     :rtype: str
     """
     h = re.compile(head).search(string) if len(head) > 0 else ''
     t = re.compile(tail).search(string)
     if h is None or t is None:
-        return put_err(f"not found with head:{head:s} and tail:{tail:s}, return string", string)
+        return mb.put_err(f"not found with head:{head:s} and tail:{tail:s}, return string", string)
     else:
         h, t = h.group(0) if h != '' else '', t.group(0)
     return get_between(string, h, t, head_r, tail_r, ret_head, ret_tail)
 
 
 def transfer_str2by(by:str):
     """
@@ -352,16 +355,31 @@
                 print('get quit sig')
                 return retList            
         for que in self.getDataQues:
             while not que.empty():
                 retList.append(que.get())
         return retList
 
-if base._Params['LAUNCH_WEB_SUB_THREAD']:
+def launch_sub_thread():
+    """
+    Launches a sub-thread to run a separate task concurrently with the main thread.
+
+    This function creates a global `statuesQue` queue and puts a dictionary with the keys `quit` and `input` into the queue. The `quit` key is set to `False` and the `input` key is set to `None`. 
+    The function then starts a new thread by calling the `_wait_for_quit` function with the `statuesQue` queue as an argument. 
+    Finally, the function prints the message "web sub thread started".
+
+    Parameters:
+    None
+
+    Returns:
+    None
+    """
+    global statuesQue
     statuesQue = Queue()
     statuesQue.put(
         {
             "quit": False,
             "input": None,
         }
     )
-    _thread.start_new_thread(_wait_for_quit, (statuesQue,))
+    _thread.start_new_thread(_wait_for_quit, (statuesQue,))
+    print('mbapy::web: web sub thread started')
```

### Comparing `mbapy-0.1.4.1/mbapy.egg-info/PKG-INFO` & `mbapy-0.1.4.2/mbapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
@@ -22,42 +22,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
  * @LastEditors: BHM-Bob 2262029386@qq.com
- * @LastEditTime: 2023-07-12 22:06:01
+ * @LastEditTime: 2023-07-13 19:32:26
  * @Description: 
 -->
 # BA_PY
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
 
 ![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy)
  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
 
 
 ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY)
 
-some helpful python scripts. (Basic for All in Python)
-Mainly contains sci-plot, stats, web-crawler and deeplearing-torch.
+mbapy contains some helpful python scripts, which aims at goal of *Basic for All in Python*.
+Mainly contains sci-plot, stats, web-crawler, sci-paper utils and deeplearing-torch.
 
 ## get start
 
-### install 
-#### pypi 
+#### install 
 Now, mbapy only support pypi install:  
-`pip install mbapy`  
-For updating:  
-`pip install --upgrade mbapy`  
+```
+pip install mbapy
+```
+
+If you find the latest release version has installing problems, you can download this repo and try:
+```
+pip install .
+```
 
-### wiki
-[wiki](https://github.com/BHM-Bob/BA_PY/wiki)
+#### wiki
+mbapy has it's wiki as API document, you can find it in [wiki](https://github.com/BHM-Bob/BA_PY/wiki).
 
 # contain  
 ## mbapy python package  
 #### \_\_version\_\_  
 *some version info*
 #### base
```

### Comparing `mbapy-0.1.4.1/mbapy.egg-info/SOURCES.txt` & `mbapy-0.1.4.2/mbapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/setup.py` & `mbapy-0.1.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-13 19:11:41
+LastEditTime: 2023-07-16 00:57:54
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 """
 
@@ -59,14 +59,15 @@
     "scipy>=1.9.1",
     "seaborn>=0.11.2",
     "selenium>=4.5.0",
     "urllib3>=1.26.12",
     "openpyxl",
     "statsmodels",
     "scikit_posthocs",
+    "rispy",
     "PyPDF2",
     "lxml",
 ]
 
 
 setup(
     name = "mbapy",
@@ -105,8 +106,8 @@
     
     install_requires=requires,
 )
 
 # pip install .
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.1.4.tar.gz
+# twine upload dist/mbapy-0.1.4.2.tar.gz
```

### Comparing `mbapy-0.1.4.1/test/test_base.py` & `mbapy-0.1.4.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4.1/test/test_web.py` & `mbapy-0.1.4.2/test/test_web.py`

 * *Files identical despite different names*

