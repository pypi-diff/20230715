# Comparing `tmp/readthis-0.0.9.tar.gz` & `tmp/readthis-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthis-0.0.9.tar", last modified: Sun Jun 18 16:28:47 2023, max compression
+gzip compressed data, was "readthis-0.1.0.tar", last modified: Sat Jul 15 14:44:05 2023, max compression
```

## Comparing `readthis-0.0.9.tar` & `readthis-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-18 16:28:33.000000 readthis-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 16:28:33.000000 readthis-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 16:28:47.885828 readthis-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-18 16:28:33.000000 readthis-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/readthis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 16:28:47.000000 readthis-0.0.9/readthis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:28:47.885828 readthis-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 16:28:33.000000 readthis-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.881828 readthis-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/src/readthis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:33.000000 readthis-0.0.9/src/readthis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:28:47.885828 readthis-0.0.9/src/readthis/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-18 16:28:33.000000 readthis-0.0.9/src/readthis/data/default_text.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-06-18 16:28:33.000000 readthis-0.0.9/src/readthis/readthis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:44:05.098462 readthis-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-15 14:43:53.000000 readthis-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 14:43:53.000000 readthis-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-15 14:44:05.098462 readthis-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-15 14:43:53.000000 readthis-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:44:05.094462 readthis-0.1.0/readthis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-15 14:44:05.000000 readthis-0.1.0/readthis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-15 14:44:05.000000 readthis-0.1.0/readthis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:44:05.000000 readthis-0.1.0/readthis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 14:44:05.000000 readthis-0.1.0/readthis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 14:44:05.000000 readthis-0.1.0/readthis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 14:44:05.000000 readthis-0.1.0/readthis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:44:05.098462 readthis-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-15 14:43:53.000000 readthis-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:44:05.094462 readthis-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:44:05.098462 readthis-0.1.0/src/readthis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:43:53.000000 readthis-0.1.0/src/readthis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:44:05.098462 readthis-0.1.0/src/readthis/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-15 14:43:53.000000 readthis-0.1.0/src/readthis/data/default_text.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-07-15 14:43:53.000000 readthis-0.1.0/src/readthis/readthis.py
```

### Comparing `readthis-0.0.9/LICENSE` & `readthis-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readthis-0.0.9/PKG-INFO` & `readthis-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.9
+Version: 0.1.0
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,14 +23,15 @@
 
 - `FILE`: The file to read aloud. Use - to read from stdin.
 
 ### Options
 
 - `-h, --help`: Show the help message and exit.
 - `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., fr for French). Defaults to English.
+- `--url, -u`: fetch an URL instead of a file
 
 ## Installation
 
 ```bash
 $ pip install readthis
 ```
 
@@ -40,14 +41,19 @@
 
 ```bash
 $ readthis --lang en sample.txt
 ```
 
 - Read from stdin in French:
 ```bash
-$ echo "Bonjour, comment ça va ?" | readthis -l fr -
+$ echo "Bonjour, comment ça va ?" | readthis -l fr
+```
+
+- Fetch and read an article:
+```bash
+$ readthis -u https://example.com
 ```
 
 ## License
 
 This project is licensed under the [MIT License](./LICENCE).
```

### Comparing `readthis-0.0.9/README.md` & `readthis-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 - `FILE`: The file to read aloud. Use - to read from stdin.
 
 ### Options
 
 - `-h, --help`: Show the help message and exit.
 - `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., fr for French). Defaults to English.
+- `--url, -u`: fetch an URL instead of a file
 
 ## Installation
 
 ```bash
 $ pip install readthis
 ```
 
@@ -29,14 +30,19 @@
 
 ```bash
 $ readthis --lang en sample.txt
 ```
 
 - Read from stdin in French:
 ```bash
-$ echo "Bonjour, comment ça va ?" | readthis -l fr -
+$ echo "Bonjour, comment ça va ?" | readthis -l fr
+```
+
+- Fetch and read an article:
+```bash
+$ readthis -u https://example.com
 ```
 
 ## License
 
 This project is licensed under the [MIT License](./LICENCE).
```

