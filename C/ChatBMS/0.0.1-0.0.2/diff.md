# Comparing `tmp/chatbms-0.0.1.tar.gz` & `tmp/chatbms-0.0.2.tar.gz`

## Comparing `chatbms-0.0.1.tar` & `chatbms-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 chatbms-0.0.1/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 chatbms-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatbms-0.0.1/src/example_package_chirux/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chatbms-0.0.1/src/example_package_chirux/example.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chatbms-0.0.1/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 chatbms-0.0.1/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 chatbms-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chatbms-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 chatbms-0.0.2/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 chatbms-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatbms-0.0.2/src/ChatBMS/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chatbms-0.0.2/src/ChatBMS/chat_completions.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chatbms-0.0.2/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 chatbms-0.0.2/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 chatbms-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chatbms-0.0.2/PKG-INFO
```

### Comparing `chatbms-0.0.1/.DS_Store` & `chatbms-0.0.2/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0007  ................
-00000050: 0000 0001 0000 1000 496c 6f63 626c 6f62  ........Ilocblob
-00000060: 0000 0010 0000 0000 0000 0000 0000 0000  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0005  ................
+00000050: 0000 0001 0000 1000 004e 0053 0045 496c  .........N.S.EIl
+00000060: 6f63 626c 0000 0000 0000 0000 0000 0000  ocbl............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,44 +26,44 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0007 0000 0004  ................
-00000210: 0064 0069 0073 0074 496c 6f63 626c 6f62  .d.i.s.tIlocblob
-00000220: 0000 0010 0000 0041 0000 002e ffff ffff  .......A........
-00000230: ffff 0000 0000 0007 004c 0049 0043 0045  .........L.I.C.E
-00000240: 004e 0053 0045 496c 6f63 626c 6f62 0000  .N.S.EIlocblob..
-00000250: 0010 0000 00af 0000 002e ffff ffff ffff  ................
-00000260: 0000 0000 000e 0070 0079 0070 0072 006f  .......p.y.p.r.o
-00000270: 006a 0065 0063 0074 002e 0074 006f 006d  .j.e.c.t...t.o.m
-00000280: 006c 496c 6f63 626c 6f62 0000 0010 0000  .lIlocblob......
-00000290: 011d 0000 002e ffff ffff ffff 0000 0000  ................
-000002a0: 0009 0052 0045 0041 0044 004d 0045 002e  ...R.E.A.D.M.E..
-000002b0: 006d 0064 496c 6f63 626c 6f62 0000 0010  .m.dIlocblob....
-000002c0: 0000 018b 0000 002e ffff ffff ffff 0000  ................
-000002d0: 0000 0003 0073 0072 0063 496c 6f63 626c  .....s.r.cIlocbl
-000002e0: 6f62 0000 0010 0000 01f9 0000 002e ffff  ob..............
-000002f0: ffff ffff 0000 0000 0003 0073 0072 0063  ...........s.r.c
-00000300: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
-00000310: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
-00000320: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00000330: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00000340: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00000350: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00000360: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00000370: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
-00000380: 3236 302c 2033 3433 7d2c 207b 3932 302c  260, 343}, {920,
-00000390: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
-000003a0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
-000003b0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
-000003c0: 0000 008b 0000 0003 0073 0072 0063 7653  .........s.r.cvS
-000003d0: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
+00000200: 0000 0000 0000 0000 0000 0005 0000 0007  ................
+00000210: 004c 0049 0043 0045 004e 0053 0045 496c  .L.I.C.E.N.S.EIl
+00000220: 6f63 626c 6f62 0000 0010 0000 00af 0000  ocblob..........
+00000230: 002e ffff ffff ffff 0000 0000 0009 0052  ...............R
+00000240: 0045 0041 0044 004d 0045 002e 006d 0064  .E.A.D.M.E...m.d
+00000250: 496c 6f63 626c 6f62 0000 0010 0000 018b  Ilocblob........
+00000260: 0000 002e ffff ffff ffff 0000 0000 0003  ................
+00000270: 0073 0072 0063 496c 6f63 626c 6f62 0000  .s.r.cIlocblob..
+00000280: 0010 0000 01f9 0000 002e ffff ffff ffff  ................
+00000290: 0000 0000 0003 0073 0072 0063 6277 7370  .......s.r.cbwsp
+000002a0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+000002b0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+000002c0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+000002d0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+000002e0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+000002f0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00000300: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00000310: 6261 7208 0908 095f 1018 7b7b 3236 302c  bar...._..{{260,
+00000320: 2033 3433 7d2c 207b 3932 302c 2034 3336   343}, {920, 436
+00000330: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00000340: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00000350: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00000360: 0000 0003 0073 0072 0063 7653 726e 6c6f  .....s.r.cvSrnlo
+00000370: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
+00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `chatbms-0.0.1/src/.DS_Store` & `chatbms-0.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `chatbms-0.0.1/LICENSE` & `chatbms-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatbms-0.0.1/pyproject.toml` & `chatbms-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ChatBMS"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Chirag Manjeshwar", email="chirunder@gmail.com" },
 ]
-description = "Wrapper for the ChatBMS API"
+description = "API Wrapper for ChatBMS API"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `chatbms-0.0.1/PKG-INFO` & `chatbms-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ChatBMS
-Version: 0.0.1
-Summary: Wrapper for the ChatBMS API
+Version: 0.0.2
+Summary: API Wrapper for ChatBMS API
 Project-URL: Homepage, https://ChatBMS.in
 Project-URL: Bug Tracker, https://ChatBMS.in/issues
 Author-email: Chirag Manjeshwar <chirunder@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

