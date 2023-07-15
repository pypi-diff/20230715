# Comparing `tmp/big_query_testing_xyz-0.3.tar.gz` & `tmp/big_query_testing_xyz-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big_query_testing_xyz-0.3.tar", last modified: Sat Jul 15 19:15:54 2023, max compression
+gzip compressed data, was "big_query_testing_xyz-0.4.tar", last modified: Sat Jul 15 20:33:05 2023, max compression
```

## Comparing `big_query_testing_xyz-0.3.tar` & `big_query_testing_xyz-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:15:54.457088 big_query_testing_xyz-0.3/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-15 18:48:38.000000 big_query_testing_xyz-0.3/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)      768 2023-07-15 19:15:54.457357 big_query_testing_xyz-0.3/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-15 18:48:00.000000 big_query_testing_xyz-0.3/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:15:54.445133 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)      768 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      306 2023-07-15 19:15:54.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       29 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       11 2023-07-15 19:15:53.000000 big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/top_level.txt
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 19:15:54.453015 big_query_testing_xyz-0.3/code_query/
--rw-r--r--   0 vedantrathi   (501) staff       (20)       19 2023-07-15 18:46:45.000000 big_query_testing_xyz-0.3/code_query/__init__.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)      724 2023-07-15 19:12:29.000000 big_query_testing_xyz-0.3/code_query/main.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-15 19:15:54.460162 big_query_testing_xyz-0.3/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1616 2023-07-15 19:12:57.000000 big_query_testing_xyz-0.3/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 20:33:05.351572 big_query_testing_xyz-0.4/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-15 18:48:38.000000 big_query_testing_xyz-0.4/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      775 2023-07-15 20:33:05.351689 big_query_testing_xyz-0.4/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-15 18:48:00.000000 big_query_testing_xyz-0.4/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 20:33:05.350712 big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      775 2023-07-15 20:33:05.000000 big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      306 2023-07-15 20:33:05.000000 big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-15 20:33:05.000000 big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       29 2023-07-15 20:33:05.000000 big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       11 2023-07-15 20:33:05.000000 big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/top_level.txt
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-15 20:33:05.351349 big_query_testing_xyz-0.4/code_query/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       19 2023-07-15 18:46:45.000000 big_query_testing_xyz-0.4/code_query/__init__.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1874 2023-07-15 20:26:14.000000 big_query_testing_xyz-0.4/code_query/main.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-15 20:33:05.352138 big_query_testing_xyz-0.4/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1623 2023-07-15 20:32:42.000000 big_query_testing_xyz-0.4/setup.py
```

### Comparing `big_query_testing_xyz-0.3/LICENSE.txt` & `big_query_testing_xyz-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `big_query_testing_xyz-0.3/PKG-INFO` & `big_query_testing_xyz-0.4/big_query_testing_xyz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: big_query_testing_xyz
-Version: 0.3
+Name: big-query-testing-xyz
+Version: 0.4
 Summary: sample package
-Home-page: https://github.com/vrathi101/big_query_test.git
-Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_03.tar.gz
+Home-page: https://github.com/vrathi101/big_query_testing_xyz.git
+Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_04.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `big_query_testing_xyz-0.3/big_query_testing_xyz.egg-info/PKG-INFO` & `big_query_testing_xyz-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: big-query-testing-xyz
-Version: 0.3
+Name: big_query_testing_xyz
+Version: 0.4
 Summary: sample package
-Home-page: https://github.com/vrathi101/big_query_test.git
-Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_03.tar.gz
+Home-page: https://github.com/vrathi101/big_query_testing_xyz.git
+Download-URL: https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_04.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `big_query_testing_xyz-0.3/setup.py` & `big_query_testing_xyz-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 setuptools.setup(
   name = 'big_query_testing_xyz',         # How you named your package
   packages = ['code_query'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'sample package',   # Give a short description about your library
   author = 'VEDANT RATHI',                   # Type in your name
   author_email = 'vedrathi10@gmail.com',      # Type in your E-Mail
-  url = 'https://github.com/vrathi101/big_query_test.git',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_03.tar.gz',    # I explain this later on
+  url = 'https://github.com/vrathi101/big_query_testing_xyz.git',   # Provide either the link to your github or to your website
+  download_url = 'https://github.com/vrathi101/big_query_testing_xyz/archive/refs/tags/v_04.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[
     'pandas',
     'google-cloud-bigquery'
 ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

