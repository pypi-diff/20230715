# Comparing `tmp/niacin-0.5.1.tar.gz` & `tmp/niacin-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/niacin-0.5.1.tar", last modified: Sat Apr  2 17:06:07 2022, max compression
+gzip compressed data, was "niacin-0.5.2.tar", last modified: Sat Jul 15 16:54:05 2023, max compression
```

## Comparing `niacin-0.5.1.tar` & `niacin-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/
--rw-r--r--   0 dillon     (501) staff       (20)     4258 2022-04-02 17:06:07.000000 niacin-0.5.1/PKG-INFO
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin.egg-info/
--rw-r--r--   0 dillon     (501) staff       (20)     4258 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin.egg-info/PKG-INFO
--rw-r--r--   0 dillon     (501) staff       (20)      692 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin.egg-info/SOURCES.txt
--rw-r--r--   0 dillon     (501) staff       (20)      168 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin.egg-info/requires.txt
--rw-r--r--   0 dillon     (501) staff       (20)        7 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin.egg-info/top_level.txt
--rw-r--r--   0 dillon     (501) staff       (20)        1 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin.egg-info/dependency_links.txt
--rw-r--r--   0 dillon     (501) staff       (20)     3140 2020-08-22 20:17:51.000000 niacin-0.5.1/README.md
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/timeseries/
--rw-r--r--   0 dillon     (501) staff       (20)     8943 2021-03-25 23:06:45.000000 niacin-0.5.1/niacin/timeseries/freq.py
--rw-r--r--   0 dillon     (501) staff       (20)    17200 2021-03-25 23:06:45.000000 niacin-0.5.1/niacin/timeseries/time.py
--rw-r--r--   0 dillon     (501) staff       (20)      958 2021-03-25 23:06:45.000000 niacin-0.5.1/niacin/timeseries/__init__.py
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/augment/
--rw-r--r--   0 dillon     (501) staff       (20)      148 2020-08-24 12:53:14.000000 niacin-0.5.1/niacin/augment/__init__.py
--rw-r--r--   0 dillon     (501) staff       (20)     2974 2020-08-24 12:53:14.000000 niacin-0.5.1/niacin/augment/randaugment.py
--rw-r--r--   0 dillon     (501) staff       (20)       21 2022-04-02 16:57:07.000000 niacin-0.5.1/niacin/__init__.py
--rw-r--r--   0 dillon     (501) staff       (20)        0 2020-02-08 23:58:26.000000 niacin-0.5.1/niacin/py.typed
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/text/
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/text/compat/
--rw-r--r--   0 dillon     (501) staff       (20)      107 2020-08-22 22:16:56.000000 niacin-0.5.1/niacin/text/compat/__init__.py
--rw-r--r--   0 dillon     (501) staff       (20)     6787 2020-08-22 22:16:56.000000 niacin-0.5.1/niacin/text/compat/pytorch.py
--rw-r--r--   0 dillon     (501) staff       (20)        0 2020-06-04 00:19:24.000000 niacin-0.5.1/niacin/text/__init__.py
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/text/en/
--rw-r--r--   0 dillon     (501) staff       (20)     8902 2022-04-02 16:54:08.000000 niacin-0.5.1/niacin/text/en/char.py
--rw-r--r--   0 dillon     (501) staff       (20)     1160 2022-04-02 16:54:08.000000 niacin-0.5.1/niacin/text/en/__init__.py
--rw-r--r--   0 dillon     (501) staff       (20)     5680 2020-06-04 00:19:24.000000 niacin-0.5.1/niacin/text/en/sentence.py
--rw-r--r--   0 dillon     (501) staff       (20)     7924 2022-04-02 16:54:08.000000 niacin-0.5.1/niacin/text/en/word.py
-drwxr-xr-x   0 dillon     (501) staff       (20)        0 2022-04-02 17:06:07.000000 niacin-0.5.1/niacin/data/
--rw-r--r--   0 dillon     (501) staff       (20)   106476 2018-11-16 11:58:21.000000 niacin-0.5.1/niacin/data/misspellings.json
--rw-r--r--   0 dillon     (501) staff       (20)      922 2018-11-16 11:58:21.000000 niacin-0.5.1/niacin/data/neighbors.json
--rw-r--r--   0 dillon     (501) staff       (20)  2003004 2020-02-08 23:42:13.000000 niacin-0.5.1/niacin/data/hyponyms.json
--rw-r--r--   0 dillon     (501) staff       (20)      392 2020-02-08 23:58:26.000000 niacin-0.5.1/niacin/data/contractions.json
--rw-r--r--   0 dillon     (501) staff       (20)  2597888 2020-02-08 23:42:13.000000 niacin-0.5.1/niacin/data/hypernyms.json
--rw-r--r--   0 dillon     (501) staff       (20)  4173951 2020-02-19 05:08:51.000000 niacin-0.5.1/niacin/data/synonyms.json
--rw-r--r--   0 dillon     (501) staff       (20)      885 2022-04-02 16:56:49.000000 niacin-0.5.1/setup.py
--rw-r--r--   0 dillon     (501) staff       (20)       38 2022-04-02 17:06:07.000000 niacin-0.5.1/setup.cfg
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.639888 niacin-0.5.2/
+-rw-r--r--   0 dillon     (501) staff       (20)     1461 2018-11-21 00:44:46.000000 niacin-0.5.2/LICENSE
+-rw-r--r--   0 dillon     (501) staff       (20)       80 2023-07-15 16:45:45.000000 niacin-0.5.2/MANIFEST.in
+-rw-r--r--   0 dillon     (501) staff       (20)     3349 2023-07-15 16:54:05.639638 niacin-0.5.2/PKG-INFO
+-rw-r--r--   0 dillon     (501) staff       (20)     3140 2020-08-22 20:17:51.000000 niacin-0.5.2/README.md
+-rw-r--r--   0 dillon     (501) staff       (20)       32 2020-08-22 22:16:56.000000 niacin-0.5.2/backtranslate-requirements.txt
+-rw-r--r--   0 dillon     (501) staff       (20)        0 2020-02-08 23:09:23.000000 niacin-0.5.2/conftest.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.625615 niacin-0.5.2/niacin/
+-rw-r--r--   0 dillon     (501) staff       (20)       21 2023-07-15 16:47:39.000000 niacin-0.5.2/niacin/__init__.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.627322 niacin-0.5.2/niacin/augment/
+-rw-r--r--   0 dillon     (501) staff       (20)      148 2020-08-24 12:53:14.000000 niacin-0.5.2/niacin/augment/__init__.py
+-rw-r--r--   0 dillon     (501) staff       (20)     2974 2020-08-24 12:53:14.000000 niacin-0.5.2/niacin/augment/randaugment.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.633091 niacin-0.5.2/niacin/data/
+-rw-r--r--   0 dillon     (501) staff       (20)      392 2020-02-08 23:58:26.000000 niacin-0.5.2/niacin/data/contractions.json
+-rw-r--r--   0 dillon     (501) staff       (20)  2597888 2020-02-08 23:42:13.000000 niacin-0.5.2/niacin/data/hypernyms.json
+-rw-r--r--   0 dillon     (501) staff       (20)  2003004 2020-02-08 23:42:13.000000 niacin-0.5.2/niacin/data/hyponyms.json
+-rw-r--r--   0 dillon     (501) staff       (20)   106476 2018-11-16 11:58:21.000000 niacin-0.5.2/niacin/data/misspellings.json
+-rw-r--r--   0 dillon     (501) staff       (20)      922 2018-11-16 11:58:21.000000 niacin-0.5.2/niacin/data/neighbors.json
+-rw-r--r--   0 dillon     (501) staff       (20)  4173951 2020-02-19 05:08:51.000000 niacin-0.5.2/niacin/data/synonyms.json
+-rw-r--r--   0 dillon     (501) staff       (20)        0 2020-02-08 23:58:26.000000 niacin-0.5.2/niacin/py.typed
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.637210 niacin-0.5.2/niacin/text/
+-rw-r--r--   0 dillon     (501) staff       (20)        0 2020-06-04 00:19:24.000000 niacin-0.5.2/niacin/text/__init__.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.637619 niacin-0.5.2/niacin/text/compat/
+-rw-r--r--   0 dillon     (501) staff       (20)      107 2020-08-22 22:16:56.000000 niacin-0.5.2/niacin/text/compat/__init__.py
+-rw-r--r--   0 dillon     (501) staff       (20)     6787 2020-08-22 22:16:56.000000 niacin-0.5.2/niacin/text/compat/pytorch.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.638493 niacin-0.5.2/niacin/text/en/
+-rw-r--r--   0 dillon     (501) staff       (20)     1160 2022-04-02 16:54:08.000000 niacin-0.5.2/niacin/text/en/__init__.py
+-rw-r--r--   0 dillon     (501) staff       (20)     8902 2022-04-02 16:54:08.000000 niacin-0.5.2/niacin/text/en/char.py
+-rw-r--r--   0 dillon     (501) staff       (20)     5680 2020-06-04 00:19:24.000000 niacin-0.5.2/niacin/text/en/sentence.py
+-rw-r--r--   0 dillon     (501) staff       (20)     7924 2022-04-02 16:54:08.000000 niacin-0.5.2/niacin/text/en/word.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.639213 niacin-0.5.2/niacin/timeseries/
+-rw-r--r--   0 dillon     (501) staff       (20)      958 2021-03-25 23:06:45.000000 niacin-0.5.2/niacin/timeseries/__init__.py
+-rw-r--r--   0 dillon     (501) staff       (20)     8943 2021-03-25 23:06:45.000000 niacin-0.5.2/niacin/timeseries/freq.py
+-rw-r--r--   0 dillon     (501) staff       (20)    17200 2021-03-25 23:06:45.000000 niacin-0.5.2/niacin/timeseries/time.py
+drwxr-xr-x   0 dillon     (501) staff       (20)        0 2023-07-15 16:54:05.626822 niacin-0.5.2/niacin.egg-info/
+-rw-r--r--   0 dillon     (501) staff       (20)     3349 2023-07-15 16:54:05.000000 niacin-0.5.2/niacin.egg-info/PKG-INFO
+-rw-r--r--   0 dillon     (501) staff       (20)      806 2023-07-15 16:54:05.000000 niacin-0.5.2/niacin.egg-info/SOURCES.txt
+-rw-r--r--   0 dillon     (501) staff       (20)        1 2023-07-15 16:54:05.000000 niacin-0.5.2/niacin.egg-info/dependency_links.txt
+-rw-r--r--   0 dillon     (501) staff       (20)      168 2023-07-15 16:54:05.000000 niacin-0.5.2/niacin.egg-info/requires.txt
+-rw-r--r--   0 dillon     (501) staff       (20)        7 2023-07-15 16:54:05.000000 niacin-0.5.2/niacin.egg-info/top_level.txt
+-rw-r--r--   0 dillon     (501) staff       (20)       61 2020-06-04 00:19:24.000000 niacin-0.5.2/pytest.ini
+-rw-r--r--   0 dillon     (501) staff       (20)       29 2020-08-22 20:06:23.000000 niacin-0.5.2/requirements.txt
+-rw-r--r--   0 dillon     (501) staff       (20)       38 2023-07-15 16:54:05.639963 niacin-0.5.2/setup.cfg
+-rw-r--r--   0 dillon     (501) staff       (20)      885 2023-07-15 16:46:53.000000 niacin-0.5.2/setup.py
+-rw-r--r--   0 dillon     (501) staff       (20)       22 2020-08-22 22:16:56.000000 niacin-0.5.2/torch-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `niacin-0.5.1/niacin.egg-info/SOURCES.txt` & `niacin-0.5.2/niacin.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+LICENSE
+MANIFEST.in
 README.md
+backtranslate-requirements.txt
+conftest.py
+pytest.ini
+requirements.txt
 setup.py
+torch-requirements.txt
 niacin/__init__.py
 niacin/py.typed
 niacin.egg-info/PKG-INFO
 niacin.egg-info/SOURCES.txt
 niacin.egg-info/dependency_links.txt
 niacin.egg-info/requires.txt
 niacin.egg-info/top_level.txt
```

