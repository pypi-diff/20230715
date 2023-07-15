# Comparing `tmp/rapidpe_rift_pipe-0.5.4.dev20230714.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.4.dev20230715.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230714.tar", last modified: Fri Jul 14 05:15:32 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230715.tar", last modified: Sat Jul 15 05:18:31 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.4.dev20230714.tar` & `rapidpe_rift_pipe-0.5.4.dev20230715.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.559000 rapidpe_rift_pipe-0.5.4.dev20230714/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-14 05:15:32.559000 rapidpe_rift_pipe-0.5.4.dev20230714/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.544999 rapidpe_rift_pipe-0.5.4.dev20230714/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.548999 rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-07 05:15:05.000000 rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-14 05:15:32.559000 rapidpe_rift_pipe-0.5.4.dev20230714/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.544999 rapidpe_rift_pipe-0.5.4.dev20230714/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.555999 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-10 17:53:47.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.557000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 05:15:20.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.557999 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 05:15:20.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31454 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-07 05:15:05.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.557999 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 05:15:20.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:15:32.557000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 05:15:32.000000 rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.783893 rapidpe_rift_pipe-0.5.4.dev20230715/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-15 05:18:31.783893 rapidpe_rift_pipe-0.5.4.dev20230715/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.765893 rapidpe_rift_pipe-0.5.4.dev20230715/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.769893 rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-15 05:18:31.784893 rapidpe_rift_pipe-0.5.4.dev20230715/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.766893 rapidpe_rift_pipe-0.5.4.dev20230715/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.780893 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-10 17:53:47.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.782893 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.782893 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31454 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.783893 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 05:18:31.782893 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 05:18:31.000000 rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/COPYING` & `rapidpe_rift_pipe-0.5.4.dev20230715/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230715/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.5.4.dev20230714
+Version: 0.5.4.dev20230715
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/setup.cfg` & `rapidpe_rift_pipe-0.5.4.dev20230715/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230714
+tag_build = dev.20230715
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.5.4.dev20230714
+Version: 0.5.4.dev20230715
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230714/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.4.dev20230715/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*
