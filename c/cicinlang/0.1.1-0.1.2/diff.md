# Comparing `tmp/cicinlang-0.1.1.tar.gz` & `tmp/cicinlang-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicinlang-0.1.1.tar", max compression
+gzip compressed data, was "cicinlang-0.1.2.tar", max compression
```

## Comparing `cicinlang-0.1.1.tar` & `cicinlang-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-07-15 03:46:59.828094 cicinlang-0.1.1/LICENSE
--rw-r--r--   0        0        0     7962 2023-07-15 10:42:54.093186 cicinlang-0.1.1/README.md
--rw-r--r--   0        0        0     6148 2023-07-15 10:12:27.242725 cicinlang-0.1.1/cicinlang/.DS_Store
--rw-r--r--   0        0        0        0 2023-07-15 09:53:10.914741 cicinlang-0.1.1/cicinlang/__init__.py
--rw-r--r--   0        0        0      760 2023-07-15 04:30:11.266793 cicinlang-0.1.1/cicinlang/cicinlang.py
--rwxr-xr-x   0        0        0     1025 2023-07-15 04:29:39.176517 cicinlang-0.1.1/cicinlang/entry.py
--rw-r--r--   0        0        0     1628 2023-07-15 02:18:52.908889 cicinlang-0.1.1/cicinlang/errors.py
--rw-r--r--   0        0        0    13724 2023-07-15 04:31:06.869573 cicinlang-0.1.1/cicinlang/interpreter.py
--rw-r--r--   0        0        0     6978 2023-07-15 04:30:23.992603 cicinlang-0.1.1/cicinlang/lexer.py
--rw-r--r--   0        0        0     5683 2023-07-11 04:39:43.431825 cicinlang-0.1.1/cicinlang/nodes.py
--rw-r--r--   0        0        0    22131 2023-07-15 04:30:48.139847 cicinlang-0.1.1/cicinlang/parser_.py
--rw-r--r--   0        0        0     2760 2023-07-11 04:34:31.117376 cicinlang-0.1.1/cicinlang/utils.py
--rw-r--r--   0        0        0      455 2023-07-15 10:45:07.796784 cicinlang-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8543 1970-01-01 00:00:00.000000 cicinlang-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-15 03:46:59.828094 cicinlang-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7963 2023-07-15 10:53:46.189115 cicinlang-0.1.2/README.md
+-rw-r--r--   0        0        0     6148 2023-07-15 10:12:27.242725 cicinlang-0.1.2/cicinlang/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-15 09:53:10.914741 cicinlang-0.1.2/cicinlang/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-15 04:30:11.266793 cicinlang-0.1.2/cicinlang/cicinlang.py
+-rwxr-xr-x   0        0        0     1025 2023-07-15 04:29:39.176517 cicinlang-0.1.2/cicinlang/entry.py
+-rw-r--r--   0        0        0     1628 2023-07-15 02:18:52.908889 cicinlang-0.1.2/cicinlang/errors.py
+-rw-r--r--   0        0        0    13724 2023-07-15 04:31:06.869573 cicinlang-0.1.2/cicinlang/interpreter.py
+-rw-r--r--   0        0        0     6978 2023-07-15 04:30:23.992603 cicinlang-0.1.2/cicinlang/lexer.py
+-rw-r--r--   0        0        0     5683 2023-07-11 04:39:43.431825 cicinlang-0.1.2/cicinlang/nodes.py
+-rw-r--r--   0        0        0    22131 2023-07-15 04:30:48.139847 cicinlang-0.1.2/cicinlang/parser_.py
+-rw-r--r--   0        0        0     2760 2023-07-11 04:34:31.117376 cicinlang-0.1.2/cicinlang/utils.py
+-rw-r--r--   0        0        0      455 2023-07-15 10:55:24.138909 cicinlang-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8544 1970-01-01 00:00:00.000000 cicinlang-0.1.2/PKG-INFO
```

### Comparing `cicinlang-0.1.1/LICENSE` & `cicinlang-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/README.md` & `cicinlang-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 - or
 
 An empty string (i.e. a string with 0 characters) is a false-y value in Cicinlang
 
 ```
 var gg = "hello" + " world"; # gg will be "hello world"
 var gg2 = not ""; # gg2 will be 1
-var gg3 = "" and "hello" # gg3 will be 0
+var gg3 = "" and "hello"; # gg3 will be 0
 ```
 
 For the logical AND and logical OR operations, strings and numbers can be combined. 
 
 ```
 var gg4 = "hello" and 5; # gg4 will be 1 since both "hello" and 5 are truth-ey values
 ```
```

### Comparing `cicinlang-0.1.1/cicinlang/.DS_Store` & `cicinlang-0.1.2/cicinlang/.DS_Store`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/cicinlang.py` & `cicinlang-0.1.2/cicinlang/cicinlang.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/entry.py` & `cicinlang-0.1.2/cicinlang/entry.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/errors.py` & `cicinlang-0.1.2/cicinlang/errors.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/interpreter.py` & `cicinlang-0.1.2/cicinlang/interpreter.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/lexer.py` & `cicinlang-0.1.2/cicinlang/lexer.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/nodes.py` & `cicinlang-0.1.2/cicinlang/nodes.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/parser_.py` & `cicinlang-0.1.2/cicinlang/parser_.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/cicinlang/utils.py` & `cicinlang-0.1.2/cicinlang/utils.py`

 * *Files identical despite different names*

### Comparing `cicinlang-0.1.1/PKG-INFO` & `cicinlang-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cicinlang
-Version: 0.1.1
+Version: 0.1.2
 Summary: A general purpose, procedural, interpreted programming language made using Python
 Author: Farhan Tajwar Romit
 Author-email: tajwarfarhan48@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -147,15 +147,15 @@
 - or
 
 An empty string (i.e. a string with 0 characters) is a false-y value in Cicinlang
 
 ```
 var gg = "hello" + " world"; # gg will be "hello world"
 var gg2 = not ""; # gg2 will be 1
-var gg3 = "" and "hello" # gg3 will be 0
+var gg3 = "" and "hello"; # gg3 will be 0
 ```
 
 For the logical AND and logical OR operations, strings and numbers can be combined. 
 
 ```
 var gg4 = "hello" and 5; # gg4 will be 1 since both "hello" and 5 are truth-ey values
 ```
```

