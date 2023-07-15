# Comparing `tmp/pptx-tools-0.1.6.tar.gz` & `tmp/pptx-tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx-tools-0.1.6.tar", last modified: Fri Jul 14 07:08:32 2023, max compression
+gzip compressed data, was "pptx-tools-0.1.7.tar", last modified: Sat Jul 15 12:39:00 2023, max compression
```

## Comparing `pptx-tools-0.1.6.tar` & `pptx-tools-0.1.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.294606 pptx-tools-0.1.6/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/pptx_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/apps/slide_add_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/apps/slide_delete_notes.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/audio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/pptx_tools/data/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/data/hello.pptx
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/data/transparent.png
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/slide_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/slide_transition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/pptx_tools/tts/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/azure_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/google_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/google_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     4956 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/video_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.294606 pptx-tools-0.1.6/pptx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2472 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/tests/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/tests/pptx_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/tests/pptx_tools/test_slide_add_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/pptx_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/apps/slide_add_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/apps/slide_check_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/apps/slide_delete_notes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/audio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/pptx_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/data/hello.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/data/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/slide_transition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/pptx_tools/tts/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/tts/azure_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/tts/azure_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/tts/google_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/tts/google_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4956 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/pptx_tools/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/pptx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-15 12:38:59.000000 pptx-tools-0.1.7/pptx_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 12:39:00.003907 pptx-tools-0.1.7/tests/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/tests/pptx_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-15 12:38:50.000000 pptx-tools-0.1.7/tests/pptx_tools/test_slide_add_voice.py
```

### Comparing `pptx-tools-0.1.6/LICENSE` & `pptx-tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/PKG-INFO` & `pptx-tools-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pptx-tools-0.1.6/README.md` & `pptx-tools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/apps/slide_add_voice.py` & `pptx-tools-0.1.7/pptx_tools/apps/slide_add_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/apps/slide_delete_notes.py` & `pptx-tools-0.1.7/pptx_tools/apps/slide_delete_notes.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/data/hello.pptx` & `pptx-tools-0.1.7/pptx_tools/data/hello.pptx`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/slide_info.py` & `pptx-tools-0.1.7/pptx_tools/slide_info.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/slide_transition.py` & `pptx-tools-0.1.7/pptx_tools/slide_transition.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/tts/azure_tts.py` & `pptx-tools-0.1.7/pptx_tools/tts/azure_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/tts/azure_tts_voice.py` & `pptx-tools-0.1.7/pptx_tools/tts/azure_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/tts/google_tts.py` & `pptx-tools-0.1.7/pptx_tools/tts/google_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/tts/google_tts_voice.py` & `pptx-tools-0.1.7/pptx_tools/tts/google_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/utils.py` & `pptx-tools-0.1.7/pptx_tools/utils.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools/video_utils.py` & `pptx-tools-0.1.7/pptx_tools/video_utils.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.6/pptx_tools.egg-info/PKG-INFO` & `pptx-tools-0.1.7/pptx_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pptx-tools-0.1.6/pptx_tools.egg-info/SOURCES.txt` & `pptx-tools-0.1.7/pptx_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pptx_tools.egg-info/dependency_links.txt
 pptx_tools.egg-info/entry_points.txt
 pptx_tools.egg-info/not-zip-safe
 pptx_tools.egg-info/requires.txt
 pptx_tools.egg-info/top_level.txt
 pptx_tools/apps/__init__.py
 pptx_tools/apps/slide_add_voice.py
+pptx_tools/apps/slide_check_fonts.py
 pptx_tools/apps/slide_delete_notes.py
 pptx_tools/data/__init__.py
 pptx_tools/data/hello.pptx
 pptx_tools/data/transparent.png
 pptx_tools/tts/__init__.py
 pptx_tools/tts/azure_tts.py
 pptx_tools/tts/azure_tts_voice.py
```

### Comparing `pptx-tools-0.1.6/setup.py` & `pptx-tools-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,44 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.6"
+version = "0.1.7"
 
 
-if sys.argv[-1] == "release":
-    # Release via github-actions.
-    commands = [
-        'git tag v{:s}'.format(version),
-        'git push origin master --tag',
-    ]
+def git(*args):
+    return subprocess.check_call(['git'] + list(args))
+
+
+def check_if_tag_exists(version):
+    try:
+        git("rev-parse", "v{:s}".format(version))
+        return True
+    except subprocess.CalledProcessError:
+        return False
+
+
+def push_tag(version):
+    commands = []
+
+    if not check_if_tag_exists(version):
+        commands.append('git tag v{:s}'.format(version))
+        commands.append('git push origin master --force --tags')
+
     for cmd in commands:
         print('+ {}'.format(cmd))
         subprocess.check_call(shlex.split(cmd))
+
+
+if sys.argv[-1] == "release":
+    # Release via github-actions.
+    push_tag(version)
     sys.exit(0)
 
 
 def listup_package_data():
     data_files = []
     for root, _, files in os.walk('pptx_tools/data'):
         for filename in files:
@@ -81,10 +99,11 @@
         'all': (install_requires
                 + azure_install_requires),
     },
     entry_points={
         "console_scripts": [
             "slide-add-voice=pptx_tools.apps.slide_add_voice:main",
             "slide-delete-notes=pptx_tools.apps.slide_delete_notes:main",
+            "slide-check-fonts=pptx_tools.apps.slide_check_fonts:main",
         ]
     },
 )
```

### Comparing `pptx-tools-0.1.6/tests/pptx_tools/test_slide_add_voice.py` & `pptx-tools-0.1.7/tests/pptx_tools/test_slide_add_voice.py`

 * *Files identical despite different names*

