# Comparing `tmp/unqlite-0.9.4.tar.gz` & `tmp/unqlite-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unqlite-0.9.4.tar", last modified: Thu Jul 13 03:11:09 2023, max compression
+gzip compressed data, was "dist/unqlite-0.9.5.tar", last modified: Sat Jul 15 17:52:29 2023, max compression
```

## Comparing `unqlite-0.9.4.tar` & `unqlite-0.9.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-13 03:11:09.000000 unqlite-0.9.4/
--rw-r--r--   0 charles   (1000) charles   (1000)     1058 2018-08-16 18:40:48.000000 unqlite-0.9.4/LICENSE
--rw-r--r--   0 charles   (1000) charles   (1000)      211 2018-08-16 18:40:48.000000 unqlite-0.9.4/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)     1371 2023-07-13 03:11:09.000000 unqlite-0.9.4/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     7663 2020-12-07 15:43:34.000000 unqlite-0.9.4/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-13 03:11:09.000000 unqlite-0.9.4/docs/
--rw-r--r--   0 charles   (1000) charles   (1000)     6794 2018-08-16 18:40:48.000000 unqlite-0.9.4/docs/Makefile
--rw-r--r--   0 charles   (1000) charles   (1000)    29341 2020-11-26 04:00:08.000000 unqlite-0.9.4/docs/api.rst
--rw-r--r--   0 charles   (1000) charles   (1000)     8007 2021-11-25 17:03:21.000000 unqlite-0.9.4/docs/conf.py
--rw-r--r--   0 charles   (1000) charles   (1000)     1837 2020-12-07 15:45:12.000000 unqlite-0.9.4/docs/index.rst
--rw-r--r--   0 charles   (1000) charles   (1000)      815 2018-08-16 18:40:48.000000 unqlite-0.9.4/docs/installation.rst
--rw-r--r--   0 charles   (1000) charles   (1000)     6726 2020-03-06 23:33:53.000000 unqlite-0.9.4/docs/quickstart.rst
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-07-13 03:11:09.000000 unqlite-0.9.4/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     2102 2023-07-13 03:09:59.000000 unqlite-0.9.4/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-13 03:11:09.000000 unqlite-0.9.4/src/
--rw-r--r--   0 charles   (1000) charles   (1000)  1955368 2023-07-13 03:08:42.000000 unqlite-0.9.4/src/unqlite.c
--rw-r--r--   0 charles   (1000) charles   (1000)    48708 2023-07-13 03:08:42.000000 unqlite-0.9.4/src/unqlite.h
--rw-r--r--   0 charles   (1000) charles   (1000)    24398 2022-04-27 16:51:36.000000 unqlite-0.9.4/tests.py
--rw-r--r--   0 charles   (1000) charles   (1000)  1354845 2023-07-13 03:09:11.000000 unqlite-0.9.4/unqlite.c
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-13 03:11:09.000000 unqlite-0.9.4/unqlite.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)     1371 2023-07-13 03:11:09.000000 unqlite-0.9.4/unqlite.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)      348 2023-07-13 03:11:09.000000 unqlite-0.9.4/unqlite.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-07-13 03:11:09.000000 unqlite-0.9.4/unqlite.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        7 2023-07-13 03:11:09.000000 unqlite-0.9.4/unqlite.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        8 2023-07-13 03:11:09.000000 unqlite-0.9.4/unqlite.egg-info/top_level.txt
--rw-r--r--   0 charles   (1000) charles   (1000)    45550 2022-10-12 16:12:38.000000 unqlite-0.9.4/unqlite.pyx
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1058 2018-08-16 18:40:48.000000 unqlite-0.9.5/LICENSE
+-rw-rw-r--   0 charles   (1000) charles   (1000)      211 2018-08-16 18:40:48.000000 unqlite-0.9.5/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)     1371 2023-07-15 17:52:29.000000 unqlite-0.9.5/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7663 2020-12-07 15:43:34.000000 unqlite-0.9.5/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/docs/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6794 2018-08-16 18:40:48.000000 unqlite-0.9.5/docs/Makefile
+-rw-rw-r--   0 charles   (1000) charles   (1000)    29341 2020-11-26 04:00:08.000000 unqlite-0.9.5/docs/api.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)     8007 2021-11-25 17:03:21.000000 unqlite-0.9.5/docs/conf.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1837 2020-12-07 15:45:12.000000 unqlite-0.9.5/docs/index.rst
+-rw-rw-r--   0 charles   (1000) charles   (1000)      815 2018-08-16 18:40:48.000000 unqlite-0.9.5/docs/installation.rst
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6726 2020-03-06 23:33:53.000000 unqlite-0.9.5/docs/quickstart.rst
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-07-15 17:52:29.000000 unqlite-0.9.5/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     2183 2023-07-15 17:52:13.000000 unqlite-0.9.5/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/src/
+-rw-r--r--   0 charles   (1000) charles   (1000)  1955368 2023-07-15 17:44:05.000000 unqlite-0.9.5/src/unqlite.c
+-rw-r--r--   0 charles   (1000) charles   (1000)    48708 2021-11-25 17:03:21.000000 unqlite-0.9.5/src/unqlite.h
+-rw-rw-r--   0 charles   (1000) charles   (1000)    24398 2022-04-26 15:29:11.000000 unqlite-0.9.5/tests.py
+-rw-r--r--   0 charles   (1000) charles   (1000)  1353651 2023-07-15 17:51:37.000000 unqlite-0.9.5/unqlite.c
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1371 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      348 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        7 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        8 2023-07-15 17:52:29.000000 unqlite-0.9.5/unqlite.egg-info/top_level.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)    45550 2023-07-15 17:51:34.000000 unqlite-0.9.5/unqlite.pyx
```

### Comparing `unqlite-0.9.4/LICENSE` & `unqlite-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/PKG-INFO` & `unqlite-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unqlite
-Version: 0.9.4
+Version: 0.9.5
 Summary: Fast Python bindings for the UnQLite embedded NoSQL database.
 Home-page: https://github.com/coleifer/unqlite-python
 Author: Charles Leifer
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `unqlite-0.9.4/README.md` & `unqlite-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/docs/Makefile` & `unqlite-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/docs/api.rst` & `unqlite-0.9.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/docs/conf.py` & `unqlite-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/docs/index.rst` & `unqlite-0.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/docs/installation.rst` & `unqlite-0.9.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/docs/quickstart.rst` & `unqlite-0.9.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/setup.py` & `unqlite-0.9.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import glob
+import sys
 import warnings
 
 from setuptools import setup
 from setuptools.extension import Extension
 try:
     from Cython.Build import cythonize
 except ImportError:
@@ -14,24 +15,29 @@
 
 if cython_installed:
     python_source = 'unqlite.pyx'
 else:
     python_source = 'unqlite.c'
     cythonize = lambda obj: obj
 
+if sys.platform.find('win') < 0:
+    libs = ['pthread']
+else:
+    libs = []
+
 library_source = ['src/unqlite.c']
 unqlite_extension = Extension(
     'unqlite',
     define_macros=[('UNQLITE_ENABLE_THREADS', '1')],
-    libraries=['pthread'],
+    libraries=libs,
     sources=[python_source] + library_source)
 
 setup(
     name='unqlite',
-    version='0.9.4',
+    version='0.9.5',
     description='Fast Python bindings for the UnQLite embedded NoSQL database.',
     author='Charles Leifer',
     author_email='',
     url='https://github.com/coleifer/unqlite-python',
     license='MIT',
     install_requires=['Cython'],
     setup_requires=['cython'],
```

