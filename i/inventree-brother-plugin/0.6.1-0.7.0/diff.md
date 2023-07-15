# Comparing `tmp/inventree-brother-plugin-0.6.1.tar.gz` & `tmp/inventree-brother-plugin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-brother-plugin-0.6.1.tar", last modified: Thu Jun  8 09:53:41 2023, max compression
+gzip compressed data, was "dist/inventree-brother-plugin-0.7.0.tar", last modified: Sat Jul 15 09:17:08 2023, max compression
```

## Comparing `inventree-brother-plugin-0.6.1.tar` & `inventree-brother-plugin-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/inventree_brother/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/inventree_brother/brother_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/inventree_brother/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:53:41.000000 inventree-brother-plugin-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-08 09:53:33.000000 inventree-brother-plugin-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/inventree_brother/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/inventree_brother/brother_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/inventree_brother/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/setup.py
```

### Comparing `inventree-brother-plugin-0.6.1/LICENSE` & `inventree-brother-plugin-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-brother-plugin-0.6.1/PKG-INFO` & `inventree-brother-plugin-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-brother-plugin
-Version: 0.6.1
+Version: 0.7.0
 Summary: Brother label printer plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-brother-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree label printer printing inventory
 Requires-Python: >=3.9
```

### Comparing `inventree-brother-plugin-0.6.1/README.md` & `inventree-brother-plugin-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `inventree-brother-plugin-0.6.1/inventree_brother/brother_plugin.py` & `inventree-brother-plugin-0.7.0/inventree_brother/brother_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,17 @@
     DESCRIPTION = "Label printing plugin for Brother printers"
     VERSION = BROTHER_PLUGIN_VERSION
 
     NAME = "Brother Labels"
     SLUG = "brother"
     TITLE = "Brother Label Printer"
 
+    # Use background printing
+    BLOCKING_PRINT = False
+
     SETTINGS = {
         'MODEL': {
             'name': _('Printer Model'),
             'description': _('Select model of Brother printer'),
             'choices': get_model_choices,
             'default': 'PT-P750W',
         },
@@ -113,16 +116,21 @@
 
         # Extract width (x) and height (y) information
         # width = kwargs['width']
         # height = kwargs['height']
         # ^ currently this width and height are those of the label template (before conversion to PDF
         # and PNG) and are of little use
 
-        # Extract image from the provided kwargs
-        label_image = kwargs['png_file']
+        # Look for png data in kwargs (if provided)
+        label_image = kwargs.get('png_file', None)
+
+        if not label_image:
+            # Convert PDF to PNG
+            pdf_data = kwargs['pdf_data']
+            label_image = self.render_to_png(label=None, pdf_data=pdf_data)
 
         # Read settings
         model = self.get_setting('MODEL')
         ip_address = self.get_setting('IP_ADDRESS')
         media_type = self.get_setting('LABEL')
 
         # Get specifications of media type
```

### Comparing `inventree-brother-plugin-0.6.1/inventree_brother_plugin.egg-info/PKG-INFO` & `inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-brother-plugin
-Version: 0.6.1
+Version: 0.7.0
 Summary: Brother label printer plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-brother-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree label printer printing inventory
 Requires-Python: >=3.9
```

### Comparing `inventree-brother-plugin-0.6.1/setup.py` & `inventree-brother-plugin-0.7.0/setup.py`

 * *Files identical despite different names*

