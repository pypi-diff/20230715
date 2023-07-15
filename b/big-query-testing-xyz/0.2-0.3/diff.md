# Comparing `tmp/big_query_testing_xyz-0.2.tar.gz` & `tmp/big_query_testing_xyz-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big_query_testing_xyz-0.2.tar", last modified: Sat Jul 15 19:08:48 2023, max compression
+gzip compressed data, was "big_query_testing_xyz-0.3.tar", last modified: Sat Jul 15 19:15:54 2023, max compression
```

## Comparing `big_query_testing_xyz-0.2.tar` & `big_query_testing_xyz-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:08:48.320074 big_query_testing_xyz-0.2/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-15 18:48:38.000000 big_query_testing_xyz-0.2/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)      768 2023-07-15 19:08:48.320255 big_query_testing_xyz-0.2/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-15 18:48:00.000000 big_query_testing_xyz-0.2/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:08:48.317316 big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)      768 2023-07-15 19:08:48.000000 big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      306 2023-07-15 19:08:48.000000 big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-15 19:08:48.000000 big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       29 2023-07-15 19:08:48.000000 big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       11 2023-07-15 19:08:48.000000 big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/top_level.txt
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:08:48.319288 big_query_testing_xyz-0.2/code_query/
--rw-r--r--   0 vedantrathi   (501) staff       (20)       19 2023-07-15 18:46:45.000000 big_query_testing_xyz-0.2/code_query/__init__.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)      717 2023-07-15 18:44:19.000000 big_query_testing_xyz-0.2/code_query/main.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-15 19:08:48.320985 big_query_testing_xyz-0.2/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1616 2023-07-15 19:08:22.000000 big_query_testing_xyz-0.2/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:15:54.457088 big_query_testing_xyz-0.3/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-15 18:48:38.000000 big_query_testing_xyz-0.3/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      768 2023-07-15 19:15:54.457357 big_query_testing_xyz-0.3/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-15 18:48:00.000000 big_query_testing_xyz-0.3/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:15:54.445133 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      768 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      306 2023-07-15 19:15:54.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       29 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       11 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/top_level.txt
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:15:54.453015 big_query_testing_xyz-0.3/code_query/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       19 2023-07-15 18:46:45.000000 big_query_testing_xyz-0.3/code_query/__init__.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      724 2023-07-15 19:12:29.000000 big_query_testing_xyz-0.3/code_query/main.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-15 19:15:54.460162 big_query_testing_xyz-0.3/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1616 2023-07-15 19:12:57.000000 big_query_testing_xyz-0.3/setup.py
```

### Comparing `big_query_testing_xyz-0.2/LICENSE.txt` & `big_query_testing_xyz-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `big_query_testing_xyz-0.2/PKG-INFO` & `big_query_testing_xyz-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: big_query_testing_xyz
-Version: 0.2
+Version: 0.3
 Summary: sample package
 Home-page: https://github.com/vrathi101/big_query_test.git
-Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_03.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `big_query_testing_xyz-0.2/big_query_testing_xyz.egg-info/PKG-INFO` & `big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: big-query-testing-xyz
-Version: 0.2
+Version: 0.3
 Summary: sample package
 Home-page: https://github.com/vrathi101/big_query_test.git
-Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_03.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `big_query_testing_xyz-0.2/code_query/main.py` & `big_query_testing_xyz-0.3/code_query/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from google.cloud import bigquery
 import pandas as pd
 
-credentials_path = '/Users/vedantrathi/Desktop/big_query_test/irsdata-pypi-4955991a9ae8.json'
+credentials_path = '/Users/vedantrathi/Desktop/big_query_testing_xyz/irsdata-pypi-4955991a9ae8.json'
 
 
 project_id = 'irsdata-pypi'
 dataset_id = 'dataset001'
 table_id = 'vw_irs_filing_test02'
 # table_id = 'irsdata-pypi.dataset001.irs_filing'
```

### Comparing `big_query_testing_xyz-0.2/setup.py` & `big_query_testing_xyz-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 setuptools.setup(
   name = 'big_query_testing_xyz',         # How you named your package
   packages = ['code_query'],   # Chose the same as "name"
-  version = '0.2',      # Start with a small number and increase it with every change you make
+  version = '0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'sample package',   # Give a short description about your library
   author = 'VEDANT RATHI',                   # Type in your name
   author_email = 'vedrathi10@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/vrathi101/big_query_test.git',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_02.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_03.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[
     'pandas',
     'google-cloud-bigquery'
 ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

