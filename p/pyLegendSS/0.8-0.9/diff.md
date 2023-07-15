# Comparing `tmp/pyLegendSS-0.8.tar.gz` & `tmp/pyLegendSS-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendSS-0.8.tar", last modified: Sat Jul 15 12:47:58 2023, max compression
+gzip compressed data, was "pyLegendSS-0.9.tar", last modified: Sat Jul 15 12:59:03 2023, max compression
```

## Comparing `pyLegendSS-0.8.tar` & `pyLegendSS-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:47:58.715787 pyLegendSS-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:47:58.711787 pyLegendSS-0.8/LegendSS/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LegendSS/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LegendSS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LegendSS/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 12:47:58.715787 pyLegendSS-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 12:47:45.000000 pyLegendSS-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:47:58.715787 pyLegendSS-0.8/pyLegendSS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 12:47:58.715787 pyLegendSS-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-15 12:47:45.000000 pyLegendSS-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:59:03.943698 pyLegendSS-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 12:58:52.000000 pyLegendSS-0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:59:03.943698 pyLegendSS-0.9/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-15 12:58:52.000000 pyLegendSS-0.9/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:58:52.000000 pyLegendSS-0.9/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-15 12:58:52.000000 pyLegendSS-0.9/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 12:59:03.943698 pyLegendSS-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 12:58:52.000000 pyLegendSS-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:59:03.943698 pyLegendSS-0.9/pyLegendSS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 12:59:03.000000 pyLegendSS-0.9/pyLegendSS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-15 12:59:03.000000 pyLegendSS-0.9/pyLegendSS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:59:03.000000 pyLegendSS-0.9/pyLegendSS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 12:59:03.000000 pyLegendSS-0.9/pyLegendSS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 12:59:03.000000 pyLegendSS-0.9/pyLegendSS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 12:59:03.943698 pyLegendSS-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-15 12:58:52.000000 pyLegendSS-0.9/setup.py
```

### Comparing `pyLegendSS-0.8/LICENSE` & `pyLegendSS-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.8/LegendSS/Data.py` & `pyLegendSS-0.9/LegendSS/Data.py`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.8/LegendSS/generate.py` & `pyLegendSS-0.9/LegendSS/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,16 @@
             )
     try:
         await client.join_chat("@LegendBot_OP")
     except BaseException:
         pass
     await client.disconnect()
     await phone_code_msg.reply(
-        "Successfully String  Session Has Been Generated \n\nPlease check your saved messages!"
-        ),
-        reply_markup=InlineKeyboardMarkup(Data.support_button),
+      "Successfully String  Session Has Been Generated \n\nPlease check your saved messages!",
+      reply_markup=InlineKeyboardMarkup(Data.support_button),
     )
 
 
 
 def helltopi(text):
     res = ''.join(
         map(
```

### Comparing `pyLegendSS-0.8/PKG-INFO` & `pyLegendSS-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.8
+Version: 0.9
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.8/pyLegendSS.egg-info/PKG-INFO` & `pyLegendSS-0.9/pyLegendSS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.8
+Version: 0.9
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.8/setup.py` & `pyLegendSS-0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendSS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.8",
+    version="0.9",
     description="This is a simple package which is used in String Generator Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendSS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

