# Comparing `tmp/bb_dirtree-0.3.0.tar.gz` & `tmp/bb_dirtree-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.3.0.tar", max compression
+gzip compressed data, was "bb_dirtree-0.3.1.tar", max compression
```

## Comparing `bb_dirtree-0.3.0.tar` & `bb_dirtree-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.3.0/LICENSE
--rw-r--r--   0        0        0     4808 2023-07-15 20:52:27.230345 bb_dirtree-0.3.0/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.3.0/bbdirtree/COLORS.py
--rw-r--r--   0        0        0      125 2023-07-15 20:51:39.277011 bb_dirtree-0.3.0/bbdirtree/__init__.py
--rw-r--r--   0        0        0    25322 2023-07-15 20:50:29.677010 bb_dirtree-0.3.0/bbdirtree/__main__.py
--rw-r--r--   0        0        0      577 2023-07-15 20:51:52.793678 bb_dirtree-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 bb_dirtree-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4869 2023-07-15 21:07:59.020363 bb_dirtree-0.3.1/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.3.1/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0      125 2023-07-15 21:08:10.373696 bb_dirtree-0.3.1/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    25319 2023-07-15 21:07:27.760362 bb_dirtree-0.3.1/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      577 2023-07-15 21:08:08.160363 bb_dirtree-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 bb_dirtree-0.3.1/PKG-INFO
```

### Comparing `bb_dirtree-0.3.0/LICENSE` & `bb_dirtree-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.3.0/README.md` & `bb_dirtree-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -156,7 +156,11 @@
 - added option to follow symlinks
 - added symlink data to output
 - added '--no-print' option for debugging
 - changed colors in output
 - changed the way the title is generated
 - updated README to reflect changes
 - cleaned up some code
+
+#### v0.3.1 - 7-15-2023
+
+- fixed title when printing to tty
```

#### html2text {}

```diff
@@ -65,8 +65,9 @@
 - added git project titles to output - searches for .SRCINFO file #### v0.2.4 -
 7-10-2023 - fixed typo in __main__ #### v0.2.6 - 7-10-2023 - bugfixes ####
 v0.3.0 - 7-15-2023 - added bb_apputils to dependencies - added bblogger for
 logging - removed __doc__ from init.py - added verbose options - added option
 to ignore errors while scanning directories - added option to follow symlinks -
 added symlink data to output - added '--no-print' option for debugging -
 changed colors in output - changed the way the title is generated - updated
-README to reflect changes - cleaned up some code
+README to reflect changes - cleaned up some code #### v0.3.1 - 7-15-2023 -
+fixed title when printing to tty
```

### Comparing `bb_dirtree-0.3.0/bbdirtree/COLORS.py` & `bb_dirtree-0.3.1/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.3.0/bbdirtree/__main__.py` & `bb_dirtree-0.3.1/bbdirtree/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
                     'text'    : f"{C_Gr()}_-_{C__()}",    # dark gray
                     'file'    : f"{C_gri()}_-_{C__()}",   # italic gray
                     'link'    : f"{C_Ci()}_-_{C__()}",    # cyan italic              # NEW
                     'filelink': f"{C_Gri()}_-_{C__()}",   # dark gray italic         # NEW
                     'dirlink' : f"{C_bi()}_-_{C__()}",    # light blue italic        # NEW
                     'tree'    : f"{C_g()}_-_{C__()}",     # green
                     'pre'     : f"\n{C_W()}    {F_U()}_-_{C__()}",  # White
-                    'title'   : f"\n{C_O()}  {F_U()}_-_{C__()}",    # orange
+                    'title'   : f"{C_O()} {F_U()}_-_{C__()}",    # orange
                     'post'    : "",
                     'nl'      : '\n' }
 
         self.__getBase()
         list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir, self.title )
 
         return list_tree
```

### Comparing `bb_dirtree-0.3.0/pyproject.toml` & `bb_dirtree-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.3.0"
+version = "0.3.1"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
```

### Comparing `bb_dirtree-0.3.0/PKG-INFO` & `bb_dirtree-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -174,7 +174,11 @@
 - added symlink data to output
 - added '--no-print' option for debugging
 - changed colors in output
 - changed the way the title is generated
 - updated README to reflect changes
 - cleaned up some code
 
+#### v0.3.1 - 7-15-2023
+
+- fixed title when printing to tty
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bb-dirtree Version: 0.3.0 Summary: Create a nice
+Metadata-Version: 2.1 Name: bb-dirtree Version: 0.3.1 Summary: Create a nice
 looking directory tree with options License: MIT Keywords: script,qt,files
 Author: Erik Beebe Author-email: beebeapps_feedback@tuta.io Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: bb-
 apputils (>=0.3.8,<0.4.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Description-
 Content-Type: text/markdown
@@ -73,8 +73,9 @@
 - added git project titles to output - searches for .SRCINFO file #### v0.2.4 -
 7-10-2023 - fixed typo in __main__ #### v0.2.6 - 7-10-2023 - bugfixes ####
 v0.3.0 - 7-15-2023 - added bb_apputils to dependencies - added bblogger for
 logging - removed __doc__ from init.py - added verbose options - added option
 to ignore errors while scanning directories - added option to follow symlinks -
 added symlink data to output - added '--no-print' option for debugging -
 changed colors in output - changed the way the title is generated - updated
-README to reflect changes - cleaned up some code
+README to reflect changes - cleaned up some code #### v0.3.1 - 7-15-2023 -
+fixed title when printing to tty
```

