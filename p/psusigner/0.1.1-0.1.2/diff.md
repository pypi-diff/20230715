# Comparing `tmp/psusigner-0.1.1.tar.gz` & `tmp/psusigner-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psusigner-0.1.1.tar", max compression
+gzip compressed data, was "psusigner-0.1.2.tar", max compression
```

## Comparing `psusigner-0.1.1.tar` & `psusigner-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1299 2023-07-14 16:56:38.298778 psusigner-0.1.1/README.md
--rw-r--r--   0        0        0       70 2023-07-14 16:10:49.545887 psusigner-0.1.1/psusigner/__init__.py
--rw-r--r--   0        0        0       44 2023-07-14 16:10:49.545887 psusigner-0.1.1/psusigner/exception.py
--rw-r--r--   0        0        0     9342 2023-07-14 16:10:49.545887 psusigner-0.1.1/psusigner/psucms.py
--rw-r--r--   0        0        0     2467 2023-07-14 16:10:49.545887 psusigner-0.1.1/psusigner/psuhsm.py
--rw-r--r--   0        0        0     3054 2023-07-14 16:39:10.345219 psusigner-0.1.1/psusigner/signers.py
--rw-r--r--   0        0        0      393 2023-07-14 16:58:37.119364 psusigner-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 psusigner-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1472 2023-07-15 10:42:39.330263 psusigner-0.1.2/README.md
+-rw-r--r--   0        0        0       70 2023-07-14 08:53:52.900150 psusigner-0.1.2/psusigner/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-14 07:28:25.442201 psusigner-0.1.2/psusigner/exception.py
+-rw-r--r--   0        0        0     9342 2023-07-14 13:37:18.397375 psusigner-0.1.2/psusigner/psucms.py
+-rw-r--r--   0        0        0     2467 2023-07-14 14:23:58.545900 psusigner-0.1.2/psusigner/psuhsm.py
+-rw-r--r--   0        0        0     3946 2023-07-15 10:40:22.494642 psusigner-0.1.2/psusigner/signers.py
+-rw-r--r--   0        0        0      393 2023-07-15 10:46:20.548128 psusigner-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 psusigner-0.1.2/PKG-INFO
```

### Comparing `psusigner-0.1.1/README.md` & `psusigner-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # PSU Signer
 Quick development for applying PSU digital signature using (Endensive)[https://github.com/m32/endesive].
 
+## Documents
+https://documenter.getpostman.com/view/644041/2s93eU1tyD
+
 ## Installation
 ```
 pip install psusigner
 ```
 
 ## Example
 
@@ -48,10 +51,13 @@
 
     )
 
     outname = fname.replace(".pdf", "-signed-cms-psuhsm-jwt.pdf")
 
     signer.sign_file(fname, dct, outname)
 
+    search_response = signer.search(certEntryCode="c1")
+    print("search output:", search_response)
+
 
 main()
 ```
```

### Comparing `psusigner-0.1.1/psusigner/psucms.py` & `psusigner-0.1.2/psusigner/psucms.py`

 * *Files identical despite different names*

### Comparing `psusigner-0.1.1/psusigner/psuhsm.py` & `psusigner-0.1.2/psusigner/psuhsm.py`

 * *Files identical despite different names*

### Comparing `psusigner-0.1.1/PKG-INFO` & `psusigner-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: psusigner
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Thanathip Limna
 Author-email: thanathip.l@coe.psu.ac.th
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: endesive (>=2.0.16,<3.0.0)
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # PSU Signer
 Quick development for applying PSU digital signature using (Endensive)[https://github.com/m32/endesive].
 
+## Documents
+https://documenter.getpostman.com/view/644041/2s93eU1tyD
+
 ## Installation
 ```
 pip install psusigner
 ```
 
 ## Example
 
@@ -62,11 +65,14 @@
 
     )
 
     outname = fname.replace(".pdf", "-signed-cms-psuhsm-jwt.pdf")
 
     signer.sign_file(fname, dct, outname)
 
+    search_response = signer.search(certEntryCode="c1")
+    print("search output:", search_response)
+
 
 main()
 ```
```

