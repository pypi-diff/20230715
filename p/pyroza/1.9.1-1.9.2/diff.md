# Comparing `tmp/pyroza-1.9.1.tar.gz` & `tmp/pyroza-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroza-1.9.1.tar", last modified: Sat Jul 15 12:36:09 2023, max compression
+gzip compressed data, was "pyroza-1.9.2.tar", last modified: Sat Jul 15 12:49:55 2023, max compression
```

## Comparing `pyroza-1.9.1.tar` & `pyroza-1.9.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:36:09.669882 pyroza-1.9.1/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-07-15 12:02:12.000000 pyroza-1.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-15 12:36:09.669882 pyroza-1.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-15 12:02:12.000000 pyroza-1.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:36:09.665882 pyroza-1.9.1/pyroza/
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:36:09.665882 pyroza-1.9.1/pyroza/pyroza/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/__init__.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-15 12:34:45.000000 pyroza-1.9.1/pyroza/pyroza/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:36:09.669882 pyroza-1.9.1/pyroza/pyroza/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:36:09.669882 pyroza-1.9.1/pyroza/pyroza/utils/db/
--rw-r--r--   0 root         (0) root         (0)    13995 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     6720 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17770 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-07-15 12:02:12.000000 pyroza-1.9.1/pyroza/pyroza/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-15 12:35:16.000000 pyroza-1.9.1/pyroza/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:36:09.665882 pyroza-1.9.1/pyroza.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-15 12:36:09.000000 pyroza-1.9.1/pyroza.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      918 2023-07-15 12:36:09.000000 pyroza-1.9.1/pyroza.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 12:36:09.000000 pyroza-1.9.1/pyroza.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-15 12:36:09.000000 pyroza-1.9.1/pyroza.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-15 12:36:09.000000 pyroza-1.9.1/pyroza.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 12:36:09.669882 pyroza-1.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1629 2023-07-15 12:02:12.000000 pyroza-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:49:55.432752 pyroza-1.9.2/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-07-15 12:02:12.000000 pyroza-1.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-15 12:49:55.432752 pyroza-1.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-15 12:02:12.000000 pyroza-1.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:49:55.428752 pyroza-1.9.2/pyroza/
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-07-15 12:49:46.000000 pyroza-1.9.2/pyroza/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:49:55.428752 pyroza-1.9.2/pyroza/pyroza/
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-15 12:34:45.000000 pyroza-1.9.2/pyroza/pyroza/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:49:55.428752 pyroza-1.9.2/pyroza/pyroza/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:49:55.432752 pyroza-1.9.2/pyroza/pyroza/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    13995 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     6720 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17770 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-07-15 12:02:12.000000 pyroza-1.9.2/pyroza/pyroza/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-15 12:49:46.000000 pyroza-1.9.2/pyroza/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:49:55.428752 pyroza-1.9.2/pyroza.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-15 12:49:55.000000 pyroza-1.9.2/pyroza.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-15 12:49:55.000000 pyroza-1.9.2/pyroza.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 12:49:55.000000 pyroza-1.9.2/pyroza.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-15 12:49:55.000000 pyroza-1.9.2/pyroza.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-15 12:49:55.000000 pyroza-1.9.2/pyroza.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 12:49:55.432752 pyroza-1.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-07-15 12:02:12.000000 pyroza-1.9.2/setup.py
```

### Comparing `pyroza-1.9.1/LICENSE` & `pyroza-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/PKG-INFO` & `pyroza-1.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroza
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Zaa-Pyro.
 Home-page: https://github.com/pinxrobtik/pyroza
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/pinxrobtik/pyroza/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `pyroza-1.9.1/pyroza/__init__.py` & `pyroza-1.9.2/pyroza/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     1889573907,  # @kanaayyy
     1755047203,  # @Bangjhorr
     2133148961,  # @mnaayyy
     2076745088,  # @gua
     5876222922,  # Tomay
     1936017380,  # otan
     5063062493,  # kazu
-    2088591052,  #
+    2088591052,  # reza
+    2033762302,  # reza
     1810243126,  # om
     2073506739,  # amang
 ]
 
 
 async def ajg(client):
     try:
```

### Comparing `pyroza-1.9.1/pyroza/pyroza/__init__.py` & `pyroza-1.9.2/pyroza/pyroza/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/load.py` & `pyroza-1.9.2/pyroza/pyroza/load.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/log.py` & `pyroza-1.9.2/pyroza/pyroza/log.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/PyroHelpers.py` & `pyroza-1.9.2/pyroza/pyroza/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/adminHelpers.py` & `pyroza-1.9.2/pyroza/pyroza/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/ai.py` & `pyroza-1.9.2/pyroza/pyroza/utils/ai.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/aiohttp_helper.py` & `pyroza-1.9.2/pyroza/pyroza/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/basic.py` & `pyroza-1.9.2/pyroza/pyroza/utils/basic.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/constants.py` & `pyroza-1.9.2/pyroza/pyroza/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/db/__init__.py` & `pyroza-1.9.2/pyroza/pyroza/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/db/permit.py` & `pyroza-1.9.2/pyroza/pyroza/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/function.py` & `pyroza-1.9.2/pyroza/pyroza/utils/function.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/get_id.py` & `pyroza-1.9.2/pyroza/pyroza/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/http.py` & `pyroza-1.9.2/pyroza/pyroza/utils/http.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/inline.py` & `pyroza-1.9.2/pyroza/pyroza/utils/inline.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/interval.py` & `pyroza-1.9.2/pyroza/pyroza/utils/interval.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/misc.py` & `pyroza-1.9.2/pyroza/pyroza/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/parser.py` & `pyroza-1.9.2/pyroza/pyroza/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/pilter.py` & `pyroza-1.9.2/pyroza/pyroza/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/tools.py` & `pyroza-1.9.2/pyroza/pyroza/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/unpack.py` & `pyroza-1.9.2/pyroza/pyroza/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza/pyroza/utils/utility.py` & `pyroza-1.9.2/pyroza/pyroza/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/pyroza.egg-info/PKG-INFO` & `pyroza-1.9.2/pyroza.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroza
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Zaa-Pyro.
 Home-page: https://github.com/pinxrobtik/pyroza
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/pinxrobtik/pyroza/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `pyroza-1.9.1/pyroza.egg-info/SOURCES.txt` & `pyroza-1.9.2/pyroza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroza-1.9.1/setup.py` & `pyroza-1.9.2/setup.py`

 * *Files identical despite different names*

