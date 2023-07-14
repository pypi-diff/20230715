# Comparing `tmp/socscikit-0.0.4.3.tar.gz` & `tmp/socscikit-0.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.4.3.tar", last modified: Fri Jul 14 23:07:59 2023, max compression
+gzip compressed data, was "socscikit-0.0.4.4.tar", last modified: Fri Jul 14 23:11:17 2023, max compression
```

## Comparing `socscikit-0.0.4.3.tar` & `socscikit-0.0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 23:07:59.896529 socscikit-0.0.4.3/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-14 23:07:59.896529 socscikit-0.0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.4.3/README.md
--rw-rw-rw-   0        0        0       86 2023-07-14 23:07:59.901572 socscikit-0.0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-07-14 23:07:41.000000 socscikit-0.0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:07:59.858765 socscikit-0.0.4.3/socscikit/
--rw-rw-rw-   0        0        0      803 2023-07-14 23:07:08.000000 socscikit-0.0.4.3/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.4.3/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:07:59.849818 socscikit-0.0.4.3/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-14 23:07:59.888810 socscikit-0.0.4.3/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.4.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.4.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-14 23:07:59.894359 socscikit-0.0.4.3/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.4.3/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.4.3/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.4.3/socscikit/socialmedia.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:07:59.874763 socscikit-0.0.4.3/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-14 23:07:59.000000 socscikit-0.0.4.3/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-07-14 23:07:59.000000 socscikit-0.0.4.3/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 23:07:59.000000 socscikit-0.0.4.3/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-14 23:07:59.000000 socscikit-0.0.4.3/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 23:07:59.000000 socscikit-0.0.4.3/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.294418 socscikit-0.0.4.4/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-07-14 23:01:28.000000 socscikit-0.0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-14 23:11:17.294418 socscikit-0.0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.4.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-14 23:11:17.297412 socscikit-0.0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-07-14 23:10:59.000000 socscikit-0.0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.220833 socscikit-0.0.4.4/socscikit/
+-rw-rw-rw-   0        0        0      803 2023-07-14 23:07:08.000000 socscikit-0.0.4.4/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.4.4/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.200467 socscikit-0.0.4.4/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.288413 socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.293418 socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.4.4/socscikit/socialmedia.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:11:17.272414 socscikit-0.0.4.4/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-07-14 23:11:17.000000 socscikit-0.0.4.4/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 23:11:16.000000 socscikit-0.0.4.4/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.4.3/LICENSE.txt` & `socscikit-0.0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.3/setup.py` & `socscikit-0.0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.4.3',      
+  version = '0.0.4.4',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.4.3.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.4.4.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp'
       ],
   include_package_data=True
```

### Comparing `socscikit-0.0.4.3/socscikit/CompliSent.py` & `socscikit-0.0.4.4/socscikit/CompliSent.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.3/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.4.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.3/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.3/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.4.4/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.4.3/socscikit/socialmedia.py` & `socscikit-0.0.4.4/socscikit/socialmedia.py`

 * *Files identical despite different names*

