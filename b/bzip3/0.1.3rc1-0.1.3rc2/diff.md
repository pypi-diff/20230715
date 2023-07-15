# Comparing `tmp/bzip3-0.1.3rc1.tar.gz` & `tmp/bzip3-0.1.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bzip3-0.1.3rc1.tar", last modified: Wed Jul 12 12:56:05 2023, max compression
+gzip compressed data, was "bzip3-0.1.3rc2.tar", last modified: Sat Jul 15 07:44:05 2023, max compression
```

## Comparing `bzip3-0.1.3rc1.tar` & `bzip3-0.1.3rc2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.753803 bzip3-0.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-12 12:56:05.749803 bzip3-0.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/README.markdown
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.745803 bzip3-0.1.3rc1/bz3/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.745803 bzip3-0.1.3rc1/bz3/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.745803 bzip3-0.1.3rc1/bz3/backends/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/backends/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/backends/cffi/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.749803 bzip3-0.1.3rc1/bz3/backends/cython/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/backends/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1443071 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bz3/backends/cython/_bz3.c
--rw-r--r--   0 runner    (1001) docker     (123)    38370 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/backends/cython/_bz3.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/backends/cython/bzip3.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/bz3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/bz3/compression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.749803 bzip3-0.1.3rc1/bzip3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bzip3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bzip3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bzip3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bzip3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bzip3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 12:56:05.000000 bzip3-0.1.3rc1/bzip3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.745803 bzip3-0.1.3rc1/dep/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.749803 bzip3-0.1.3rc1/dep/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-12 12:55:48.000000 bzip3-0.1.3rc1/dep/include/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-12 12:55:48.000000 bzip3-0.1.3rc1/dep/include/getopt-shim.h
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-12 12:55:48.000000 bzip3-0.1.3rc1/dep/include/libbz3.h
--rw-r--r--   0 runner    (1001) docker     (123)   214460 2023-07-12 12:55:48.000000 bzip3-0.1.3rc1/dep/include/libsais.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.749803 bzip3-0.1.3rc1/dep/src/
--rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-12 12:55:48.000000 bzip3-0.1.3rc1/dep/src/libbz3.c
--rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-07-12 12:55:48.000000 bzip3-0.1.3rc1/dep/src/main.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:56:05.753803 bzip3-0.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:56:05.749803 bzip3-0.1.3rc1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/test/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/test/test_mem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/test/test_omp.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/test/test_seek.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-12 12:55:47.000000 bzip3-0.1.3rc1/test/test_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/README.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/backends/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cffi/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/backends/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1442982 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bz3/backends/cython/_bz3.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38368 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cython/_bz3.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cython/bzip3.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/bz3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/compression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bzip3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.950868 bzip3-0.1.3rc2/dep/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/dep/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/getopt-shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/libbz3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   214460 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/libsais.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/dep/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/src/libbz3.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_omp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_seek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_thread.py
```

### Comparing `bzip3-0.1.3rc1/PKG-INFO` & `bzip3-0.1.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bzip3
-Version: 0.1.3rc1
+Version: 0.1.3rc2
 Summary: bz3 compress and decompress
 Home-page: https://github.com/synodriver/python-bz3
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: bz3,compress,decompress
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bzip3-0.1.3rc1/README.markdown` & `bzip3-0.1.3rc2/README.markdown`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/bz3/backends/__init__.py` & `bzip3-0.1.3rc2/bz3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/bz3/backends/cffi/__init__.py` & `bzip3-0.1.3rc2/bz3/backends/cffi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         # cdef int32_t new_size, old_size, block_size
         if input_size > 0:
             # if PyByteArray_Resize(self.unused, input_size+PyByteArray_GET_SIZE(self.unused)) < 0:
             #     raise
             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
             self.unused.extend(data)
             if (
-                len(self.unused) > 9 and not self.have_magic_number
+                len(self.unused) >= 9 and not self.have_magic_number
             ):  # 9 bytes magic number
                 if bytes(self.unused[:5]) != b"BZ3v1":
                     raise ValueError("Invalid signature")
                 temp = self.unused[5:9]
                 block_size = lib.read_neutral_s32(
                     ffi.cast("uint8_t*", ffi.from_buffer(temp))
                 )
```

