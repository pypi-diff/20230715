# Comparing `tmp/wiggler_studiorabota-0.0.5.tar.gz` & `tmp/wiggler_studiorabota-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.5.tar", last modified: Sat Jul 15 10:22:44 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.6.tar", last modified: Sat Jul 15 10:50:43 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.5.tar` & `wiggler_studiorabota-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 10:22:44.550339 wiggler_studiorabota-0.0.5/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 10:22:44.550189 wiggler_studiorabota-0.0.5/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.5/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      597 2023-07-15 10:22:37.000000 wiggler_studiorabota-0.0.5/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 10:22:44.550377 wiggler_studiorabota-0.0.5/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 10:22:44.548860 wiggler_studiorabota-0.0.5/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.5/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.5/wiggler/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)     1104 2023-07-15 10:21:58.000000 wiggler_studiorabota-0.0.5/wiggler/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 10:22:44.549993 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 10:22:44.000000 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      341 2023-07-15 10:22:44.000000 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 10:22:44.000000 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 10:22:44.000000 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)      100 2023-07-15 10:22:44.000000 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 10:22:44.000000 wiggler_studiorabota-0.0.5/wiggler_studiorabota.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 10:50:43.303774 wiggler_studiorabota-0.0.6/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 10:50:43.303644 wiggler_studiorabota-0.0.6/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.6/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)      544 2023-07-15 10:50:36.000000 wiggler_studiorabota-0.0.6/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 10:50:43.303808 wiggler_studiorabota-0.0.6/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 10:50:43.302471 wiggler_studiorabota-0.0.6/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.6/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.6/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1198 2023-07-15 10:48:52.000000 wiggler_studiorabota-0.0.6/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 10:50:43.303473 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 10:50:43.000000 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      341 2023-07-15 10:50:43.000000 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 10:50:43.000000 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 10:50:43.000000 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       58 2023-07-15 10:50:43.000000 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 10:50:43.000000 wiggler_studiorabota-0.0.6/wiggler_studiorabota.egg-info/top_level.txt
```

### Comparing `wiggler_studiorabota-0.0.5/pyproject.toml` & `wiggler_studiorabota-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [project]
 name = "wiggler_studiorabota"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Vincent Kranendonk" },
 ]
 description = "WiggleR - Desktop research unit for making controlled experiments"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'fastapi>=0.68.0,<0.69.0',
-  'pydantic>=1.8.0,<2.0.0',
-  'uvicorn>=0.15.0,<0.16.0',
-  'python-crontab>=3.0.0,<4.0.0',
+  'fastapi[all]>=0.68.0,<0.69.0',
+  'python-crontab>=3.0.0,<4.0.0'
 ]
 
 [project.scripts]
 wiggler = "wiggler.cli:main"
 
 [project.urls]
 "Homepage" = "https://github.com/studiorabota/wiggle-bin"
```

### Comparing `wiggler_studiorabota-0.0.5/wiggler/main.py` & `wiggler_studiorabota-0.0.6/wiggler/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,13 +31,14 @@
     now = datetime.now()
     fileName = now.strftime("%Y-%m-%d-%H-%M")
     filePath = f"{IMG_FOLDER}/{fileName}.jpg"
     os.system(f"libcamera-jpeg --width 1024 --height 768 --nopreview -t 1 -o {filePath}")
     return {"picture": f"image/{fileName}.jpg"}
 
 
-@app.get("/take_picture_every_minute")
-def images():
-    cron = CronTab(user='root')
-    job = cron.new(command='curl localhost:8000/take_picture')
-    job.minute.every(1)
+@app.get("/schedule_picture/{minutes}")
+def images(minutes: int = 1):
+    cron = CronTab(user=os.getlogin())
+    cron.remove(comment='take_picture')
+    job = cron.new(command='curl localhost:8000/take_picture', comment='take_picture')
+    job.minute.every(minutes)
     cron.write()
```

