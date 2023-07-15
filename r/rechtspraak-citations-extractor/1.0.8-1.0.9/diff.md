# Comparing `tmp/rechtspraak_citations_extractor-1.0.8.tar.gz` & `tmp/rechtspraak_citations_extractor-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_citations_extractor-1.0.8.tar", last modified: Tue Jun 20 19:24:11 2023, max compression
+gzip compressed data, was "rechtspraak_citations_extractor-1.0.9.tar", last modified: Mon Jul  3 07:37:40 2023, max compression
```

## Comparing `rechtspraak_citations_extractor-1.0.8.tar` & `rechtspraak_citations_extractor-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:24:11.499824 rechtspraak_citations_extractor-1.0.8/
--rw-rw-rw-   0        0        0     4818 2023-06-20 19:24:11.498824 rechtspraak_citations_extractor-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 19:24:11.487824 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/
--rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/__init__.py
--rw-rw-rw-   0        0        0    13457 2023-06-20 19:22:48.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/citations_extractor.py
--rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:24:11.496824 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/
--rw-rw-rw-   0        0        0     4818 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 19:24:11.499824 rechtspraak_citations_extractor-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-06-20 19:24:05.000000 rechtspraak_citations_extractor-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 07:37:40.717403 rechtspraak_citations_extractor-1.0.9/
+-rw-rw-rw-   0        0        0     4818 2023-07-03 07:37:40.716402 rechtspraak_citations_extractor-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 07:37:40.703401 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor/
+-rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor/__init__.py
+-rw-rw-rw-   0        0        0    13406 2023-07-03 07:37:35.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor/citations_extractor.py
+-rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor/testing.py
+drwxrwxrwx   0        0        0        0 2023-07-03 07:37:40.714403 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/
+-rw-rw-rw-   0        0        0     4818 2023-07-03 07:37:40.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-03 07:37:40.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 07:37:40.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-03 07:37:40.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-03 07:37:40.000000 rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 07:37:40.717403 rechtspraak_citations_extractor-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-07-03 07:37:35.000000 rechtspraak_citations_extractor-1.0.9/setup.py
```

### Comparing `rechtspraak_citations_extractor-1.0.8/PKG-INFO` & `rechtspraak_citations_extractor-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_citations_extractor
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.8
+Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.9
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.8/README.md` & `rechtspraak_citations_extractor-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/citations_extractor.py` & `rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor/citations_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,16 +252,15 @@
                             added_sth_new = add_legislations_no_duplicates(legislation_citations, sub_ref)
 
                 for the_citations in sub.iterchildren(incoming):
                     for sub_ref in the_citations.iterchildren():
                         if is_case_law(sub_ref):
                             added_sth_new = add_citations_no_duplicates(case_law_citations_incoming, sub_ref)
 
-        if not added_sth_new or start_page > 15:
-            #print(start_page)
+        if not added_sth_new:
             end_of_pages = True
 
     # Remove duplicates empties
 
     for item in case_law_citations_incoming:
         if item[target_ecli] == "":
             case_law_citations_incoming.remove(item)
```

### Comparing `rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/PKG-INFO` & `rechtspraak_citations_extractor-1.0.9/rechtspraak_citations_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-citations-extractor
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.8
+Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.9
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.8/setup.py` & `rechtspraak_citations_extractor-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_citations_extractor',
     packages=find_packages(include=['rechtspraak_citations_extractor']),
-    version='1.0.8',
+    version='1.0.9',
     description='Library for extracting rechtspraak citations via LIDO',
     author='LawTech Lab',
     license='MIT',
     install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'citations', 'rechtspraak citations', 'RS citations'],
     long_description=long_descr,
```