### Comparing `bzip3-0.1.3rc1/bz3/backends/cffi/build.py` & `bzip3-0.1.3rc2/bz3/backends/cffi/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,12 +131,12 @@
 print(c_sources)
 
 ffibuilder.set_source(
     "bz3.backends.cffi._bz3",
     source,
     sources=c_sources,
     include_dirs=["./dep/include"],
-    define_macros=[("VERSION", '"1.3.1.r4-g6d041f4"')],
+    define_macros=[("VERSION", '"1.3.1.r5-g646212a"')],
 )
 
 if __name__ == "__main__":
     ffibuilder.compile()
```

### Comparing `bzip3-0.1.3rc1/bz3/backends/cython/_bz3.c` & `bzip3-0.1.3rc2/bz3/backends/cython/_bz3.c`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "VERSION",
-                "\"1.3.1.r4-g6d041f4\""
+                "\"1.3.1.r5-g646212a\""
             ]
         ],
         "depends": [
             "dep/include/common.h",
             "dep/include/libbz3.h"
         ],
         "extra_compile_args": [
@@ -4642,15 +4642,15 @@
   __pyx_t_2 = ((__pyx_v_input_size > 0) != 0);
   if (__pyx_t_2) {
 
     /* "bz3/backends/cython/_bz3.pyx":169
  *             #     raise
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data)             # <<<<<<<<<<<<<<
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->unused, __pyx_n_s_extend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint8_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
@@ -4670,61 +4670,61 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "bz3/backends/cython/_bz3.pyx":170
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data)
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  */
     __pyx_t_1 = __pyx_v_self->unused;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_6 = ((PyByteArray_GET_SIZE(__pyx_t_1) > 9) != 0);
+    __pyx_t_6 = ((PyByteArray_GET_SIZE(__pyx_t_1) >= 9) != 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_6) {
     } else {
       __pyx_t_2 = __pyx_t_6;
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_6 = ((!(__pyx_v_self->have_magic_number != 0)) != 0);
     __pyx_t_2 = __pyx_t_6;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_2) {
 
       /* "bz3/backends/cython/_bz3.pyx":171
  *             self.unused.extend(data)
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  */
       __pyx_t_1 = __pyx_v_self->unused;
       __Pyx_INCREF(__pyx_t_1);
       __pyx_t_2 = ((strncmp(PyByteArray_AS_STRING(__pyx_t_1), __pyx_v_3bz3_8backends_6cython_4_bz3_magic, 5) != 0) != 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(__pyx_t_2)) {
 
         /* "bz3/backends/cython/_bz3.pyx":172
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")             # <<<<<<<<<<<<<<
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  */
         __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __PYX_ERR(0, 172, __pyx_L1_error)
 
         /* "bz3/backends/cython/_bz3.pyx":171
  *             self.unused.extend(data)
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  */
       }
 
       /* "bz3/backends/cython/_bz3.pyx":173
@@ -4809,15 +4809,15 @@
  *             while True:
  */
       __pyx_v_self->have_magic_number = 1;
 
       /* "bz3/backends/cython/_bz3.pyx":170
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data)
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  */
     }
 
     /* "bz3/backends/cython/_bz3.pyx":180
  *                 self.have_magic_number = 1
@@ -11985,15 +11985,15 @@
           (void)(memcpy((&(PyByteArray_AS_STRING(__pyx_v_ret)[(PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_i]))])), (__pyx_v_self->buffers[__pyx_v_i]), ((size_t)(__pyx_v_self->sizes[__pyx_v_i]))));
         }
 
         /* "bz3/backends/cython/_bz3.pyx":624
  *                         memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]]), self.buffers[i], <size_t>self.sizes[i])
  * 
  *                     del self.uncompressed[:all_blocks_size]             # <<<<<<<<<<<<<<
- *             return bytes(ret)
+ *         return bytes(ret)
  * 
  */
         if (unlikely(__pyx_v_self->uncompressed == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
           __PYX_ERR(0, 624, __pyx_L1_error)
         }
         if (__Pyx_PyObject_DelSlice(__pyx_v_self->uncompressed, 0, __pyx_v_all_blocks_size, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 624, __pyx_L1_error)
@@ -12004,48 +12004,46 @@
  *             self.uncompressed.extend(data)
  *             if PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # able to perform a compress             # <<<<<<<<<<<<<<
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks
  *                     for i in range(self.numthreads):
  */
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":625
- * 
- *                     del self.uncompressed[:all_blocks_size]
- *             return bytes(ret)             # <<<<<<<<<<<<<<
- * 
- *     cpdef inline bytes flush(self):
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_r = ((PyObject*)__pyx_t_1);
-    __pyx_t_1 = 0;
-    goto __pyx_L0;
-
     /* "bz3/backends/cython/_bz3.pyx":602
  *             self.have_magic_number = 1
  *         cdef uint32_t i
  *         if input_size > 0:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(self.uncompressed, input_size+PyByteArray_GET_SIZE(self.uncompressed)) < 0:
  *             #     raise
  */
   }
 
+  /* "bz3/backends/cython/_bz3.pyx":625
+ * 
+ *                     del self.uncompressed[:all_blocks_size]
+ *         return bytes(ret)             # <<<<<<<<<<<<<<
+ * 
+ *     cpdef inline bytes flush(self):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
   /* "bz3/backends/cython/_bz3.pyx":589
  *             self.old_sizes = NULL
  * 
  *     cpdef inline bytes compress(self, const uint8_t[::1] data):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t new_size
  */
 
   /* function exit code */
-  __pyx_r = ((PyObject*)Py_None); __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpCompressor.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
@@ -12108,15 +12106,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_data, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "bz3/backends/cython/_bz3.pyx":627
- *             return bytes(ret)
+ *         return bytes(ret)
  * 
  *     cpdef inline bytes flush(self):             # <<<<<<<<<<<<<<
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t new_size
  */
 
 static PyObject *__pyx_pw_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_7flush(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
@@ -12425,15 +12423,15 @@
   __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "bz3/backends/cython/_bz3.pyx":627
- *             return bytes(ret)
+ *         return bytes(ret)
  * 
  *     cpdef inline bytes flush(self):             # <<<<<<<<<<<<<<
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t new_size
  */
 
   /* function exit code */
@@ -14194,15 +14192,15 @@
   __pyx_t_2 = ((__pyx_v_input_size > 0) != 0);
   if (__pyx_t_2) {
 
     /* "bz3/backends/cython/_bz3.pyx":793
  *             #     raise
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data) # read header             # <<<<<<<<<<<<<<
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->unused, __pyx_n_s_extend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint8_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 793, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
@@ -14222,61 +14220,61 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "bz3/backends/cython/_bz3.pyx":794
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data) # read header
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  */
     __pyx_t_1 = __pyx_v_self->unused;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_6 = ((PyByteArray_GET_SIZE(__pyx_t_1) > 9) != 0);
+    __pyx_t_6 = ((PyByteArray_GET_SIZE(__pyx_t_1) >= 9) != 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_6) {
     } else {
       __pyx_t_2 = __pyx_t_6;
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_6 = ((!(__pyx_v_self->have_magic_number != 0)) != 0);
     __pyx_t_2 = __pyx_t_6;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_2) {
 
       /* "bz3/backends/cython/_bz3.pyx":795
  *             self.unused.extend(data) # read header
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  */
       __pyx_t_1 = __pyx_v_self->unused;
       __Pyx_INCREF(__pyx_t_1);
       __pyx_t_2 = ((strncmp(PyByteArray_AS_STRING(__pyx_t_1), __pyx_v_3bz3_8backends_6cython_4_bz3_magic, 5) != 0) != 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(__pyx_t_2)) {
 
         /* "bz3/backends/cython/_bz3.pyx":796
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")             # <<<<<<<<<<<<<<
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  */
         __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 796, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __PYX_ERR(0, 796, __pyx_L1_error)
 
         /* "bz3/backends/cython/_bz3.pyx":795
  *             self.unused.extend(data) # read header
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  */
       }
 
       /* "bz3/backends/cython/_bz3.pyx":797
@@ -14361,15 +14359,15 @@
  *             while not should_break:
  */
       __pyx_v_self->have_magic_number = 1;
 
       /* "bz3/backends/cython/_bz3.pyx":794
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data) # read header
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  */
     }
 
     /* "bz3/backends/cython/_bz3.pyx":804
  *                 self.have_magic_number = 1
@@ -29896,15 +29894,15 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "bz3/backends/cython/_bz3.pyx":172
- *             if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+ *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")             # <<<<<<<<<<<<<<
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Invalid_signature); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
```

