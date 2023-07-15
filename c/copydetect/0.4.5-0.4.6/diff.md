# Comparing `tmp/copydetect-0.4.5.tar.gz` & `tmp/copydetect-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copydetect-0.4.5.tar", last modified: Wed Apr 26 03:30:22 2023, max compression
+gzip compressed data, was "copydetect-0.4.6.tar", last modified: Sat Jul 15 16:27:56 2023, max compression
```

## Comparing `copydetect-0.4.5.tar` & `copydetect-0.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.280610 copydetect-0.4.5/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     1063 2020-10-17 00:41:54.000000 copydetect-0.4.5/LICENSE
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8631 2023-04-26 03:30:22.280610 copydetect-0.4.5/PKG-INFO
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     7839 2023-04-26 03:15:29.000000 copydetect-0.4.5/README.md
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       90 2023-04-26 03:20:41.000000 copydetect-0.4.5/copydetect/__init__.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     6031 2023-04-26 03:15:29.000000 copydetect-0.4.5/copydetect/__main__.py
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect/data/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     2907 2023-04-26 03:15:29.000000 copydetect-0.4.5/copydetect/data/report.html
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       71 2022-05-29 22:08:04.000000 copydetect-0.4.5/copydetect/defaults.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)    28649 2023-04-26 03:21:43.000000 copydetect-0.4.5/copydetect/detector.py
--rw-r--r--   0 bryson    (1000) bryson    (1000)      928 2022-05-15 19:40:01.000000 copydetect-0.4.5/copydetect/pywinnow.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8342 2022-11-12 00:10:46.000000 copydetect-0.4.5/copydetect/utils.py
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect/winnow/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     3046 2020-10-17 00:41:54.000000 copydetect-0.4.5/copydetect/winnow/winnow.c
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect.egg-info/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8631 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/PKG-INFO
--rw-rw-r--   0 bryson    (1000) bryson    (1000)      543 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/SOURCES.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)        1 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/dependency_links.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       56 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/entry_points.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/requires.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       11 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/top_level.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-04-26 03:30:22.280610 copydetect-0.4.5/setup.cfg
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     1588 2023-04-26 03:29:32.000000 copydetect-0.4.5/setup.py
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/tests/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8689 2023-04-25 02:05:20.000000 copydetect-0.4.5/tests/test_detector.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     2252 2020-10-22 01:47:17.000000 copydetect-0.4.5/tests/test_pywinnowing.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     1069 2022-07-16 17:40:53.000000 copydetect-0.4.5/tests/test_sanity_checks.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8314 2023-03-25 21:00:07.000000 copydetect-0.4.5/tests/test_utils.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     2718 2020-10-22 01:47:17.000000 copydetect-0.4.5/tests/test_winnowing.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-07-15 16:27:56.696900 copydetect-0.4.6/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     1063 2020-10-17 00:41:54.000000 copydetect-0.4.6/LICENSE
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8875 2023-07-15 16:27:56.696900 copydetect-0.4.6/PKG-INFO
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8083 2023-07-09 21:51:37.000000 copydetect-0.4.6/README.md
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-07-15 16:27:56.692900 copydetect-0.4.6/copydetect/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       90 2023-07-09 21:50:48.000000 copydetect-0.4.6/copydetect/__init__.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     6400 2023-07-09 21:51:43.000000 copydetect-0.4.6/copydetect/__main__.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-07-15 16:27:56.696900 copydetect-0.4.6/copydetect/data/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     2907 2023-07-09 21:51:25.000000 copydetect-0.4.6/copydetect/data/report.html
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       71 2022-05-29 22:08:04.000000 copydetect-0.4.6/copydetect/defaults.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)    29982 2023-07-09 21:51:43.000000 copydetect-0.4.6/copydetect/detector.py
+-rw-r--r--   0 bryson    (1000) bryson    (1000)      928 2022-05-15 19:40:01.000000 copydetect-0.4.6/copydetect/pywinnow.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8342 2022-11-12 00:10:46.000000 copydetect-0.4.6/copydetect/utils.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-07-15 16:27:56.696900 copydetect-0.4.6/copydetect/winnow/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     3046 2020-10-17 00:41:54.000000 copydetect-0.4.6/copydetect/winnow/winnow.c
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-07-15 16:27:56.696900 copydetect-0.4.6/copydetect.egg-info/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8875 2023-07-15 16:27:56.000000 copydetect-0.4.6/copydetect.egg-info/PKG-INFO
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)      543 2023-07-15 16:27:56.000000 copydetect-0.4.6/copydetect.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)        1 2023-07-15 16:27:56.000000 copydetect-0.4.6/copydetect.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       56 2023-07-15 16:27:56.000000 copydetect-0.4.6/copydetect.egg-info/entry_points.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-07-15 16:27:56.000000 copydetect-0.4.6/copydetect.egg-info/requires.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       11 2023-07-15 16:27:56.000000 copydetect-0.4.6/copydetect.egg-info/top_level.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-07-15 16:27:56.696900 copydetect-0.4.6/setup.cfg
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     1588 2023-07-15 16:27:24.000000 copydetect-0.4.6/setup.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-07-15 16:27:56.696900 copydetect-0.4.6/tests/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     9136 2023-07-09 21:51:43.000000 copydetect-0.4.6/tests/test_detector.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     2252 2020-10-22 01:47:17.000000 copydetect-0.4.6/tests/test_pywinnowing.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     1069 2022-07-16 17:40:53.000000 copydetect-0.4.6/tests/test_sanity_checks.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8314 2023-03-25 21:00:07.000000 copydetect-0.4.6/tests/test_utils.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     2718 2020-10-22 01:47:17.000000 copydetect-0.4.6/tests/test_winnowing.py
```

### Comparing `copydetect-0.4.5/LICENSE` & `copydetect-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/PKG-INFO` & `copydetect-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copydetect
-Version: 0.4.5
+Version: 0.4.6
 Summary: Code plagiarism detection tool
 Home-page: https://github.com/blingenf/copydetect
 Author: Bryson Lingenfelter
 Author-email: blingenfelter@nevada.unr.edu
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -53,14 +53,15 @@
 - `force_language` (`-o`, `--force-language`): forces the tokenizer to tokenize input as a specific language, rather than automatically detecting the language using the file extension.
 - `same_name_only` (`-s`, `--same-name`): if `true`, the detector will only compare files that have the same name (for example, `decision_tree.py` will not be compared to `k_nn.py`). Note that this also means that, for example, `bryson_k_nn.py` will not be compared to `sara_k_nn.py`.
 - `ignore_leaf` (`-l`, `--ignore-leaf`):  if `true`, the detector will not compare files located in the same leaf directory.
 - `disable_filtering` (`-f`, `--disable-filter`):  if `true`, the detector will not tokenize and filter code before generating file fingerprints.
 - `disable_autoopen` (`-a`, `--disable-autoopen`):  if `true`, the detector will not automatically open a browser window to display the report.
 - `truncate` (`-T`, `--truncate`):  if `true`, highlighted code will be truncated to remove non-highlighted regions from the displayed output (sections not within 10 lines of highlighted code will be replaced with "...").
 - `out_file` (`-O`, `--out-file`): path to save output report to. A '.html' extension will be added to the path if not provided. If a directory is provided instead of a file, the report will be saved to that directory as report.html.
