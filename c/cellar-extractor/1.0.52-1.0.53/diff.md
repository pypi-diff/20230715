# Comparing `tmp/cellar_extractor-1.0.52.tar.gz` & `tmp/cellar_extractor-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.52.tar", last modified: Sat Jul 15 13:17:40 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.53.tar", last modified: Sat Jul 15 13:25:18 2023, max compression
```

## Comparing `cellar_extractor-1.0.52.tar` & `cellar_extractor-1.0.53.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 13:17:40.597864 cellar_extractor-1.0.52/
--rw-rw-rw-   0        0        0     6921 2023-07-15 13:17:40.596865 cellar_extractor-1.0.52/PKG-INFO
--rw-rw-rw-   0        0        0     6474 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 13:17:40.586863 cellar_extractor-1.0.52/cellar_extractor/
--rw-rw-rw-   0        0        0      704 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      163 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3329 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11308 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6475 2023-07-15 13:17:23.000000 cellar_extractor-1.0.52/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1040 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2023-07-15 13:08:30.000000 cellar_extractor-1.0.52/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:17:40.595863 cellar_extractor-1.0.52/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     6921 2023-07-15 13:17:40.000000 cellar_extractor-1.0.52/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-07-15 13:17:40.000000 cellar_extractor-1.0.52/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 13:17:40.000000 cellar_extractor-1.0.52/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-07-15 13:17:40.000000 cellar_extractor-1.0.52/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 13:17:40.000000 cellar_extractor-1.0.52/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 13:17:40.598864 cellar_extractor-1.0.52/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-07-15 13:17:33.000000 cellar_extractor-1.0.52/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:25:18.291472 cellar_extractor-1.0.53/
+-rw-rw-rw-   0        0        0     6921 2023-07-15 13:25:18.290471 cellar_extractor-1.0.53/PKG-INFO
+-rw-rw-rw-   0        0        0     6474 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 13:25:18.280472 cellar_extractor-1.0.53/cellar_extractor/
+-rw-rw-rw-   0        0        0      704 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      163 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3329 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11308 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1334 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6477 2023-07-15 13:25:06.000000 cellar_extractor-1.0.53/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1040 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2023-07-15 13:24:49.000000 cellar_extractor-1.0.53/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:25:18.288470 cellar_extractor-1.0.53/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     6921 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 13:25:18.000000 cellar_extractor-1.0.53/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 13:25:18.291472 cellar_extractor-1.0.53/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-15 13:25:13.000000 cellar_extractor-1.0.53/setup.py
```

### Comparing `cellar_extractor-1.0.52/PKG-INFO` & `cellar_extractor-1.0.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.52
+Version: 1.0.53
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.52 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.53 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.52/README.md` & `cellar_extractor-1.0.53/README.md`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.53/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/cellar.py` & `cellar_extractor-1.0.53/cellar_extractor/cellar.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.53/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.53/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.53/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.53/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.53/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.53/cellar_extractor/fulltext_saving.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,10 +169,10 @@
 Used for adding columns easier to a dataframe for add_sections().
 """
 
 
 def add_column_frow_list(data, name, list):
     column = pd.Series([], dtype='string')
     for l in list:
-        column = pd.concat(column,l)
+        column = pd.concat([column,l])
     column.sort_index(inplace=True)
     data.insert(1, name, column)
```

### Comparing `cellar_extractor-1.0.52/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.53/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.53/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor/sparql.py` & `cellar_extractor-1.0.53/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.53/cellar_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.52
+Version: 1.0.53
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.52 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.53 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.52/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.53/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.52/setup.py` & `cellar_extractor-1.0.53/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.52',
+    version='1.0.53',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

