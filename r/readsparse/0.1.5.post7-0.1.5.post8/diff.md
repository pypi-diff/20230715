# Comparing `tmp/readsparse-0.1.5.post7.tar.gz` & `tmp/readsparse-0.1.5.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readsparse-0.1.5.post7.tar", last modified: Sun Mar 19 19:48:34 2023, max compression
+gzip compressed data, was "readsparse-0.1.5.post8.tar", last modified: Sat Jul 15 11:14:40 2023, max compression
```

## Comparing `readsparse-0.1.5.post7.tar` & `readsparse-0.1.5.post8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 19:48:34.991929 readsparse-0.1.5.post7/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2021-01-02 12:50:02.000000 readsparse-0.1.5.post7/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      371 2021-08-22 23:35:24.000000 readsparse-0.1.5.post7/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      245 2023-03-19 19:48:34.991929 readsparse-0.1.5.post7/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       86 2021-04-15 16:03:50.000000 readsparse-0.1.5.post7/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 19:48:34.991929 readsparse-0.1.5.post7/readsparse/
--rw-r--r--   0 david     (1000) david     (1000)    26933 2021-11-02 03:31:29.000000 readsparse-0.1.5.post7/readsparse/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    70879 2021-06-25 15:16:58.000000 readsparse-0.1.5.post7/readsparse/cpp_interface.pxi
--rw-r--r--   0 david     (1000) david     (1000)       83 2021-01-04 13:36:06.000000 readsparse-0.1.5.post7/readsparse/cpp_interface_size_t.pyx
--rw-r--r--   0 david     (1000) david     (1000)      120 2021-01-04 13:31:53.000000 readsparse-0.1.5.post7/readsparse/cpp_interface_uint64_t.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 19:48:34.991929 readsparse-0.1.5.post7/readsparse.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      245 2023-03-19 19:48:34.000000 readsparse-0.1.5.post7/readsparse.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      512 2023-03-19 19:48:34.000000 readsparse-0.1.5.post7/readsparse.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-03-19 19:48:34.000000 readsparse-0.1.5.post7/readsparse.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       11 2023-03-19 19:48:34.000000 readsparse-0.1.5.post7/readsparse.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       69 2023-03-19 19:47:22.000000 readsparse-0.1.5.post7/readsparse_compiler_testing.cpp
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-03-19 19:48:34.991929 readsparse-0.1.5.post7/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     9648 2023-03-19 19:46:43.000000 readsparse-0.1.5.post7/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 19:48:34.991929 readsparse-0.1.5.post7/src/
--rw-r--r--   0 david     (1000) david     (1000)     5594 2021-07-25 03:01:47.000000 readsparse-0.1.5.post7/src/python_streams.hpp
--rw-r--r--   0 david     (1000) david     (1000)    89722 2021-06-25 15:11:19.000000 readsparse-0.1.5.post7/src/reader.cpp
--rw-r--r--   0 david     (1000) david     (1000)    58520 2022-01-16 21:05:53.000000 readsparse-0.1.5.post7/src/reader.hpp
--rw-r--r--   0 david     (1000) david     (1000)    15446 2021-06-25 15:12:25.000000 readsparse-0.1.5.post7/src/readsparse.hpp
--rw-r--r--   0 david     (1000) david     (1000)    95786 2021-06-25 15:11:19.000000 readsparse-0.1.5.post7/src/readsparse_detemplated.hpp
--rw-r--r--   0 david     (1000) david     (1000)    10285 2022-09-11 18:48:32.000000 readsparse-0.1.5.post7/src/readsparse_internal.hpp
--rw-r--r--   0 david     (1000) david     (1000)     7226 2021-08-25 00:18:42.000000 readsparse-0.1.5.post7/src/utils.hpp
--rw-r--r--   0 david     (1000) david     (1000)    71373 2021-06-25 15:11:19.000000 readsparse-0.1.5.post7/src/writer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    37907 2021-07-14 01:23:59.000000 readsparse-0.1.5.post7/src/writer.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2021-01-02 12:50:02.000000 readsparse-0.1.5.post8/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      371 2021-08-22 23:35:24.000000 readsparse-0.1.5.post8/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      245 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       86 2021-04-15 16:03:50.000000 readsparse-0.1.5.post8/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.632311 readsparse-0.1.5.post8/readsparse/
+-rw-r--r--   0 david     (1000) david     (1000)    26992 2023-07-03 19:01:43.000000 readsparse-0.1.5.post8/readsparse/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    70879 2021-06-25 15:16:58.000000 readsparse-0.1.5.post8/readsparse/cpp_interface.pxi
+-rw-r--r--   0 david     (1000) david     (1000)       83 2021-01-04 13:36:06.000000 readsparse-0.1.5.post8/readsparse/cpp_interface_size_t.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      120 2021-01-04 13:31:53.000000 readsparse-0.1.5.post8/readsparse/cpp_interface_uint64_t.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.632311 readsparse-0.1.5.post8/readsparse.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      245 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      480 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       11 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     9648 2023-07-15 11:14:08.000000 readsparse-0.1.5.post8/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/src/
+-rw-r--r--   0 david     (1000) david     (1000)     5594 2021-07-25 03:01:47.000000 readsparse-0.1.5.post8/src/python_streams.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    89722 2021-06-25 15:11:19.000000 readsparse-0.1.5.post8/src/reader.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    58520 2022-01-16 21:05:53.000000 readsparse-0.1.5.post8/src/reader.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    15446 2021-06-25 15:12:25.000000 readsparse-0.1.5.post8/src/readsparse.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    95786 2021-06-25 15:11:19.000000 readsparse-0.1.5.post8/src/readsparse_detemplated.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    10285 2022-09-11 18:48:32.000000 readsparse-0.1.5.post8/src/readsparse_internal.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     7226 2021-08-25 00:18:42.000000 readsparse-0.1.5.post8/src/utils.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    71373 2021-06-25 15:11:19.000000 readsparse-0.1.5.post8/src/writer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    37907 2021-07-14 01:23:59.000000 readsparse-0.1.5.post8/src/writer.hpp
```

### Comparing `readsparse-0.1.5.post7/LICENSE` & `readsparse-0.1.5.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/readsparse/__init__.py` & `readsparse-0.1.5.post8/readsparse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import numpy as np
 import os, warnings
 import ctypes