+- `encoding` (`--encoding`): encoding to use for reading files (the default is UTF-8). If files use varying encodings, --encoding DETECT can be used to detect the encoding of all files *(note: encoding detection requires the chardet package)*.
 
 ## API
 Copydetect can also be run via the python API. An example of basic usage is provided below. API documentation is available [here](https://copydetect.readthedocs.io/en/latest/api.html).
 ```
 >>> from copydetect import CopyDetector
 >>> detector = CopyDetector(test_dirs=["tests"], extensions=["py"],
 ...                         display_t=0.5)
```

### Comparing `copydetect-0.4.5/README.md` & `copydetect-0.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 - `force_language` (`-o`, `--force-language`): forces the tokenizer to tokenize input as a specific language, rather than automatically detecting the language using the file extension.
 - `same_name_only` (`-s`, `--same-name`): if `true`, the detector will only compare files that have the same name (for example, `decision_tree.py` will not be compared to `k_nn.py`). Note that this also means that, for example, `bryson_k_nn.py` will not be compared to `sara_k_nn.py`.
 - `ignore_leaf` (`-l`, `--ignore-leaf`):  if `true`, the detector will not compare files located in the same leaf directory.
 - `disable_filtering` (`-f`, `--disable-filter`):  if `true`, the detector will not tokenize and filter code before generating file fingerprints.
 - `disable_autoopen` (`-a`, `--disable-autoopen`):  if `true`, the detector will not automatically open a browser window to display the report.
 - `truncate` (`-T`, `--truncate`):  if `true`, highlighted code will be truncated to remove non-highlighted regions from the displayed output (sections not within 10 lines of highlighted code will be replaced with "...").
 - `out_file` (`-O`, `--out-file`): path to save output report to. A '.html' extension will be added to the path if not provided. If a directory is provided instead of a file, the report will be saved to that directory as report.html.
+- `encoding` (`--encoding`): encoding to use for reading files (the default is UTF-8). If files use varying encodings, --encoding DETECT can be used to detect the encoding of all files *(note: encoding detection requires the chardet package)*.
 
 ## API
 Copydetect can also be run via the python API. An example of basic usage is provided below. API documentation is available [here](https://copydetect.readthedocs.io/en/latest/api.html).
 ```
 >>> from copydetect import CopyDetector
 >>> detector = CopyDetector(test_dirs=["tests"], extensions=["py"],
 ...                         display_t=0.5)
```

### Comparing `copydetect-0.4.5/copydetect/__main__.py` & `copydetect-0.4.6/copydetect/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,19 @@
                         "extension will be added to the path if not provided. "
                         "If a directory is provided instead of a file, the "
                         "report will be saved  to that directory as "
                         "report.html.")
     parser.add_argument('--version', action='version',
                         version="copydetect v" + __version__,
                         help="print version number and exit")
+    parser.add_argument("--encoding", default="utf-8",
+                        help="encoding to use for reading files. If files use "
+                        "varying encodings, --encoding DETECT can be used to "
+                        "detect the encoding of all files (requires the "
+                        "chardet package)")
     args = parser.parse_args()
 
     if args.conf:
         with open(args.conf, encoding="utf-8") as json_fp:
             config = json.load(json_fp)
     elif args.test_dirs:
         if not args.ref_dirs:
@@ -102,14 +107,15 @@
           "force_language" : args.language,
           "same_name_only" : args.same_name,
           "ignore_leaf" : args.ignore_leaf,
           "disable_filtering" : args.filter,
           "disable_autoopen" : args.autoopen,
           "truncate" : args.truncate,
           "out_file" : args.out_file,
+          "encoding": args.encoding,
         }
     else:
         parser.error("either a path to a configuration file (-c) or a "
                      "list of test directories (-t) must be provided.")
 
     # get overlapping code
     detector = CopyDetector.from_config(config)
