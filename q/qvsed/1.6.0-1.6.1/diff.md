# Comparing `tmp/qvsed-1.6.0.tar.gz` & `tmp/qvsed-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.6.0.tar", last modified: Fri Jul 14 22:31:14 2023, max compression
+gzip compressed data, was "qvsed-1.6.1.tar", last modified: Fri Jul 14 23:11:11 2023, max compression
```

## Comparing `qvsed-1.6.0.tar` & `qvsed-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 22:31:14.309876 qvsed-1.6.0/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-14 22:31:14.309876 qvsed-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 22:31:14.283219 qvsed-1.6.0/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.6.0/qvsed/__init__.py
--rw-rw-rw-   0        0        0      905 2023-07-14 22:10:14.000000 qvsed-1.6.0/qvsed/config_default.py
--rw-rw-rw-   0        0        0    30654 2023-07-14 22:30:09.000000 qvsed-1.6.0/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7852 2023-07-14 22:26:54.000000 qvsed-1.6.0/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.6.0/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-14 22:31:14.307667 qvsed-1.6.0/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 22:31:14.309876 qvsed-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-14 22:30:56.000000 qvsed-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:11.124935 qvsed-1.6.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-14 23:11:11.124935 qvsed-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:11.099974 qvsed-1.6.1/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.6.1/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-07-14 22:10:14.000000 qvsed-1.6.1/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    31000 2023-07-14 23:09:19.000000 qvsed-1.6.1/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7852 2023-07-14 22:26:54.000000 qvsed-1.6.1/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.6.1/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:11.123375 qvsed-1.6.1/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-14 23:11:10.000000 qvsed-1.6.1/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 23:11:10.000000 qvsed-1.6.1/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 23:11:10.000000 qvsed-1.6.1/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-14 23:11:10.000000 qvsed-1.6.1/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 23:11:10.000000 qvsed-1.6.1/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 23:11:10.000000 qvsed-1.6.1/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 23:11:11.124935 qvsed-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-14 23:10:52.000000 qvsed-1.6.1/setup.py
```

### Comparing `qvsed-1.6.0/LICENSE.txt` & `qvsed-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.6.0/PKG-INFO` & `qvsed-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.6.0
+Version: 1.6.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.6.0/README.md` & `qvsed-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.6.0/qvsed/config_default.py` & `qvsed-1.6.1/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.6.0/qvsed/qvsed.py` & `qvsed-1.6.1/qvsed/qvsed.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,43 @@
     color: {button_text_color};
     border: 2px solid {button_hover_color};
     background: {button_color};
     padding: 2px;
 }}
 
 QPushButton:hover {{
-    color: {text_color};
+    color: {button_text_color};
     background: {button_hover_color};
 }}
 
 QPushButton:pressed {{
-    color: {text_color};
+    color: {button_text_color};
     background: {button_pressed_color};
 }}
 
+QMenu {{
+    color: {button_text_color};
+    background: {button_color};
+    padding: 6px;
+}}
+
+QMenu::item {{
+    padding: 6px 10px;
+}}
+
+QMenu::item:selected {{
+    color: {button_text_color};
+    background: {button_hover_color};
+}}
+
+QMenu::item:disabled {{
+    color: gray;
+    background: {button_color};
+}}
+
 QScrollBar:vertical {{
     background-color: {scroll_bar_background_color};
     width: 16px;
     margin: 16px 0 16px 0;
 }}
 
 QScrollBar::handle:vertical {{
```

### Comparing `qvsed-1.6.0/qvsed/qvsed.ui` & `qvsed-1.6.1/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.6.0/qvsed/qvsed_dialog.ui` & `qvsed-1.6.1/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.6.0/qvsed.egg-info/PKG-INFO` & `qvsed-1.6.1/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.6.0
+Version: 1.6.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.6.0/setup.py` & `qvsed-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.6.0',
+    version='1.6.1',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

