# Comparing `tmp/mkdocs_exporter-4.0.0.tar.gz` & `tmp/mkdocs_exporter-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-4.0.0.tar", max compression
+gzip compressed data, was "mkdocs_exporter-4.0.1.tar", max compression
```

## Comparing `mkdocs_exporter-4.0.0.tar` & `mkdocs_exporter-4.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1071 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/LICENSE
--rw-r--r--   0        0        0     4007 2023-05-30 06:07:05.064243 mkdocs_exporter-4.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0      264 2023-05-30 09:11:11.210921 mkdocs_exporter-4.0.0/mkdocs_exporter/config.py
--rw-r--r--   0        0        0       96 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      543 2023-05-30 06:07:05.064243 mkdocs_exporter-4.0.0/mkdocs_exporter/page.py
--rw-r--r--   0        0        0     1935 2023-05-30 09:11:04.720870 mkdocs_exporter-4.0.0/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      867 2023-05-30 06:10:52.764231 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0     1150 2023-06-16 09:48:23.446211 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0     2282 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/browser.py
--rw-r--r--   0        0        0      566 2023-06-16 09:51:58.339820 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1291 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4932 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2512 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3845 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.064243 mkdocs_exporter-4.0.0/mkdocs_exporter/resources/css/__init__.py
--rw-r--r--   0        0        0       93 2023-05-30 06:07:05.064243 mkdocs_exporter-4.0.0/mkdocs_exporter/resources/css/readthedocs.css
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-4.0.0/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   504034 2023-05-30 06:07:05.074243 mkdocs_exporter-4.0.0/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0      237 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/resources/js/pdf.js
--rw-r--r--   0        0        0      599 2023-05-30 06:07:05.074243 mkdocs_exporter-4.0.0/mkdocs_exporter/theme.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/__init__.py
--rw-r--r--   0        0        0      650 2023-05-30 09:09:34.115672 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/factory.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/material/__init__.py
--rw-r--r--   0        0        0      681 2023-05-30 06:07:05.074243 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/material/icons.py
--rw-r--r--   0        0        0     1310 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/material/theme.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     1219 2023-06-16 09:44:47.903644 mkdocs_exporter-4.0.0/mkdocs_exporter/themes/readthedocs/theme.py
--rw-r--r--   0        0        0     1618 2023-06-16 09:45:00.186012 mkdocs_exporter-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 mkdocs_exporter-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-4.0.1/LICENSE
+-rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-4.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-4.0.1/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-4.0.1/mkdocs_exporter/config.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-4.0.1/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-4.0.1/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0     1150 2023-07-15 09:42:24.432276 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0     2282 2023-06-15 12:58:56.312600 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/browser.py
+-rw-r--r--   0        0        0      566 2023-07-15 09:42:24.432276 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1291 2023-06-13 18:20:29.951946 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4932 2023-06-15 12:36:54.752732 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2544 2023-07-15 09:42:24.442276 mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3845 2023-06-02 11:44:31.861490 mkdocs_exporter-4.0.1/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-4.0.1/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-4.0.1/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/resources/css/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/resources/css/readthedocs.css
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-4.0.1/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0      237 2023-06-15 12:58:27.282604 mkdocs_exporter-4.0.1/mkdocs_exporter/resources/js/pdf.js
+-rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/__init__.py
+-rw-r--r--   0        0        0      650 2023-06-14 18:42:45.067998 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/factory.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/material/__init__.py
+-rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/material/icons.py
+-rw-r--r--   0        0        0     1310 2023-06-14 18:33:07.838054 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/material/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-15 09:42:24.442276 mkdocs_exporter-4.0.1/mkdocs_exporter/themes/readthedocs/theme.py
+-rw-r--r--   0        0        0     1618 2023-07-15 09:43:39.392257 mkdocs_exporter-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-4.0.1/PKG-INFO
```

### Comparing `mkdocs_exporter-4.0.0/LICENSE` & `mkdocs_exporter-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/README.md` & `mkdocs_exporter-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/page.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugin.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/browser.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,24 +53,24 @@
     base = os.path.dirname(page.file.abs_dest_path)
     root = base.replace(unquote(page.url).rstrip('/'), '', 1).rstrip('/')
 
     preprocessor.preprocess(page.html)
     preprocessor.set_attribute('details:not([open])', 'open', 'open')
     page.theme.preprocess(preprocessor)
 
-    preprocessor.script(importlib_resources.files(js).joinpath('pdf.js').read_text())
+    preprocessor.script(importlib_resources.files(js).joinpath('pdf.js').read_text(encoding='utf-8'))
 
     for stylesheet in self.stylesheets:
       with open(stylesheet, 'r', encoding='utf-8') as file:
         preprocessor.stylesheet(file.read())
     for script in self.scripts:
       with open(script, 'r', encoding='utf-8') as file:
         preprocessor.script(file.read())
 
