# Comparing `tmp/zenodo_get-1.3.4.tar.gz` & `tmp/zenodo_get-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenodo_get-1.3.4.tar", last modified: Fri Nov 19 23:35:12 2021, max compression
+gzip compressed data, was "zenodo_get-1.4.0.tar", last modified: Sat Jul 15 18:14:04 2023, max compression
```

## Comparing `zenodo_get-1.3.4.tar` & `zenodo_get-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,32 @@
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2021-11-19 23:35:12.317928 zenodo_get-1.3.4/
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)    34520 2021-11-19 23:25:30.000000 zenodo_get-1.3.4/LICENSE.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       70 2021-11-19 23:25:30.000000 zenodo_get-1.3.4/MANIFEST.in
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1104 2021-11-19 23:35:12.317928 zenodo_get-1.3.4/PKG-INFO
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     4227 2021-11-19 23:25:30.000000 zenodo_get-1.3.4/README.md
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       79 2021-11-19 23:35:12.317928 zenodo_get-1.3.4/setup.cfg
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1296 2021-11-19 23:33:56.000000 zenodo_get-1.3.4/setup.py
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2021-11-19 23:35:12.316928 zenodo_get-1.3.4/zenodo_get/
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1159 2021-11-19 23:34:13.000000 zenodo_get-1.3.4/zenodo_get/__init__.py
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)       97 2021-11-19 23:25:30.000000 zenodo_get-1.3.4/zenodo_get/__main__.py
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)    11066 2021-11-19 23:30:43.000000 zenodo_get-1.3.4/zenodo_get/zget.py
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2021-11-19 23:35:12.317928 zenodo_get-1.3.4/zenodo_get.egg-info/
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1104 2021-11-19 23:35:12.000000 zenodo_get-1.3.4/zenodo_get.egg-info/PKG-INFO
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      323 2021-11-19 23:35:12.000000 zenodo_get-1.3.4/zenodo_get.egg-info/SOURCES.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)        1 2021-11-19 23:35:12.000000 zenodo_get-1.3.4/zenodo_get.egg-info/dependency_links.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       59 2021-11-19 23:35:12.000000 zenodo_get-1.3.4/zenodo_get.egg-info/entry_points.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2021-11-19 23:35:12.000000 zenodo_get-1.3.4/zenodo_get.egg-info/requires.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       11 2021-11-19 23:35:12.000000 zenodo_get-1.3.4/zenodo_get.egg-info/top_level.txt
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-07-15 18:14:04.472240 zenodo_get-1.4.0/
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-07-15 18:14:04.471240 zenodo_get-1.4.0/.circleci/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1428 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/.circleci/config.yml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       40 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/.coveragerc
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1009 2023-05-29 11:52:10.000000 zenodo_get-1.4.0/.pre-commit-config.yaml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      761 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/.travis.yml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)    34520 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/LICENSE.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       70 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/MANIFEST.in
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      388 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/Makefile
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      985 2023-07-15 18:14:04.472240 zenodo_get-1.4.0/PKG-INFO
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     4227 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/README.md
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      746 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/appveyor.yml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/requirements.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       79 2023-07-15 18:14:04.472240 zenodo_get-1.4.0/setup.cfg
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1199 2023-07-15 18:09:18.000000 zenodo_get-1.4.0/setup.py
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-07-15 18:14:04.471240 zenodo_get-1.4.0/tests/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       35 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/tests/Makefile
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)      473 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/tests/test.sh
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)      241 2021-11-19 23:25:30.000000 zenodo_get-1.4.0/tests/win-test.bat
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-07-15 18:14:04.471240 zenodo_get-1.4.0/zenodo_get/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1159 2023-07-15 18:13:17.000000 zenodo_get-1.4.0/zenodo_get/__init__.py
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)       97 2023-05-29 11:52:10.000000 zenodo_get-1.4.0/zenodo_get/__main__.py
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)     8935 2023-06-19 06:19:08.000000 zenodo_get-1.4.0/zenodo_get/gpt4click.py
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)    11435 2023-07-15 18:07:44.000000 zenodo_get-1.4.0/zenodo_get/zget.py
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-07-15 18:14:04.472240 zenodo_get-1.4.0/zenodo_get.egg-info/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      985 2023-07-15 18:14:04.000000 zenodo_get-1.4.0/zenodo_get.egg-info/PKG-INFO
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      515 2023-07-15 18:14:04.000000 zenodo_get-1.4.0/zenodo_get.egg-info/SOURCES.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)        1 2023-07-15 18:14:04.000000 zenodo_get-1.4.0/zenodo_get.egg-info/dependency_links.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       58 2023-07-15 18:14:04.000000 zenodo_get-1.4.0/zenodo_get.egg-info/entry_points.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2023-07-15 18:14:04.000000 zenodo_get-1.4.0/zenodo_get.egg-info/requires.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       11 2023-07-15 18:14:04.000000 zenodo_get-1.4.0/zenodo_get.egg-info/top_level.txt
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)     8692 2023-05-29 11:52:10.000000 zenodo_get-1.4.0/zenodofs.py
```

### Comparing `zenodo_get-1.3.4/LICENSE.txt` & `zenodo_get-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zenodo_get-1.3.4/PKG-INFO` & `zenodo_get-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: zenodo_get
-Version: 1.3.4
+Version: 1.4.0
 Summary: Zenodo_get - a downloader for Zenodo records
 Home-page: https://gitlab.com/dvolgyes/zenodo_get
 Author: David Völgyes
 Author-email: david.volgyes@ieee.org
 License: AGPL v3
 Keywords: zenodo download
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 This program is meant to download complete Zenodo records based
 on the Zenodo record ID or the DOI. The primary goal is to ease access
 to large records with dozens of files.
