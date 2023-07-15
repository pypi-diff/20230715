# Comparing `tmp/medisynth-0.0.3.tar.gz` & `tmp/medisynth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisynth-0.0.3.tar", last modified: Sat Jul 15 18:32:39 2023, max compression
+gzip compressed data, was "medisynth-0.0.4.tar", last modified: Sat Jul 15 18:41:04 2023, max compression
```

## Comparing `medisynth-0.0.3.tar` & `medisynth-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 18:32:39.992509 medisynth-0.0.3/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6238 2023-07-15 18:32:39.992509 medisynth-0.0.3/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5520 2023-07-15 18:00:31.000000 medisynth-0.0.3/README.md
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 18:32:39.992509 medisynth-0.0.3/medisynth.egg-info/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6238 2023-07-15 18:32:39.000000 medisynth-0.0.3/medisynth.egg-info/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      188 2023-07-15 18:32:39.000000 medisynth-0.0.3/medisynth.egg-info/SOURCES.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 18:32:39.000000 medisynth-0.0.3/medisynth.egg-info/dependency_links.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-07-15 18:32:39.000000 medisynth-0.0.3/medisynth.egg-info/requires.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 18:32:39.000000 medisynth-0.0.3/medisynth.egg-info/top_level.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     1037 2023-07-15 18:30:53.000000 medisynth-0.0.3/pyproject.toml
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       38 2023-07-15 18:32:39.992509 medisynth-0.0.3/setup.cfg
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 18:41:04.372373 medisynth-0.0.4/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6224 2023-07-15 18:41:04.372373 medisynth-0.0.4/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5520 2023-07-15 18:00:31.000000 medisynth-0.0.4/README.md
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 18:41:04.372373 medisynth-0.0.4/medisynth.egg-info/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6224 2023-07-15 18:41:04.000000 medisynth-0.0.4/medisynth.egg-info/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      188 2023-07-15 18:41:04.000000 medisynth-0.0.4/medisynth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 18:41:04.000000 medisynth-0.0.4/medisynth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-07-15 18:41:04.000000 medisynth-0.0.4/medisynth.egg-info/requires.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 18:41:04.000000 medisynth-0.0.4/medisynth.egg-info/top_level.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     1040 2023-07-15 18:38:44.000000 medisynth-0.0.4/pyproject.toml
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       38 2023-07-15 18:41:04.372373 medisynth-0.0.4/setup.cfg
```

### Comparing `medisynth-0.0.3/PKG-INFO` & `medisynth-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: medisynth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python-based library for Synthesis of Ultrasound Fetal Imaging
-Author-email: Miguel Xochicale <your@email.com>
-Maintainer-email: Harvey Mannering <your@email.com>, Sofía Miñano <your@email.com>
+Author-email: Miguel Xochicale <your0@email.com>, Harvey Mannering <your1@email.com>, Sofía Miñano <your2@email.com>
 License: MIT
 Project-URL: homepage, https://github.com/budai4medtech/medisynth
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: medisynth Version: 0.0.3 Summary: Python-based
+Metadata-Version: 2.1 Name: medisynth Version: 0.0.4 Summary: Python-based
 library for Synthesis of Ultrasound Fetal Imaging Author-email: Miguel
 Xochicale
-email.com> Maintainer-email: Harvey Mannering
+email.com>, Harvey Mannering
 email.com>, SofÃ­a MiÃ±ano
 email.com> License: MIT Project-URL: homepage, https://github.com/
 budai4medtech/medisynth Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.8 Requires-Python: >=3.11 Description-
```

### Comparing `medisynth-0.0.3/README.md` & `medisynth-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `medisynth-0.0.3/medisynth.egg-info/PKG-INFO` & `medisynth-0.0.4/medisynth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: medisynth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python-based library for Synthesis of Ultrasound Fetal Imaging
-Author-email: Miguel Xochicale <your@email.com>
-Maintainer-email: Harvey Mannering <your@email.com>, Sofía Miñano <your@email.com>
+Author-email: Miguel Xochicale <your0@email.com>, Harvey Mannering <your1@email.com>, Sofía Miñano <your2@email.com>
 License: MIT
 Project-URL: homepage, https://github.com/budai4medtech/medisynth
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: medisynth Version: 0.0.3 Summary: Python-based
+Metadata-Version: 2.1 Name: medisynth Version: 0.0.4 Summary: Python-based
 library for Synthesis of Ultrasound Fetal Imaging Author-email: Miguel
 Xochicale
-email.com> Maintainer-email: Harvey Mannering
+email.com>, Harvey Mannering
 email.com>, SofÃ­a MiÃ±ano
 email.com> License: MIT Project-URL: homepage, https://github.com/
 budai4medtech/medisynth Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.8 Requires-Python: >=3.11 Description-
```

### Comparing `medisynth-0.0.3/pyproject.toml` & `medisynth-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "medisynth"
 description = "Python-based library for Synthesis of Ultrasound Fetal Imaging"
 keywords = ["artificial intelligence", "diffusion models"]
 authors = [
-	{name="Miguel Xochicale", email= "your@email.com"},
+	{name="Miguel Xochicale", email= "your0@email.com"},
+	{name="Harvey Mannering", email="your1@email.com"},
+	{name="Sofía Miñano", email="your2@email.com"},
 ]
 maintainers = [
-	{name="Harvey Mannering", email="your@email.com"},
-	{name="Sofía Miñano", email="your@email.com"},
 ]
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 classifiers=[
 	"Development Status :: 2 - Pre-Alpha",
 	"Intended Audience :: Developers",
 	"Topic :: Scientific/Engineering :: Artificial Intelligence",
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python :: 3.8",
```

