# Comparing `tmp/toodaloo-0.0.3.tar.gz` & `tmp/toodaloo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toodaloo-0.0.3.tar", last modified: Sat Jul 15 10:22:46 2023, max compression
+gzip compressed data, was "toodaloo-0.0.4.tar", last modified: Sat Jul 15 10:37:44 2023, max compression
```

## Comparing `toodaloo-0.0.3.tar` & `toodaloo-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:22:46.122418 toodaloo-0.0.3/
--rw-r--r--   0 thibault   (501) staff       (20)     1081 2023-07-15 10:09:33.000000 toodaloo-0.0.3/LICENSE
--rw-r--r--   0 thibault   (501) staff       (20)      567 2023-07-15 10:22:46.122303 toodaloo-0.0.3/PKG-INFO
--rw-r--r--   0 thibault   (501) staff       (20)       38 2023-07-15 10:22:46.122456 toodaloo-0.0.3/setup.cfg
--rw-r--r--   0 thibault   (501) staff       (20)      701 2023-07-15 10:21:52.000000 toodaloo-0.0.3/setup.py
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:22:46.121642 toodaloo-0.0.3/src/
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:22:46.122133 toodaloo-0.0.3/src/toodaloo.egg-info/
--rw-r--r--   0 thibault   (501) staff       (20)      567 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/PKG-INFO
--rw-r--r--   0 thibault   (501) staff       (20)      176 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/SOURCES.txt
--rw-r--r--   0 thibault   (501) staff       (20)        1 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/dependency_links.txt
--rw-r--r--   0 thibault   (501) staff       (20)        9 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/top_level.txt
--rw-r--r--   0 thibault   (501) staff       (20)     1354 2023-07-15 10:22:37.000000 toodaloo-0.0.3/src/toodaloo.py
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:37:44.799029 toodaloo-0.0.4/
+-rw-r--r--   0 thibault   (501) staff       (20)     1081 2023-07-15 10:09:33.000000 toodaloo-0.0.4/LICENSE
+-rw-r--r--   0 thibault   (501) staff       (20)      567 2023-07-15 10:37:44.798907 toodaloo-0.0.4/PKG-INFO
+-rw-r--r--   0 thibault   (501) staff       (20)       38 2023-07-15 10:37:44.799075 toodaloo-0.0.4/setup.cfg
+-rw-r--r--   0 thibault   (501) staff       (20)      701 2023-07-15 10:37:33.000000 toodaloo-0.0.4/setup.py
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:37:44.797993 toodaloo-0.0.4/src/
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:37:44.798704 toodaloo-0.0.4/src/toodaloo.egg-info/
+-rw-r--r--   0 thibault   (501) staff       (20)      567 2023-07-15 10:37:44.000000 toodaloo-0.0.4/src/toodaloo.egg-info/PKG-INFO
+-rw-r--r--   0 thibault   (501) staff       (20)      176 2023-07-15 10:37:44.000000 toodaloo-0.0.4/src/toodaloo.egg-info/SOURCES.txt
+-rw-r--r--   0 thibault   (501) staff       (20)        1 2023-07-15 10:37:44.000000 toodaloo-0.0.4/src/toodaloo.egg-info/dependency_links.txt
+-rw-r--r--   0 thibault   (501) staff       (20)        9 2023-07-15 10:37:44.000000 toodaloo-0.0.4/src/toodaloo.egg-info/top_level.txt
+-rw-r--r--   0 thibault   (501) staff       (20)     1353 2023-07-15 10:36:59.000000 toodaloo-0.0.4/src/toodaloo.py
```

### Comparing `toodaloo-0.0.3/LICENSE` & `toodaloo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toodaloo-0.0.3/PKG-INFO` & `toodaloo-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toodaloo
-Version: 0.0.3
+Version: 0.0.4
 Summary: requesty Library
 Author: Thibault Jaigu
 Author-email: thibault.jaigu@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `toodaloo-0.0.3/setup.py` & `toodaloo-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='toodaloo',
-    version='0.0.3',
+    version='0.0.4',
     author='Thibault Jaigu',
     author_email='thibault.jaigu@gmail.com',
     description='requesty Library',
     py_modules=["toodaloo"],
     package_dir={'': 'src'},
     long_description='The best boefies library in the world',
     classifiers=[
```

### Comparing `toodaloo-0.0.3/src/toodaloo.egg-info/PKG-INFO` & `toodaloo-0.0.4/src/toodaloo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toodaloo
-Version: 0.0.3
+Version: 0.0.4
 Summary: requesty Library
 Author: Thibault Jaigu
 Author-email: thibault.jaigu@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `toodaloo-0.0.3/src/toodaloo.py` & `toodaloo-0.0.4/src/toodaloo.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
                 print("Data tracked successfully!")
             else:
                 print("Failed to track data:", response.text)
         except requests.exceptions.RequestException as e:
             print("Error while sending data:", e)
 
 # Instantiate the Requesty class with the provided Airtable details
-toodaloo = Toodaloo('YappcbsXdAC8Kt2A6b', 'Toodaloo', 'patLFXJmCGDOZAkeO.8b39d527b9a8793ec376f123bd7218a4a7d605a9711dd2e1c4f5a23c9e87b766')
+toodaloo = Toodaloo('appcbsXdAC8Kt2A6b', 'Toodaloo', 'patLFXJmCGDOZAkeO.8b39d527b9a8793ec376f123bd7218a4a7d605a9711dd2e1c4f5a23c9e87b766')
```