### Comparing `bzip3-0.1.3rc1/bz3/backends/cython/_bz3.pyx` & `bzip3-0.1.3rc2/bz3/backends/cython/_bz3.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         cdef bytearray ret = bytearray()
         cdef int32_t new_size, old_size, block_size
         if input_size > 0:
             # if PyByteArray_Resize(self.unused, input_size+PyByteArray_GET_SIZE(self.unused)) < 0:
             #     raise
             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
             self.unused.extend(data)
-            if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+            if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
                     raise ValueError("Invalid signature")
                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
                 if block_size  < KiB(65) or block_size >MiB(511):
                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
                 self.init_state(block_size)
                 del self.unused[:9]
@@ -618,15 +618,15 @@
                         #     raise
                         ret.extend((self.sizes[i] + 8)*b"\x00")
                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-8]), self.sizes[i])
                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-4]), self.block_size)
                         memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]]), self.buffers[i], <size_t>self.sizes[i])
 
                     del self.uncompressed[:all_blocks_size]
-            return bytes(ret)
+        return bytes(ret)
 
     cpdef inline bytes flush(self):
         cdef bytearray ret = bytearray()
         cdef int32_t new_size
         cdef int32_t remain_size = <int32_t>PyByteArray_GET_SIZE(self.uncompressed)
         cdef:
             int i = 0  # thread count
