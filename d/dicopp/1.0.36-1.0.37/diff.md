# Comparing `tmp/dicopp-1.0.36.tar.gz` & `tmp/dicopp-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicopp-1.0.36.tar", last modified: Fri May 12 13:08:08 2023, max compression
+gzip compressed data, was "dicopp-1.0.37.tar", last modified: Sat Jul 15 08:32:10 2023, max compression
```

## Comparing `dicopp-1.0.36.tar` & `dicopp-1.0.37.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-05-12 13:08:08.645580 dicopp-1.0.36/
--rw-rw-r--   0 bc        (1000) bc        (1000)       30 2023-05-12 11:46:51.000000 dicopp-1.0.36/MANIFEST.in
--rw-rw-r--   0 bc        (1000) bc        (1000)      385 2023-05-12 13:08:08.645580 dicopp-1.0.36/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      894 2023-03-23 11:57:18.000000 dicopp-1.0.36/README.md
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-05-12 13:08:08.629580 dicopp-1.0.36/dicopp/
--rw-rw-r--   0 bc        (1000) bc        (1000)     1236 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/base.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1909 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/com.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      359 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/con.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1468 2022-07-07 04:32:27.000000 dicopp-1.0.36/dicopp/daem.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1553 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/details.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     2640 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/dload.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1429 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/extension.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      688 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/first.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1976 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/flist.py
--rw-rw-r--   0 bc        (1000) bc        (1000)    29689 2023-05-12 11:12:57.000000 dicopp-1.0.36/dicopp/hublist.xml.gz
--rw-rw-r--   0 bc        (1000) bc        (1000)     4379 2023-05-12 11:46:51.000000 dicopp-1.0.36/dicopp/hubs.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1195 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/hubscon.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1519 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/hubson.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1436 2022-05-05 03:24:34.000000 dicopp-1.0.36/dicopp/layout.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1323 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/limit.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1028 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/log.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      994 2022-05-07 04:49:33.000000 dicopp-1.0.36/dicopp/main.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      895 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/nick.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      205 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/overrides.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      980 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/reqs.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     4641 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/search.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1374 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/sets.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      612 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/share.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1503 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/stor2.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      661 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/userinfo.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1514 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/users.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      540 2022-01-31 07:04:25.000000 dicopp-1.0.36/dicopp/usersloc.py
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-05-12 13:08:08.641580 dicopp-1.0.36/dicopp.egg-info/
--rw-rw-r--   0 bc        (1000) bc        (1000)      385 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      658 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/SOURCES.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        1 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/dependency_links.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       44 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/entry_points.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       60 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/requires.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        7 2023-05-12 13:08:08.000000 dicopp-1.0.36/dicopp.egg-info/top_level.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       38 2023-05-12 13:08:08.645580 dicopp-1.0.36/setup.cfg
--rw-rw-r--   0 bc        (1000) bc        (1000)      912 2023-05-12 11:46:51.000000 dicopp-1.0.36/setup.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-15 08:32:10.838813 dicopp-1.0.37/
+-rw-rw-r--   0 bc        (1000) bc        (1000)       30 2023-05-12 11:46:51.000000 dicopp-1.0.37/MANIFEST.in
+-rw-rw-r--   0 bc        (1000) bc        (1000)      387 2023-07-15 08:32:10.838813 dicopp-1.0.37/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      894 2023-03-23 11:57:18.000000 dicopp-1.0.37/README.md
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-15 08:32:10.834813 dicopp-1.0.37/dicopp/
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1252 2023-07-15 06:20:45.000000 dicopp-1.0.37/dicopp/base.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1909 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/com.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      359 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/con.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1468 2022-07-07 04:32:27.000000 dicopp-1.0.37/dicopp/daem.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1553 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/details.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2640 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/dload.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1429 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/extension.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      688 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/first.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1976 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/flist.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)    32953 2023-07-15 06:02:55.000000 dicopp-1.0.37/dicopp/hublist.xml.gz
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4579 2023-07-15 06:20:45.000000 dicopp-1.0.37/dicopp/hubs.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1195 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/hubscon.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1519 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/hubson.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1436 2022-05-05 03:24:34.000000 dicopp-1.0.37/dicopp/layout.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1323 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/limit.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1028 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/log.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      994 2022-05-07 04:49:33.000000 dicopp-1.0.37/dicopp/main.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      895 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/nick.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      205 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/overrides.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      980 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/reqs.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4641 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/search.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1374 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/sets.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      612 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/share.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1503 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/stor2.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      661 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/userinfo.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1514 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/users.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      540 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/usersloc.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-15 08:32:10.838813 dicopp-1.0.37/dicopp.egg-info/
+-rw-rw-r--   0 bc        (1000) bc        (1000)      387 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      658 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/SOURCES.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        1 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/dependency_links.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       44 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/entry_points.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       60 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/requires.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        7 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/top_level.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       38 2023-07-15 08:32:10.838813 dicopp-1.0.37/setup.cfg
+-rw-rw-r--   0 bc        (1000) bc        (1000)      945 2023-07-15 06:20:45.000000 dicopp-1.0.37/setup.py
```

### Comparing `dicopp-1.0.36/README.md` & `dicopp-1.0.37/README.md`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/base.py` & `dicopp-1.0.37/dicopp/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from . import search
 from . import daem
 from . import com
 
 import json
 from gi.repository import Gdk
 
+pkname='dicopp'
+
 import appdirs
 import os.path
 import pathlib
 def get_client_dir():
-	return pathlib.Path(appdirs.user_config_dir('dicopp'))
-get_client_dir().mkdir(exist_ok=True)
+	return pathlib.Path(appdirs.user_config_dir(pkname))
 def get_client():
 	return os.path.join(get_client_dir(),'config.json')
 
 def write(win):
 	d={}
 	dim=win.get_default_size()
 	d['width']=dim.width
@@ -35,14 +36,15 @@
 	search.store(d)
 	daem.store(d)
 	com.store(d)
 	with open(get_client(), "w") as write_file:
 		json.dump(d, write_file)
 
 def read(win):
+	get_client_dir().mkdir(exist_ok=True)
 	try:
 		with open(get_client()) as f:
 			d=json.load(f)
 			win.set_default_size(d['width'],d['height'])
 			if(d['max']):
 				win.maximize()
 			if(d['min']):
```

