# Comparing `tmp/bzip3-0.1.3rc2.tar.gz` & `tmp/bzip3-0.1.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bzip3-0.1.3rc2.tar", last modified: Sat Jul 15 07:44:05 2023, max compression
+gzip compressed data, was "bzip3-0.1.3rc3.tar", last modified: Sat Jul 15 08:15:23 2023, max compression
```

## Comparing `bzip3-0.1.3rc2.tar` & `bzip3-0.1.3rc3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/README.markdown
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/backends/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cffi/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bz3/backends/cython/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1442982 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bz3/backends/cython/_bz3.c
--rw-r--r--   0 runner    (1001) docker     (123)    38368 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cython/_bz3.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/backends/cython/bzip3.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/bz3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/bz3/compression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/bzip3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 07:44:05.000000 bzip3-0.1.3rc2/bzip3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.950868 bzip3-0.1.3rc2/dep/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.954868 bzip3-0.1.3rc2/dep/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/getopt-shim.h
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/libbz3.h
--rw-r--r--   0 runner    (1001) docker     (123)   214460 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/include/libsais.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/dep/src/
--rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/src/libbz3.c
--rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-07-15 07:43:48.000000 bzip3-0.1.3rc2/dep/src/main.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:44:05.958868 bzip3-0.1.3rc2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_mem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_omp.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_seek.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-15 07:43:47.000000 bzip3-0.1.3rc2/test/test_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/README.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.675428 bzip3-0.1.3rc3/bz3/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.675428 bzip3-0.1.3rc3/bz3/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.675428 bzip3-0.1.3rc3/bz3/backends/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/backends/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/backends/cffi/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.675428 bzip3-0.1.3rc3/bz3/backends/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/backends/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1442970 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bz3/backends/cython/_bz3.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38344 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/backends/cython/_bz3.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/backends/cython/bzip3.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/bz3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/bz3/compression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/bzip3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bzip3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bzip3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bzip3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bzip3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bzip3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 08:15:23.000000 bzip3-0.1.3rc3/bzip3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.675428 bzip3-0.1.3rc3/dep/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/dep/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-15 08:15:05.000000 bzip3-0.1.3rc3/dep/include/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-15 08:15:05.000000 bzip3-0.1.3rc3/dep/include/getopt-shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-15 08:15:05.000000 bzip3-0.1.3rc3/dep/include/libbz3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   214460 2023-07-15 08:15:05.000000 bzip3-0.1.3rc3/dep/include/libsais.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/dep/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-15 08:15:05.000000 bzip3-0.1.3rc3/dep/src/libbz3.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-07-15 08:15:05.000000 bzip3-0.1.3rc3/dep/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:15:23.679428 bzip3-0.1.3rc3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/test/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/test/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/test/test_omp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/test/test_seek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-15 08:15:04.000000 bzip3-0.1.3rc3/test/test_thread.py
```

### Comparing `bzip3-0.1.3rc2/PKG-INFO` & `bzip3-0.1.3rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bzip3
-Version: 0.1.3rc2
+Version: 0.1.3rc3
 Summary: bz3 compress and decompress
 Home-page: https://github.com/synodriver/python-bz3
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: bz3,compress,decompress
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bzip3-0.1.3rc2/README.markdown` & `bzip3-0.1.3rc3/README.markdown`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bz3/backends/__init__.py` & `bzip3-0.1.3rc3/bz3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bz3/backends/cffi/__init__.py` & `bzip3-0.1.3rc3/bz3/backends/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bz3/backends/cffi/build.py` & `bzip3-0.1.3rc3/bz3/backends/cffi/build.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bz3/backends/cython/_bz3.c` & `bzip3-0.1.3rc3/bz3/backends/cython/_bz3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1202,15 +1202,15 @@
   int32_t block_size;
   PyObject *uncompressed;
   int have_magic_number;
   uint32_t numthreads;
 };
 
 
-/* "bz3/backends/cython/_bz3.pyx":682
+/* "bz3/backends/cython/_bz3.pyx":681
  * @cython.no_gc
  * @cython.final
  * cdef class BZ3OmpDecompressor:             # <<<<<<<<<<<<<<
  *     cdef:
  *         bz3_state ** states
  */
 struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor {
@@ -1363,15 +1363,15 @@
 static CYTHON_INLINE void __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_free_states(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor *);
 static CYTHON_INLINE void __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_free_buffers(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor *);
 static CYTHON_INLINE PyObject *__pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_compress(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor *, __Pyx_memviewslice, int __pyx_skip_dispatch);
 static CYTHON_INLINE PyObject *__pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_flush(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor *, int __pyx_skip_dispatch);
 static CYTHON_INLINE PyObject *__pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_error(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor *, int __pyx_skip_dispatch);
 
 
-/* "bz3/backends/cython/_bz3.pyx":682
+/* "bz3/backends/cython/_bz3.pyx":681
  * @cython.no_gc
  * @cython.final
  * cdef class BZ3OmpDecompressor:             # <<<<<<<<<<<<<<
  *     cdef:
  *         bz3_state ** states
  */
 
@@ -11428,16 +11428,16 @@
   __Pyx_RefNannyFinishContext();
 }
 
 /* "bz3/backends/cython/_bz3.pyx":568
  *                     self.buffers[i] = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
- *         cdef uint32_t i
  *         self.free_states()
+ *         self.free_buffers()
  */
 
 /* Python wrapper */
 static void __pyx_pw_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
@@ -11448,229 +11448,229 @@
 }
 
 static void __pyx_pf_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_2__dealloc__(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":570
+  /* "bz3/backends/cython/_bz3.pyx":569
+ * 
  *     def __dealloc__(self):
- *         cdef uint32_t i
  *         self.free_states()             # <<<<<<<<<<<<<<
  *         self.free_buffers()
  *         if self.states:
  */
   __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_free_states(__pyx_v_self);
 
-  /* "bz3/backends/cython/_bz3.pyx":571
- *         cdef uint32_t i
+  /* "bz3/backends/cython/_bz3.pyx":570
+ *     def __dealloc__(self):
  *         self.free_states()
  *         self.free_buffers()             # <<<<<<<<<<<<<<
  *         if self.states:
  *             PyMem_Free(self.states)
  */
   __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_free_buffers(__pyx_v_self);
 
-  /* "bz3/backends/cython/_bz3.pyx":572
+  /* "bz3/backends/cython/_bz3.pyx":571
  *         self.free_states()
  *         self.free_buffers()
  *         if self.states:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)
  */
   __pyx_t_1 = (__pyx_v_self->states != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":573
+    /* "bz3/backends/cython/_bz3.pyx":572
  *         self.free_buffers()
  *         if self.states:
  *             PyMem_Free(self.states)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL
  */
     PyMem_Free(__pyx_v_self->states);
 
-    /* "bz3/backends/cython/_bz3.pyx":574
+    /* "bz3/backends/cython/_bz3.pyx":573
  *         if self.states:
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)             # <<<<<<<<<<<<<<
  *             self.states = NULL
  *         if self.buffers:
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->states);
 
-    /* "bz3/backends/cython/_bz3.pyx":575
+    /* "bz3/backends/cython/_bz3.pyx":574
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL             # <<<<<<<<<<<<<<
  *         if self.buffers:
  *             PyMem_Free(self.buffers)
  */
     __pyx_v_self->states = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":572
+    /* "bz3/backends/cython/_bz3.pyx":571
  *         self.free_states()
  *         self.free_buffers()
  *         if self.states:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":576
+  /* "bz3/backends/cython/_bz3.pyx":575
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL
  *         if self.buffers:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  */
   __pyx_t_1 = (__pyx_v_self->buffers != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":577
+    /* "bz3/backends/cython/_bz3.pyx":576
  *             self.states = NULL
  *         if self.buffers:
  *             PyMem_Free(self.buffers)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL
  */
     PyMem_Free(__pyx_v_self->buffers);
 
-    /* "bz3/backends/cython/_bz3.pyx":578
+    /* "bz3/backends/cython/_bz3.pyx":577
  *         if self.buffers:
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)             # <<<<<<<<<<<<<<
  *             self.buffers = NULL
  *         if self.sizes:
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->buffers);
 
-    /* "bz3/backends/cython/_bz3.pyx":579
+    /* "bz3/backends/cython/_bz3.pyx":578
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL             # <<<<<<<<<<<<<<
  *         if self.sizes:
  *             PyMem_Free(self.sizes)
  */
     __pyx_v_self->buffers = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":576
+    /* "bz3/backends/cython/_bz3.pyx":575
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL
  *         if self.buffers:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":580
+  /* "bz3/backends/cython/_bz3.pyx":579
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL
  *         if self.sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  */
   __pyx_t_1 = (__pyx_v_self->sizes != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":581
+    /* "bz3/backends/cython/_bz3.pyx":580
  *             self.buffers = NULL
  *         if self.sizes:
  *             PyMem_Free(self.sizes)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL
  */
     PyMem_Free(__pyx_v_self->sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":582
+    /* "bz3/backends/cython/_bz3.pyx":581
  *         if self.sizes:
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)             # <<<<<<<<<<<<<<
  *             self.sizes = NULL
  *         if self.old_sizes:
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":583
+    /* "bz3/backends/cython/_bz3.pyx":582
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL             # <<<<<<<<<<<<<<
  *         if self.old_sizes:
  *             PyMem_Free(self.old_sizes)
  */
     __pyx_v_self->sizes = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":580
+    /* "bz3/backends/cython/_bz3.pyx":579
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL
  *         if self.sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":584
+  /* "bz3/backends/cython/_bz3.pyx":583
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL
  *         if self.old_sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  */
   __pyx_t_1 = (__pyx_v_self->old_sizes != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":585
+    /* "bz3/backends/cython/_bz3.pyx":584
  *             self.sizes = NULL
  *         if self.old_sizes:
  *             PyMem_Free(self.old_sizes)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  *             self.old_sizes = NULL
  */
     PyMem_Free(__pyx_v_self->old_sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":586
+    /* "bz3/backends/cython/_bz3.pyx":585
  *         if self.old_sizes:
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)             # <<<<<<<<<<<<<<
  *             self.old_sizes = NULL
  * 
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->old_sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":587
+    /* "bz3/backends/cython/_bz3.pyx":586
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  *             self.old_sizes = NULL             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bytes compress(self, const uint8_t[::1] data):
  */
     __pyx_v_self->old_sizes = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":584
+    /* "bz3/backends/cython/_bz3.pyx":583
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL
  *         if self.old_sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  */
   }
 
   /* "bz3/backends/cython/_bz3.pyx":568
  *                     self.buffers[i] = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
- *         cdef uint32_t i
  *         self.free_states()
+ *         self.free_buffers()
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bz3/backends/cython/_bz3.pyx":589
+/* "bz3/backends/cython/_bz3.pyx":588
  *             self.old_sizes = NULL
  * 
  *     cpdef inline bytes compress(self, const uint8_t[::1] data):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t new_size
  */
 
@@ -11692,350 +11692,350 @@
   uint32_t __pyx_t_8;
   int32_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compress", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":590
+  /* "bz3/backends/cython/_bz3.pyx":589
  * 
  *     cpdef inline bytes compress(self, const uint8_t[::1] data):
  *         cdef Py_ssize_t input_size = data.shape[0]             # <<<<<<<<<<<<<<
  *         cdef int32_t new_size
  *         cdef bytearray ret = bytearray()
  */
   __pyx_v_input_size = (__pyx_v_data.shape[0]);
 
-  /* "bz3/backends/cython/_bz3.pyx":592
+  /* "bz3/backends/cython/_bz3.pyx":591
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t new_size
  *         cdef bytearray ret = bytearray()             # <<<<<<<<<<<<<<
  *         cdef int32_t all_blocks_size = self.block_size * self.numthreads
  *         if not self.have_magic_number:
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":593
+  /* "bz3/backends/cython/_bz3.pyx":592
  *         cdef int32_t new_size
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t all_blocks_size = self.block_size * self.numthreads             # <<<<<<<<<<<<<<
  *         if not self.have_magic_number:
  *             # if PyByteArray_Resize(ret, 9) < 0:
  */
   __pyx_v_all_blocks_size = (__pyx_v_self->block_size * __pyx_v_self->numthreads);
 
-  /* "bz3/backends/cython/_bz3.pyx":594
+  /* "bz3/backends/cython/_bz3.pyx":593
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t all_blocks_size = self.block_size * self.numthreads
  *         if not self.have_magic_number:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(ret, 9) < 0:
  *             #     raise
  */
   __pyx_t_2 = ((!(__pyx_v_self->have_magic_number != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "bz3/backends/cython/_bz3.pyx":598
+    /* "bz3/backends/cython/_bz3.pyx":597
  *             #     raise
  *             # memcpy(PyByteArray_AS_STRING(ret), magic, 5)
  *             ret.extend(<bytes>magic[:5]+b"\x00\x00\x00\x00")  # 9 bytes             # <<<<<<<<<<<<<<
  *             write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[5]), self.block_size)
  *             self.have_magic_number = 1
  */
-    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_3bz3_8backends_6cython_4_bz3_magic + 0, 5 - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_3bz3_8backends_6cython_4_bz3_magic + 0, 5 - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 597, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_kp_b__4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 598, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_kp_b__4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 597, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 597, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bz3/backends/cython/_bz3.pyx":599
+    /* "bz3/backends/cython/_bz3.pyx":598
  *             # memcpy(PyByteArray_AS_STRING(ret), magic, 5)
  *             ret.extend(<bytes>magic[:5]+b"\x00\x00\x00\x00")  # 9 bytes
  *             write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[5]), self.block_size)             # <<<<<<<<<<<<<<
  *             self.have_magic_number = 1
  *         cdef uint32_t i
  */
     write_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_v_ret)[5]))), __pyx_v_self->block_size);
 
-    /* "bz3/backends/cython/_bz3.pyx":600
+    /* "bz3/backends/cython/_bz3.pyx":599
  *             ret.extend(<bytes>magic[:5]+b"\x00\x00\x00\x00")  # 9 bytes
  *             write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[5]), self.block_size)
  *             self.have_magic_number = 1             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         if input_size > 0:
  */
     __pyx_v_self->have_magic_number = 1;
 
-    /* "bz3/backends/cython/_bz3.pyx":594
+    /* "bz3/backends/cython/_bz3.pyx":593
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t all_blocks_size = self.block_size * self.numthreads
  *         if not self.have_magic_number:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(ret, 9) < 0:
  *             #     raise
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":602
+  /* "bz3/backends/cython/_bz3.pyx":601
  *             self.have_magic_number = 1
  *         cdef uint32_t i
  *         if input_size > 0:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(self.uncompressed, input_size+PyByteArray_GET_SIZE(self.uncompressed)) < 0:
  *             #     raise
  */
   __pyx_t_2 = ((__pyx_v_input_size > 0) != 0);
   if (__pyx_t_2) {
 
-    /* "bz3/backends/cython/_bz3.pyx":606
+    /* "bz3/backends/cython/_bz3.pyx":605
  *             #     raise
  *             # memcpy(&(PyByteArray_AS_STRING(self.uncompressed)[PyByteArray_GET_SIZE(self.uncompressed)-input_size]), &data[0], input_size) # todo? direct copy to bytearray
  *             self.uncompressed.extend(data)             # <<<<<<<<<<<<<<
  *             if PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # able to perform a compress
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->uncompressed, __pyx_n_s_extend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->uncompressed, __pyx_n_s_extend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint8_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 606, __pyx_L1_error)
+    __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint8_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bz3/backends/cython/_bz3.pyx":607
+    /* "bz3/backends/cython/_bz3.pyx":606
  *             # memcpy(&(PyByteArray_AS_STRING(self.uncompressed)[PyByteArray_GET_SIZE(self.uncompressed)-input_size]), &data[0], input_size) # todo? direct copy to bytearray
  *             self.uncompressed.extend(data)
  *             if PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # able to perform a compress             # <<<<<<<<<<<<<<
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks
  *                     for i in range(self.numthreads):
  */
     __pyx_t_1 = __pyx_v_self->uncompressed;
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = ((PyByteArray_GET_SIZE(__pyx_t_1) >= __pyx_v_all_blocks_size) != 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_2) {
 
-      /* "bz3/backends/cython/_bz3.pyx":608
+      /* "bz3/backends/cython/_bz3.pyx":607
  *             self.uncompressed.extend(data)
  *             if PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # able to perform a compress
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks             # <<<<<<<<<<<<<<
  *                     for i in range(self.numthreads):
  *                         self.sizes[i] = self.block_size  # fill the sizes array
  */
       while (1) {
         __pyx_t_1 = __pyx_v_self->uncompressed;
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_2 = ((PyByteArray_GET_SIZE(__pyx_t_1) >= __pyx_v_all_blocks_size) != 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (!__pyx_t_2) break;
 
-        /* "bz3/backends/cython/_bz3.pyx":609
+        /* "bz3/backends/cython/_bz3.pyx":608
  *             if PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # able to perform a compress
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks
  *                     for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *                         self.sizes[i] = self.block_size  # fill the sizes array
  *                         memcpy(self.buffers[i], &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size], <size_t>self.block_size)
  */
         __pyx_t_6 = __pyx_v_self->numthreads;
         __pyx_t_7 = __pyx_t_6;
         for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
           __pyx_v_i = __pyx_t_8;
 
-          /* "bz3/backends/cython/_bz3.pyx":610
+          /* "bz3/backends/cython/_bz3.pyx":609
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks
  *                     for i in range(self.numthreads):
  *                         self.sizes[i] = self.block_size  # fill the sizes array             # <<<<<<<<<<<<<<
  *                         memcpy(self.buffers[i], &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size], <size_t>self.block_size)
  *                         # make a copy
  */
           __pyx_t_9 = __pyx_v_self->block_size;
           (__pyx_v_self->sizes[__pyx_v_i]) = __pyx_t_9;
 
-          /* "bz3/backends/cython/_bz3.pyx":611
+          /* "bz3/backends/cython/_bz3.pyx":610
  *                     for i in range(self.numthreads):
  *                         self.sizes[i] = self.block_size  # fill the sizes array
  *                         memcpy(self.buffers[i], &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size], <size_t>self.block_size)             # <<<<<<<<<<<<<<
  *                         # make a copy
  *                     bz3_encode_blocks(self.states, self.buffers, self.sizes, <int32_t>self.numthreads)
  */
           __pyx_t_1 = __pyx_v_self->uncompressed;
           __Pyx_INCREF(__pyx_t_1);
           (void)(memcpy((__pyx_v_self->buffers[__pyx_v_i]), (&(PyByteArray_AS_STRING(__pyx_t_1)[(__pyx_v_i * __pyx_v_self->block_size)])), ((size_t)__pyx_v_self->block_size)));
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":613
+        /* "bz3/backends/cython/_bz3.pyx":612
  *                         memcpy(self.buffers[i], &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size], <size_t>self.block_size)
  *                         # make a copy
  *                     bz3_encode_blocks(self.states, self.buffers, self.sizes, <int32_t>self.numthreads)             # <<<<<<<<<<<<<<
  *                     for i in range(self.numthreads):
  *                         if bz3_last_error(self.states[i]) != BZ3_OK:
  */
         __pyx_f_3bz3_8backends_6cython_4_bz3_bz3_encode_blocks(__pyx_v_self->states, __pyx_v_self->buffers, __pyx_v_self->sizes, ((int32_t)__pyx_v_self->numthreads));
 
-        /* "bz3/backends/cython/_bz3.pyx":614
+        /* "bz3/backends/cython/_bz3.pyx":613
  *                         # make a copy
  *                     bz3_encode_blocks(self.states, self.buffers, self.sizes, <int32_t>self.numthreads)
  *                     for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *                         if bz3_last_error(self.states[i]) != BZ3_OK:
  *                             raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[i]))
  */
         __pyx_t_6 = __pyx_v_self->numthreads;
         __pyx_t_7 = __pyx_t_6;
         for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
           __pyx_v_i = __pyx_t_8;
 
-          /* "bz3/backends/cython/_bz3.pyx":615
+          /* "bz3/backends/cython/_bz3.pyx":614
  *                     bz3_encode_blocks(self.states, self.buffers, self.sizes, <int32_t>self.numthreads)
  *                     for i in range(self.numthreads):
  *                         if bz3_last_error(self.states[i]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                             raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[i]))
  *                         # if PyByteArray_Resize(ret, PyByteArray_GET_SIZE(ret) + new_size + 8) < 0:
  */
           __pyx_t_2 = ((bz3_last_error((__pyx_v_self->states[__pyx_v_i])) != BZ3_OK) != 0);
           if (unlikely(__pyx_t_2)) {
 
-            /* "bz3/backends/cython/_bz3.pyx":616
+            /* "bz3/backends/cython/_bz3.pyx":615
  *                     for i in range(self.numthreads):
  *                         if bz3_last_error(self.states[i]) != BZ3_OK:
  *                             raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[i]))             # <<<<<<<<<<<<<<
  *                         # if PyByteArray_Resize(ret, PyByteArray_GET_SIZE(ret) + new_size + 8) < 0:
  *                         #     raise
  */
-            __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_i]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_i]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_Failed_to_encode_a_block_s, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
+            __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_Failed_to_encode_a_block_s, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 615, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_Raise(__pyx_t_1, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __PYX_ERR(0, 616, __pyx_L1_error)
+            __PYX_ERR(0, 615, __pyx_L1_error)
 
-            /* "bz3/backends/cython/_bz3.pyx":615
+            /* "bz3/backends/cython/_bz3.pyx":614
  *                     bz3_encode_blocks(self.states, self.buffers, self.sizes, <int32_t>self.numthreads)
  *                     for i in range(self.numthreads):
  *                         if bz3_last_error(self.states[i]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                             raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[i]))
  *                         # if PyByteArray_Resize(ret, PyByteArray_GET_SIZE(ret) + new_size + 8) < 0:
  */
           }
 
-          /* "bz3/backends/cython/_bz3.pyx":619
+          /* "bz3/backends/cython/_bz3.pyx":618
  *                         # if PyByteArray_Resize(ret, PyByteArray_GET_SIZE(ret) + new_size + 8) < 0:
  *                         #     raise
  *                         ret.extend((self.sizes[i] + 8)*b"\x00")             # <<<<<<<<<<<<<<
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-8]), self.sizes[i])
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-4]), self.block_size)
  */
-          __pyx_t_1 = __Pyx_PyInt_From_long(((__pyx_v_self->sizes[__pyx_v_i]) + 8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyInt_From_long(((__pyx_v_self->sizes[__pyx_v_i]) + 8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_kp_b__5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_kp_b__5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 618, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-          /* "bz3/backends/cython/_bz3.pyx":620
+          /* "bz3/backends/cython/_bz3.pyx":619
  *                         #     raise
  *                         ret.extend((self.sizes[i] + 8)*b"\x00")
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-8]), self.sizes[i])             # <<<<<<<<<<<<<<
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-4]), self.block_size)
  *                         memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]]), self.buffers[i], <size_t>self.sizes[i])
  */
           write_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_v_ret)[((PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_i])) - 8)]))), (__pyx_v_self->sizes[__pyx_v_i]));
 
-          /* "bz3/backends/cython/_bz3.pyx":621
+          /* "bz3/backends/cython/_bz3.pyx":620
  *                         ret.extend((self.sizes[i] + 8)*b"\x00")
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-8]), self.sizes[i])
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-4]), self.block_size)             # <<<<<<<<<<<<<<
  *                         memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]]), self.buffers[i], <size_t>self.sizes[i])
  * 
  */
           write_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_v_ret)[((PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_i])) - 4)]))), __pyx_v_self->block_size);
 
-          /* "bz3/backends/cython/_bz3.pyx":622
+          /* "bz3/backends/cython/_bz3.pyx":621
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-8]), self.sizes[i])
  *                         write_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]-4]), self.block_size)
  *                         memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]]), self.buffers[i], <size_t>self.sizes[i])             # <<<<<<<<<<<<<<
  * 
  *                     del self.uncompressed[:all_blocks_size]
  */
           (void)(memcpy((&(PyByteArray_AS_STRING(__pyx_v_ret)[(PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_i]))])), (__pyx_v_self->buffers[__pyx_v_i]), ((size_t)(__pyx_v_self->sizes[__pyx_v_i]))));
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":624
+        /* "bz3/backends/cython/_bz3.pyx":623
  *                         memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret)-self.sizes[i]]), self.buffers[i], <size_t>self.sizes[i])
  * 
  *                     del self.uncompressed[:all_blocks_size]             # <<<<<<<<<<<<<<
  *         return bytes(ret)
  * 
  */
         if (unlikely(__pyx_v_self->uncompressed == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 624, __pyx_L1_error)
+          __PYX_ERR(0, 623, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_DelSlice(__pyx_v_self->uncompressed, 0, __pyx_v_all_blocks_size, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 624, __pyx_L1_error)
+        if (__Pyx_PyObject_DelSlice(__pyx_v_self->uncompressed, 0, __pyx_v_all_blocks_size, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 623, __pyx_L1_error)
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":607
+      /* "bz3/backends/cython/_bz3.pyx":606
  *             # memcpy(&(PyByteArray_AS_STRING(self.uncompressed)[PyByteArray_GET_SIZE(self.uncompressed)-input_size]), &data[0], input_size) # todo? direct copy to bytearray
  *             self.uncompressed.extend(data)
  *             if PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # able to perform a compress             # <<<<<<<<<<<<<<
  *                 while PyByteArray_GET_SIZE(self.uncompressed) >= all_blocks_size:  # ensure fill all blocks
  *                     for i in range(self.numthreads):
  */
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":602
+    /* "bz3/backends/cython/_bz3.pyx":601
  *             self.have_magic_number = 1
  *         cdef uint32_t i
  *         if input_size > 0:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(self.uncompressed, input_size+PyByteArray_GET_SIZE(self.uncompressed)) < 0:
  *             #     raise
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":625
+  /* "bz3/backends/cython/_bz3.pyx":624
  * 
  *                     del self.uncompressed[:all_blocks_size]
  *         return bytes(ret)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bytes flush(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 624, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "bz3/backends/cython/_bz3.pyx":589
+  /* "bz3/backends/cython/_bz3.pyx":588
  *             self.old_sizes = NULL
  * 
  *     cpdef inline bytes compress(self, const uint8_t[::1] data):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t new_size
  */
 
@@ -12062,15 +12062,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compress (wrapper)", 0);
   assert(__pyx_arg_data); {
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint8_t__const__(__pyx_arg_data, 0); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 589, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint8_t__const__(__pyx_arg_data, 0); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 588, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpCompressor.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -12086,16 +12086,16 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compress", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 589, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_compress(__pyx_v_self, __pyx_v_data, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 588, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_compress(__pyx_v_self, __pyx_v_data, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12105,15 +12105,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_data, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":627
+/* "bz3/backends/cython/_bz3.pyx":626
  *         return bytes(ret)
  * 
  *     cpdef inline bytes flush(self):             # <<<<<<<<<<<<<<
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t new_size
  */
 
@@ -12134,303 +12134,303 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("flush", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":628
+  /* "bz3/backends/cython/_bz3.pyx":627
  * 
  *     cpdef inline bytes flush(self):
  *         cdef bytearray ret = bytearray()             # <<<<<<<<<<<<<<
  *         cdef int32_t new_size
  *         cdef int32_t remain_size = <int32_t>PyByteArray_GET_SIZE(self.uncompressed)
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":630
+  /* "bz3/backends/cython/_bz3.pyx":629
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t new_size
  *         cdef int32_t remain_size = <int32_t>PyByteArray_GET_SIZE(self.uncompressed)             # <<<<<<<<<<<<<<
  *         cdef:
  *             int i = 0  # thread count
  */
   __pyx_t_1 = __pyx_v_self->uncompressed;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_remain_size = ((int32_t)PyByteArray_GET_SIZE(__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":632
+  /* "bz3/backends/cython/_bz3.pyx":631
  *         cdef int32_t remain_size = <int32_t>PyByteArray_GET_SIZE(self.uncompressed)
  *         cdef:
  *             int i = 0  # thread count             # <<<<<<<<<<<<<<
  *             int j
  *         if self.uncompressed:  # will perform a compress
  */
   __pyx_v_i = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":634
+  /* "bz3/backends/cython/_bz3.pyx":633
  *             int i = 0  # thread count
  *             int j
  *         if self.uncompressed:  # will perform a compress             # <<<<<<<<<<<<<<
  *             while self.block_size * (i+1) < remain_size:
  *                 memcpy(self.buffers[i],
  */
   __pyx_t_2 = (__pyx_v_self->uncompressed != Py_None)&&(PyByteArray_GET_SIZE(__pyx_v_self->uncompressed) != 0);
   if (__pyx_t_2) {
 
-    /* "bz3/backends/cython/_bz3.pyx":635
+    /* "bz3/backends/cython/_bz3.pyx":634
  *             int j
  *         if self.uncompressed:  # will perform a compress
  *             while self.block_size * (i+1) < remain_size:             # <<<<<<<<<<<<<<
  *                 memcpy(self.buffers[i],
  *                        &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size],
  */
     while (1) {
       __pyx_t_2 = (((__pyx_v_self->block_size * (__pyx_v_i + 1)) < __pyx_v_remain_size) != 0);
       if (!__pyx_t_2) break;
 
-      /* "bz3/backends/cython/_bz3.pyx":637
+      /* "bz3/backends/cython/_bz3.pyx":636
  *             while self.block_size * (i+1) < remain_size:
  *                 memcpy(self.buffers[i],
  *                        &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size],             # <<<<<<<<<<<<<<
  *                        <size_t>self.block_size)
  *                 self.sizes[i] = self.old_sizes[i] = self.block_size
  */
       __pyx_t_1 = __pyx_v_self->uncompressed;
       __Pyx_INCREF(__pyx_t_1);
 
-      /* "bz3/backends/cython/_bz3.pyx":636
+      /* "bz3/backends/cython/_bz3.pyx":635
  *         if self.uncompressed:  # will perform a compress
  *             while self.block_size * (i+1) < remain_size:
  *                 memcpy(self.buffers[i],             # <<<<<<<<<<<<<<
  *                        &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size],
  *                        <size_t>self.block_size)
  */
       (void)(memcpy((__pyx_v_self->buffers[__pyx_v_i]), (&(PyByteArray_AS_STRING(__pyx_t_1)[(__pyx_v_i * __pyx_v_self->block_size)])), ((size_t)__pyx_v_self->block_size)));
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "bz3/backends/cython/_bz3.pyx":639
+      /* "bz3/backends/cython/_bz3.pyx":638
  *                        &PyByteArray_AS_STRING(self.uncompressed)[i*self.block_size],
  *                        <size_t>self.block_size)
  *                 self.sizes[i] = self.old_sizes[i] = self.block_size             # <<<<<<<<<<<<<<
  *                 # old_sizes[i] = self.block_size
  *                 i += 1
  */
       __pyx_t_3 = __pyx_v_self->block_size;
       (__pyx_v_self->sizes[__pyx_v_i]) = __pyx_t_3;
       (__pyx_v_self->old_sizes[__pyx_v_i]) = __pyx_t_3;
 
-      /* "bz3/backends/cython/_bz3.pyx":641
+      /* "bz3/backends/cython/_bz3.pyx":640
  *                 self.sizes[i] = self.old_sizes[i] = self.block_size
  *                 # old_sizes[i] = self.block_size
  *                 i += 1             # <<<<<<<<<<<<<<
  *             memcpy(self.buffers[i],
  *                    &PyByteArray_AS_STRING(self.uncompressed)[i * self.block_size],
  */
       __pyx_v_i = (__pyx_v_i + 1);
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":643
+    /* "bz3/backends/cython/_bz3.pyx":642
  *                 i += 1
  *             memcpy(self.buffers[i],
  *                    &PyByteArray_AS_STRING(self.uncompressed)[i * self.block_size],             # <<<<<<<<<<<<<<
  *                    <size_t> (remain_size-i*self.block_size))  # fill as many blocks as possible
  *             self.sizes[i] = self.old_sizes[i] = remain_size-i*self.block_size
  */
     __pyx_t_1 = __pyx_v_self->uncompressed;
     __Pyx_INCREF(__pyx_t_1);
 
-    /* "bz3/backends/cython/_bz3.pyx":642
+    /* "bz3/backends/cython/_bz3.pyx":641
  *                 # old_sizes[i] = self.block_size
  *                 i += 1
  *             memcpy(self.buffers[i],             # <<<<<<<<<<<<<<
  *                    &PyByteArray_AS_STRING(self.uncompressed)[i * self.block_size],
  *                    <size_t> (remain_size-i*self.block_size))  # fill as many blocks as possible
  */
     (void)(memcpy((__pyx_v_self->buffers[__pyx_v_i]), (&(PyByteArray_AS_STRING(__pyx_t_1)[(__pyx_v_i * __pyx_v_self->block_size)])), ((size_t)(__pyx_v_remain_size - (__pyx_v_i * __pyx_v_self->block_size)))));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bz3/backends/cython/_bz3.pyx":645
+    /* "bz3/backends/cython/_bz3.pyx":644
  *                    &PyByteArray_AS_STRING(self.uncompressed)[i * self.block_size],
  *                    <size_t> (remain_size-i*self.block_size))  # fill as many blocks as possible
  *             self.sizes[i] = self.old_sizes[i] = remain_size-i*self.block_size             # <<<<<<<<<<<<<<
  *             # old_sizes[i] = remain_size-i*self.block_size
  *             i += 1
  */
     __pyx_t_3 = (__pyx_v_remain_size - (__pyx_v_i * __pyx_v_self->block_size));
     (__pyx_v_self->sizes[__pyx_v_i]) = __pyx_t_3;
     (__pyx_v_self->old_sizes[__pyx_v_i]) = __pyx_t_3;
 
-    /* "bz3/backends/cython/_bz3.pyx":647
+    /* "bz3/backends/cython/_bz3.pyx":646
  *             self.sizes[i] = self.old_sizes[i] = remain_size-i*self.block_size
  *             # old_sizes[i] = remain_size-i*self.block_size
  *             i += 1             # <<<<<<<<<<<<<<
  *             bz3_encode_blocks(self.states, self.buffers, self.sizes, i)
  *             for j in range(i):  # state index
  */
     __pyx_v_i = (__pyx_v_i + 1);
 
-    /* "bz3/backends/cython/_bz3.pyx":648
+    /* "bz3/backends/cython/_bz3.pyx":647
  *             # old_sizes[i] = remain_size-i*self.block_size
  *             i += 1
  *             bz3_encode_blocks(self.states, self.buffers, self.sizes, i)             # <<<<<<<<<<<<<<
  *             for j in range(i):  # state index
  *                 if bz3_last_error(self.states[j]) != BZ3_OK:
  */
     __pyx_f_3bz3_8backends_6cython_4_bz3_bz3_encode_blocks(__pyx_v_self->states, __pyx_v_self->buffers, __pyx_v_self->sizes, __pyx_v_i);
 
-    /* "bz3/backends/cython/_bz3.pyx":649
+    /* "bz3/backends/cython/_bz3.pyx":648
  *             i += 1
  *             bz3_encode_blocks(self.states, self.buffers, self.sizes, i)
  *             for j in range(i):  # state index             # <<<<<<<<<<<<<<
  *                 if bz3_last_error(self.states[j]) != BZ3_OK:
  *                     raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[j]))
  */
     __pyx_t_4 = __pyx_v_i;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_j = __pyx_t_6;
 
-      /* "bz3/backends/cython/_bz3.pyx":650
+      /* "bz3/backends/cython/_bz3.pyx":649
  *             bz3_encode_blocks(self.states, self.buffers, self.sizes, i)
  *             for j in range(i):  # state index
  *                 if bz3_last_error(self.states[j]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[j]))
  * 
  */
       __pyx_t_2 = ((bz3_last_error((__pyx_v_self->states[__pyx_v_j])) != BZ3_OK) != 0);
       if (unlikely(__pyx_t_2)) {
 
-        /* "bz3/backends/cython/_bz3.pyx":651
+        /* "bz3/backends/cython/_bz3.pyx":650
  *             for j in range(i):  # state index
  *                 if bz3_last_error(self.states[j]) != BZ3_OK:
  *                     raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[j]))             # <<<<<<<<<<<<<<
  * 
  *                 ret.extend((self.sizes[j] + 8) * b"\x00")
  */
-        __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_j]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_j]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_7 = PyUnicode_Format(__pyx_kp_u_Failed_to_encode_a_block_s, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 651, __pyx_L1_error)
+        __pyx_t_7 = PyUnicode_Format(__pyx_kp_u_Failed_to_encode_a_block_s, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 650, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __PYX_ERR(0, 651, __pyx_L1_error)
+        __PYX_ERR(0, 650, __pyx_L1_error)
 
-        /* "bz3/backends/cython/_bz3.pyx":650
+        /* "bz3/backends/cython/_bz3.pyx":649
  *             bz3_encode_blocks(self.states, self.buffers, self.sizes, i)
  *             for j in range(i):  # state index
  *                 if bz3_last_error(self.states[j]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[j]))
  * 
  */
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":653
+      /* "bz3/backends/cython/_bz3.pyx":652
  *                     raise ValueError("Failed to encode a block: %s" % bz3_strerror(self.states[j]))
  * 
  *                 ret.extend((self.sizes[j] + 8) * b"\x00")             # <<<<<<<<<<<<<<
  *                 write_neutral_s32(<uint8_t *> &(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j] - 8]),
  *                                   self.sizes[j])
  */
-      __pyx_t_1 = __Pyx_PyInt_From_long(((__pyx_v_self->sizes[__pyx_v_j]) + 8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_long(((__pyx_v_self->sizes[__pyx_v_j]) + 8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = PyNumber_Multiply(__pyx_t_1, __pyx_kp_b__5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_7 = PyNumber_Multiply(__pyx_t_1, __pyx_kp_b__5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 652, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "bz3/backends/cython/_bz3.pyx":654
+      /* "bz3/backends/cython/_bz3.pyx":653
  * 
  *                 ret.extend((self.sizes[j] + 8) * b"\x00")
  *                 write_neutral_s32(<uint8_t *> &(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j] - 8]),             # <<<<<<<<<<<<<<
  *                                   self.sizes[j])
  *                 write_neutral_s32(<uint8_t *> &(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j] - 4]),
  */
       write_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_v_ret)[((PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_j])) - 8)]))), (__pyx_v_self->sizes[__pyx_v_j]));
 
-      /* "bz3/backends/cython/_bz3.pyx":656
+      /* "bz3/backends/cython/_bz3.pyx":655
  *                 write_neutral_s32(<uint8_t *> &(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j] - 8]),
  *                                   self.sizes[j])
  *                 write_neutral_s32(<uint8_t *> &(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j] - 4]),             # <<<<<<<<<<<<<<
  *                                   self.old_sizes[j])
  *                 memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j]]), self.buffers[j],
  */
       write_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_v_ret)[((PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_j])) - 4)]))), (__pyx_v_self->old_sizes[__pyx_v_j]));
 
-      /* "bz3/backends/cython/_bz3.pyx":658
+      /* "bz3/backends/cython/_bz3.pyx":657
  *                 write_neutral_s32(<uint8_t *> &(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j] - 4]),
  *                                   self.old_sizes[j])
  *                 memcpy(&(PyByteArray_AS_STRING(ret)[PyByteArray_GET_SIZE(ret) - self.sizes[j]]), self.buffers[j],             # <<<<<<<<<<<<<<
  *                        <size_t> self.sizes[j])
  * 
  */
       (void)(memcpy((&(PyByteArray_AS_STRING(__pyx_v_ret)[(PyByteArray_GET_SIZE(__pyx_v_ret) - (__pyx_v_self->sizes[__pyx_v_j]))])), (__pyx_v_self->buffers[__pyx_v_j]), ((size_t)(__pyx_v_self->sizes[__pyx_v_j]))));
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":661
+    /* "bz3/backends/cython/_bz3.pyx":660
  *                        <size_t> self.sizes[j])
  * 
  *             self.uncompressed.clear()             # <<<<<<<<<<<<<<
  *         return bytes(ret)
  * 
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->uncompressed, __pyx_n_s_clear); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 661, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->uncompressed, __pyx_n_s_clear); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 661, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bz3/backends/cython/_bz3.pyx":634
+    /* "bz3/backends/cython/_bz3.pyx":633
  *             int i = 0  # thread count
  *             int j
  *         if self.uncompressed:  # will perform a compress             # <<<<<<<<<<<<<<
  *             while self.block_size * (i+1) < remain_size:
  *                 memcpy(self.buffers[i],
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":662
+  /* "bz3/backends/cython/_bz3.pyx":661
  * 
  *             self.uncompressed.clear()
  *         return bytes(ret)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline list error(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 661, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "bz3/backends/cython/_bz3.pyx":627
+  /* "bz3/backends/cython/_bz3.pyx":626
  *         return bytes(ret)
  * 
  *     cpdef inline bytes flush(self):             # <<<<<<<<<<<<<<
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t new_size
  */
 
@@ -12467,15 +12467,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("flush", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_flush(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_flush(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 626, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12484,15 +12484,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":664
+/* "bz3/backends/cython/_bz3.pyx":663
  *         return bytes(ret)
  * 
  *     cpdef inline list error(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         cdef list ret = []
  */
 
@@ -12510,90 +12510,90 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":666
+  /* "bz3/backends/cython/_bz3.pyx":665
  *     cpdef inline list error(self):
  *         cdef uint32_t i
  *         cdef list ret = []             # <<<<<<<<<<<<<<
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 666, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":667
+  /* "bz3/backends/cython/_bz3.pyx":666
  *         cdef uint32_t i
  *         cdef list ret = []
  *         for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  *                 ret.append((<bytes>bz3_strerror(self.states[i])).decode())
  */
   __pyx_t_2 = __pyx_v_self->numthreads;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "bz3/backends/cython/_bz3.pyx":668
+    /* "bz3/backends/cython/_bz3.pyx":667
  *         cdef list ret = []
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                 ret.append((<bytes>bz3_strerror(self.states[i])).decode())
  *         return ret
  */
     __pyx_t_5 = ((bz3_last_error((__pyx_v_self->states[__pyx_v_i])) != BZ3_OK) != 0);
     if (__pyx_t_5) {
 
-      /* "bz3/backends/cython/_bz3.pyx":669
+      /* "bz3/backends/cython/_bz3.pyx":668
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  *                 ret.append((<bytes>bz3_strerror(self.states[i])).decode())             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
-      __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_i]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_i]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 668, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (unlikely(__pyx_t_1 == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
-        __PYX_ERR(0, 669, __pyx_L1_error)
+        __PYX_ERR(0, 668, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 669, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 668, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_ret, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 669, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_ret, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 668, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "bz3/backends/cython/_bz3.pyx":668
+      /* "bz3/backends/cython/_bz3.pyx":667
  *         cdef list ret = []
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                 ret.append((<bytes>bz3_strerror(self.states[i])).decode())
  *         return ret
  */
     }
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":670
+  /* "bz3/backends/cython/_bz3.pyx":669
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  *                 ret.append((<bytes>bz3_strerror(self.states[i])).decode())
  *         return ret             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ret);
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "bz3/backends/cython/_bz3.pyx":664
+  /* "bz3/backends/cython/_bz3.pyx":663
  *         return bytes(ret)
  * 
  *     cpdef inline list error(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         cdef list ret = []
  */
 
@@ -12629,15 +12629,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_error(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 664, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_16BZ3OmpCompressor_error(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12855,15 +12855,15 @@
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpCompressor.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":673
+/* "bz3/backends/cython/_bz3.pyx":672
  * 
  * 
  * cdef void bz3_decode_blocks(bz3_state ** states, uint8_t ** buffers, int32_t* sizes, int32_t* orig_size, int32_t numthreads):             # <<<<<<<<<<<<<<
  *     cdef int32_t i
  *     for i in prange(numthreads, nogil=True, schedule='static', num_threads=numthreads):
  */
 
@@ -12871,15 +12871,15 @@
   int32_t __pyx_v_i;
   __Pyx_RefNannyDeclarations
   int32_t __pyx_t_1;
   int32_t __pyx_t_2;
   int32_t __pyx_t_3;
   __Pyx_RefNannySetupContext("bz3_decode_blocks", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":675
+  /* "bz3/backends/cython/_bz3.pyx":674
  * cdef void bz3_decode_blocks(bz3_state ** states, uint8_t ** buffers, int32_t* sizes, int32_t* orig_size, int32_t numthreads):
  *     cdef int32_t i
  *     for i in prange(numthreads, nogil=True, schedule='static', num_threads=numthreads):             # <<<<<<<<<<<<<<
  *         bz3_decode_block(states[i], buffers[i], sizes[i], orig_size[i])
  * 
  */
   {
@@ -12908,15 +12908,15 @@
                     #ifdef _OPENMP
                     #pragma omp for firstprivate(__pyx_v_i) lastprivate(__pyx_v_i) schedule(static)
                     #endif /* _OPENMP */
                     for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_3; __pyx_t_2++){
                         {
                             __pyx_v_i = (int32_t)(0 + 1 * __pyx_t_2);
 
-                            /* "bz3/backends/cython/_bz3.pyx":676
+                            /* "bz3/backends/cython/_bz3.pyx":675
  *     cdef int32_t i
  *     for i in prange(numthreads, nogil=True, schedule='static', num_threads=numthreads):
  *         bz3_decode_block(states[i], buffers[i], sizes[i], orig_size[i])             # <<<<<<<<<<<<<<
  * 
  * 
  */
                             (void)(bz3_decode_block((__pyx_v_states[__pyx_v_i]), (__pyx_v_buffers[__pyx_v_i]), (__pyx_v_sizes[__pyx_v_i]), (__pyx_v_orig_size[__pyx_v_i])));
@@ -12929,15 +12929,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":675
+      /* "bz3/backends/cython/_bz3.pyx":674
  * cdef void bz3_decode_blocks(bz3_state ** states, uint8_t ** buffers, int32_t* sizes, int32_t* orig_size, int32_t numthreads):
  *     cdef int32_t i
  *     for i in prange(numthreads, nogil=True, schedule='static', num_threads=numthreads):             # <<<<<<<<<<<<<<
  *         bz3_decode_block(states[i], buffers[i], sizes[i], orig_size[i])
  * 
  */
       /*finally:*/ {
@@ -12948,27 +12948,27 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":673
+  /* "bz3/backends/cython/_bz3.pyx":672
  * 
  * 
  * cdef void bz3_decode_blocks(bz3_state ** states, uint8_t ** buffers, int32_t* sizes, int32_t* orig_size, int32_t numthreads):             # <<<<<<<<<<<<<<
  *     cdef int32_t i
  *     for i in prange(numthreads, nogil=True, schedule='static', num_threads=numthreads):
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bz3/backends/cython/_bz3.pyx":694
+/* "bz3/backends/cython/_bz3.pyx":693
  *         readonly bint ignore_error  # decode
  * 
  *     cdef inline int init_state(self, int32_t block_size) except -1:             # <<<<<<<<<<<<<<
  *         """should exec only once"""
  *         if not self.states:
  */
 
@@ -12987,145 +12987,145 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("init_state", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":696
+  /* "bz3/backends/cython/_bz3.pyx":695
  *     cdef inline int init_state(self, int32_t block_size) except -1:
  *         """should exec only once"""
  *         if not self.states:             # <<<<<<<<<<<<<<
  *             self.states = <bz3_state **> PyMem_Calloc(self.numthreads, sizeof(bz3_state *))  # prepare the array
  *             if not self.states:
  */
   __pyx_t_1 = ((!(__pyx_v_self->states != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":697
+    /* "bz3/backends/cython/_bz3.pyx":696
  *         """should exec only once"""
  *         if not self.states:
  *             self.states = <bz3_state **> PyMem_Calloc(self.numthreads, sizeof(bz3_state *))  # prepare the array             # <<<<<<<<<<<<<<
  *             if not self.states:
  *                 raise MemoryError
  */
     __pyx_v_self->states = ((struct bz3_state **)PyMem_Calloc(__pyx_v_self->numthreads, (sizeof(struct bz3_state *))));
 
-    /* "bz3/backends/cython/_bz3.pyx":698
+    /* "bz3/backends/cython/_bz3.pyx":697
  *         if not self.states:
  *             self.states = <bz3_state **> PyMem_Calloc(self.numthreads, sizeof(bz3_state *))  # prepare the array
  *             if not self.states:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.states)
  */
     __pyx_t_1 = ((!(__pyx_v_self->states != 0)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "bz3/backends/cython/_bz3.pyx":699
+      /* "bz3/backends/cython/_bz3.pyx":698
  *             self.states = <bz3_state **> PyMem_Calloc(self.numthreads, sizeof(bz3_state *))  # prepare the array
  *             if not self.states:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Malloc %p\n", self.states)
  *         if not self.buffers:
  */
-      PyErr_NoMemory(); __PYX_ERR(0, 699, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(0, 698, __pyx_L1_error)
 
-      /* "bz3/backends/cython/_bz3.pyx":698
+      /* "bz3/backends/cython/_bz3.pyx":697
  *         if not self.states:
  *             self.states = <bz3_state **> PyMem_Calloc(self.numthreads, sizeof(bz3_state *))  # prepare the array
  *             if not self.states:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.states)
  */
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":700
+    /* "bz3/backends/cython/_bz3.pyx":699
  *             if not self.states:
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.states)             # <<<<<<<<<<<<<<
  *         if not self.buffers:
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))
  */
     MEMLOG(((char const *)"PyMem_Malloc %p\n"), __pyx_v_self->states);
 
-    /* "bz3/backends/cython/_bz3.pyx":696
+    /* "bz3/backends/cython/_bz3.pyx":695
  *     cdef inline int init_state(self, int32_t block_size) except -1:
  *         """should exec only once"""
  *         if not self.states:             # <<<<<<<<<<<<<<
  *             self.states = <bz3_state **> PyMem_Calloc(self.numthreads, sizeof(bz3_state *))  # prepare the array
  *             if not self.states:
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":701
+  /* "bz3/backends/cython/_bz3.pyx":700
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.states)
  *         if not self.buffers:             # <<<<<<<<<<<<<<
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))
  *             if not self.buffers:
  */
   __pyx_t_1 = ((!(__pyx_v_self->buffers != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":702
+    /* "bz3/backends/cython/_bz3.pyx":701
  *             MEMLOG("PyMem_Malloc %p\n", self.states)
  *         if not self.buffers:
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))             # <<<<<<<<<<<<<<
  *             if not self.buffers:
  *                 raise MemoryError
  */
     __pyx_v_self->buffers = ((uint8_t **)PyMem_Calloc(__pyx_v_self->numthreads, (sizeof(uint8_t *))));
 
-    /* "bz3/backends/cython/_bz3.pyx":703
+    /* "bz3/backends/cython/_bz3.pyx":702
  *         if not self.buffers:
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))
  *             if not self.buffers:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)
  */
     __pyx_t_1 = ((!(__pyx_v_self->buffers != 0)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "bz3/backends/cython/_bz3.pyx":704
+      /* "bz3/backends/cython/_bz3.pyx":703
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))
  *             if not self.buffers:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)
  *         cdef uint32_t i
  */
-      PyErr_NoMemory(); __PYX_ERR(0, 704, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(0, 703, __pyx_L1_error)
 
-      /* "bz3/backends/cython/_bz3.pyx":703
+      /* "bz3/backends/cython/_bz3.pyx":702
  *         if not self.buffers:
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))
  *             if not self.buffers:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)
  */
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":705
+    /* "bz3/backends/cython/_bz3.pyx":704
  *             if not self.buffers:
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         try:
  */
     MEMLOG(((char const *)"PyMem_Malloc %p\n"), __pyx_v_self->buffers);
 
-    /* "bz3/backends/cython/_bz3.pyx":701
+    /* "bz3/backends/cython/_bz3.pyx":700
  *                 raise MemoryError
  *             MEMLOG("PyMem_Malloc %p\n", self.states)
  *         if not self.buffers:             # <<<<<<<<<<<<<<
  *             self.buffers = <uint8_t **> PyMem_Calloc(self.numthreads, sizeof(uint8_t *))
  *             if not self.buffers:
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":707
+  /* "bz3/backends/cython/_bz3.pyx":706
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)
  *         cdef uint32_t i
  *         try:             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 self.states[i] = bz3_new(block_size)
  */
   {
@@ -13133,215 +13133,215 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "bz3/backends/cython/_bz3.pyx":708
+      /* "bz3/backends/cython/_bz3.pyx":707
  *         cdef uint32_t i
  *         try:
  *             for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *                 self.states[i] = bz3_new(block_size)
  *                 if self.states[i] == NULL:
  */
       __pyx_t_5 = __pyx_v_self->numthreads;
       __pyx_t_6 = __pyx_t_5;
       for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
         __pyx_v_i = __pyx_t_7;
 
-        /* "bz3/backends/cython/_bz3.pyx":709
+        /* "bz3/backends/cython/_bz3.pyx":708
  *         try:
  *             for i in range(self.numthreads):
  *                 self.states[i] = bz3_new(block_size)             # <<<<<<<<<<<<<<
  *                 if self.states[i] == NULL:
  *                     raise MemoryError("Failed to create a block encoder state")  # todo
  */
         (__pyx_v_self->states[__pyx_v_i]) = bz3_new(__pyx_v_block_size);
 
-        /* "bz3/backends/cython/_bz3.pyx":710
+        /* "bz3/backends/cython/_bz3.pyx":709
  *             for i in range(self.numthreads):
  *                 self.states[i] = bz3_new(block_size)
  *                 if self.states[i] == NULL:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Failed to create a block encoder state")  # todo
  *                 MEMLOG("bz3_new %p\n", self.states[i])
  */
         __pyx_t_1 = (((__pyx_v_self->states[__pyx_v_i]) == NULL) != 0);
         if (unlikely(__pyx_t_1)) {
 
-          /* "bz3/backends/cython/_bz3.pyx":711
+          /* "bz3/backends/cython/_bz3.pyx":710
  *                 self.states[i] = bz3_new(block_size)
  *                 if self.states[i] == NULL:
  *                     raise MemoryError("Failed to create a block encoder state")  # todo             # <<<<<<<<<<<<<<
  *                 MEMLOG("bz3_new %p\n", self.states[i])
  *                 self.buffers[i] = <uint8_t *> PyMem_Malloc(bz3_bound(block_size))
  */
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 711, __pyx_L7_error)
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 710, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_Raise(__pyx_t_8, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          __PYX_ERR(0, 711, __pyx_L7_error)
+          __PYX_ERR(0, 710, __pyx_L7_error)
 
-          /* "bz3/backends/cython/_bz3.pyx":710
+          /* "bz3/backends/cython/_bz3.pyx":709
  *             for i in range(self.numthreads):
  *                 self.states[i] = bz3_new(block_size)
  *                 if self.states[i] == NULL:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Failed to create a block encoder state")  # todo
  *                 MEMLOG("bz3_new %p\n", self.states[i])
  */
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":712
+        /* "bz3/backends/cython/_bz3.pyx":711
  *                 if self.states[i] == NULL:
  *                     raise MemoryError("Failed to create a block encoder state")  # todo
  *                 MEMLOG("bz3_new %p\n", self.states[i])             # <<<<<<<<<<<<<<
  *                 self.buffers[i] = <uint8_t *> PyMem_Malloc(bz3_bound(block_size))
  *                 if self.buffers[i] == NULL:
  */
         MEMLOG(((char const *)"bz3_new %p\n"), (__pyx_v_self->states[__pyx_v_i]));
 
-        /* "bz3/backends/cython/_bz3.pyx":713
+        /* "bz3/backends/cython/_bz3.pyx":712
  *                     raise MemoryError("Failed to create a block encoder state")  # todo
  *                 MEMLOG("bz3_new %p\n", self.states[i])
  *                 self.buffers[i] = <uint8_t *> PyMem_Malloc(bz3_bound(block_size))             # <<<<<<<<<<<<<<
  *                 if self.buffers[i] == NULL:
  *                     raise MemoryError("Failed to allocate memory")
  */
         (__pyx_v_self->buffers[__pyx_v_i]) = ((uint8_t *)PyMem_Malloc(bz3_bound(__pyx_v_block_size)));
 
-        /* "bz3/backends/cython/_bz3.pyx":714
+        /* "bz3/backends/cython/_bz3.pyx":713
  *                 MEMLOG("bz3_new %p\n", self.states[i])
  *                 self.buffers[i] = <uint8_t *> PyMem_Malloc(bz3_bound(block_size))
  *                 if self.buffers[i] == NULL:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Failed to allocate memory")
  *                 MEMLOG("PyMem_Malloc %p\n", self.buffers[i])
  */
         __pyx_t_1 = (((__pyx_v_self->buffers[__pyx_v_i]) == NULL) != 0);
         if (unlikely(__pyx_t_1)) {
 
-          /* "bz3/backends/cython/_bz3.pyx":715
+          /* "bz3/backends/cython/_bz3.pyx":714
  *                 self.buffers[i] = <uint8_t *> PyMem_Malloc(bz3_bound(block_size))
  *                 if self.buffers[i] == NULL:
  *                     raise MemoryError("Failed to allocate memory")             # <<<<<<<<<<<<<<
  *                 MEMLOG("PyMem_Malloc %p\n", self.buffers[i])
  *         except:
  */
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 715, __pyx_L7_error)
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 714, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_Raise(__pyx_t_8, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          __PYX_ERR(0, 715, __pyx_L7_error)
+          __PYX_ERR(0, 714, __pyx_L7_error)
 
-          /* "bz3/backends/cython/_bz3.pyx":714
+          /* "bz3/backends/cython/_bz3.pyx":713
  *                 MEMLOG("bz3_new %p\n", self.states[i])
  *                 self.buffers[i] = <uint8_t *> PyMem_Malloc(bz3_bound(block_size))
  *                 if self.buffers[i] == NULL:             # <<<<<<<<<<<<<<
  *                     raise MemoryError("Failed to allocate memory")
  *                 MEMLOG("PyMem_Malloc %p\n", self.buffers[i])
  */
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":716
+        /* "bz3/backends/cython/_bz3.pyx":715
  *                 if self.buffers[i] == NULL:
  *                     raise MemoryError("Failed to allocate memory")
  *                 MEMLOG("PyMem_Malloc %p\n", self.buffers[i])             # <<<<<<<<<<<<<<
  *         except:
  *             self.free_states()
  */
         MEMLOG(((char const *)"PyMem_Malloc %p\n"), (__pyx_v_self->buffers[__pyx_v_i]));
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":707
+      /* "bz3/backends/cython/_bz3.pyx":706
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)
  *         cdef uint32_t i
  *         try:             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 self.states[i] = bz3_new(block_size)
  */
     }
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L12_try_end;
     __pyx_L7_error:;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "bz3/backends/cython/_bz3.pyx":717
+    /* "bz3/backends/cython/_bz3.pyx":716
  *                     raise MemoryError("Failed to allocate memory")
  *                 MEMLOG("PyMem_Malloc %p\n", self.buffers[i])
  *         except:             # <<<<<<<<<<<<<<
  *             self.free_states()
  *             self.free_buffers()
  */
     /*except:*/ {
       __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpDecompressor.init_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10) < 0) __PYX_ERR(0, 717, __pyx_L9_except_error)
+      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10) < 0) __PYX_ERR(0, 716, __pyx_L9_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_10);
 
-      /* "bz3/backends/cython/_bz3.pyx":718
+      /* "bz3/backends/cython/_bz3.pyx":717
  *                 MEMLOG("PyMem_Malloc %p\n", self.buffers[i])
  *         except:
  *             self.free_states()             # <<<<<<<<<<<<<<
  *             self.free_buffers()
  *             raise
  */
       __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_free_states(__pyx_v_self);
 
-      /* "bz3/backends/cython/_bz3.pyx":719
+      /* "bz3/backends/cython/_bz3.pyx":718
  *         except:
  *             self.free_states()
  *             self.free_buffers()             # <<<<<<<<<<<<<<
  *             raise
  *         self.block_size = block_size
  */
       __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_free_buffers(__pyx_v_self);
 
-      /* "bz3/backends/cython/_bz3.pyx":720
+      /* "bz3/backends/cython/_bz3.pyx":719
  *             self.free_states()
  *             self.free_buffers()
  *             raise             # <<<<<<<<<<<<<<
  *         self.block_size = block_size
  * 
  */
       __Pyx_GIVEREF(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_9);
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_ErrRestoreWithState(__pyx_t_8, __pyx_t_9, __pyx_t_10);
       __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; 
-      __PYX_ERR(0, 720, __pyx_L9_except_error)
+      __PYX_ERR(0, 719, __pyx_L9_except_error)
     }
     __pyx_L9_except_error:;
 
-    /* "bz3/backends/cython/_bz3.pyx":707
+    /* "bz3/backends/cython/_bz3.pyx":706
  *             MEMLOG("PyMem_Malloc %p\n", self.buffers)
  *         cdef uint32_t i
  *         try:             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 self.states[i] = bz3_new(block_size)
  */
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L12_try_end:;
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":721
+  /* "bz3/backends/cython/_bz3.pyx":720
  *             self.free_buffers()
  *             raise
  *         self.block_size = block_size             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self,  uint32_t numthreads, bint ignore_error = False):
  */
   __pyx_v_self->block_size = __pyx_v_block_size;
 
-  /* "bz3/backends/cython/_bz3.pyx":694
+  /* "bz3/backends/cython/_bz3.pyx":693
  *         readonly bint ignore_error  # decode
  * 
  *     cdef inline int init_state(self, int32_t block_size) except -1:             # <<<<<<<<<<<<<<
  *         """should exec only once"""
  *         if not self.states:
  */
 
@@ -13355,15 +13355,15 @@
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpDecompressor.init_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":723
+/* "bz3/backends/cython/_bz3.pyx":722
  *         self.block_size = block_size
  * 
  *     def __cinit__(self,  uint32_t numthreads, bint ignore_error = False):             # <<<<<<<<<<<<<<
  *         self.states = NULL
  *         self.buffers = NULL
  */
 
@@ -13401,35 +13401,35 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ignore_error);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 723, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 722, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_numthreads = __Pyx_PyInt_As_uint32_t(values[0]); if (unlikely((__pyx_v_numthreads == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
+    __pyx_v_numthreads = __Pyx_PyInt_As_uint32_t(values[0]); if (unlikely((__pyx_v_numthreads == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_ignore_error = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_ignore_error == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L3_error)
+      __pyx_v_ignore_error = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_ignore_error == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L3_error)
     } else {
       __pyx_v_ignore_error = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 723, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 722, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpDecompressor.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor___cinit__(((struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *)__pyx_v_self), __pyx_v_numthreads, __pyx_v_ignore_error);
 
@@ -13444,194 +13444,194 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":724
+  /* "bz3/backends/cython/_bz3.pyx":723
  * 
  *     def __cinit__(self,  uint32_t numthreads, bint ignore_error = False):
  *         self.states = NULL             # <<<<<<<<<<<<<<
  *         self.buffers = NULL
  *         self.unused = bytearray()
  */
   __pyx_v_self->states = NULL;
 
-  /* "bz3/backends/cython/_bz3.pyx":725
+  /* "bz3/backends/cython/_bz3.pyx":724
  *     def __cinit__(self,  uint32_t numthreads, bint ignore_error = False):
  *         self.states = NULL
  *         self.buffers = NULL             # <<<<<<<<<<<<<<
  *         self.unused = bytearray()
  *         self.have_magic_number = 0 # magic number
  */
   __pyx_v_self->buffers = NULL;
 
-  /* "bz3/backends/cython/_bz3.pyx":726
+  /* "bz3/backends/cython/_bz3.pyx":725
  *         self.states = NULL
  *         self.buffers = NULL
  *         self.unused = bytearray()             # <<<<<<<<<<<<<<
  *         self.have_magic_number = 0 # magic number
  *         self.numthreads = numthreads
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 725, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->unused);
   __Pyx_DECREF(__pyx_v_self->unused);
   __pyx_v_self->unused = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":727
+  /* "bz3/backends/cython/_bz3.pyx":726
  *         self.buffers = NULL
  *         self.unused = bytearray()
  *         self.have_magic_number = 0 # magic number             # <<<<<<<<<<<<<<
  *         self.numthreads = numthreads
  *         self.ignore_error = ignore_error
  */
   __pyx_v_self->have_magic_number = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":728
+  /* "bz3/backends/cython/_bz3.pyx":727
  *         self.unused = bytearray()
  *         self.have_magic_number = 0 # magic number
  *         self.numthreads = numthreads             # <<<<<<<<<<<<<<
  *         self.ignore_error = ignore_error
  * 
  */
   __pyx_v_self->numthreads = __pyx_v_numthreads;
 
-  /* "bz3/backends/cython/_bz3.pyx":729
+  /* "bz3/backends/cython/_bz3.pyx":728
  *         self.have_magic_number = 0 # magic number
  *         self.numthreads = numthreads
  *         self.ignore_error = ignore_error             # <<<<<<<<<<<<<<
  * 
  *         self.sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  */
   __pyx_v_self->ignore_error = __pyx_v_ignore_error;
 
-  /* "bz3/backends/cython/_bz3.pyx":731
+  /* "bz3/backends/cython/_bz3.pyx":730
  *         self.ignore_error = ignore_error
  * 
  *         self.sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)             # <<<<<<<<<<<<<<
  *         if not self.sizes:
  *             raise MemoryError
  */
   __pyx_v_self->sizes = ((int32_t *)PyMem_Malloc(((sizeof(int32_t)) * __pyx_v_numthreads)));
 
-  /* "bz3/backends/cython/_bz3.pyx":732
+  /* "bz3/backends/cython/_bz3.pyx":731
  * 
  *         self.sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.sizes:             # <<<<<<<<<<<<<<
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)
  */
   __pyx_t_2 = ((!(__pyx_v_self->sizes != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "bz3/backends/cython/_bz3.pyx":733
+    /* "bz3/backends/cython/_bz3.pyx":732
  *         self.sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.sizes:
  *             raise MemoryError             # <<<<<<<<<<<<<<
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)
  *         self.old_sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 733, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 732, __pyx_L1_error)
 
-    /* "bz3/backends/cython/_bz3.pyx":732
+    /* "bz3/backends/cython/_bz3.pyx":731
  * 
  *         self.sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.sizes:             # <<<<<<<<<<<<<<
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":734
+  /* "bz3/backends/cython/_bz3.pyx":733
  *         if not self.sizes:
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)             # <<<<<<<<<<<<<<
  *         self.old_sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.old_sizes:
  */
   MEMLOG(((char const *)"PyMem_Malloc %p\n"), __pyx_v_self->sizes);
 
-  /* "bz3/backends/cython/_bz3.pyx":735
+  /* "bz3/backends/cython/_bz3.pyx":734
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)
  *         self.old_sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)             # <<<<<<<<<<<<<<
  *         if not self.old_sizes:
  *             PyMem_Free(self.sizes)
  */
   __pyx_v_self->old_sizes = ((int32_t *)PyMem_Malloc(((sizeof(int32_t)) * __pyx_v_numthreads)));
 
-  /* "bz3/backends/cython/_bz3.pyx":736
+  /* "bz3/backends/cython/_bz3.pyx":735
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)
  *         self.old_sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.old_sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.sizes)
  *             self.sizes = NULL
  */
   __pyx_t_2 = ((!(__pyx_v_self->old_sizes != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "bz3/backends/cython/_bz3.pyx":737
+    /* "bz3/backends/cython/_bz3.pyx":736
  *         self.old_sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.old_sizes:
  *             PyMem_Free(self.sizes)             # <<<<<<<<<<<<<<
  *             self.sizes = NULL
  *             raise MemoryError
  */
     PyMem_Free(__pyx_v_self->sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":738
+    /* "bz3/backends/cython/_bz3.pyx":737
  *         if not self.old_sizes:
  *             PyMem_Free(self.sizes)
  *             self.sizes = NULL             # <<<<<<<<<<<<<<
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.old_sizes)
  */
     __pyx_v_self->sizes = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":739
+    /* "bz3/backends/cython/_bz3.pyx":738
  *             PyMem_Free(self.sizes)
  *             self.sizes = NULL
  *             raise MemoryError             # <<<<<<<<<<<<<<
  *         MEMLOG("PyMem_Malloc %p\n", self.old_sizes)
  *         MEMLOG("BZ3OmpDecompressor __cinit__ %p\n", <void*>self)
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 739, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 738, __pyx_L1_error)
 
-    /* "bz3/backends/cython/_bz3.pyx":736
+    /* "bz3/backends/cython/_bz3.pyx":735
  *         MEMLOG("PyMem_Malloc %p\n", self.sizes)
  *         self.old_sizes = <int32_t *> PyMem_Malloc(sizeof(int32_t) * numthreads)
  *         if not self.old_sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.sizes)
  *             self.sizes = NULL
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":740
+  /* "bz3/backends/cython/_bz3.pyx":739
  *             self.sizes = NULL
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.old_sizes)             # <<<<<<<<<<<<<<
  *         MEMLOG("BZ3OmpDecompressor __cinit__ %p\n", <void*>self)
  * 
  */
   MEMLOG(((char const *)"PyMem_Malloc %p\n"), __pyx_v_self->old_sizes);
 
-  /* "bz3/backends/cython/_bz3.pyx":741
+  /* "bz3/backends/cython/_bz3.pyx":740
  *             raise MemoryError
  *         MEMLOG("PyMem_Malloc %p\n", self.old_sizes)
  *         MEMLOG("BZ3OmpDecompressor __cinit__ %p\n", <void*>self)             # <<<<<<<<<<<<<<
  * 
  *     cdef inline void free_states(self):
  */
   MEMLOG(((char const *)"BZ3OmpDecompressor __cinit__ %p\n"), ((void *)__pyx_v_self));
 
-  /* "bz3/backends/cython/_bz3.pyx":723
+  /* "bz3/backends/cython/_bz3.pyx":722
  *         self.block_size = block_size
  * 
  *     def __cinit__(self,  uint32_t numthreads, bint ignore_error = False):             # <<<<<<<<<<<<<<
  *         self.states = NULL
  *         self.buffers = NULL
  */
 
@@ -13643,15 +13643,15 @@
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpDecompressor.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":743
+/* "bz3/backends/cython/_bz3.pyx":742
  *         MEMLOG("BZ3OmpDecompressor __cinit__ %p\n", <void*>self)
  * 
  *     cdef inline void free_states(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         if self.states: # statesinit_states
  */
 
@@ -13660,105 +13660,105 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   uint32_t __pyx_t_2;
   uint32_t __pyx_t_3;
   uint32_t __pyx_t_4;
   __Pyx_RefNannySetupContext("free_states", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":745
+  /* "bz3/backends/cython/_bz3.pyx":744
  *     cdef inline void free_states(self):
  *         cdef uint32_t i
  *         if self.states: # statesinit_states             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 if self.states[i]:
  */
   __pyx_t_1 = (__pyx_v_self->states != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":746
+    /* "bz3/backends/cython/_bz3.pyx":745
  *         cdef uint32_t i
  *         if self.states: # statesinit_states
  *             for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *                 if self.states[i]:
  *                     bz3_free(self.states[i])
  */
     __pyx_t_2 = __pyx_v_self->numthreads;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "bz3/backends/cython/_bz3.pyx":747
+      /* "bz3/backends/cython/_bz3.pyx":746
  *         if self.states: # statesinit_states
  *             for i in range(self.numthreads):
  *                 if self.states[i]:             # <<<<<<<<<<<<<<
  *                     bz3_free(self.states[i])
  *                     MEMLOG("bz3_free %p\n", self.states[i])
  */
       __pyx_t_1 = ((__pyx_v_self->states[__pyx_v_i]) != 0);
       if (__pyx_t_1) {
 
-        /* "bz3/backends/cython/_bz3.pyx":748
+        /* "bz3/backends/cython/_bz3.pyx":747
  *             for i in range(self.numthreads):
  *                 if self.states[i]:
  *                     bz3_free(self.states[i])             # <<<<<<<<<<<<<<
  *                     MEMLOG("bz3_free %p\n", self.states[i])
  *                     self.states[i] = NULL
  */
         bz3_free((__pyx_v_self->states[__pyx_v_i]));
 
-        /* "bz3/backends/cython/_bz3.pyx":749
+        /* "bz3/backends/cython/_bz3.pyx":748
  *                 if self.states[i]:
  *                     bz3_free(self.states[i])
  *                     MEMLOG("bz3_free %p\n", self.states[i])             # <<<<<<<<<<<<<<
  *                     self.states[i] = NULL
  * 
  */
         MEMLOG(((char const *)"bz3_free %p\n"), (__pyx_v_self->states[__pyx_v_i]));
 
-        /* "bz3/backends/cython/_bz3.pyx":750
+        /* "bz3/backends/cython/_bz3.pyx":749
  *                     bz3_free(self.states[i])
  *                     MEMLOG("bz3_free %p\n", self.states[i])
  *                     self.states[i] = NULL             # <<<<<<<<<<<<<<
  * 
  *     cdef inline void free_buffers(self):
  */
         (__pyx_v_self->states[__pyx_v_i]) = NULL;
 
-        /* "bz3/backends/cython/_bz3.pyx":747
+        /* "bz3/backends/cython/_bz3.pyx":746
  *         if self.states: # statesinit_states
  *             for i in range(self.numthreads):
  *                 if self.states[i]:             # <<<<<<<<<<<<<<
  *                     bz3_free(self.states[i])
  *                     MEMLOG("bz3_free %p\n", self.states[i])
  */
       }
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":745
+    /* "bz3/backends/cython/_bz3.pyx":744
  *     cdef inline void free_states(self):
  *         cdef uint32_t i
  *         if self.states: # statesinit_states             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 if self.states[i]:
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":743
+  /* "bz3/backends/cython/_bz3.pyx":742
  *         MEMLOG("BZ3OmpDecompressor __cinit__ %p\n", <void*>self)
  * 
  *     cdef inline void free_states(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         if self.states: # statesinit_states
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bz3/backends/cython/_bz3.pyx":752
+/* "bz3/backends/cython/_bz3.pyx":751
  *                     self.states[i] = NULL
  * 
  *     cdef inline void free_buffers(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i # statesinit_states
  *         if self.buffers: # statesinit_states
  */
 
@@ -13767,105 +13767,105 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   uint32_t __pyx_t_2;
   uint32_t __pyx_t_3;
   uint32_t __pyx_t_4;
   __Pyx_RefNannySetupContext("free_buffers", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":754
+  /* "bz3/backends/cython/_bz3.pyx":753
  *     cdef inline void free_buffers(self):
  *         cdef uint32_t i # statesinit_states
  *         if self.buffers: # statesinit_states             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 if self.buffers[i]:
  */
   __pyx_t_1 = (__pyx_v_self->buffers != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":755
+    /* "bz3/backends/cython/_bz3.pyx":754
  *         cdef uint32_t i # statesinit_states
  *         if self.buffers: # statesinit_states
  *             for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *                 if self.buffers[i]:
  *                     PyMem_Free(self.buffers[i])
  */
     __pyx_t_2 = __pyx_v_self->numthreads;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "bz3/backends/cython/_bz3.pyx":756
+      /* "bz3/backends/cython/_bz3.pyx":755
  *         if self.buffers: # statesinit_states
  *             for i in range(self.numthreads):
  *                 if self.buffers[i]:             # <<<<<<<<<<<<<<
  *                     PyMem_Free(self.buffers[i])
  *                     MEMLOG("PyMem_Free %p\n", self.buffers[i])
  */
       __pyx_t_1 = ((__pyx_v_self->buffers[__pyx_v_i]) != 0);
       if (__pyx_t_1) {
 
-        /* "bz3/backends/cython/_bz3.pyx":757
+        /* "bz3/backends/cython/_bz3.pyx":756
  *             for i in range(self.numthreads):
  *                 if self.buffers[i]:
  *                     PyMem_Free(self.buffers[i])             # <<<<<<<<<<<<<<
  *                     MEMLOG("PyMem_Free %p\n", self.buffers[i])
  *                     self.buffers[i] = NULL
  */
         PyMem_Free((__pyx_v_self->buffers[__pyx_v_i]));
 
-        /* "bz3/backends/cython/_bz3.pyx":758
+        /* "bz3/backends/cython/_bz3.pyx":757
  *                 if self.buffers[i]:
  *                     PyMem_Free(self.buffers[i])
  *                     MEMLOG("PyMem_Free %p\n", self.buffers[i])             # <<<<<<<<<<<<<<
  *                     self.buffers[i] = NULL
  * 
  */
         MEMLOG(((char const *)"PyMem_Free %p\n"), (__pyx_v_self->buffers[__pyx_v_i]));
 
-        /* "bz3/backends/cython/_bz3.pyx":759
+        /* "bz3/backends/cython/_bz3.pyx":758
  *                     PyMem_Free(self.buffers[i])
  *                     MEMLOG("PyMem_Free %p\n", self.buffers[i])
  *                     self.buffers[i] = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
         (__pyx_v_self->buffers[__pyx_v_i]) = NULL;
 
-        /* "bz3/backends/cython/_bz3.pyx":756
+        /* "bz3/backends/cython/_bz3.pyx":755
  *         if self.buffers: # statesinit_states
  *             for i in range(self.numthreads):
  *                 if self.buffers[i]:             # <<<<<<<<<<<<<<
  *                     PyMem_Free(self.buffers[i])
  *                     MEMLOG("PyMem_Free %p\n", self.buffers[i])
  */
       }
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":754
+    /* "bz3/backends/cython/_bz3.pyx":753
  *     cdef inline void free_buffers(self):
  *         cdef uint32_t i # statesinit_states
  *         if self.buffers: # statesinit_states             # <<<<<<<<<<<<<<
  *             for i in range(self.numthreads):
  *                 if self.buffers[i]:
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":752
+  /* "bz3/backends/cython/_bz3.pyx":751
  *                     self.states[i] = NULL
  * 
  *     cdef inline void free_buffers(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i # statesinit_states
  *         if self.buffers: # statesinit_states
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bz3/backends/cython/_bz3.pyx":761
+/* "bz3/backends/cython/_bz3.pyx":760
  *                     self.buffers[i] = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self.free_states()
  *         self.free_buffers()
  */
 
@@ -13881,238 +13881,238 @@
 }
 
 static void __pyx_pf_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_2__dealloc__(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":762
+  /* "bz3/backends/cython/_bz3.pyx":761
  * 
  *     def __dealloc__(self):
  *         self.free_states()             # <<<<<<<<<<<<<<
  *         self.free_buffers()
  *         if self.states:
  */
   __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_free_states(__pyx_v_self);
 
-  /* "bz3/backends/cython/_bz3.pyx":763
+  /* "bz3/backends/cython/_bz3.pyx":762
  *     def __dealloc__(self):
  *         self.free_states()
  *         self.free_buffers()             # <<<<<<<<<<<<<<
  *         if self.states:
  *             PyMem_Free(self.states)
  */
   __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_free_buffers(__pyx_v_self);
 
-  /* "bz3/backends/cython/_bz3.pyx":764
+  /* "bz3/backends/cython/_bz3.pyx":763
  *         self.free_states()
  *         self.free_buffers()
  *         if self.states:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)
  */
   __pyx_t_1 = (__pyx_v_self->states != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":765
+    /* "bz3/backends/cython/_bz3.pyx":764
  *         self.free_buffers()
  *         if self.states:
  *             PyMem_Free(self.states)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL
  */
     PyMem_Free(__pyx_v_self->states);
 
-    /* "bz3/backends/cython/_bz3.pyx":766
+    /* "bz3/backends/cython/_bz3.pyx":765
  *         if self.states:
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)             # <<<<<<<<<<<<<<
  *             self.states = NULL
  *         if self.buffers:
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->states);
 
-    /* "bz3/backends/cython/_bz3.pyx":767
+    /* "bz3/backends/cython/_bz3.pyx":766
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL             # <<<<<<<<<<<<<<
  *         if self.buffers:
  *             PyMem_Free(self.buffers)
  */
     __pyx_v_self->states = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":764
+    /* "bz3/backends/cython/_bz3.pyx":763
  *         self.free_states()
  *         self.free_buffers()
  *         if self.states:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.states)
  *             MEMLOG("PyMem_Free %p\n", self.states)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":768
+  /* "bz3/backends/cython/_bz3.pyx":767
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL
  *         if self.buffers:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  */
   __pyx_t_1 = (__pyx_v_self->buffers != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":769
+    /* "bz3/backends/cython/_bz3.pyx":768
  *             self.states = NULL
  *         if self.buffers:
  *             PyMem_Free(self.buffers)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL
  */
     PyMem_Free(__pyx_v_self->buffers);
 
-    /* "bz3/backends/cython/_bz3.pyx":770
+    /* "bz3/backends/cython/_bz3.pyx":769
  *         if self.buffers:
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)             # <<<<<<<<<<<<<<
  *             self.buffers = NULL
  *         if self.sizes:
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->buffers);
 
-    /* "bz3/backends/cython/_bz3.pyx":771
+    /* "bz3/backends/cython/_bz3.pyx":770
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL             # <<<<<<<<<<<<<<
  *         if self.sizes:
  *             PyMem_Free(self.sizes)
  */
     __pyx_v_self->buffers = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":768
+    /* "bz3/backends/cython/_bz3.pyx":767
  *             MEMLOG("PyMem_Free %p\n", self.states)
  *             self.states = NULL
  *         if self.buffers:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.buffers)
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":772
+  /* "bz3/backends/cython/_bz3.pyx":771
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL
  *         if self.sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  */
   __pyx_t_1 = (__pyx_v_self->sizes != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":773
+    /* "bz3/backends/cython/_bz3.pyx":772
  *             self.buffers = NULL
  *         if self.sizes:
  *             PyMem_Free(self.sizes)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL
  */
     PyMem_Free(__pyx_v_self->sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":774
+    /* "bz3/backends/cython/_bz3.pyx":773
  *         if self.sizes:
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)             # <<<<<<<<<<<<<<
  *             self.sizes = NULL
  *         if self.old_sizes:
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":775
+    /* "bz3/backends/cython/_bz3.pyx":774
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL             # <<<<<<<<<<<<<<
  *         if self.old_sizes:
  *             PyMem_Free(self.old_sizes)
  */
     __pyx_v_self->sizes = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":772
+    /* "bz3/backends/cython/_bz3.pyx":771
  *             MEMLOG("PyMem_Free %p\n", self.buffers)
  *             self.buffers = NULL
  *         if self.sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.sizes)
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":776
+  /* "bz3/backends/cython/_bz3.pyx":775
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL
  *         if self.old_sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  */
   __pyx_t_1 = (__pyx_v_self->old_sizes != 0);
   if (__pyx_t_1) {
 
-    /* "bz3/backends/cython/_bz3.pyx":777
+    /* "bz3/backends/cython/_bz3.pyx":776
  *             self.sizes = NULL
  *         if self.old_sizes:
  *             PyMem_Free(self.old_sizes)             # <<<<<<<<<<<<<<
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  *             self.old_sizes = NULL
  */
     PyMem_Free(__pyx_v_self->old_sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":778
+    /* "bz3/backends/cython/_bz3.pyx":777
  *         if self.old_sizes:
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)             # <<<<<<<<<<<<<<
  *             self.old_sizes = NULL
  *         MEMLOG("BZ3OmpDecompressor __dealloc__ %p\n", <void *> self)
  */
     MEMLOG(((char const *)"PyMem_Free %p\n"), __pyx_v_self->old_sizes);
 
-    /* "bz3/backends/cython/_bz3.pyx":779
+    /* "bz3/backends/cython/_bz3.pyx":778
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  *             self.old_sizes = NULL             # <<<<<<<<<<<<<<
  *         MEMLOG("BZ3OmpDecompressor __dealloc__ %p\n", <void *> self)
  * 
  */
     __pyx_v_self->old_sizes = NULL;
 
-    /* "bz3/backends/cython/_bz3.pyx":776
+    /* "bz3/backends/cython/_bz3.pyx":775
  *             MEMLOG("PyMem_Free %p\n", self.sizes)
  *             self.sizes = NULL
  *         if self.old_sizes:             # <<<<<<<<<<<<<<
  *             PyMem_Free(self.old_sizes)
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":780
+  /* "bz3/backends/cython/_bz3.pyx":779
  *             MEMLOG("PyMem_Free %p\n", self.old_sizes)
  *             self.old_sizes = NULL
  *         MEMLOG("BZ3OmpDecompressor __dealloc__ %p\n", <void *> self)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bytes decompress(self, const uint8_t[::1] data):
  */
   MEMLOG(((char const *)"BZ3OmpDecompressor __dealloc__ %p\n"), ((void *)__pyx_v_self));
 
-  /* "bz3/backends/cython/_bz3.pyx":761
+  /* "bz3/backends/cython/_bz3.pyx":760
  *                     self.buffers[i] = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self.free_states()
  *         self.free_buffers()
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "bz3/backends/cython/_bz3.pyx":782
+/* "bz3/backends/cython/_bz3.pyx":781
  *         MEMLOG("BZ3OmpDecompressor __dealloc__ %p\n", <void *> self)
  * 
  *     cpdef inline bytes decompress(self, const uint8_t[::1] data):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t code
  */
 
@@ -14139,93 +14139,93 @@
   uint32_t __pyx_t_9;
   uint32_t __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decompress", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":783
+  /* "bz3/backends/cython/_bz3.pyx":782
  * 
  *     cpdef inline bytes decompress(self, const uint8_t[::1] data):
  *         cdef Py_ssize_t input_size = data.shape[0]             # <<<<<<<<<<<<<<
  *         cdef int32_t code
  *         cdef bytearray ret = bytearray()
  */
   __pyx_v_input_size = (__pyx_v_data.shape[0]);
 
-  /* "bz3/backends/cython/_bz3.pyx":785
+  /* "bz3/backends/cython/_bz3.pyx":784
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t code
  *         cdef bytearray ret = bytearray()             # <<<<<<<<<<<<<<
  *         cdef int32_t  block_size
  *         cdef uint32_t i, thread_count, j, should_delete=0
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 785, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)(&PyByteArray_Type))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":787
+  /* "bz3/backends/cython/_bz3.pyx":786
  *         cdef bytearray ret = bytearray()
  *         cdef int32_t  block_size
  *         cdef uint32_t i, thread_count, j, should_delete=0             # <<<<<<<<<<<<<<
  *         cdef int should_break = 0
  *         if input_size > 0:
  */
   __pyx_v_should_delete = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":788
+  /* "bz3/backends/cython/_bz3.pyx":787
  *         cdef int32_t  block_size
  *         cdef uint32_t i, thread_count, j, should_delete=0
  *         cdef int should_break = 0             # <<<<<<<<<<<<<<
  *         if input_size > 0:
  *             # if PyByteArray_Resize(self.unused, input_size+PyByteArray_GET_SIZE(self.unused)) < 0:
  */
   __pyx_v_should_break = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":789
+  /* "bz3/backends/cython/_bz3.pyx":788
  *         cdef uint32_t i, thread_count, j, should_delete=0
  *         cdef int should_break = 0
  *         if input_size > 0:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(self.unused, input_size+PyByteArray_GET_SIZE(self.unused)) < 0:
  *             #     raise
  */
   __pyx_t_2 = ((__pyx_v_input_size > 0) != 0);
   if (__pyx_t_2) {
 
-    /* "bz3/backends/cython/_bz3.pyx":793
+    /* "bz3/backends/cython/_bz3.pyx":792
  *             #     raise
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data) # read header             # <<<<<<<<<<<<<<
  *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->unused, __pyx_n_s_extend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->unused, __pyx_n_s_extend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint8_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 793, __pyx_L1_error)
+    __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint8_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bz3/backends/cython/_bz3.pyx":794
+    /* "bz3/backends/cython/_bz3.pyx":793
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data) # read header
  *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  */
     __pyx_t_1 = __pyx_v_self->unused;
@@ -14238,62 +14238,62 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_6 = ((!(__pyx_v_self->have_magic_number != 0)) != 0);
     __pyx_t_2 = __pyx_t_6;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "bz3/backends/cython/_bz3.pyx":795
+      /* "bz3/backends/cython/_bz3.pyx":794
  *             self.unused.extend(data) # read header
  *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  */
       __pyx_t_1 = __pyx_v_self->unused;
       __Pyx_INCREF(__pyx_t_1);
       __pyx_t_2 = ((strncmp(PyByteArray_AS_STRING(__pyx_t_1), __pyx_v_3bz3_8backends_6cython_4_bz3_magic, 5) != 0) != 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(__pyx_t_2)) {
 
-        /* "bz3/backends/cython/_bz3.pyx":796
+        /* "bz3/backends/cython/_bz3.pyx":795
  *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")             # <<<<<<<<<<<<<<
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  */
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 796, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __PYX_ERR(0, 796, __pyx_L1_error)
+        __PYX_ERR(0, 795, __pyx_L1_error)
 
-        /* "bz3/backends/cython/_bz3.pyx":795
+        /* "bz3/backends/cython/_bz3.pyx":794
  *             self.unused.extend(data) # read header
  *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:             # <<<<<<<<<<<<<<
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  */
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":797
+      /* "bz3/backends/cython/_bz3.pyx":796
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))             # <<<<<<<<<<<<<<
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  *                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
  */
       __pyx_t_1 = __pyx_v_self->unused;
       __Pyx_INCREF(__pyx_t_1);
       __pyx_v_block_size = read_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_t_1)[5]))));
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "bz3/backends/cython/_bz3.pyx":798
+      /* "bz3/backends/cython/_bz3.pyx":797
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):             # <<<<<<<<<<<<<<
  *                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
  *                 self.init_state(block_size)
  */
       __pyx_t_6 = ((__pyx_v_block_size < KiB(65)) != 0);
@@ -14303,173 +14303,173 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_6 = ((__pyx_v_block_size > MiB(0x1FF)) != 0);
       __pyx_t_2 = __pyx_t_6;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_2)) {
 
-        /* "bz3/backends/cython/_bz3.pyx":799
+        /* "bz3/backends/cython/_bz3.pyx":798
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  *                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")             # <<<<<<<<<<<<<<
  *                 self.init_state(block_size)
  *                 del self.unused[:9]
  */
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 799, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 798, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __PYX_ERR(0, 799, __pyx_L1_error)
+        __PYX_ERR(0, 798, __pyx_L1_error)
 
-        /* "bz3/backends/cython/_bz3.pyx":798
+        /* "bz3/backends/cython/_bz3.pyx":797
  *                     raise ValueError("Invalid signature")
  *                 block_size = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[5]))
  *                 if block_size  < KiB(65) or block_size >MiB(511):             # <<<<<<<<<<<<<<
  *                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
  *                 self.init_state(block_size)
  */
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":800
+      /* "bz3/backends/cython/_bz3.pyx":799
  *                 if block_size  < KiB(65) or block_size >MiB(511):
  *                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
  *                 self.init_state(block_size)             # <<<<<<<<<<<<<<
  *                 del self.unused[:9]
  *                 self.have_magic_number = 1
  */
-      __pyx_t_7 = __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_init_state(__pyx_v_self, __pyx_v_block_size); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 800, __pyx_L1_error)
+      __pyx_t_7 = __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_init_state(__pyx_v_self, __pyx_v_block_size); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 799, __pyx_L1_error)
 
-      /* "bz3/backends/cython/_bz3.pyx":801
+      /* "bz3/backends/cython/_bz3.pyx":800
  *                     raise ValueError("The input file is corrupted. Reason: Invalid block size in the header")
  *                 self.init_state(block_size)
  *                 del self.unused[:9]             # <<<<<<<<<<<<<<
  *                 self.have_magic_number = 1
  *             # block
  */
       if (unlikely(__pyx_v_self->unused == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 801, __pyx_L1_error)
+        __PYX_ERR(0, 800, __pyx_L1_error)
       }
-      if (__Pyx_PyObject_DelSlice(__pyx_v_self->unused, 0, 9, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 801, __pyx_L1_error)
+      if (__Pyx_PyObject_DelSlice(__pyx_v_self->unused, 0, 9, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
 
-      /* "bz3/backends/cython/_bz3.pyx":802
+      /* "bz3/backends/cython/_bz3.pyx":801
  *                 self.init_state(block_size)
  *                 del self.unused[:9]
  *                 self.have_magic_number = 1             # <<<<<<<<<<<<<<
  *             # block
  *             while not should_break:
  */
       __pyx_v_self->have_magic_number = 1;
 
-      /* "bz3/backends/cython/_bz3.pyx":794
+      /* "bz3/backends/cython/_bz3.pyx":793
  *             # memcpy(&(PyByteArray_AS_STRING(self.unused)[PyByteArray_GET_SIZE(self.unused)-input_size]), &data[0], input_size) # self.unused.extend
  *             self.unused.extend(data) # read header
  *             if PyByteArray_GET_SIZE(self.unused) >= 9 and not self.have_magic_number: # 9 bytes magic number             # <<<<<<<<<<<<<<
  *                 if strncmp(PyByteArray_AS_STRING(self.unused), magic, 5) != 0:
  *                     raise ValueError("Invalid signature")
  */
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":804
+    /* "bz3/backends/cython/_bz3.pyx":803
  *                 self.have_magic_number = 1
  *             # block
  *             while not should_break:             # <<<<<<<<<<<<<<
  *                 thread_count = 0  # thread
  *                 # should_delete = 0 # self.unused
  */
     while (1) {
       __pyx_t_2 = ((!(__pyx_v_should_break != 0)) != 0);
       if (!__pyx_t_2) break;
 
-      /* "bz3/backends/cython/_bz3.pyx":805
+      /* "bz3/backends/cython/_bz3.pyx":804
  *             # block
  *             while not should_break:
  *                 thread_count = 0  # thread             # <<<<<<<<<<<<<<
  *                 # should_delete = 0 # self.unused
  *                 for i in range(self.numthreads):
  */
       __pyx_v_thread_count = 0;
 
-      /* "bz3/backends/cython/_bz3.pyx":807
+      /* "bz3/backends/cython/_bz3.pyx":806
  *                 thread_count = 0  # thread
  *                 # should_delete = 0 # self.unused
  *                 for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete)<8: # 8 byte header
  *                         should_break = 1
  */
       __pyx_t_8 = __pyx_v_self->numthreads;
       __pyx_t_9 = __pyx_t_8;
       for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
         __pyx_v_i = __pyx_t_10;
 
-        /* "bz3/backends/cython/_bz3.pyx":808
+        /* "bz3/backends/cython/_bz3.pyx":807
  *                 # should_delete = 0 # self.unused
  *                 for i in range(self.numthreads):
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete)<8: # 8 byte header             # <<<<<<<<<<<<<<
  *                         should_break = 1
  *                         break
  */
         __pyx_t_1 = __pyx_v_self->unused;
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_2 = (((PyByteArray_GET_SIZE(__pyx_t_1) - __pyx_v_should_delete) < 8) != 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (__pyx_t_2) {
 
-          /* "bz3/backends/cython/_bz3.pyx":809
+          /* "bz3/backends/cython/_bz3.pyx":808
  *                 for i in range(self.numthreads):
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete)<8: # 8 byte header
  *                         should_break = 1             # <<<<<<<<<<<<<<
  *                         break
  *                     self.sizes[i] = read_neutral_s32(<uint8_t*>&PyByteArray_AS_STRING(self.unused)[should_delete]) # todo gcc warning but bytes is const
  */
           __pyx_v_should_break = 1;
 
-          /* "bz3/backends/cython/_bz3.pyx":810
+          /* "bz3/backends/cython/_bz3.pyx":809
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete)<8: # 8 byte header
  *                         should_break = 1
  *                         break             # <<<<<<<<<<<<<<
  *                     self.sizes[i] = read_neutral_s32(<uint8_t*>&PyByteArray_AS_STRING(self.unused)[should_delete]) # todo gcc warning but bytes is const
  *                     self.old_sizes[i] = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[should_delete+4]))
  */
           goto __pyx_L14_break;
 
-          /* "bz3/backends/cython/_bz3.pyx":808
+          /* "bz3/backends/cython/_bz3.pyx":807
  *                 # should_delete = 0 # self.unused
  *                 for i in range(self.numthreads):
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete)<8: # 8 byte header             # <<<<<<<<<<<<<<
  *                         should_break = 1
  *                         break
  */
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":811
+        /* "bz3/backends/cython/_bz3.pyx":810
  *                         should_break = 1
  *                         break
  *                     self.sizes[i] = read_neutral_s32(<uint8_t*>&PyByteArray_AS_STRING(self.unused)[should_delete]) # todo gcc warning but bytes is const             # <<<<<<<<<<<<<<
  *                     self.old_sizes[i] = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[should_delete+4]))
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):
  */
         __pyx_t_1 = __pyx_v_self->unused;
         __Pyx_INCREF(__pyx_t_1);
         (__pyx_v_self->sizes[__pyx_v_i]) = read_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_t_1)[__pyx_v_should_delete]))));
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "bz3/backends/cython/_bz3.pyx":812
+        /* "bz3/backends/cython/_bz3.pyx":811
  *                         break
  *                     self.sizes[i] = read_neutral_s32(<uint8_t*>&PyByteArray_AS_STRING(self.unused)[should_delete]) # todo gcc warning but bytes is const
  *                     self.old_sizes[i] = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[should_delete+4]))             # <<<<<<<<<<<<<<
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")
  */
         __pyx_t_1 = __pyx_v_self->unused;
         __Pyx_INCREF(__pyx_t_1);
         (__pyx_v_self->old_sizes[__pyx_v_i]) = read_neutral_s32(((uint8_t *)(&(PyByteArray_AS_STRING(__pyx_t_1)[(__pyx_v_should_delete + 4)]))));
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "bz3/backends/cython/_bz3.pyx":813
+        /* "bz3/backends/cython/_bz3.pyx":812
  *                     self.sizes[i] = read_neutral_s32(<uint8_t*>&PyByteArray_AS_STRING(self.unused)[should_delete]) # todo gcc warning but bytes is const
  *                     self.old_sizes[i] = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[should_delete+4]))
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):             # <<<<<<<<<<<<<<
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #
  */
         __pyx_t_6 = (((__pyx_v_self->old_sizes[__pyx_v_i]) > ((int32_t)bz3_bound(__pyx_v_self->block_size))) != 0);
@@ -14479,290 +14479,290 @@
           goto __pyx_L17_bool_binop_done;
         }
         __pyx_t_6 = (((__pyx_v_self->sizes[__pyx_v_i]) > ((int32_t)bz3_bound(__pyx_v_self->block_size))) != 0);
         __pyx_t_2 = __pyx_t_6;
         __pyx_L17_bool_binop_done:;
         if (unlikely(__pyx_t_2)) {
 
-          /* "bz3/backends/cython/_bz3.pyx":814
+          /* "bz3/backends/cython/_bz3.pyx":813
  *                     self.old_sizes[i] = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[should_delete+4]))
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")             # <<<<<<<<<<<<<<
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #
  *                         should_break = 1
  */
-          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 814, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 813, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_Raise(__pyx_t_1, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __PYX_ERR(0, 814, __pyx_L1_error)
+          __PYX_ERR(0, 813, __pyx_L1_error)
 
-          /* "bz3/backends/cython/_bz3.pyx":813
+          /* "bz3/backends/cython/_bz3.pyx":812
  *                     self.sizes[i] = read_neutral_s32(<uint8_t*>&PyByteArray_AS_STRING(self.unused)[should_delete]) # todo gcc warning but bytes is const
  *                     self.old_sizes[i] = read_neutral_s32(<uint8_t*>&(PyByteArray_AS_STRING(self.unused)[should_delete+4]))
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):             # <<<<<<<<<<<<<<
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #
  */
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":815
+        /* "bz3/backends/cython/_bz3.pyx":814
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #             # <<<<<<<<<<<<<<
  *                         should_break = 1
  *                         break
  */
         __pyx_t_1 = __pyx_v_self->unused;
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_2 = (((PyByteArray_GET_SIZE(__pyx_t_1) - __pyx_v_should_delete) < ((__pyx_v_self->sizes[__pyx_v_i]) + 8)) != 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (__pyx_t_2) {
 
-          /* "bz3/backends/cython/_bz3.pyx":816
+          /* "bz3/backends/cython/_bz3.pyx":815
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #
  *                         should_break = 1             # <<<<<<<<<<<<<<
  *                         break
  *                     memcpy(self.buffers[i], &(PyByteArray_AS_STRING(self.unused)[should_delete+8]), <size_t>self.sizes[i])
  */
           __pyx_v_should_break = 1;
 
-          /* "bz3/backends/cython/_bz3.pyx":817
+          /* "bz3/backends/cython/_bz3.pyx":816
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #
  *                         should_break = 1
  *                         break             # <<<<<<<<<<<<<<
  *                     memcpy(self.buffers[i], &(PyByteArray_AS_STRING(self.unused)[should_delete+8]), <size_t>self.sizes[i])
  *                     should_delete += (self.sizes[i] + 8)
  */
           goto __pyx_L14_break;
 
-          /* "bz3/backends/cython/_bz3.pyx":815
+          /* "bz3/backends/cython/_bz3.pyx":814
  *                     if self.old_sizes[i] > <int32_t>bz3_bound(self.block_size) or self.sizes[i] > <int32_t>bz3_bound(self.block_size):
  *                         raise ValueError("Failed to decode a block: Inconsistent headers.")
  *                     if (PyByteArray_GET_SIZE(self.unused)-should_delete) < self.sizes[i]+8: #             # <<<<<<<<<<<<<<
  *                         should_break = 1
  *                         break
  */
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":818
+        /* "bz3/backends/cython/_bz3.pyx":817
  *                         should_break = 1
  *                         break
  *                     memcpy(self.buffers[i], &(PyByteArray_AS_STRING(self.unused)[should_delete+8]), <size_t>self.sizes[i])             # <<<<<<<<<<<<<<
  *                     should_delete += (self.sizes[i] + 8)
  *                     thread_count += 1
  */
         __pyx_t_1 = __pyx_v_self->unused;
         __Pyx_INCREF(__pyx_t_1);
         (void)(memcpy((__pyx_v_self->buffers[__pyx_v_i]), (&(PyByteArray_AS_STRING(__pyx_t_1)[(__pyx_v_should_delete + 8)])), ((size_t)(__pyx_v_self->sizes[__pyx_v_i]))));
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "bz3/backends/cython/_bz3.pyx":819
+        /* "bz3/backends/cython/_bz3.pyx":818
  *                         break
  *                     memcpy(self.buffers[i], &(PyByteArray_AS_STRING(self.unused)[should_delete+8]), <size_t>self.sizes[i])
  *                     should_delete += (self.sizes[i] + 8)             # <<<<<<<<<<<<<<
  *                     thread_count += 1
  *                 if thread_count:  # blockdecodejb
  */
         __pyx_v_should_delete = (__pyx_v_should_delete + ((__pyx_v_self->sizes[__pyx_v_i]) + 8));
 
-        /* "bz3/backends/cython/_bz3.pyx":820
+        /* "bz3/backends/cython/_bz3.pyx":819
  *                     memcpy(self.buffers[i], &(PyByteArray_AS_STRING(self.unused)[should_delete+8]), <size_t>self.sizes[i])
  *                     should_delete += (self.sizes[i] + 8)
  *                     thread_count += 1             # <<<<<<<<<<<<<<
  *                 if thread_count:  # blockdecodejb
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)
  */
         __pyx_v_thread_count = (__pyx_v_thread_count + 1);
       }
       __pyx_L14_break:;
 
-      /* "bz3/backends/cython/_bz3.pyx":821
+      /* "bz3/backends/cython/_bz3.pyx":820
  *                     should_delete += (self.sizes[i] + 8)
  *                     thread_count += 1
  *                 if thread_count:  # blockdecodejb             # <<<<<<<<<<<<<<
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)
  *                 for j in range(thread_count):
  */
       __pyx_t_2 = (__pyx_v_thread_count != 0);
       if (__pyx_t_2) {
 
-        /* "bz3/backends/cython/_bz3.pyx":822
+        /* "bz3/backends/cython/_bz3.pyx":821
  *                     thread_count += 1
  *                 if thread_count:  # blockdecodejb
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)             # <<<<<<<<<<<<<<
  *                 for j in range(thread_count):
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:
  */
         __pyx_f_3bz3_8backends_6cython_4_bz3_bz3_decode_blocks(__pyx_v_self->states, __pyx_v_self->buffers, __pyx_v_self->sizes, __pyx_v_self->old_sizes, ((int32_t)__pyx_v_thread_count));
 
-        /* "bz3/backends/cython/_bz3.pyx":821
+        /* "bz3/backends/cython/_bz3.pyx":820
  *                     should_delete += (self.sizes[i] + 8)
  *                     thread_count += 1
  *                 if thread_count:  # blockdecodejb             # <<<<<<<<<<<<<<
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)
  *                 for j in range(thread_count):
  */
       }
 
-      /* "bz3/backends/cython/_bz3.pyx":823
+      /* "bz3/backends/cython/_bz3.pyx":822
  *                 if thread_count:  # blockdecodejb
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)
  *                 for j in range(thread_count):             # <<<<<<<<<<<<<<
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:
  *                         if self.ignore_error:
  */
       __pyx_t_8 = __pyx_v_thread_count;
       __pyx_t_9 = __pyx_t_8;
       for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
         __pyx_v_j = __pyx_t_10;
 
-        /* "bz3/backends/cython/_bz3.pyx":824
+        /* "bz3/backends/cython/_bz3.pyx":823
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)
  *                 for j in range(thread_count):
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                         if self.ignore_error:
  *                             fprintf(stderr, "Writing invalid block: %s\n", bz3_strerror(self.states[j]))
  */
         __pyx_t_2 = ((bz3_last_error((__pyx_v_self->states[__pyx_v_j])) != BZ3_OK) != 0);
         if (__pyx_t_2) {
 
-          /* "bz3/backends/cython/_bz3.pyx":825
+          /* "bz3/backends/cython/_bz3.pyx":824
  *                 for j in range(thread_count):
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:
  *                         if self.ignore_error:             # <<<<<<<<<<<<<<
  *                             fprintf(stderr, "Writing invalid block: %s\n", bz3_strerror(self.states[j]))
  *                         else:
  */
           __pyx_t_2 = (__pyx_v_self->ignore_error != 0);
           if (likely(__pyx_t_2)) {
 
-            /* "bz3/backends/cython/_bz3.pyx":826
+            /* "bz3/backends/cython/_bz3.pyx":825
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:
  *                         if self.ignore_error:
  *                             fprintf(stderr, "Writing invalid block: %s\n", bz3_strerror(self.states[j]))             # <<<<<<<<<<<<<<
  *                         else:
  *                             raise ValueError("Failed to decode data: %s" % bz3_strerror(self.states[j]))
  */
             (void)(fprintf(stderr, ((char const *)"Writing invalid block: %s\n"), bz3_strerror((__pyx_v_self->states[__pyx_v_j]))));
 
-            /* "bz3/backends/cython/_bz3.pyx":825
+            /* "bz3/backends/cython/_bz3.pyx":824
  *                 for j in range(thread_count):
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:
  *                         if self.ignore_error:             # <<<<<<<<<<<<<<
  *                             fprintf(stderr, "Writing invalid block: %s\n", bz3_strerror(self.states[j]))
  *                         else:
  */
             goto __pyx_L24;
           }
 
-          /* "bz3/backends/cython/_bz3.pyx":828
+          /* "bz3/backends/cython/_bz3.pyx":827
  *                             fprintf(stderr, "Writing invalid block: %s\n", bz3_strerror(self.states[j]))
  *                         else:
  *                             raise ValueError("Failed to decode data: %s" % bz3_strerror(self.states[j]))             # <<<<<<<<<<<<<<
  *                     ret.extend(<bytes>self.buffers[j][:self.old_sizes[j]])
  *             if should_delete:
  */
           /*else*/ {
-            __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_j]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_j]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 827, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_Failed_to_decode_data_s, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 828, __pyx_L1_error)
+            __pyx_t_3 = PyUnicode_Format(__pyx_kp_u_Failed_to_decode_data_s, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 827, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 827, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_Raise(__pyx_t_1, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __PYX_ERR(0, 828, __pyx_L1_error)
+            __PYX_ERR(0, 827, __pyx_L1_error)
           }
           __pyx_L24:;
 
-          /* "bz3/backends/cython/_bz3.pyx":824
+          /* "bz3/backends/cython/_bz3.pyx":823
  *                     bz3_decode_blocks(self.states, self.buffers, self.sizes, self.old_sizes, <int32_t>thread_count)
  *                 for j in range(thread_count):
  *                     if bz3_last_error(self.states[j]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                         if self.ignore_error:
  *                             fprintf(stderr, "Writing invalid block: %s\n", bz3_strerror(self.states[j]))
  */
         }
 
-        /* "bz3/backends/cython/_bz3.pyx":829
+        /* "bz3/backends/cython/_bz3.pyx":828
  *                         else:
  *                             raise ValueError("Failed to decode data: %s" % bz3_strerror(self.states[j]))
  *                     ret.extend(<bytes>self.buffers[j][:self.old_sizes[j]])             # <<<<<<<<<<<<<<
  *             if should_delete:
  *                 del self.unused[:should_delete]
  */
-        __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_self->buffers[__pyx_v_j])) + 0, (__pyx_v_self->old_sizes[__pyx_v_j]) - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 829, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_self->buffers[__pyx_v_j])) + 0, (__pyx_v_self->old_sizes[__pyx_v_j]) - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_3 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 829, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyByteArray_Type_extend, __pyx_v_ret, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 828, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":830
+    /* "bz3/backends/cython/_bz3.pyx":829
  *                             raise ValueError("Failed to decode data: %s" % bz3_strerror(self.states[j]))
  *                     ret.extend(<bytes>self.buffers[j][:self.old_sizes[j]])
  *             if should_delete:             # <<<<<<<<<<<<<<
  *                 del self.unused[:should_delete]
  *         return bytes(ret)
  */
     __pyx_t_2 = (__pyx_v_should_delete != 0);
     if (__pyx_t_2) {
 
-      /* "bz3/backends/cython/_bz3.pyx":831
+      /* "bz3/backends/cython/_bz3.pyx":830
  *                     ret.extend(<bytes>self.buffers[j][:self.old_sizes[j]])
  *             if should_delete:
  *                 del self.unused[:should_delete]             # <<<<<<<<<<<<<<
  *         return bytes(ret)
  * 
  */
       if (unlikely(__pyx_v_self->unused == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 831, __pyx_L1_error)
+        __PYX_ERR(0, 830, __pyx_L1_error)
       }
-      if (__Pyx_PyObject_DelSlice(__pyx_v_self->unused, 0, __pyx_v_should_delete, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 831, __pyx_L1_error)
+      if (__Pyx_PyObject_DelSlice(__pyx_v_self->unused, 0, __pyx_v_should_delete, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(0, 830, __pyx_L1_error)
 
-      /* "bz3/backends/cython/_bz3.pyx":830
+      /* "bz3/backends/cython/_bz3.pyx":829
  *                             raise ValueError("Failed to decode data: %s" % bz3_strerror(self.states[j]))
  *                     ret.extend(<bytes>self.buffers[j][:self.old_sizes[j]])
  *             if should_delete:             # <<<<<<<<<<<<<<
  *                 del self.unused[:should_delete]
  *         return bytes(ret)
  */
     }
 
-    /* "bz3/backends/cython/_bz3.pyx":789
+    /* "bz3/backends/cython/_bz3.pyx":788
  *         cdef uint32_t i, thread_count, j, should_delete=0
  *         cdef int should_break = 0
  *         if input_size > 0:             # <<<<<<<<<<<<<<
  *             # if PyByteArray_Resize(self.unused, input_size+PyByteArray_GET_SIZE(self.unused)) < 0:
  *             #     raise
  */
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":832
+  /* "bz3/backends/cython/_bz3.pyx":831
  *             if should_delete:
  *                 del self.unused[:should_delete]
  *         return bytes(ret)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 832, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "bz3/backends/cython/_bz3.pyx":782
+  /* "bz3/backends/cython/_bz3.pyx":781
  *         MEMLOG("BZ3OmpDecompressor __dealloc__ %p\n", <void *> self)
  * 
  *     cpdef inline bytes decompress(self, const uint8_t[::1] data):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t input_size = data.shape[0]
  *         cdef int32_t code
  */
 
@@ -14789,15 +14789,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("decompress (wrapper)", 0);
   assert(__pyx_arg_data); {
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint8_t__const__(__pyx_arg_data, 0); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 782, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint8_t__const__(__pyx_arg_data, 0); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 781, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("bz3.backends.cython._bz3.BZ3OmpDecompressor.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -14813,16 +14813,16 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decompress", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 782, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_decompress(__pyx_v_self, __pyx_v_data, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 782, __pyx_L1_error)
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 781, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_decompress(__pyx_v_self, __pyx_v_data, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 781, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14832,15 +14832,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_data, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":835
+/* "bz3/backends/cython/_bz3.pyx":834
  * 
  *     @property
  *     def unused_data(self):             # <<<<<<<<<<<<<<
  *         """Data found after the end of the compressed stream."""
  *         return bytes(self.unused)
  */
 
@@ -14862,29 +14862,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":837
+  /* "bz3/backends/cython/_bz3.pyx":836
  *     def unused_data(self):
  *         """Data found after the end of the compressed stream."""
  *         return bytes(self.unused)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline list error(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_self->unused); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_self->unused); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 836, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "bz3/backends/cython/_bz3.pyx":835
+  /* "bz3/backends/cython/_bz3.pyx":834
  * 
  *     @property
  *     def unused_data(self):             # <<<<<<<<<<<<<<
  *         """Data found after the end of the compressed stream."""
  *         return bytes(self.unused)
  */
 
@@ -14895,15 +14895,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":839
+/* "bz3/backends/cython/_bz3.pyx":838
  *         return bytes(self.unused)
  * 
  *     cpdef inline list error(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         cdef list ret = []
  */
 
@@ -14921,87 +14921,87 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error", 0);
 
-  /* "bz3/backends/cython/_bz3.pyx":841
+  /* "bz3/backends/cython/_bz3.pyx":840
  *     cpdef inline list error(self):
  *         cdef uint32_t i
  *         cdef list ret = []             # <<<<<<<<<<<<<<
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 840, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bz3/backends/cython/_bz3.pyx":842
+  /* "bz3/backends/cython/_bz3.pyx":841
  *         cdef uint32_t i
  *         cdef list ret = []
  *         for i in range(self.numthreads):             # <<<<<<<<<<<<<<
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  *                 ret.append((<bytes> bz3_strerror(self.states[i])).decode())
  */
   __pyx_t_2 = __pyx_v_self->numthreads;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "bz3/backends/cython/_bz3.pyx":843
+    /* "bz3/backends/cython/_bz3.pyx":842
  *         cdef list ret = []
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                 ret.append((<bytes> bz3_strerror(self.states[i])).decode())
  *         return ret
  */
     __pyx_t_5 = ((bz3_last_error((__pyx_v_self->states[__pyx_v_i])) != BZ3_OK) != 0);
     if (__pyx_t_5) {
 
-      /* "bz3/backends/cython/_bz3.pyx":844
+      /* "bz3/backends/cython/_bz3.pyx":843
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  *                 ret.append((<bytes> bz3_strerror(self.states[i])).decode())             # <<<<<<<<<<<<<<
  *         return ret
  */
-      __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_i]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 844, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyBytes_FromString(bz3_strerror((__pyx_v_self->states[__pyx_v_i]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 843, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (unlikely(__pyx_t_1 == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
-        __PYX_ERR(0, 844, __pyx_L1_error)
+        __PYX_ERR(0, 843, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 844, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 843, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_ret, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 844, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_ret, __pyx_t_6); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 843, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "bz3/backends/cython/_bz3.pyx":843
+      /* "bz3/backends/cython/_bz3.pyx":842
  *         cdef list ret = []
  *         for i in range(self.numthreads):
  *             if bz3_last_error(self.states[i]) != BZ3_OK:             # <<<<<<<<<<<<<<
  *                 ret.append((<bytes> bz3_strerror(self.states[i])).decode())
  *         return ret
  */
     }
   }
 
-  /* "bz3/backends/cython/_bz3.pyx":845
+  /* "bz3/backends/cython/_bz3.pyx":844
  *             if bz3_last_error(self.states[i]) != BZ3_OK:
  *                 ret.append((<bytes> bz3_strerror(self.states[i])).decode())
  *         return ret             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ret);
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "bz3/backends/cython/_bz3.pyx":839
+  /* "bz3/backends/cython/_bz3.pyx":838
  *         return bytes(self.unused)
  * 
  *     cpdef inline list error(self):             # <<<<<<<<<<<<<<
  *         cdef uint32_t i
  *         cdef list ret = []
  */
 
@@ -15037,15 +15037,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_error(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 839, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_error(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 838, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15054,15 +15054,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":688
+/* "bz3/backends/cython/_bz3.pyx":687
  *         int32_t * sizes   # compressed
  *         int32_t * old_sizes  # origin
  *         readonly int32_t block_size             # <<<<<<<<<<<<<<
  *         bytearray unused  #
  *         bint have_magic_number
  */
 
@@ -15084,15 +15084,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_self->block_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_self->block_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 687, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15101,15 +15101,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":691
+/* "bz3/backends/cython/_bz3.pyx":690
  *         bytearray unused  #
  *         bint have_magic_number
  *         readonly uint32_t numthreads  # how many threads to use             # <<<<<<<<<<<<<<
  *         readonly bint ignore_error  # decode
  * 
  */
 
@@ -15131,15 +15131,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->numthreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 691, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->numthreads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15148,15 +15148,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bz3/backends/cython/_bz3.pyx":692
+/* "bz3/backends/cython/_bz3.pyx":691
  *         bint have_magic_number
  *         readonly uint32_t numthreads  # how many threads to use
  *         readonly bint ignore_error  # decode             # <<<<<<<<<<<<<<
  * 
  *     cdef inline int init_state(self, int32_t block_size) except -1:
  */
 
@@ -15178,15 +15178,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->ignore_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->ignore_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 691, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -30421,24 +30421,24 @@
   __pyx_ptype_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor = &__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpCompressor;
   __pyx_vtabptr_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor = &__pyx_vtable_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor;
   __pyx_vtable_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.init_state = (int (*)(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *, int32_t))__pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_init_state;
   __pyx_vtable_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.free_states = (void (*)(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *))__pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_free_states;
   __pyx_vtable_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.free_buffers = (void (*)(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *))__pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_free_buffers;
   __pyx_vtable_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.decompress = (PyObject *(*)(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *, __Pyx_memviewslice, int __pyx_skip_dispatch))__pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_decompress;
   __pyx_vtable_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.error = (PyObject *(*)(struct __pyx_obj_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor *, int __pyx_skip_dispatch))__pyx_f_3bz3_8backends_6cython_4_bz3_18BZ3OmpDecompressor_error;
-  if (PyType_Ready(&__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 682, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.tp_dictoffset && __pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (__Pyx_SetVtable(__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.tp_dict, __pyx_vtabptr_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 682, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BZ3OmpDecompressor, (PyObject *)&__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 682, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 682, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor.tp_dict, __pyx_vtabptr_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BZ3OmpDecompressor, (PyObject *)&__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
   __pyx_ptype_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor = &__pyx_type_3bz3_8backends_6cython_4_bz3_BZ3OmpDecompressor;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
```