@@ -787,15 +787,15 @@
         cdef uint32_t i, thread_count, j, should_delete=0
         cdef int should_break = 0
         if input_size > 0:
             # if PyByteArray_Resize(self.unused, input_size+PyByteArray_GET_SIZE(self.unused)) < 0:
             #     raise
             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
             self.unused.extend(data) # read header
-            if PyByteArray_GET_SIZE(self.unused) > 9 and not self.have_magic_number: # 9 bytes magic number
+            if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
                     raise ValueError("Invalid signature")
                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
                 if block_size  < KiB(65) or block_size >MiB(511):
                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
                 self.init_state(block_size)
                 del self.unused[:9]
```

### Comparing `bzip3-0.1.3rc1/bz3/backends/cython/bzip3.pxd` & `bzip3-0.1.3rc2/bz3/backends/cython/bzip3.pxd`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/bz3/bz3.py` & `bzip3-0.1.3rc2/bz3/bz3.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/bz3/compression.py` & `bzip3-0.1.3rc2/bz3/compression.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/bzip3.egg-info/PKG-INFO` & `bzip3-0.1.3rc2/bzip3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bzip3
-Version: 0.1.3rc1
+Version: 0.1.3rc2
 Summary: bz3 compress and decompress
 Home-page: https://github.com/synodriver/python-bz3
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: bz3,compress,decompress
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bzip3-0.1.3rc1/bzip3.egg-info/SOURCES.txt` & `bzip3-0.1.3rc2/bzip3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/dep/include/common.h` & `bzip3-0.1.3rc2/dep/include/common.h`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  */
 
 #ifndef _COMMON_H
 #define _COMMON_H
 
 #define KiB(x) ((x)*1024)
 #define MiB(x) ((x)*1024 * 1024)
-#define BWT_BOUND(x) ((x) + 128)
+#define BWT_BOUND(x) (bz3_bound(x) + 128)
 
 #include <inttypes.h>
 #include <stdint.h>
 
 typedef uint8_t u8;
 typedef uint16_t u16;
 typedef uint32_t u32;
```

### Comparing `bzip3-0.1.3rc1/dep/include/getopt-shim.h` & `bzip3-0.1.3rc2/dep/include/getopt-shim.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/dep/include/libbz3.h` & `bzip3-0.1.3rc2/dep/include/libbz3.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/dep/include/libsais.h` & `bzip3-0.1.3rc2/dep/include/libsais.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/dep/src/libbz3.c` & `bzip3-0.1.3rc2/dep/src/libbz3.c`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/dep/src/main.c` & `bzip3-0.1.3rc2/dep/src/main.c`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/setup.py` & `bzip3-0.1.3rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             if self.compiler.compiler_type == "msvc":
                 ext.define_macros.extend([("restrict", "__restrict")])
         super().build_extensions()
 
 
 c_sources = ["bz3/backends/cython/_bz3.pyx"] + glob.glob("./dep/src/*.c")
 c_sources = list(filter(lambda x: "main" not in x, c_sources))