```

### Comparing `copydetect-0.4.5/copydetect/data/report.html` & `copydetect-0.4.6/copydetect/data/report.html`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/copydetect/detector.py` & `copydetect-0.4.6/copydetect/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     filter : bool, default=True
         If set to to False, code will not be tokenized & filtered.
     fp : TextIO, default=None
         I/O stream for data to create a fingerprint for. If provided,
         the "file" argument will not be used to load a file from disk
         but will still be used for language detection and displayed on
         the report.
+    encoding : str, default="utf-8"
+        Text encoding to use for reading the file. If "DETECT", the
+        chardet library will be used (if installed) to automatically
+        detect file encoding
 
     Attributes
     ----------
     filename : str
         Name of the originally provided file.
     raw_code : str
         Unfiltered code.
@@ -71,19 +75,36 @@
         rather than guessing from the file extension.
     token_coverage : int
         The number of tokens in the tokenized code which are considered
         for fingerprint comparison, after dropping duplicate k-grams and
         performing winnowing.
     """
     def __init__(self, file, k, win_size, boilerplate=[], filter=True,
-                 language=None, fp=None):
+                 language=None, fp=None, encoding: str = "utf-8"):
         if fp is not None:
             code = fp.read()
+        elif encoding == "DETECT":
+            try:
+                import chardet
+                with open(file, "rb") as code_fp:
+                    code = code_fp.read()
+                detected_encoding = chardet.detect(code)["encoding"]
+                if detected_encoding is not None:
+                    code = code.decode(detected_encoding)
+                else:
+                    # if encoding can't be detected, just use the default
+                    # encoding (the file may be empty)
+                    code = code.decode()
+            except ModuleNotFoundError as e:
+                logging.error(
+                    "encoding detection requires chardet to be installed"
+                )
+                raise e
         else:
-            with open(file, encoding="utf-8") as code_fp:
+            with open(file, encoding=encoding) as code_fp:
                 code = code_fp.read()
         if filter:
             filtered_code, offsets = filter_code(code, file, language)
         else:
             filtered_code, offsets = code, np.array([])
         hashes, idx = get_document_fingerprints(filtered_code, k, win_size,
                                                 boilerplate)
@@ -219,23 +240,28 @@
     truncate : bool
         If true, highlighted code will be truncated to remove non-
         highlighted regions from the displayed output
     out_file : str
         Path to output report file.
     silent : bool
         If true, all logging output will be supressed.
+    encoding : str, default="utf-8"
+        Text encoding to use for reading the file. If "DETECT", the
+        chardet library will be used (if installed) to automatically
+        detect file encoding
     """
     def __init__(self, config=None, test_dirs=[], ref_dirs=[],
                  boilerplate_dirs=[], extensions=["*"],
                  noise_t=defaults.NOISE_THRESHOLD,
                  guarantee_t=defaults.GUARANTEE_THRESHOLD,
                  display_t=defaults.DISPLAY_THRESHOLD,
                  same_name_only=False, ignore_leaf=False, autoopen=True,
                  disable_filtering=False, force_language=None,
-                 truncate=False, out_file="./report.html", silent=False):
+                 truncate=False, out_file="./report.html", silent=False,
+                 encoding: str = "utf-8"):
         if config is not None:
             # temporary workaround to ensure existing code continues
             # to work
             warnings.warn(
                 "use CopyDetector.from_config to initialize CopyDetector from "
                 "a config file. The config parameter is deprecated and will be"
                 " removed in a future version.",
@@ -261,14 +287,15 @@
         self.same_name_only = same_name_only
         self.ignore_leaf = ignore_leaf
         self.autoopen = autoopen
         self.disable_filtering = disable_filtering
         self.force_language = force_language
         self.truncate = truncate
         self.out_file = out_file
+        self.encoding = encoding
 
         self._check_arguments()
 
         out_path = Path(self.out_file)
         if out_path.is_dir():
             self.out_file += "/report.html"
         elif out_path.suffix != ".html":
@@ -454,18 +481,19 @@
         found in the boilerplate directories.
         """
         boilerplate_hashes = []
         for file in self.boilerplate_files:
             try:
                 fingerprint=CodeFingerprint(file, self.noise_t, 1,
                                             filter=not self.disable_filtering,
-                                            language=self.force_language)
+                                            language=self.force_language,
+                                            encoding=self.encoding)
                 boilerplate_hashes.extend(fingerprint.hashes)
             except UnicodeDecodeError:
-                logging.warning(f"Skipping {file}: file not ASCII text")
+                logging.warning(f"Skipping {file}: file not UTF-8 text")
                 continue
 
         return np.unique(np.array(boilerplate_hashes))
 
     def _preprocess_code(self, file_list):
         """Generates a CodeFingerprint object for each file in the
         provided file list. This is where the winnowing algorithm is
@@ -475,18 +503,18 @@
         for code_f in tqdm(file_list, bar_format= '   {l_bar}{bar}{r_bar}',
                            disable=self.silent):
             if code_f not in self.file_data:
                 try:
                     self.file_data[code_f] = CodeFingerprint(
                         code_f, self.noise_t, self.window_size,
                         boilerplate_hashes, not self.disable_filtering,
-                        self.force_language)
+                        self.force_language, encoding=self.encoding)
 
                 except UnicodeDecodeError:
-                    logging.warning(f"Skipping {code_f}: file not ASCII text")
+                    logging.warning(f"Skipping {code_f}: file not UTF-8 text")
                     continue
 
     def _comparison_loop(self):
         """The core code used to determine code overlap. The overlap
         between each test file and each compare file is computed and
         stored in similarity_matrix. Token overlap information and the
         locations of copied code are stored in slice_matrix and
```

