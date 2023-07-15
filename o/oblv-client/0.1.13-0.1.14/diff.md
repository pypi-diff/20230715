# Comparing `tmp/oblv_client-0.1.13-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/oblv_client-0.1.14-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6181953 bytes, number of entries: 5
--rw-r--r--  4.6 unx     2079 b- defN 23-Jul-13 16:57 oblv_client-0.1.13.dist-info/METADATA
--rw-r--r--  4.6 unx      136 b- defN 23-Jul-13 16:57 oblv_client-0.1.13.dist-info/WHEEL
--rw-r--r--  4.6 unx    13552 b- defN 23-Jul-13 16:57 oblv_client/__init__.py
--rwxr-xr-x  4.6 unx 18388104 b- defN 23-Jul-13 16:57 oblv_client/oblv_client.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      419 b- defN 23-Jul-13 16:57 oblv_client-0.1.13.dist-info/RECORD
-5 files, 18404290 bytes uncompressed, 6181183 bytes compressed:  66.4%
+Zip file size: 5943520 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2079 b- defN 23-Jul-15 13:00 oblv_client-0.1.14.dist-info/METADATA
+-rw-r--r--  4.6 unx      133 b- defN 23-Jul-15 13:00 oblv_client-0.1.14.dist-info/WHEEL
+-rw-r--r--  4.6 unx    14052 b- defN 23-Jul-15 13:00 oblv_client/__init__.py
+-rwxr-xr-x  4.6 unx 17761192 b- defN 23-Jul-15 13:00 oblv_client/oblv_client.cpython-310-aarch64-linux-gnu.so
+-rw-r--r--  4.6 unx      420 b- defN 23-Jul-15 13:00 oblv_client-0.1.14.dist-info/RECORD
+5 files, 17777876 bytes uncompressed, 5942748 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: oblv_client-0.1.13.dist-info/METADATA
+Filename: oblv_client-0.1.14.dist-info/METADATA
 Comment: 
 
-Filename: oblv_client-0.1.13.dist-info/WHEEL
+Filename: oblv_client-0.1.14.dist-info/WHEEL
 Comment: 
 
 Filename: oblv_client/__init__.py
 Comment: 
 
-Filename: oblv_client/oblv_client.pypy39-pp73-x86_64-linux-gnu.so
+Filename: oblv_client/oblv_client.cpython-310-aarch64-linux-gnu.so
 Comment: 
 
-Filename: oblv_client-0.1.13.dist-info/RECORD
+Filename: oblv_client-0.1.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oblv_client/__init__.py

```diff
@@ -24,16 +24,26 @@
         body: str: The http response body
     """
 
     def __init__(self, _oblvResp):
         self.status = _oblvResp.status()
         self.status_code = _oblvResp.status()
         self.headers = _oblvResp.headers()
-        self.body = bytearray(_oblvResp.body()).decode()
-        self.text = bytearray(_oblvResp.body()).decode()
+        if self.status != 200:
+            for i in self.headers:
+                if i.lower() == "content-type":
+                    if self.headers[i].lower() == "application/json":
+                         self.body = ''.join(map(chr, _oblvResp.body()))
+                         self.text = ''.join(map(chr, _oblvResp.body()))
+            else:
+                self.body = bytearray(_oblvResp.body()).decode()
+                self.text = bytearray(_oblvResp.body()).decode()
+        else:
+            self.body = bytearray(_oblvResp.body()).decode()
+            self.text = bytearray(_oblvResp.body()).decode()
         self.content = _oblvResp.body()
 
     def json(self):
         return json.loads(self.body)
 
 
 class Enclave:
```

## Comparing `oblv_client-0.1.13.dist-info/METADATA` & `oblv_client-0.1.14.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oblv-client
-Version: 0.1.13
+Version: 0.1.14
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: urllib3
 Summary: python bindings for using enclaves with oblivious tooling
 Home-Page: https://oblivious.ai
 Author: OBLV Devs <hello@oblivious.ai>
```