### Comparing `unqlite-0.9.4/src/unqlite.c` & `unqlite-0.9.5/src/unqlite.c`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/src/unqlite.h` & `unqlite-0.9.5/src/unqlite.h`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/tests.py` & `unqlite-0.9.5/tests.py`

 * *Files identical despite different names*

### Comparing `unqlite-0.9.4/unqlite.c` & `unqlite-0.9.5/unqlite.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.36 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "UNQLITE_ENABLE_THREADS",
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_36"
-#define CYTHON_HEX_VERSION 0x001D24F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -99,22 +99,18 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,14 +386,17 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define Py_OptimizeFlag 0
+#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -467,19 +466,14 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
-#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
-  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
-#else
-  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
-#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1958,30 +1952,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
-#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#ifndef __PYX_HAVE_RT_ImportType_proto
+#define __PYX_HAVE_RT_ImportType_proto
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_36 {
-   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
+enum __Pyx_ImportType_CheckSize {
+   __Pyx_ImportType_CheckSize_Error = 0,
+   __Pyx_ImportType_CheckSize_Warn = 1,
+   __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
@@ -25646,15 +25640,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_UnQLite(PyObject *o) {
   struct __pyx_obj_7unqlite_UnQLite *p = (struct __pyx_obj_7unqlite_UnQLite *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -25827,15 +25821,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_7unqlite_Transaction(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_Transaction *p;
   PyObject *o;
@@ -25849,15 +25843,15 @@
   p->unqlite = ((struct __pyx_obj_7unqlite_UnQLite *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Transaction(PyObject *o) {
   struct __pyx_obj_7unqlite_Transaction *p = (struct __pyx_obj_7unqlite_Transaction *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->unqlite);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -25951,15 +25945,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7unqlite_Cursor __pyx_vtable_7unqlite_Cursor;
 
 static PyObject *__pyx_tp_new_7unqlite_Cursor(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7unqlite_Cursor *p;
@@ -25979,15 +25973,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Cursor(PyObject *o) {
   struct __pyx_obj_7unqlite_Cursor *p = (struct __pyx_obj_7unqlite_Cursor *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -26103,15 +26097,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7unqlite_VM __pyx_vtable_7unqlite_VM;
 
 static PyObject *__pyx_tp_new_7unqlite_VM(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7unqlite_VM *p;
@@ -26134,15 +26128,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_VM(PyObject *o) {
   struct __pyx_obj_7unqlite_VM *p = (struct __pyx_obj_7unqlite_VM *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -26322,15 +26316,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7unqlite_Context __pyx_vtable_7unqlite_Context;
 
 static PyObject *__pyx_tp_new_7unqlite_Context(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_Context *p;
@@ -26348,15 +26342,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Context(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_7unqlite_Context[] = {
@@ -26429,15 +26423,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7unqlite_Collection __pyx_vtable_7unqlite_Collection;
 
 static PyObject *__pyx_tp_new_7unqlite_Collection(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_Collection *p;
@@ -26454,15 +26448,15 @@
   p->name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7unqlite_Collection(PyObject *o) {
   struct __pyx_obj_7unqlite_Collection *p = (struct __pyx_obj_7unqlite_Collection *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->unqlite);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
@@ -26610,15 +26604,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_7unqlite_CollectionIterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7unqlite_CollectionIterator *p;
   PyObject *o;
@@ -26634,15 +26628,15 @@
   p->collection = ((struct __pyx_obj_7unqlite_Collection *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7unqlite_CollectionIterator(PyObject *o) {
   struct __pyx_obj_7unqlite_CollectionIterator *p = (struct __pyx_obj_7unqlite_CollectionIterator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->vm);
   Py_CLEAR(p->unqlite);
   Py_CLEAR(p->collection);
@@ -26769,15 +26763,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct__commit_on_success *__pyx_freelist_7unqlite___pyx_scope_struct__commit_on_success[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct__commit_on_success = 0;
 
@@ -26894,15 +26888,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_1_keys *__pyx_freelist_7unqlite___pyx_scope_struct_1_keys[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_1_keys = 0;
 
@@ -27023,15 +27017,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_2_values *__pyx_freelist_7unqlite___pyx_scope_struct_2_values[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_2_values = 0;
 
@@ -27152,15 +27146,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_3_items *__pyx_freelist_7unqlite___pyx_scope_struct_3_items[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_3_items = 0;
 
@@ -27289,15 +27283,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_4_range *__pyx_freelist_7unqlite___pyx_scope_struct_4_range[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_4_range = 0;
 
@@ -27430,15 +27424,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7unqlite___pyx_scope_struct_5_fetch_until *__pyx_freelist_7unqlite___pyx_scope_struct_5_fetch_until[8];
 static int __pyx_freecount_7unqlite___pyx_scope_struct_5_fetch_until = 0;
 
@@ -27555,15 +27549,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -28277,21 +28271,22 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -30691,18 +30686,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -31635,18 +31627,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_36
-#define __PYX_HAVE_RT_ImportType_0_29_36
-static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
+#ifndef __PYX_HAVE_RT_ImportType
+#define __PYX_HAVE_RT_ImportType
+static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -31692,22 +31684,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -32168,15 +32160,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -32364,15 +32356,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -32598,15 +32590,15 @@
                         } else if (8 * sizeof(sxi64) >= 4 * PyLong_SHIFT) {
                             return (sxi64) (((((((((sxi64)digits[3]) << PyLong_SHIFT) | (sxi64)digits[2]) << PyLong_SHIFT) | (sxi64)digits[1]) << PyLong_SHIFT) | (sxi64)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33870,18 +33862,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `unqlite-0.9.4/unqlite.egg-info/PKG-INFO` & `unqlite-0.9.5/unqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unqlite
-Version: 0.9.4
+Version: 0.9.5
 Summary: Fast Python bindings for the UnQLite embedded NoSQL database.
 Home-page: https://github.com/coleifer/unqlite-python
 Author: Charles Leifer
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `unqlite-0.9.4/unqlite.pyx` & `unqlite-0.9.5/unqlite.pyx`

 * *Files identical despite different names*