-
-
```

### Comparing `zenodo_get-1.3.4/README.md` & `zenodo_get-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `zenodo_get-1.3.4/setup.py` & `zenodo_get-1.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,25 +14,23 @@
     long_description_content_type='text/markdown',
     url=zget.__uri__,
     license=zget.__license__,
     packages=setuptools.find_packages(),
     entry_points={'console_scripts': [
                       'zenodo_get = zenodo_get.zget:zenodo_get'
                       ]},
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     setup_requires=[],
     install_requires=['requests', 'wget'],
     keywords='zenodo download',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU Affero General Public License v3',
     ],
 )
```

### Comparing `zenodo_get-1.3.4/zenodo_get/__init__.py` & `zenodo_get-1.4.0/zenodo_get/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = '1.3.4'
+__version__ = '1.4.0'
 __title__ = 'zenodo_get'
 __summary__ = 'Zenodo_get - a downloader for Zenodo records'
 __uri__ = 'https://gitlab.com/dvolgyes/zenodo_get'
 __license__ = 'AGPL v3'
 __author__ = 'David Völgyes'
 __email__ = 'david.volgyes@ieee.org'
 __doi__ = '10.5281/zenodo.1261812'
```

### Comparing `zenodo_get-1.3.4/zenodo_get/zget.py` & `zenodo_get-1.4.0/zenodo_get/zget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 #!/usr/bin/env python3
-
 import zenodo_get as zget
-
 import requests
-import json
 import hashlib
 import sys
 import os
 from optparse import OptionParser
 import wget
 import time
 import signal
@@ -209,14 +206,24 @@
         '--sandbox',
         action='store_true',
         dest='sandbox',
         help='Use Zenodo Sandbox URL.',
         default=False,
     )
 
+    parser.add_option(
+        '-a',
+        '--access-token',
+        action='store',
+        type=str,
+        dest='access_token',
+        default=None,
+        help='Optional access token for the requests query.',
+    )
+
     (options, args) = parser.parse_args(argv)
 
     if options.cite:
         print('Reference for this software:')
         print(zget.__reference__)
         print()
         print('Bibtex format:')
@@ -273,31 +280,35 @@
         recordID = recordID.strip()
 
         if not options.sandbox:
             url = 'https://zenodo.org/api/records/'
         else:
             url = 'https://sandbox.zenodo.org/api/records/'
 
+        params = {}
+        if options.access_token:
+            params['access_token'] = options.access_token
+
         try:
-            r = requests.get(url + recordID, timeout=options.timeout)
+            r = requests.get(url + recordID, params=params, timeout=options.timeout)
         except requests.exceptions.ConnectTimeout:
             eprint('Connection timeout during metadata reading.')
             if exceptions:
                 raise
             else:
                 sys.exit(1)
         except Exception:
             eprint('Connection error during metadata reading.')
             if exceptions:
                 raise
             else:
                 sys.exit(1)
 
         if r.ok:
-            js = json.loads(r.text)
+            js = r.json()
             files = js['files']
             total_size = sum(f['size'] for f in files)
 
             if options.md5 is not None:
                 with open('md5sums.txt', 'wt') as md5file:
                     for f in files:
                         fname = f['key']
@@ -342,15 +353,15 @@
                     if remote_hash == local_hash and options.cont:
                         eprint(f'{fname} is already downloaded correctly.')
                         continue
 
                     for _ in range(options.retry + 1):
                         try:
                             link = url = unquote(link)
-                            filename = wget.download(link)
+                            filename = wget.download(f"{link}?access_token={options.access_token}")
                         except Exception:
                             eprint(f'  Download error. Original link: {link}')
                             time.sleep(options.pause)
                         else:
                             break
                     else:
                         eprint('  Too many errors.')
```

### Comparing `zenodo_get-1.3.4/zenodo_get.egg-info/PKG-INFO` & `zenodo_get-1.4.0/zenodo_get.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: zenodo-get
-Version: 1.3.4
+Version: 1.4.0
 Summary: Zenodo_get - a downloader for Zenodo records
 Home-page: https://gitlab.com/dvolgyes/zenodo_get
 Author: David Völgyes
 Author-email: david.volgyes@ieee.org
 License: AGPL v3
 Keywords: zenodo download
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 This program is meant to download complete Zenodo records based
 on the Zenodo record ID or the DOI. The primary goal is to ease access
 to large records with dozens of files.
-
-
```