-    preprocessor.script(importlib_resources.files(js).joinpath('pagedjs.min.js').read_text())
+    preprocessor.script(importlib_resources.files(js).joinpath('pagedjs.min.js').read_text(encoding='utf-8'))
     preprocessor.teleport()
     preprocessor.update_links(base, root)
 
     return preprocessor.done()
 
 
   async def render(self, page: str | Page) -> bytes:
```

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-4.0.1/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/theme.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/themes/factory.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/themes/factory.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/themes/material/icons.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/themes/material/icons.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/themes/material/theme.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/themes/material/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-4.0.0/mkdocs_exporter/themes/readthedocs/theme.py` & `mkdocs_exporter-4.0.1/mkdocs_exporter/themes/readthedocs/theme.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   """The name of the theme."""
 
 
   def preprocess(self, preprocessor: Preprocessor) -> None:
     """Preprocesses the DOM before rendering a document."""
 
     preprocessor.remove(['.rst-content > div[role="navigation"]', 'nav.wy-nav-side'])
-    preprocessor.stylesheet(importlib_resources.files(css).joinpath('readthedocs.css').read_text())
+    preprocessor.stylesheet(importlib_resources.files(css).joinpath('readthedocs.css').read_text(encoding='utf-8'))
 
 
   def button(self, preprocessor: Preprocessor, title: str, icon: str, attributes: dict = {}):
     """Inserts a custom themed button."""
 
     button = preprocessor.html.new_tag('a', title=title, attrs={'class': 'btn btn-neutral float-right', **attributes})
     button.string = title
```

### Comparing `mkdocs_exporter-4.0.0/pyproject.toml` & `mkdocs_exporter-4.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "4.0.0"
+version = "4.0.1"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-4.0.0/PKG-INFO` & `mkdocs_exporter-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 4.0.0
+Version: 4.0.1
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Dist: beautifulsoup4 (>=4.12.2)
 Requires-Dist: importlib-metadata (<5.0)
 Requires-Dist: importlib-resources (>=5.0)
 Requires-Dist: libsass (>=0.22.0)
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: mkdocs-exporter Version: 4.0.0 Summary: A highly-
+Metadata-Version: 2.1 Name: mkdocs-exporter Version: 4.0.1 Summary: A highly-
 configurable plugin for MkDocs that exports your pages to PDF files. Home-page:
 https://github.com/adrienbrignon/mkdocs-exporter Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon Author-email: adrien@brignon.dev Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
-Topic :: Documentation Classifier: Topic :: Software Development ::
-Documentation Classifier: Topic :: Text Processing :: Markup :: HTML Requires-
-Dist: beautifulsoup4 (>=4.12.2) Requires-Dist: importlib-metadata (<5.0)
-Requires-Dist: importlib-resources (>=5.0) Requires-Dist: libsass (>=0.22.0)
-Requires-Dist: lxml (>=4.9) Requires-Dist: mkdocs (>=1.4) Requires-Dist: nest-
-asyncio (>=1.5.6) Requires-Dist: playwright (>=1.33) Project-URL: Bug Tracker,
-https://github.com/adrienbrignon/mkdocs-exporter/issues Project-URL:
-Repository, https://github.com/adrienbrignon/mkdocs-exporter Description-
+Python :: 3.11 Classifier: Topic :: Documentation Classifier: Topic :: Software
+Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
+HTML Requires-Dist: beautifulsoup4 (>=4.12.2) Requires-Dist: importlib-metadata
+(<5.0) Requires-Dist: importlib-resources (>=5.0) Requires-Dist: libsass
+(>=0.22.0) Requires-Dist: lxml (>=4.9) Requires-Dist: mkdocs (>=1.4) Requires-
+Dist: nest-asyncio (>=1.5.6) Requires-Dist: playwright (>=1.33) Project-URL:
+Bug Tracker, https://github.com/adrienbrignon/mkdocs-exporter/issues Project-
+URL: Repository, https://github.com/adrienbrignon/mkdocs-exporter Description-
 Content-Type: text/markdown # MkDocs Exporter
 [https://img.shields.io/pypi/v/mkdocs-exporter?color=blue] [https://
 img.shields.io/pypi/pyversions/mkdocs-exporter?color=blue] [https://
 img.shields.io/pypi/dm/mkdocs-exporter?color=cactus] [https://img.shields.io/
 github/license/adrienbrignon/mkdocs-exporter?color=white]
 
 A highly-configurable plugin for [*MkDocs*](https://github.com/mkdocs/mkdocs)
```

