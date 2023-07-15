# Comparing `tmp/wagtailimagecaptions-0.1.2.tar.gz` & `tmp/wagtailimagecaptions-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailimagecaptions-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtailimagecaptions-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtailimagecaptions-0.1.2.tar` & `wagtailimagecaptions-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.2/LICENSE
--rw-r--r--   0        0        0     1202 2023-07-14 11:53:40.061369 wagtailimagecaptions-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.2/media/.gitkeep
--rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.2/setup.cfg
--rw-r--r--   0        0        0      164 2023-07-14 11:59:35.930790 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/__init__.py
--rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/apps.py
--rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/migrations/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/models.py
--rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/services.py
--rw-r--r--   0        0        0     1187 2023-07-13 20:58:55.147909 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/signals.py
--rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.2/test_project/__init__.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.2/test_project/asgi.py
--rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.2/test_project/settings.py
--rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.2/test_project/urls.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.2/test_project/wsgi.py
--rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1475 2023-07-14 13:50:22.365434 wagtailimagecaptions-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.3/media/.gitkeep
+-rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.3/setup.cfg
+-rw-r--r--   0        0        0      164 2023-07-15 12:16:33.025900 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/apps.py
+-rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/migrations/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/models.py
+-rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/services.py
+-rw-r--r--   0        0        0     1123 2023-07-15 12:07:14.107381 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/signals.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.3/test_project/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.3/test_project/asgi.py
+-rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.3/test_project/settings.py
+-rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.3/test_project/urls.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.3/test_project/wsgi.py
+-rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.3/PKG-INFO
```

### Comparing `wagtailimagecaptions-0.1.2/LICENSE` & `wagtailimagecaptions-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/README.md` & `wagtailimagecaptions-0.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 You will also need to set a custom Image model in your setting files:
 
 ```python
 # settings.py
 WAGTAILIMAGES_IMAGE_MODEL = "wagtailimagecaptions.CaptionedImage"
 ```
 
+### Migrating
+
+Heads up! If you have existing images, you will need to create a [data migration operation](https://docs.wagtail.org/en/latest/advanced_topics/images/custom_image_model.html#migrating-from-the-builtin-image-model) to move the old images into
+the new model.
+
 ## How to Use
 
 The custom Image model, `CaptionedImage`, adds four new fields to the Wagtail Image model: `alt`, `caption`, `credit`, `iptc_data`. When a new image is uploaded via Wagtail's media library, the app will attempt to extract any IPTC meta data found in the file and fill
 the `alt`, `caption` and `credit` fields. All IPTC meta data  extracted is also stored in `iptc_data`.
 
 Example use in a template:
```

### Comparing `wagtailimagecaptions-0.1.2/pyproject.toml` & `wagtailimagecaptions-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/setup.cfg` & `wagtailimagecaptions-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/migrations/0001_initial.py` & `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/models.py` & `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/models.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/services.py` & `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/services.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/signals.py` & `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,11 +29,10 @@
         instance.alt = trimmed_title
 
     if credit := meta_dict.get("credit", ""):
         trimmed_credit = Truncator(credit.strip()).chars(255)
         instance.credit = trimmed_credit
 
     if caption := meta_dict.get("caption", ""):
-        trimmed_caption = Truncator(caption.strip()).chars(255)
-        instance.caption = trimmed_caption
+        instance.caption = caption.strip()
 
     instance.iptc_data = meta_dict
```

### Comparing `wagtailimagecaptions-0.1.2/test_project/settings.py` & `wagtailimagecaptions-0.1.3/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/test_project/urls.py` & `wagtailimagecaptions-0.1.3/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.2/PKG-INFO` & `wagtailimagecaptions-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailimagecaptions
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django app for extending the Wagtail Image model to add captions and alt fields as
 Author-email: Stephan Rohde <appsupport@newshour.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -48,14 +48,19 @@
 You will also need to set a custom Image model in your setting files:
 
 ```python
 # settings.py
 WAGTAILIMAGES_IMAGE_MODEL = "wagtailimagecaptions.CaptionedImage"
 ```
 
+### Migrating
+
+Heads up! If you have existing images, you will need to create a [data migration operation](https://docs.wagtail.org/en/latest/advanced_topics/images/custom_image_model.html#migrating-from-the-builtin-image-model) to move the old images into
+the new model.
+
 ## How to Use
 
 The custom Image model, `CaptionedImage`, adds four new fields to the Wagtail Image model: `alt`, `caption`, `credit`, `iptc_data`. When a new image is uploaded via Wagtail's media library, the app will attempt to extract any IPTC meta data found in the file and fill
 the `alt`, `caption` and `credit` fields. All IPTC meta data  extracted is also stored in `iptc_data`.
 
 Example use in a template:
```