### Comparing `copydetect-0.4.5/copydetect/pywinnow.py` & `copydetect-0.4.6/copydetect/pywinnow.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/copydetect/utils.py` & `copydetect-0.4.6/copydetect/utils.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/copydetect/winnow/winnow.c` & `copydetect-0.4.6/copydetect/winnow/winnow.c`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/copydetect.egg-info/PKG-INFO` & `copydetect-0.4.6/copydetect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copydetect
-Version: 0.4.5
+Version: 0.4.6
 Summary: Code plagiarism detection tool
 Home-page: https://github.com/blingenf/copydetect
 Author: Bryson Lingenfelter
 Author-email: blingenfelter@nevada.unr.edu
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -53,14 +53,15 @@
 - `force_language` (`-o`, `--force-language`): forces the tokenizer to tokenize input as a specific language, rather than automatically detecting the language using the file extension.
 - `same_name_only` (`-s`, `--same-name`): if `true`, the detector will only compare files that have the same name (for example, `decision_tree.py` will not be compared to `k_nn.py`). Note that this also means that, for example, `bryson_k_nn.py` will not be compared to `sara_k_nn.py`.
 - `ignore_leaf` (`-l`, `--ignore-leaf`):  if `true`, the detector will not compare files located in the same leaf directory.
 - `disable_filtering` (`-f`, `--disable-filter`):  if `true`, the detector will not tokenize and filter code before generating file fingerprints.
 - `disable_autoopen` (`-a`, `--disable-autoopen`):  if `true`, the detector will not automatically open a browser window to display the report.
 - `truncate` (`-T`, `--truncate`):  if `true`, highlighted code will be truncated to remove non-highlighted regions from the displayed output (sections not within 10 lines of highlighted code will be replaced with "...").
 - `out_file` (`-O`, `--out-file`): path to save output report to. A '.html' extension will be added to the path if not provided. If a directory is provided instead of a file, the report will be saved to that directory as report.html.
