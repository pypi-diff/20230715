# Comparing `tmp/stream-write-ods-0.0.8.tar.gz` & `tmp/stream-write-ods-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream-write-ods-0.0.8.tar", last modified: Fri Dec 31 08:05:34 2021, max compression
+gzip compressed data, was "stream-write-ods-0.0.9.tar", last modified: Fri Dec 31 12:44:32 2021, max compression
```

## Comparing `stream-write-ods-0.0.8.tar` & `stream-write-ods-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-31 08:05:34.609467 stream-write-ods-0.0.8/
--rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-12-30 06:50:46.000000 stream-write-ods-0.0.8/LICENSE
--rw-r--r--   0 dituser    (501) staff       (20)     6712 2021-12-31 08:05:34.608816 stream-write-ods-0.0.8/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)     6107 2021-12-31 07:59:44.000000 stream-write-ods-0.0.8/README.md
--rw-r--r--   0 dituser    (501) staff       (20)       38 2021-12-31 08:05:34.609557 stream-write-ods-0.0.8/setup.cfg
--rw-r--r--   0 dituser    (501) staff       (20)      883 2021-12-31 08:04:43.000000 stream-write-ods-0.0.8/setup.py
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-31 08:05:34.608356 stream-write-ods-0.0.8/stream_write_ods.egg-info/
--rw-r--r--   0 dituser    (501) staff       (20)     6712 2021-12-31 08:05:34.000000 stream-write-ods-0.0.8/stream_write_ods.egg-info/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)      245 2021-12-31 08:05:34.000000 stream-write-ods-0.0.8/stream_write_ods.egg-info/SOURCES.txt
--rw-r--r--   0 dituser    (501) staff       (20)        1 2021-12-31 08:05:34.000000 stream-write-ods-0.0.8/stream_write_ods.egg-info/dependency_links.txt
--rw-r--r--   0 dituser    (501) staff       (20)       19 2021-12-31 08:05:34.000000 stream-write-ods-0.0.8/stream_write_ods.egg-info/requires.txt
--rw-r--r--   0 dituser    (501) staff       (20)       17 2021-12-31 08:05:34.000000 stream-write-ods-0.0.8/stream_write_ods.egg-info/top_level.txt
--rw-r--r--   0 dituser    (501) staff       (20)     3807 2021-12-30 22:42:10.000000 stream-write-ods-0.0.8/stream_write_ods.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-31 12:44:32.848025 stream-write-ods-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-12-30 06:50:46.000000 stream-write-ods-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     6760 2021-12-31 12:44:32.847293 stream-write-ods-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     6155 2021-12-31 12:36:14.000000 stream-write-ods-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-12-31 12:44:32.848139 stream-write-ods-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      883 2021-12-31 12:44:08.000000 stream-write-ods-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-31 12:44:32.846785 stream-write-ods-0.0.9/stream_write_ods.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     6760 2021-12-31 12:44:32.000000 stream-write-ods-0.0.9/stream_write_ods.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      245 2021-12-31 12:44:32.000000 stream-write-ods-0.0.9/stream_write_ods.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-12-31 12:44:32.000000 stream-write-ods-0.0.9/stream_write_ods.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       19 2021-12-31 12:44:32.000000 stream-write-ods-0.0.9/stream_write_ods.egg-info/requires.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       17 2021-12-31 12:44:32.000000 stream-write-ods-0.0.9/stream_write_ods.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)     3986 2021-12-31 12:39:00.000000 stream-write-ods-0.0.9/stream_write_ods.py
```

### Comparing `stream-write-ods-0.0.8/LICENSE` & `stream-write-ods-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stream-write-ods-0.0.8/PKG-INFO` & `stream-write-ods-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-write-ods
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python function to construct an ODS spreadsheet on the fly - without having to store the entire file in memory or disk
 Home-page: https://github.com/uktrade/stream-write-ods
 Author: Department for International Trade
 Author-email: sre@digital.trade.gov.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -191,14 +191,15 @@
 |:------------|:------------------------------|
 | boolean     | boolean                       |
 | date        | date - without time component |
 | datetime    | date - with time component    |
 | int         | float                         |
 | float       | float                         |
 | str         | string                        |
