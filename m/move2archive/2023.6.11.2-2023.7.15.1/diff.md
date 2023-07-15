# Comparing `tmp/move2archive-2023.6.11.2-py3-none-any.whl.zip` & `tmp/move2archive-2023.7.15.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10008 bytes, number of entries: 6
--rw-r--r--  2.0 unx    26388 b- defN 23-Jun-11 12:09 move2archive/__init__.py
--rw-r--r--  2.0 unx     2041 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       75 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      530 b- defN 23-Jun-11 12:10 move2archive-2023.6.11.2.dist-info/RECORD
-6 files, 29139 bytes uncompressed, 9036 bytes compressed:  69.0%
+Zip file size: 10100 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26696 b- defN 23-Jul-15 16:44 move2archive/__init__.py
+-rw-r--r--  2.0 unx     2041 b- defN 23-Jul-15 16:45 move2archive-2023.7.15.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 16:45 move2archive-2023.7.15.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       75 b- defN 23-Jul-15 16:45 move2archive-2023.7.15.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-15 16:45 move2archive-2023.7.15.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-Jul-15 16:45 move2archive-2023.7.15.1.dist-info/RECORD
+6 files, 29447 bytes uncompressed, 9128 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: move2archive/__init__.py
 Comment: 
 
-Filename: move2archive-2023.6.11.2.dist-info/METADATA
+Filename: move2archive-2023.7.15.1.dist-info/METADATA
 Comment: 
 
-Filename: move2archive-2023.6.11.2.dist-info/WHEEL
+Filename: move2archive-2023.7.15.1.dist-info/WHEEL
 Comment: 
 
-Filename: move2archive-2023.6.11.2.dist-info/entry_points.txt
+Filename: move2archive-2023.7.15.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: move2archive-2023.6.11.2.dist-info/top_level.txt
+Filename: move2archive-2023.7.15.1.dist-info/top_level.txt
 Comment: 
 
-Filename: move2archive-2023.6.11.2.dist-info/RECORD
+Filename: move2archive-2023.7.15.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## move2archive/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-PROG_VERSION = u"Time-stamp: <2023-06-11 14:09:43 vk>"
+PROG_VERSION = u"Time-stamp: <2023-07-15 18:44:41 vk>"
 
 import os
 import sys
 import re
 import logging
 from optparse import OptionParser
 from datetime import datetime
@@ -458,16 +458,18 @@
 
     # omit path and filename extensions:
     file1 = os.path.basename(os.path.splitext(filename1)[0])
     file2 = os.path.basename(os.path.splitext(filename2)[0])
     
     if startswith_datestamp(file1) and startswith_datestamp(file2):
         # cut most probably identical datestamp to avoid false positive matchstring:
-        substring = longestSubstringFinder(file1[10:], file2[10:])
+        logging.debug('guess_new_directory_basename: finding longest common prefix after omitting time- or datestamps (remove anything before first space or underliner)')
+        substring = longestSubstringFinder(re.sub(r'.*?[ _](.*)', r'\1', file1), re.sub(r'.*?[ _](.*)', r'\1', file2))
     else:
+        logging.debug('guess_new_directory_basename: finding longest common prefix')
         substring = longestSubstringFinder(file1, file2)
 
     if substring:
         # delete any pre- or postfixes with a dash and space:
         strippedsubstring = substring.replace(' -', '').replace('- ', '').strip()
         if len(strippedsubstring) > 3:
             # FIXXME assumption: a potential substring candidate for a directory name needs at least 4 characters.
```

## Comparing `move2archive-2023.6.11.2.dist-info/METADATA` & `move2archive-2023.7.15.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: move2archive
-Version: 2023.6.11.2
+Version: 2023.7.15.1
 Summary: Managing event-related files in a folder hierarchy like <ARCHIVE>/2013/2013-05-17 Event name/
 Home-page: https://github.com/novoid/move2archive
 Download-URL: https://github.com/novoid/move2archive/zipball/master
 Author: Karl Voit
 Author-email: tools@Karl-Voit.at
 Keywords: file managing,file management,files,date,time,time-stamps
 Classifier: Programming Language :: Python :: 3 :: Only
```

## Comparing `move2archive-2023.6.11.2.dist-info/RECORD` & `move2archive-2023.7.15.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-move2archive/__init__.py,sha256=cERCcfIjq21v_ZG6FKljZgdB65oZAv4lna_UYeYI82A,26388
-move2archive-2023.6.11.2.dist-info/METADATA,sha256=DOv6pyRMgZgLYb--JubKRFBlMBPQdd1ms1d197i7Kq8,2041
-move2archive-2023.6.11.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-move2archive-2023.6.11.2.dist-info/entry_points.txt,sha256=9rwbiqLkMf-N8FGi4YdKaSorRf2nY5h41xuMfznxQPw,75
-move2archive-2023.6.11.2.dist-info/top_level.txt,sha256=_BlnGMLPt0wrUk9v3Qis-6_2nOVYRaxIJkY_JfkJZZU,13
-move2archive-2023.6.11.2.dist-info/RECORD,,
+move2archive/__init__.py,sha256=IWBk8SPKxB4uFXf7mNFfPAo6pUlTvN9vqEQPldC6k74,26696
+move2archive-2023.7.15.1.dist-info/METADATA,sha256=KvMZB80vk1D-AEJXSS93espVf218zpYOwMtNMK0jteA,2041
+move2archive-2023.7.15.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+move2archive-2023.7.15.1.dist-info/entry_points.txt,sha256=9rwbiqLkMf-N8FGi4YdKaSorRf2nY5h41xuMfznxQPw,75
+move2archive-2023.7.15.1.dist-info/top_level.txt,sha256=_BlnGMLPt0wrUk9v3Qis-6_2nOVYRaxIJkY_JfkJZZU,13
+move2archive-2023.7.15.1.dist-info/RECORD,,
```