### Comparing `readthis-0.0.9/readthis.egg-info/PKG-INFO` & `readthis-0.1.0/readthis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthis
-Version: 0.0.9
+Version: 0.1.0
 Summary: readthis - A command line tool to read a text file aloud
 Home-page: https://github.com/entropyqueen/readthis
 Author: Emy Canton
 Author-email: emy.canton@proton.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,14 +23,15 @@
 
 - `FILE`: The file to read aloud. Use - to read from stdin.
 
 ### Options
 
 - `-h, --help`: Show the help message and exit.
 - `--lang LANG, -l LANG`: Choose the language to use for reading. Specify the language using the language code (e.g., fr for French). Defaults to English.
+- `--url, -u`: fetch an URL instead of a file
 
 ## Installation
 
 ```bash
 $ pip install readthis
 ```
 
@@ -40,14 +41,19 @@
 
 ```bash
 $ readthis --lang en sample.txt
 ```
 
 - Read from stdin in French:
 ```bash
-$ echo "Bonjour, comment ça va ?" | readthis -l fr -
+$ echo "Bonjour, comment ça va ?" | readthis -l fr
+```
+
+- Fetch and read an article:
+```bash
+$ readthis -u https://example.com
 ```
 
 ## License
 
 This project is licensed under the [MIT License](./LICENCE).
```

### Comparing `readthis-0.0.9/setup.py` & `readthis-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='readthis',
-    version='0.0.9',
+    version='0.1.0',
     description='readthis - A command line tool to read a text file aloud',
     author='Emy Canton',
     author_email='emy.canton@proton.me',
     url='https://github.com/entropyqueen/readthis',
     license='MIT',
     setup_requires=[
         'setuptools',
```

### Comparing `readthis-0.0.9/src/readthis/data/default_text.txt` & `readthis-0.1.0/src/readthis/data/default_text.txt`

 * *Files identical despite different names*

### Comparing `readthis-0.0.9/src/readthis/readthis.py` & `readthis-0.1.0/src/readthis/readthis.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from io import BytesIO
 from pydub import AudioSegment
 from pydub.playback import play as pydub_play
 import argparse
 import sys, os
 import concurrent.futures
 import pkg_resources
+import validators
+import trafilatura
 
 
 DATA_PATH = pkg_resources.resource_filename('readthis', 'data/')
 
 MAX_GTTS_INPUT = 300 # Max bytes (found 5000 online)
 MAX_GTTS_RQTS = 1000 # Max requests *per minutes* (found 1000 online)
 
@@ -26,15 +28,19 @@
     mp3_fp = BytesIO()
     tts.write_to_fp(mp3_fp)
     mp3_fp.seek(0)
     return mp3_fp
 
 def read_text(fragments, lang):
 
-    mp3_fp = get_audio(fragments[0], lang)
+    try:
+        mp3_fp = get_audio(fragments[0], lang)
+    except AssertionError:
+        print("No text to read.")
+        return
     if len(fragments) == 1:
         play_audio(mp3_fp)
 
     for i in range(1, min(MAX_GTTS_RQTS, len(fragments))):
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
             executor.submit(play_audio, mp3_fp)
@@ -63,26 +69,38 @@
 
     parser = argparse.ArgumentParser(description='reads a text using google API')
     parser.add_argument(
         '--lang', '-l', metavar='LANG', default='en',
         help='Choose language to use for reading.'
     )
     parser.add_argument(
+        '--url', '-u', default=False, action='store_true',
+        help='Treat file as URL for downloading'
+    )
+    parser.add_argument(
         'text', metavar='FILE', nargs='?', default=default_text,
         help='File to read, or - for stdin'
     )
     args = parser.parse_args()
 
     text = ''
-    # Get input from file or stdin
-    if args.text == '-':
+    # Get input from file or stdin and remove easter egg
+    if (args.text == '-' or args.text == default_text) and not args.url:
         text = sys.stdin.read()
     else:
-        with open(args.text) as f:
-            text = f.read()
+        if args.url:
+            if validators.url(args.text):
+                dl_text = trafilatura.fetch_url(args.text)
+                text = trafilatura.extract(dl_text)
+            else:
+                print("Please provide a url when using --url or -u")
+                return
+        else:
+            with open(args.text) as f:
+                text = f.read()
 
     fragments = handle_limits(text)
     read_text(fragments, args.lang)
 
 
 if __name__ == '__main__':
     main()
```