+| bytes       | string - base64 encoded       |
 | NoneType    | string - as #NA               |
 
 
 ## Limitations
 
 ODS spreadsheets are essentially ZIP archives containing several member files. While in general ZIP archives can be up to 16EiB (exbibyte) in size using [ZIP64](https://en.wikipedia.org/wiki/ZIP_(file_format)#ZIP64), [LibreOffice does not support ZIP64](https://bugs.documentfoundation.org/show_bug.cgi?id=128244), and so ODS files are de-facto limited to 4GiB (gibibyte). This limit applies to the size of the entire compressed archive, the compressed size of each member file, and the uncompressed size of each member file.
```

### Comparing `stream-write-ods-0.0.8/README.md` & `stream-write-ods-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -175,13 +175,14 @@
 |:------------|:------------------------------|
 | boolean     | boolean                       |
 | date        | date - without time component |
 | datetime    | date - with time component    |
 | int         | float                         |
 | float       | float                         |
 | str         | string                        |
+| bytes       | string - base64 encoded       |
 | NoneType    | string - as #NA               |
 
 
 ## Limitations
 
 ODS spreadsheets are essentially ZIP archives containing several member files. While in general ZIP archives can be up to 16EiB (exbibyte) in size using [ZIP64](https://en.wikipedia.org/wiki/ZIP_(file_format)#ZIP64), [LibreOffice does not support ZIP64](https://bugs.documentfoundation.org/show_bug.cgi?id=128244), and so ODS files are de-facto limited to 4GiB (gibibyte). This limit applies to the size of the entire compressed archive, the compressed size of each member file, and the uncompressed size of each member file.
```

### Comparing `stream-write-ods-0.0.8/setup.py` & `stream-write-ods-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 setuptools.setup(
     name='stream-write-ods',
-    version='0.0.8',
+    version='0.0.9',
     author='Department for International Trade',
     author_email='sre@digital.trade.gov.uk',
     description='Python function to construct an ODS spreadsheet on the fly - without having to store the entire file in memory or disk',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/uktrade/stream-write-ods',
     classifiers=[
```

### Comparing `stream-write-ods-0.0.8/stream_write_ods.egg-info/PKG-INFO` & `stream-write-ods-0.0.9/stream_write_ods.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-write-ods
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python function to construct an ODS spreadsheet on the fly - without having to store the entire file in memory or disk
 Home-page: https://github.com/uktrade/stream-write-ods
 Author: Department for International Trade
 Author-email: sre@digital.trade.gov.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -191,14 +191,15 @@
 |:------------|:------------------------------|
 | boolean     | boolean                       |
 | date        | date - without time component |
 | datetime    | date - with time component    |
 | int         | float                         |
 | float       | float                         |
 | str         | string                        |
+| bytes       | string - base64 encoded       |
 | NoneType    | string - as #NA               |
 
 
 ## Limitations
 
 ODS spreadsheets are essentially ZIP archives containing several member files. While in general ZIP archives can be up to 16EiB (exbibyte) in size using [ZIP64](https://en.wikipedia.org/wiki/ZIP_(file_format)#ZIP64), [LibreOffice does not support ZIP64](https://bugs.documentfoundation.org/show_bug.cgi?id=128244), and so ODS files are de-facto limited to 4GiB (gibibyte). This limit applies to the size of the entire compressed archive, the compressed size of each member file, and the uncompressed size of each member file.
```

### Comparing `stream-write-ods-0.0.8/stream_write_ods.py` & `stream-write-ods-0.0.9/stream_write_ods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from base64 import b64encode
 from codecs import iterencode
 from datetime import datetime, date
 from xml.sax.saxutils import escape, quoteattr
 
 from stream_zip import ZIP, NO_COMPRESSION, stream_zip
 
 
@@ -13,14 +14,15 @@
         to_cell = {
             type(False): lambda v: f'<table:table-cell office:value-type="boolean" office:boolean-value={quoteattr(str(v).lower())}><text:p>{escape(str(v).lower())}</text:p></table:table-cell>',
             type(date(1970, 1, 1)): lambda v: f'<table:table-cell office:value-type="date" office:date-value={quoteattr(v.isoformat())}><text:p>{escape(quoteattr(v.isoformat()))}</text:p></table:table-cell>',
             type(datetime(1970, 1, 1, 0, 0)): lambda v: f'<table:table-cell office:value-type="date" office:date-value={quoteattr(v.isoformat())}><text:p>{escape(quoteattr(v.isoformat()))}</text:p></table:table-cell>',
             type(0): lambda v: f'<table:table-cell office:value-type="float" office:value={quoteattr(str(v))}><text:p>{escape(str(v))}</text:p></table:table-cell>',
             type(0.0): lambda v: f'<table:table-cell office:value-type="float" office:value={quoteattr(str(v))}><text:p>{escape(str(v))}</text:p></table:table-cell>',
             type(''): lambda v: f'<table:table-cell office:value-type="string"><text:p>{escape(v)}</text:p></table:table-cell>',
+            type(b''): lambda v: f'<table:table-cell office:value-type="string"><text:p>{escape(b64encode(v).decode())}</text:p></table:table-cell>',
             type(None): lambda v: f'<table:table-cell office:value-type="string"><text:p>#N/A</text:p></table:table-cell>',
         }
 
         # To validate, mimetype must be first
         yield 'mimetype', modified_at, perms, NO_COMPRESSION, (
             b'application/vnd.oasis.opendocument.spreadsheet',
         )
```