### Comparing `bzip3-0.1.3rc2/bz3/backends/cython/_bz3.pyx` & `bzip3-0.1.3rc3/bz3/backends/cython/_bz3.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -562,15 +562,14 @@
             for i in range(self.numthreads):
                 if self.buffers[i]:
                     PyMem_Free(self.buffers[i])
                     MEMLOG("PyMem_Free %p\n", self.buffers[i])
                     self.buffers[i] = NULL
 
     def __dealloc__(self):
-        cdef uint32_t i
         self.free_states()
         self.free_buffers()
         if self.states:
             PyMem_Free(self.states)
             MEMLOG("PyMem_Free %p\n", self.states)
             self.states = NULL
         if self.buffers:
```

### Comparing `bzip3-0.1.3rc2/bz3/backends/cython/bzip3.pxd` & `bzip3-0.1.3rc3/bz3/backends/cython/bzip3.pxd`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bz3/bz3.py` & `bzip3-0.1.3rc3/bz3/bz3.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bz3/compression.py` & `bzip3-0.1.3rc3/bz3/compression.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/bzip3.egg-info/PKG-INFO` & `bzip3-0.1.3rc3/bzip3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bzip3
-Version: 0.1.3rc2
+Version: 0.1.3rc3
 Summary: bz3 compress and decompress
 Home-page: https://github.com/synodriver/python-bz3
 Author: synodriver
 Author-email: diguohuangjiajinweijun@gmail.com
 License: BSD
 Keywords: bz3,compress,decompress
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bzip3-0.1.3rc2/bzip3.egg-info/SOURCES.txt` & `bzip3-0.1.3rc3/bzip3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/dep/include/common.h` & `bzip3-0.1.3rc3/dep/include/common.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/dep/include/getopt-shim.h` & `bzip3-0.1.3rc3/dep/include/getopt-shim.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/dep/include/libbz3.h` & `bzip3-0.1.3rc3/dep/include/libbz3.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/dep/include/libsais.h` & `bzip3-0.1.3rc3/dep/include/libsais.h`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/dep/src/libbz3.c` & `bzip3-0.1.3rc3/dep/src/libbz3.c`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/dep/src/main.c` & `bzip3-0.1.3rc3/dep/src/main.c`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/setup.py` & `bzip3-0.1.3rc3/setup.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/test/test_compress.py` & `bzip3-0.1.3rc3/test/test_compress.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/test/test_mem.py` & `bzip3-0.1.3rc3/test/test_mem.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/test/test_omp.py` & `bzip3-0.1.3rc3/test/test_omp.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/test/test_seek.py` & `bzip3-0.1.3rc3/test/test_seek.py`

 * *Files identical despite different names*

### Comparing `bzip3-0.1.3rc2/test/test_thread.py` & `bzip3-0.1.3rc3/test/test_thread.py`

 * *Files identical despite different names*

