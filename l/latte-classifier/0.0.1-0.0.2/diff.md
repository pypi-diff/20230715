# Comparing `tmp/latte_classifier-0.0.1.tar.gz` & `tmp/latte_classifier-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latte_classifier-0.0.1.tar", last modified: Sat Jul 15 06:10:16 2023, max compression
+gzip compressed data, was "latte_classifier-0.0.2.tar", last modified: Sat Jul 15 06:54:36 2023, max compression
```

## Comparing `latte_classifier-0.0.1.tar` & `latte_classifier-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 06:10:16.388864 latte_classifier-0.0.1/
--rw-rw-rw-   0        0        0       81 2023-07-15 04:17:22.000000 latte_classifier-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2023-07-15 04:20:58.000000 latte_classifier-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-15 04:35:12.000000 latte_classifier-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      677 2023-07-15 06:10:16.373237 latte_classifier-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-07-15 06:09:45.000000 latte_classifier-0.0.1/README.txt
--rw-rw-rw-   0        0        0     5301 2023-07-02 08:53:38.000000 latte_classifier-0.0.1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:10:16.341988 latte_classifier-0.0.1/latte.egg-info/
--rw-rw-rw-   0        0        0      248 2023-07-15 04:55:11.000000 latte_classifier-0.0.1/latte.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 04:55:11.000000 latte_classifier-0.0.1/latte.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-15 04:55:11.000000 latte_classifier-0.0.1/latte.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 04:55:11.000000 latte_classifier-0.0.1/latte.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 06:10:16.373237 latte_classifier-0.0.1/latte_classifier.egg-info/
--rw-rw-rw-   0        0        0      677 2023-07-15 06:10:16.000000 latte_classifier-0.0.1/latte_classifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-07-15 06:10:16.000000 latte_classifier-0.0.1/latte_classifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 06:10:16.000000 latte_classifier-0.0.1/latte_classifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-15 06:10:16.000000 latte_classifier-0.0.1/latte_classifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 06:10:16.000000 latte_classifier-0.0.1/latte_classifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-02 08:48:24.000000 latte_classifier-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 06:10:16.388864 latte_classifier-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-07-15 06:07:55.000000 latte_classifier-0.0.1/setup.py
--rw-rw-rw-   0        0        0      173 2023-07-02 08:53:50.000000 latte_classifier-0.0.1/test.py
--rw-rw-rw-   0        0        0     2253 2023-07-01 14:14:27.000000 latte_classifier-0.0.1/testfn.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:54:36.527557 latte_classifier-0.0.2/
+-rw-rw-rw-   0        0        0       81 2023-07-15 06:48:53.000000 latte_classifier-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2023-07-15 04:20:58.000000 latte_classifier-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-15 04:35:12.000000 latte_classifier-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3722 2023-07-15 06:54:36.527557 latte_classifier-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3119 2023-07-15 06:28:09.000000 latte_classifier-0.0.2/README.txt
+-rw-rw-rw-   0        0        0     5301 2023-07-02 08:53:38.000000 latte_classifier-0.0.2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:54:36.519559 latte_classifier-0.0.2/latte_classifier.egg-info/
+-rw-rw-rw-   0        0        0     3722 2023-07-15 06:54:36.000000 latte_classifier-0.0.2/latte_classifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-15 06:54:36.000000 latte_classifier-0.0.2/latte_classifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 06:54:36.000000 latte_classifier-0.0.2/latte_classifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-15 06:54:36.000000 latte_classifier-0.0.2/latte_classifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 06:54:36.000000 latte_classifier-0.0.2/latte_classifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       65 2023-07-15 06:34:37.000000 latte_classifier-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 06:54:36.535559 latte_classifier-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      778 2023-07-15 06:53:07.000000 latte_classifier-0.0.2/setup.py
+-rw-rw-rw-   0        0        0      173 2023-07-02 08:53:50.000000 latte_classifier-0.0.2/test.py
+-rw-rw-rw-   0        0        0     2253 2023-07-01 14:14:27.000000 latte_classifier-0.0.2/testfn.py
```

### Comparing `latte_classifier-0.0.1/LICENCE.txt` & `latte_classifier-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `latte_classifier-0.0.1/__init__.py` & `latte_classifier-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `latte_classifier-0.0.1/setup.py` & `latte_classifier-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='latte_classifier',
-  version='0.0.1',
+  version='0.0.2',
   description='simple classification algorithms',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Sebinmon Vr ',
   author_email='nthn8777@gmail.com',
   license='MIT', 
   classifiers=classifiers,
-  keywords='latte', 
+  keywords='latte_classifier', 
   packages=find_packages(),
-  install_requires=['numpy','matplotlib','sklearn','sklearn.svm','sklearn.tree','sklearn.linear_model','libsvm'] 
+  install_requires=['numpy','matplotlib','sklearn','sklearn.tree','sklearn.linear_model'] 
 )
```

### Comparing `latte_classifier-0.0.1/testfn.py` & `latte_classifier-0.0.2/testfn.py`

 * *Files identical despite different names*