-from scipy.sparse import csr_matrix, isspmatrix_csr
+from scipy.sparse import csr_array, issparse
 from . import _cpp_interface 
 
 __all__ = ["read_sparse", "write_sparse"]
 
+def _as_csr(X):
+    if not (issparse(X) and (X.format == "csr")):
+        X = csr_array(X)
+    return X
 
 ### Main functions
 def read_sparse(
         file, multilabel=False, has_qid=False, integer_labels=False,
         index1=True, sort_indices=True, ignore_zeros=True,
         min_cols=0, min_classes=0, limit_nrows=0, no_trailing_ws = False,
         use_int64=False, use_double=True, use_cpp=True, from_string=False
@@ -157,20 +161,20 @@
         If passing ``from_string=True``, then ``file`` is assumed to be a variable with the
         data contents on it.
 
     Returns
     -------
     data : dict
         A dict with the following entries:
-            - 'X' : the features, as a CSR Matrix from SciPy, with data of type ``np.float64``
+            - 'X' : the features, as a CSR array from SciPy, with data of type ``np.float64``
               or ``np.float32`` depending on argument ``use_double``.
             - 'y' : the labels. If passing ``multilabel=False`` (the default), will be a vector
               (NumPy 1-d array, with dtype float64 when passing ``integer_labels=False``, or
               dtype `equal to the indices of 'X' when passing ``integer_labels=True``),
-              otherwise will be a binary CSR Matrix (same dtype as the values of 'X').
+              otherwise will be a binary CSR array (same dtype as the values of 'X').
             - 'qid' : the query IDs used for ranking, as an integer vector.
               This entry will **only** be present when passing ``has_qid=True``
 
 
     References
     ----------
     Datasets in this format can be found here:
@@ -237,21 +241,21 @@
 
     if len(r) == 0:
         raise ValueError("Error: could not read file successfully.")
 
     r["ncols"] = max(r["ncols"], min_cols)
     r["nclasses"] = max(r["nclasses"], min_classes)
 
-    features = csr_matrix((r["values"], r["indices"], r["indptr"]),
-                          shape=(r["nrows"], r["ncols"]))
+    features = csr_array((r["values"], r["indices"], r["indptr"]),
+                         shape=(r["nrows"], r["ncols"]))
 
     if multilabel:
-        labels = csr_matrix((np.ones_like(r["indices_lab"], dtype=r["values"].dtype),
+        labels = csr_array((np.ones_like(r["indices_lab"], dtype=r["values"].dtype),
                              r["indices_lab"], r["indptr_lab"]),
-                            shape=(r["nrows"], r["nclasses"]))
+                           shape=(r["nrows"], r["nclasses"]))
     else:
         labels = r["labels"]
         if integer_labels:
             if use_int64:
                 labels = labels.astype(np.int64)
             else:
                 labels = labels.astype(ctypes.c_int)
@@ -312,15 +316,15 @@
     Parameters
     ----------
     file : str or None
         Output file path into which to write the data.
         Will be ignored when passing ``to_string=True``.
     X : CSR(n_samples, n_labels)
         Sparse data to write. Can be a sparse matrix from SciPy, a dense array from NumPy,
-        or a DataFrame from Pandas, but will be converted to a CSR matrix if it isn't already.
+        or a DataFrame from Pandas, but will be converted to a CSR array if it isn't already.
 
         If ``X`` is a vector (1-d NumPy array), will be assumed to
         be a row vector and will thus write one row only.
     y : array(n_samples,) or CSR(n_samples, n_labels)
         Labels for the data. Can be passed as a vector
         if each observation has one label, or as a sparse or dense matrix (same format as ``X``)
         if each observation can have more than 1 label. In the latter case, only the non-missing
@@ -335,15 +339,15 @@
          For multilabel classification, the labels will always be written as integers.
     index1 : bool
         Whether the column and label indices (if multi-label) should have numeration
         starting at 1. Most software assumes this is ``True``.
     sort_indices : bool
         Whether to sort the indices of ``X`` (and of ``y`` if multi-label) before
         writing the data. Note that this will cause in-place modifications if either ``X`` or ``y``
-        are passed as CSR matrices.
+        are passed as CSR arrays/matrices.
     ignore_zeros : bool
         Whether to ignore (not write) features with a value of zero
         after rounding to the specified decimal places.
     add_header : bool
         Whether to add a header with metadata as the first line (number of rows,
         number of columns, number of classes). If passing ``integer_label=False`` and ``y`` is a
         vector, will write zero as the number of labels. This is not supported by most software.
@@ -395,17 +399,17 @@
         to_string = True
     if not use_cpp:
         to_string = True
 
     ### Note: this check should be made right here due to potential
     ### in-place modifications of the data which would render the input unusable
     if sort_indices:
-        if isspmatrix_csr(y):
+        if issparse(y) and (y.format == "csr"):
             y.sort_indices()
-        if isspmatrix_csr(X):
+        if issparse(X) and (X.format == "csr"):
             X.sort_indices()
         sort_indices = False
 
     indptr, indices, values, nrows, ncols = _process_X(X)
     indptr_lab, indices_lab, labels, nrows_y, nclasses = _process_y(y, add_header, integer_labels)
     qid = _process_qid(qid)
     if nrows != nrows_y:
@@ -517,16 +521,15 @@
 
 ### Helpers
 dtypes_indices = [ctypes.c_int, np.int64, ctypes.c_size_t]
 dtypes_values = [np.float32, np.float64]
 dtypes_labels = dtypes_indices + dtypes_values
 
 def _process_X(X):
-    if not isspmatrix_csr(X):
-        X = csr_matrix(X)
+    X = _as_csr(X)
     return (
         X.indptr,
         X.indices,
         X.data if X.data.dtype in dtypes_values else X.data.astype(np.float64),
         X.shape[0], X.shape[1]
     )
 
@@ -569,16 +572,15 @@
                     nclasses = int(nclasses)
 
             if (integer_labels) and (y.dtype not in dtypes_indices):
                 y = y.astype(np.int64)
 
             return None, None, y, y.shape[0], nclasses
 
-    if not isspmatrix_csr(y):
-        y = csr_matrix(y)
+    y = _as_csr(y)
     return (
         y.indptr,
         y.indices,
         None, y.shape[0], y.shape[1]
     )
 
 def _process_qid(qid):
```

### Comparing `readsparse-0.1.5.post7/readsparse/cpp_interface.pxi` & `readsparse-0.1.5.post8/readsparse/cpp_interface.pxi`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/setup.py` & `readsparse-0.1.5.post8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     platform_is_32 = True
 
 is_windows = sys.platform[:3] == "win"
 
 setup(
     name  = "readsparse",
     packages = ["readsparse"],
-    version = '0.1.5-7',
+    version = '0.1.5-8',
     description = 'Read and Write Sparse Matrices in Text Format',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/readsparse',
     keywords = ['sparse', 'svmlight', 'libsvm'],
     cmdclass = {'build_ext': build_ext_subclass},
     ext_modules = [Extension(
                                 "readsparse._cpp_interface",
```

### Comparing `readsparse-0.1.5.post7/src/python_streams.hpp` & `readsparse-0.1.5.post8/src/python_streams.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/reader.cpp` & `readsparse-0.1.5.post8/src/reader.cpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/reader.hpp` & `readsparse-0.1.5.post8/src/reader.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/readsparse.hpp` & `readsparse-0.1.5.post8/src/readsparse.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/readsparse_detemplated.hpp` & `readsparse-0.1.5.post8/src/readsparse_detemplated.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/readsparse_internal.hpp` & `readsparse-0.1.5.post8/src/readsparse_internal.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/utils.hpp` & `readsparse-0.1.5.post8/src/utils.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/writer.cpp` & `readsparse-0.1.5.post8/src/writer.cpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post7/src/writer.hpp` & `readsparse-0.1.5.post8/src/writer.hpp`

 * *Files identical despite different names*