+- `encoding` (`--encoding`): encoding to use for reading files (the default is UTF-8). If files use varying encodings, --encoding DETECT can be used to detect the encoding of all files *(note: encoding detection requires the chardet package)*.
 
 ## API
 Copydetect can also be run via the python API. An example of basic usage is provided below. API documentation is available [here](https://copydetect.readthedocs.io/en/latest/api.html).
 ```
 >>> from copydetect import CopyDetector
 >>> detector = CopyDetector(test_dirs=["tests"], extensions=["py"],
 ...                         display_t=0.5)
```

### Comparing `copydetect-0.4.5/copydetect.egg-info/SOURCES.txt` & `copydetect-0.4.6/copydetect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/setup.py` & `copydetect-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # the C extension is not currently built for versions uploaded to PyPI.
 # Speedup is not meaningful and it makes cross-platform support quite
 # a bit more painful
 
 setup(name="copydetect",
       author="Bryson Lingenfelter",
       author_email="blingenfelter@nevada.unr.edu",
-      version="0.4.5",
+      version="0.4.6",
       description="Code plagiarism detection tool",
       long_description=readme,
       long_description_content_type="text/markdown",
       url="https://github.com/blingenf/copydetect",
       packages=["copydetect"],
       #ext_modules=[Extension("copydetect.winnow",
       #                       sources=["copydetect/winnow/winnow.c"],
```

### Comparing `copydetect-0.4.5/tests/test_detector.py` & `copydetect-0.4.6/tests/test_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,7 +207,17 @@
 
         detector = CopyDetector(test_dirs=[TESTS_DIR + "/sample_py"],
             silent=True, out_file=tmpdir, autoopen=False)
         detector.run()
         detector.generate_html_report()
 
         assert Path(tmpdir + "/report.html").exists()
+
+    def test_encoding_specification(self):
+        detector = CopyDetector(test_dirs=[TESTS_DIR + "/sample_py"],
+                                extensions=["c"], encoding="utf-16",
+                                silent=True)
+        detector.add_file(TESTS_DIR + "/sample_other/c_sample_utf16.c")
+        detector.run()
+
+        # make sure utf-16 file was loaded correctly
+        assert len(list(detector.file_data.values())[0].raw_code) > 0
```

### Comparing `copydetect-0.4.5/tests/test_pywinnowing.py` & `copydetect-0.4.6/tests/test_pywinnowing.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/tests/test_sanity_checks.py` & `copydetect-0.4.6/tests/test_sanity_checks.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/tests/test_utils.py` & `copydetect-0.4.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.5/tests/test_winnowing.py` & `copydetect-0.4.6/tests/test_winnowing.py`

 * *Files identical despite different names*