### Comparing `niacin-0.5.1/README.md` & `niacin-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/timeseries/freq.py` & `niacin-0.5.2/niacin/timeseries/freq.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/timeseries/time.py` & `niacin-0.5.2/niacin/timeseries/time.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/timeseries/__init__.py` & `niacin-0.5.2/niacin/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/augment/randaugment.py` & `niacin-0.5.2/niacin/augment/randaugment.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/text/compat/pytorch.py` & `niacin-0.5.2/niacin/text/compat/pytorch.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/text/en/char.py` & `niacin-0.5.2/niacin/text/en/char.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/text/en/__init__.py` & `niacin-0.5.2/niacin/text/en/__init__.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/text/en/sentence.py` & `niacin-0.5.2/niacin/text/en/sentence.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/text/en/word.py` & `niacin-0.5.2/niacin/text/en/word.py`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/data/misspellings.json` & `niacin-0.5.2/niacin/data/misspellings.json`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/data/neighbors.json` & `niacin-0.5.2/niacin/data/neighbors.json`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/data/hyponyms.json` & `niacin-0.5.2/niacin/data/hyponyms.json`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/data/hypernyms.json` & `niacin-0.5.2/niacin/data/hypernyms.json`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/niacin/data/synonyms.json` & `niacin-0.5.2/niacin/data/synonyms.json`

 * *Files identical despite different names*

### Comparing `niacin-0.5.1/setup.py` & `niacin-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     extras[extra] = requirements
     combined.update(requirements)
 extras['all'] = sorted(combined)
 
 
 setup(
     name='niacin',
-    version='0.5.1',
+    version='0.5.2',
     packages=find_packages(),
     package_data={
         'niacin': ['data/*', 'py.typed']
     },
     python_requires=">=3.6",
     install_requires=install_requirements,
     extras_require=extras,
```

