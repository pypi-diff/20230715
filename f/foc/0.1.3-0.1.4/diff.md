# Comparing `tmp/foc-0.1.3.tar.gz` & `tmp/foc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.3.tar", last modified: Sat Jun 17 16:46:10 2023, max compression
+gzip compressed data, was "foc-0.1.4.tar", last modified: Sat Jul 15 21:06:18 2023, max compression
```

## Comparing `foc-0.1.3.tar` & `foc-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.717319 foc-0.1.3/
--rw-r--r--   0 thyeem     (501) staff       (20)      313 2023-06-17 16:43:38.000000 foc-0.1.3/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.3/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.3/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-17 16:46:10.717432 foc-0.1.3/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-06-17 16:37:04.000000 foc-0.1.3/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.715128 foc-0.1.3/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    18551 2023-06-17 16:37:04.000000 foc-0.1.3/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.716466 foc-0.1.3/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-06-17 16:46:10.000000 foc-0.1.3/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-06-17 16:46:10.717896 foc-0.1.3/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-17 16:37:59.000000 foc-0.1.3/setup.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-17 16:46:10.717048 foc-0.1.3/tests/
--rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.3/tests/__init__.py
--rw-r--r--   0 thyeem     (501) staff       (20)     8030 2023-06-16 13:26:37.000000 foc-0.1.3/tests/test_foc.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.546649 foc-0.1.4/
+-rw-r--r--   0 thyeem     (501) staff       (20)      412 2023-07-15 21:05:41.000000 foc-0.1.4/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.4/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.4/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-15 21:06:18.546802 foc-0.1.4/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-15 21:05:41.000000 foc-0.1.4/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.544744 foc-0.1.4/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    18950 2023-07-15 21:05:41.000000 foc-0.1.4/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.545914 foc-0.1.4/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-15 21:06:18.547502 foc-0.1.4/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-15 21:05:41.000000 foc-0.1.4/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.546413 foc-0.1.4/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.4/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     8330 2023-07-15 21:05:41.000000 foc-0.1.4/tests/test_foc.py
```

### Comparing `foc-0.1.3/LICENSE` & `foc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.3/README.md` & `foc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `foc-0.1.3/foc/__init__.py` & `foc-0.1.4/foc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     "combination",
     "cartprod",
     "cartprodl",
     "concat",
     "concatl",
     "concatmap",
     "concatmapl",
+    "intersperse",
+    "intercalate",
     "lazy",
     "force",
     "mforce",
     "flat",
     "flatl",
     "flatt",
     "flatd",
@@ -110,14 +112,15 @@
     "chunk_of",
     "capture",
     "captures",
     "error",
     "HOME",
     "cd",
     "pwd",
+    "ls",
     "normpath",
     "exists",
     "dirname",
     "basename",
     "mkdir",
     "rmdir",
     "bytes_to_int",
@@ -577,14 +580,23 @@
 concatmap.__doc__ = "map a function over the given iterable then concat it"
 
 
 concatmapl = cfd(list)(concatmap)
 concatmapl.__doc__ = "unpacks the result in list after `concatmap`"
 
 
+def intersperse(sep, x):
+    """inserts an element between the elements of the list"""
+    return concatl(zip(repeat(sep), x))[1:]
+
+
+intercalate = cfd(concatl)(intersperse)
+intersperse.__doc__ = "inserts the given list between the lists then concat it"
+
+
 def lazy(f, *args, **kwargs):
     """delays the evaluation of a function(or expression) using generator"""
 
     f = bop(f)
 
     def g(*a, **k):
         yield f(*a, **k) if callable(f) else f
@@ -698,14 +710,18 @@
     return pwd()
 
 
 def pwd():
     return os.getcwd()
 
 
+def ls(path="."):
+    return os.listdir(normpath(path, abs=True))
+
+
 def normpath(path, abs=False):
     return cf_(
         os.path.abspath if abs else id,
         os.path.normpath,
         os.path.expanduser,
     )(path)
 
@@ -722,15 +738,16 @@
 
 def dirname(*args, prefix=False, abs=False):
     if len(args) > 1:
         args = [normpath(a, abs=True) for a in args]
         return os.path.commonprefix(args) if prefix else os.path.commonpath(args)
     else:
         args = [normpath(a, abs=abs) for a in args]
-        return os.path.dirname(*args)
+        d = os.path.dirname(*args)
+        return d if d else "."
 
 
 def basename(path):
     return cf_(os.path.basename, normpath)(path)
 
 
 def mkdir(path, mode=0o755):
```

### Comparing `foc-0.1.3/setup.py` & `foc-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as f:
-    long_decription = f.read()
+    long_description = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.3",
+    version="0.1.4",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
-    long_decription=long_decription,
-    long_decription_content_type="text/markdown",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `foc-0.1.3/tests/test_foc.py` & `foc-0.1.4/tests/test_foc.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,30 @@
         (1, 3),
         (2, 2),
         (2, 3),
         (3, 3),
     ]
 
 
+def test_intersperse():
+    assert (
+        "".join(
+            intersperse("-", words("sofia maria claire")),
+        )
+        == "sofia-maria-claire"
+    )
+
+
+def test_intercalate():
+    assert intercalate(
+        [-55],
+        [[1, 2], [3, 4], [5, 6]],
+    ) == [1, 2, -55, 3, 4, -55, 5, 6]
+
+
 def test_lazy():
     assert not lazy(pow, 2, 10) == 1024
 
 
 def test_force():
     assert force(lazy(pow, 2, 10)) == 1024
```

