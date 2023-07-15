# Comparing `tmp/pyriddle-0.0.2.tar.gz` & `tmp/pyriddle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriddle-0.0.2.tar", last modified: Mon Jul 10 21:54:48 2023, max compression
+gzip compressed data, was "pyriddle-0.0.3.tar", last modified: Sat Jul 15 10:05:10 2023, max compression
```

## Comparing `pyriddle-0.0.2.tar` & `pyriddle-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:54:48.401336 pyriddle-0.0.2/
--rw-rw-r--   0 clementp  (1000) clementp  (1000)     1554 2023-07-10 21:54:48.401336 pyriddle-0.0.2/PKG-INFO
--rw-rw-r--   0 clementp  (1000) clementp  (1000)      982 2023-07-10 21:52:04.000000 pyriddle-0.0.2/README.md
-drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:54:48.401336 pyriddle-0.0.2/pyriddle/
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-10 21:05:55.000000 pyriddle-0.0.2/pyriddle/__init__.py
-drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-10 21:54:48.401336 pyriddle-0.0.2/pyriddle.egg-info/
--rw-rw-r--   0 clementp  (1000) clementp  (1000)     1554 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/PKG-INFO
--rw-rw-r--   0 clementp  (1000) clementp  (1000)      198 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/SOURCES.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/dependency_links.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        6 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/requires.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)        9 2023-07-10 21:54:48.000000 pyriddle-0.0.2/pyriddle.egg-info/top_level.txt
--rw-rw-r--   0 clementp  (1000) clementp  (1000)       38 2023-07-10 21:54:48.401336 pyriddle-0.0.2/setup.cfg
--rw-rw-r--   0 clementp  (1000) clementp  (1000)     1133 2023-07-10 21:53:19.000000 pyriddle-0.0.2/setup.py
+drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-15 10:05:10.714628 pyriddle-0.0.3/
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1554 2023-07-15 10:05:10.714628 pyriddle-0.0.3/PKG-INFO
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)      982 2023-07-10 21:52:04.000000 pyriddle-0.0.3/README.md
+drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-15 10:05:10.714628 pyriddle-0.0.3/pyriddle/
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)       27 2023-07-11 21:21:19.000000 pyriddle-0.0.3/pyriddle/__init__.py
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     2734 2023-07-11 22:31:42.000000 pyriddle-0.0.3/pyriddle/text_stream.py
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1230 2023-07-11 21:25:50.000000 pyriddle-0.0.3/pyriddle/video_stream.py
+drwxrwxr-x   0 clementp  (1000) clementp  (1000)        0 2023-07-15 10:05:10.714628 pyriddle-0.0.3/pyriddle.egg-info/
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1554 2023-07-15 10:05:10.000000 pyriddle-0.0.3/pyriddle.egg-info/PKG-INFO
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)      247 2023-07-15 10:05:10.000000 pyriddle-0.0.3/pyriddle.egg-info/SOURCES.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)        1 2023-07-15 10:05:10.000000 pyriddle-0.0.3/pyriddle.egg-info/dependency_links.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)       52 2023-07-15 10:05:10.000000 pyriddle-0.0.3/pyriddle.egg-info/requires.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)        9 2023-07-15 10:05:10.000000 pyriddle-0.0.3/pyriddle.egg-info/top_level.txt
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)       38 2023-07-15 10:05:10.714628 pyriddle-0.0.3/setup.cfg
+-rw-rw-r--   0 clementp  (1000) clementp  (1000)     1188 2023-07-13 11:59:38.000000 pyriddle-0.0.3/setup.py
```

### Comparing `pyriddle-0.0.2/PKG-INFO` & `pyriddle-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriddle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Browser based fully customisable User Interface
 Home-page: UNKNOWN
 Author: Tech0ne
 Author-email: <null@noemail.com>
 License: UNKNOWN
 Keywords: python,ui,stream,video,stats
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyriddle Version: 0.0.2 Summary: Browser based
+Metadata-Version: 2.1 Name: pyriddle Version: 0.0.3 Summary: Browser based
 fully customisable User Interface Home-page: UNKNOWN Author: Tech0ne Author-
 email:
 noemail.com> License: UNKNOWN Keywords: python,ui,stream,video,stats Platform:
 UNKNOWN Classifier: Development Status :: 1 - Planning Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
```

### Comparing `pyriddle-0.0.2/README.md` & `pyriddle-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyriddle-0.0.2/pyriddle.egg-info/PKG-INFO` & `pyriddle-0.0.3/pyriddle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriddle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Browser based fully customisable User Interface
 Home-page: UNKNOWN
 Author: Tech0ne
 Author-email: <null@noemail.com>
 License: UNKNOWN
 Keywords: python,ui,stream,video,stats
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyriddle Version: 0.0.2 Summary: Browser based
+Metadata-Version: 2.1 Name: pyriddle Version: 0.0.3 Summary: Browser based
 fully customisable User Interface Home-page: UNKNOWN Author: Tech0ne Author-
 email:
 noemail.com> License: UNKNOWN Keywords: python,ui,stream,video,stats Platform:
 UNKNOWN Classifier: Development Status :: 1 - Planning Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
```

### Comparing `pyriddle-0.0.2/setup.py` & `pyriddle-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION                     = "0.0.2"
+VERSION                     = "0.0.3"
 DESCRIPTION                 = "Browser based fully customisable User Interface"
 LONG_DESCRIPTION            = "pyriddle gives you a simple and powerfull way to display graphics, text infos, video stream and so on, only using your browser as support."
 if os.path.isfile("./README.md"):
     with open("./README.md", 'r') as f:
         LONG_DESCRIPTION    = f.read()
 
 # Setting up
@@ -15,15 +15,15 @@
     version=VERSION,
     author="Tech0ne",
     author_email="<null@noemail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=["flask"],
+    install_requires=["flask", "simple-websocket", "flask_socketio", "opencv-python"],
     keywords=["python", "ui", "stream", "video", "stats"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