### Comparing `dicopp-1.0.36/dicopp/com.py` & `dicopp-1.0.37/dicopp/com.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/daem.py` & `dicopp-1.0.37/dicopp/daem.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/details.py` & `dicopp-1.0.37/dicopp/details.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/dload.py` & `dicopp-1.0.37/dicopp/dload.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/extension.py` & `dicopp-1.0.37/dicopp/extension.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/first.py` & `dicopp-1.0.37/dicopp/first.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/flist.py` & `dicopp-1.0.37/dicopp/flist.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/hubs.py` & `dicopp-1.0.37/dicopp/hubs.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,16 +126,20 @@
 			print("hubs list error")
 			if file.get_text():
 				tree = ET.parse(file.get_text())
 				root = tree.getroot()
 			else:
 				#if the module has never been imported before (== not present in sys.modules), then it is loaded and added to sys.modules.
 				import gzip
-				import os.path
-				with gzip.open(os.path.join(os.path.dirname(__file__),'hublist.xml.gz'), mode='r') as zipfile:
+
+				#https://setuptools.pypa.io/en/latest/userguide/datafiles.html
+				#import os.path
+				from importlib.resources import files
+				#with gzip.open(os.path.join(os.path.dirname(__file__),'hublist.xml.gz'), mode='r') as zipfile:
+				with gzip.open(files(base.pkname).joinpath('hublist.xml.gz'), mode='r') as zipfile:
 					root = ET.fromstring(zipfile.read())
 		ini_result(root)
 	return False
 def ini_result(root):
 	try:
 		hbs=root.find("Hubs").findall("Hub")
 	except Exception:
```

### Comparing `dicopp-1.0.36/dicopp/hubscon.py` & `dicopp-1.0.37/dicopp/hubscon.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/hubson.py` & `dicopp-1.0.37/dicopp/hubson.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/layout.py` & `dicopp-1.0.37/dicopp/layout.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/limit.py` & `dicopp-1.0.37/dicopp/limit.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/log.py` & `dicopp-1.0.37/dicopp/log.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/main.py` & `dicopp-1.0.37/dicopp/main.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/nick.py` & `dicopp-1.0.37/dicopp/nick.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/reqs.py` & `dicopp-1.0.37/dicopp/reqs.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/search.py` & `dicopp-1.0.37/dicopp/search.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/sets.py` & `dicopp-1.0.37/dicopp/sets.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/share.py` & `dicopp-1.0.37/dicopp/share.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/stor2.py` & `dicopp-1.0.37/dicopp/stor2.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/userinfo.py` & `dicopp-1.0.37/dicopp/userinfo.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/users.py` & `dicopp-1.0.37/dicopp/users.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp/usersloc.py` & `dicopp-1.0.37/dicopp/usersloc.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/dicopp.egg-info/SOURCES.txt` & `dicopp-1.0.37/dicopp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.36/setup.py` & `dicopp-1.0.37/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from setuptools import setup
 setup(name=pkname,
 	packages=[pkname],
 	#data_files = [('', [pkname+'/hublist.xml.gz'])], #still is not placing it in the same folder
 	version=ver,
 	#opt
 	include_package_data=True,
-	python_requires='>=3',
+	python_requires='>=3.9', #for importlib.resources.files
 	install_requires=["PyGObject>=3.40","requests>=2.21","appdirs>=1.4.3",\
 		"psutil>=5.5.1"],
 	description='Direct Connect ++ client',
 	long_description=README,
 	long_description_content_type="text/markdown",
 	url='https://github.com/colin-i/dico',
 	author='bot',
```

