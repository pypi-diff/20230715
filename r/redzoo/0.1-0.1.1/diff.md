# Comparing `tmp/redzoo-0.1.tar.gz` & `tmp/redzoo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redzoo-0.1.tar", last modified: Sat Jul 15 08:08:16 2023, max compression
+gzip compressed data, was "redzoo-0.1.1.tar", last modified: Sat Jul 15 08:01:21 2023, max compression
```

## Comparing `redzoo-0.1.tar` & `redzoo-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:08:16.788339 redzoo-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 08:07:54.000000 redzoo-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-15 08:08:16.788339 redzoo-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 08:07:54.000000 redzoo-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-15 08:07:54.000000 redzoo-0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:08:16.788339 redzoo-0.1/redzoo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:07:54.000000 redzoo-0.1/redzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:08:16.788339 redzoo-0.1/redzoo/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:07:54.000000 redzoo-0.1/redzoo/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-15 08:07:54.000000 redzoo-0.1/redzoo/database/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:08:16.788339 redzoo-0.1/redzoo/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:07:54.000000 redzoo-0.1/redzoo/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-15 08:07:54.000000 redzoo-0.1/redzoo/math/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:08:16.788339 redzoo-0.1/redzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-15 08:08:16.000000 redzoo-0.1/redzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-15 08:08:16.000000 redzoo-0.1/redzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 08:08:16.000000 redzoo-0.1/redzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 08:08:16.000000 redzoo-0.1/redzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 08:08:16.000000 redzoo-0.1/redzoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 08:08:16.792339 redzoo-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:08:16.788339 redzoo-0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-15 08:07:54.000000 redzoo-0.1/test/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-15 08:07:54.000000 redzoo-0.1/test/test_simpledb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 08:01:09.000000 redzoo-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 08:01:21.277086 redzoo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 08:01:09.000000 redzoo-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-15 08:01:09.000000 redzoo-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/database/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/math/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 08:01:21.277086 redzoo-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-15 08:01:09.000000 redzoo-0.1.1/test/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-15 08:01:09.000000 redzoo-0.1.1/test/test_simpledb.py
```

### Comparing `redzoo-0.1/LICENSE` & `redzoo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redzoo-0.1/redzoo/database/simple.py` & `redzoo-0.1.1/redzoo/database/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     def __init__(self, name: str, sync_period_sec:int = None):
         self.sync_period_sec = sync_period_sec
         self.__name = name
         self.__directory = site_data_dir("simpledb", appauthor=False)
         self.__data = self.__load()
         self.__last_time_stored = datetime.now()
-        logging.debug("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries)")
+        logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries)")
 
     @property
     def filename(self):
         if not os.path.exists(self.__directory):
             logging.info("directory " + self.__directory + " does not exits. Creating it")
             os.makedirs(self.__directory)
         return os.path.join(self.__directory, self.__name + ".json.gz")
```

### Comparing `redzoo-0.1/redzoo/math/display.py` & `redzoo-0.1.1/redzoo/math/display.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.1/test/test_simpledb.py` & `redzoo-0.1.1/test/test_simpledb.py`

 * *Files identical despite different names*

