# Comparing `tmp/lifr-0.0.1.tar.gz` & `tmp/lifr-0.0.2.tar.gz`

## Comparing `lifr-0.0.1.tar` & `lifr-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lifr-0.0.1/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.1/src/LIFR/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifr-0.0.1/src/LIFR/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lifr-0.0.1/src/LIFR/__main__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lifr-0.0.1/LICENSE
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 lifr-0.0.1/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lifr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 lifr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lifr-0.0.2/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.2/src/LIFR/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifr-0.0.2/src/LIFR/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lifr-0.0.2/src/LIFR/__main__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lifr-0.0.2/LICENSE
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 lifr-0.0.2/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lifr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 lifr-0.0.2/PKG-INFO
```

### Comparing `lifr-0.0.1/.DS_Store` & `lifr-0.0.2/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -267,17 +267,17 @@
 000010a0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 000010b0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
 000010c0: 3130 342c 2034 3336 7d2c 207b 3932 302c  104, 436}, {920,
 000010d0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 000010e0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 000010f0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001100: 0000 008b 0000 0004 0064 0069 0073 0074  .........d.i.s.t
-00001110: 6c67 3153 636f 6d70 0000 0000 0000 2bd7  lg1Scomp......+.
+00001110: 6c67 3153 636f 6d70 0000 0000 0000 2acc  lg1Scomp......*.
 00001120: 0000 0004 0064 0069 0073 0074 6d6f 4444  .....d.i.s.tmoDD
-00001130: 626c 6f62 0000 0008 0000 0025 6531 c541  blob.......%e1.A
+00001130: 626c 6f62 0000 0008 0000 0048 6431 c541  blob.......Hd1.A
 00001140: 0000 0004 0064 0069 0073 0074 6d6f 6444  .....d.i.s.tmodD
 00001150: 626c 6f62 0000 0008 0000 0048 6431 c541  blob.......Hd1.A
 00001160: 0000 0004 0064 0069 0073 0074 7068 3153  .....d.i.s.tph1S
 00001170: 636f 6d70 0000 0000 0000 4000 0000 0004  comp......@.....
 00001180: 0064 0069 0073 0074 7653 726e 6c6f 6e67  .d.i.s.tvSrnlong
 00001190: 0000 0001 0000 0007 004c 0049 0043 0045  .........L.I.C.E
 000011a0: 004e 0053 0045 496c 6f63 626c 6f62 0000  .N.S.EIlocblob..
```

### Comparing `lifr-0.0.1/src/.DS_Store` & `lifr-0.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `lifr-0.0.1/src/LIFR/.DS_Store` & `lifr-0.0.2/src/LIFR/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 00000050: 0000 0001 0000 1000 0069 0074 005f 005f  .........i.t._._
 00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0002 0000 000b  ................
 00000090: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000000a0: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
 000000b0: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
-000000c0: 0000 0000 000b 005f 005f 006d 0061 0069  ......._._.m.a.i
-000000d0: 006e 005f 005f 002e 0070 0079 496c 6f63  .n._._...p.yIloc
-000000e0: 626c 6f62 0000 0010 0000 00af 0000 002e  blob............
-000000f0: ffff ffff ffff 0000 0000 0000 0000 0000  ................
+000000c0: 0000 0000 0007 004c 0049 0046 0052 002e  .......L.I.F.R..
+000000d0: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
+000000e0: 0000 00af 0000 002e ffff ffff ffff 0000  ................
+000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `lifr-0.0.1/src/LIFR/__main__.py` & `lifr-0.0.2/src/LIFR/__main__.py`

 * *Files identical despite different names*

### Comparing `lifr-0.0.1/LICENSE` & `lifr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lifr-0.0.1/PKG-INFO` & `lifr-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LIFR
-Version: 0.0.1
+Version: 0.0.2
 Summary: this package allows the user to connect with the LIFR model
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Raphael Scott <raphael.scott06@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

