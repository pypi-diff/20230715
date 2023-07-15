# Comparing `tmp/wiggler_studiorabota-0.0.7.tar.gz` & `tmp/wiggler_studiorabota-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.7.tar", last modified: Sat Jul 15 11:02:25 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.8.tar", last modified: Sat Jul 15 16:24:14 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.7.tar` & `wiggler_studiorabota-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 11:02:25.499242 wiggler_studiorabota-0.0.7/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 11:02:25.499100 wiggler_studiorabota-0.0.7/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.7/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      544 2023-07-15 11:02:17.000000 wiggler_studiorabota-0.0.7/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 11:02:25.499278 wiggler_studiorabota-0.0.7/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 11:02:25.497857 wiggler_studiorabota-0.0.7/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.7/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.7/wiggler/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)     1202 2023-07-15 11:01:46.000000 wiggler_studiorabota-0.0.7/wiggler/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 11:02:25.498920 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 11:02:25.000000 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      341 2023-07-15 11:02:25.000000 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 11:02:25.000000 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 11:02:25.000000 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)       58 2023-07-15 11:02:25.000000 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 11:02:25.000000 wiggler_studiorabota-0.0.7/wiggler_studiorabota.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:24:14.189909 wiggler_studiorabota-0.0.8/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 16:24:14.189749 wiggler_studiorabota-0.0.8/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.8/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)      544 2023-07-15 16:23:44.000000 wiggler_studiorabota-0.0.8/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 16:24:14.189947 wiggler_studiorabota-0.0.8/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:24:14.188295 wiggler_studiorabota-0.0.8/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.8/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      611 2023-07-15 16:24:09.000000 wiggler_studiorabota-0.0.8/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1234 2023-07-15 11:06:24.000000 wiggler_studiorabota-0.0.8/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:24:14.189516 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      341 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       58 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/top_level.txt
```

### Comparing `wiggler_studiorabota-0.0.7/pyproject.toml` & `wiggler_studiorabota-0.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wiggler_studiorabota"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Vincent Kranendonk" },
 ]
 description = "WiggleR - Desktop research unit for making controlled experiments"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `wiggler_studiorabota-0.0.7/wiggler/main.py` & `wiggler_studiorabota-0.0.8/wiggler/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 
 @app.get("/schedule_picture/{minutes}")
 def images(minutes: int = 1):
     cron = CronTab(user=os.getlogin())
     cron.remove_all(comment='take picture')
     job = cron.new(command='curl localhost:8000/take_picture', comment='take picture')
     job.minute.every(minutes)
-    cron.write()
+    cron.write()
+    return {"minutes": minutes}
```