-define_macros = [("VERSION", '"1.3.1.r4-g6d041f4"')]
+define_macros = [("VERSION", '"1.3.1.r5-g646212a"')]
 if has_option("--debug"):
     define_macros.append(("MEMDEBUG", None))
 
 extensions = [
     Extension(
         "bz3.backends.cython._bz3",
         c_sources,
```

### Comparing `bzip3-0.1.3rc1/test/test_compress.py` & `bzip3-0.1.3rc2/test/test_compress.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Copyright (c) 2008-2023 synodriver <diguohuangjiajinweijun@gmail.com>
 """
 import sys
 
+import bz3
+
 sys.path.append(".")
 import os
 from random import randint
 from unittest import TestCase
 
 from bz3 import (
     bound,
@@ -15,14 +17,15 @@
     decompress_file,
     decompress_into,
     libversion,
 )
 from bz3 import open as bz3_open
 from bz3 import test_file
 
+
 # os.environ["BZ3_USE_CFFI"] = "1"
 
 
 class TestCompress(TestCase):
     def test_compress(self):
         with open("test_input.tar", "rb") as inp, open("compressed.bz3", "wb") as out:
             compress_file(inp, out, 1000 * 1000)
@@ -54,12 +57,15 @@
             buffer_updated = compress_into(inp, out)
             buffer_updated = decompress_into(out[:buffer_updated], out2)
             self.assertEqual(bytes(out2[:buffer_updated]), inp)
 
     def test_version(self):
         self.assertTrue(isinstance(libversion(), str))
 
+    def test_zerosize(self):
+        self.assertEqual(bz3.decompress(bz3.compress(b"")), b"", "fail to compress b\"\"")
+
 
 if __name__ == "__main__":
     import unittest
 
     unittest.main()
```

### Comparing `bzip3-0.1.3rc1/test/test_mem.py` & `bzip3-0.1.3rc2/test/test_mem.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/test/test_omp.py` & `bzip3-0.1.3rc2/test/test_omp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import sys
+import traceback
 from unittest import TestCase
 
 sys.path.append(".")
 
 import os
 
+import bz3
 from bz3 import compress, decompress
 from bz3 import open as _open
 from bz3.backends.cython import BZ3OmpCompressor, BZ3OmpDecompressor
 
-origin_data = b"124" * (100 * 10**6 + 7)
+origin_data = b"124" * (100 * 10 ** 6 + 7)
 
 
 class TestOmp(TestCase):
     def test_compress(self):
-        compressor = BZ3OmpCompressor(10**6, os.cpu_count())
+        compressor = BZ3OmpCompressor(10 ** 6, os.cpu_count())
         # origin_data = b"124" * (600*10 ** 6 + 7)
         compressed_data = compressor.compress(origin_data) + compressor.flush()
         self.assertEqual(decompress(compressed_data), origin_data)
 
     def test_decompress(self):
         # origin_data = b"124" * (10 ** 6 + 7)
         compressed_data = compress(origin_data)
@@ -27,12 +29,17 @@
 
     def test_stream(self):
         with _open("test.bz3", "wb", num_threads=16) as f:
             f.write(origin_data)
         with _open("test.bz3", "rb", num_threads=16) as f:
             self.assertEqual(f.read(), origin_data)
 
+    def test_zerosize(self):
+        self.assertEqual(bz3.decompress(bz3.compress(b"", num_threads=os.cpu_count()), num_threads=os.cpu_count()),
+                         b"",
+                         "fail to compress b\"\"")
+
 
 if __name__ == "__main__":
     import unittest
 
     unittest.main()
```

### Comparing `bzip3-0.1.3rc1/test/test_seek.py` & `bzip3-0.1.3rc2/test/test_seek.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc1/test/test_thread.py` & `bzip3-0.1.3rc2/test/test_thread.py`

 * *Files identical despite different names*

