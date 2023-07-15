# Comparing `tmp/py-draughts-1.0.4.tar.gz` & `tmp/py-draughts-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.4.tar", last modified: Thu Jul 13 22:44:46 2023, max compression
+gzip compressed data, was "py-draughts-1.0.6.tar", last modified: Sat Jul 15 07:09:42 2023, max compression
```

## Comparing `py-draughts-1.0.4.tar` & `py-draughts-1.0.6.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.404502 py-draughts-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-07-13 22:43:03.000000 py-draughts-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-13 22:43:03.000000 py-draughts-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6258 2023-07-13 22:44:46.396414 py-draughts-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4841 2023-07-13 22:43:03.000000 py-draughts-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.103001 py-draughts-1.0.4/draughts/
--rw-rw-rw-   0        0        0      964 2023-07-13 22:43:20.000000 py-draughts-1.0.4/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/american.py
--rw-rw-rw-   0        0        0    11486 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/base.py
--rw-rw-rw-   0        0        0      671 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/models.py
--rw-rw-rw-   0        0        0     4197 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/move.py
--rw-rw-rw-   0        0        0     5323 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:45.790761 py-draughts-1.0.4/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.135020 py-draughts-1.0.4/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.196396 py-draughts-1.0.4/draughts/static/js/
--rw-rw-rw-   0        0        0     5993 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.278271 py-draughts-1.0.4/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2860 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.330852 py-draughts-1.0.4/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6258 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 22:43:03.000000 py-draughts-1.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 22:44:46.404502 py-draughts-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1905 2023-07-13 22:43:10.000000 py-draughts-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.388892 py-draughts-1.0.4/test/
--rw-rw-rw-   0        0        0     1123 2023-07-13 22:43:03.000000 py-draughts-1.0.4/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-13 22:43:03.000000 py-draughts-1.0.4/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.866606 py-draughts-1.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-13 22:43:03.000000 py-draughts-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-13 22:43:03.000000 py-draughts-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6258 2023-07-15 07:09:42.866606 py-draughts-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4841 2023-07-13 22:43:03.000000 py-draughts-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.754490 py-draughts-1.0.6/draughts/
+-rw-rw-rw-   0        0        0      964 2023-07-15 07:09:12.000000 py-draughts-1.0.6/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/american.py
+-rw-rw-rw-   0        0        0    11486 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/base.py
+-rw-rw-rw-   0        0        0      671 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/models.py
+-rw-rw-rw-   0        0        0     4197 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/move.py
+-rw-rw-rw-   0        0        0     5323 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.653457 py-draughts-1.0.6/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.762530 py-draughts-1.0.6/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.777042 py-draughts-1.0.6/draughts/static/img/
+-rw-rw-rw-   0        0        0     1386 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/static/img/crown-icon.svg
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.786608 py-draughts-1.0.6/draughts/static/js/
+-rw-rw-rw-   0        0        0     5993 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.810607 py-draughts-1.0.6/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2860 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.842609 py-draughts-1.0.6/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6258 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 22:43:03.000000 py-draughts-1.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:09:42.866606 py-draughts-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2001 2023-07-15 07:08:11.000000 py-draughts-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.866606 py-draughts-1.0.6/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-13 22:43:03.000000 py-draughts-1.0.6/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-13 22:43:03.000000 py-draughts-1.0.6/test/test_board.py
```

### Comparing `py-draughts-1.0.4/LICENSE` & `py-draughts-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/PKG-INFO` & `py-draughts-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.4
+Version: 1.0.6
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
```

### Comparing `py-draughts-1.0.4/README.md` & `py-draughts-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/__init__.py` & `py-draughts-1.0.6/draughts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
-__version__ = "1.0.4"
+__version__ = "1.0.6"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-1.0.4/draughts/american.py` & `py-draughts-1.0.6/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/base.py` & `py-draughts-1.0.6/draughts/base.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/models.py` & `py-draughts-1.0.6/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/move.py` & `py-draughts-1.0.6/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/server.py` & `py-draughts-1.0.6/draughts/server.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/standard.py` & `py-draughts-1.0.6/draughts/standard.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/static/css/style.css` & `py-draughts-1.0.6/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/static/js/script.js` & `py-draughts-1.0.6/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/templates/base.html` & `py-draughts-1.0.6/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/templates/index.html` & `py-draughts-1.0.6/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/draughts/utils.py` & `py-draughts-1.0.6/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.6/py_draughts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.4
+Version: 1.0.6
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
```

### Comparing `py-draughts-1.0.4/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.6/py_draughts.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 draughts/base.py
 draughts/models.py
 draughts/move.py
 draughts/server.py
 draughts/standard.py
 draughts/utils.py
 draughts/static/css/style.css
+draughts/static/img/crown-icon.svg
 draughts/static/js/script.js
 draughts/templates/base.html
 draughts/templates/index.html
 py_draughts.egg-info/PKG-INFO
 py_draughts.egg-info/SOURCES.txt
 py_draughts.egg-info/dependency_links.txt
 py_draughts.egg-info/requires.txt
```

### Comparing `py-draughts-1.0.4/setup.py` & `py-draughts-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,22 @@
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     # rst
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    package_data={"draughts": ["static/js/*", "static/css/*", "templates/*"]},
+    package_data={
+        "draughts": [
+            "static/js/*",
+            "static/css/*",
+            "templates/*",
+            "static/img/*",
+        ]
+    },
     install_requires=requirements,
     license="GPL-3.0+",
     keywords=" draughts, checkers, AI mini-max, game, board",
     url="https://github.com/michalskibinski109/draughts",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `py-draughts-1.0.4/test/test_american_board.py` & `py-draughts-1.0.6/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.4/test/test_board.py` & `py-draughts-1.0.6/test/test_board.py`

 * *Files identical despite different names*

