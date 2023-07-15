# Comparing `tmp/sortedness-1.230712.1.tar.gz` & `tmp/sortedness-1.230712.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedness-1.230712.1.tar", max compression
+gzip compressed data, was "sortedness-1.230712.2.tar", max compression
```

## Comparing `sortedness-1.230712.1.tar` & `sortedness-1.230712.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-1.230712.1/LICENSE
--rw-r--r--   0        0        0     7251 2023-07-12 15:53:01.162358 sortedness-1.230712.1/README.md
--rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-1.230712.1/build.py
--rw-r--r--   0        0        0     1368 2023-07-12 15:53:04.218353 sortedness-1.230712.1/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-02 18:43:33.326749 sortedness-1.230712.1/src/sortedness/__init__.py
--rw-r--r--   0        0        0     7224 2023-07-07 00:44:07.161305 sortedness-1.230712.1/src/sortedness/agnostic.py
--rw-r--r--   0        0        0     1281 2023-05-02 18:58:14.909747 sortedness-1.230712.1/src/sortedness/config.py
--rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-1.230712.1/src/sortedness/evaluation/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-02 18:58:14.873747 sortedness-1.230712.1/src/sortedness/evaluation/plot.py
--rw-r--r--   0        0        0     5145 2023-05-02 18:58:14.889747 sortedness-1.230712.1/src/sortedness/global_.py
--rw-r--r--   0        0        0     3043 2023-07-07 00:44:07.169305 sortedness-1.230712.1/src/sortedness/gtau.py
--rw-r--r--   0        0        0    33215 2023-07-12 15:48:36.350842 sortedness-1.230712.1/src/sortedness/local.py
--rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-1.230712.1/src/sortedness/matrices.py
--rw-r--r--   0        0        0     2983 2023-07-11 23:12:22.741346 sortedness-1.230712.1/src/sortedness/parallel.py
--rw-r--r--   0        0        0     8399 2023-07-07 00:56:13.866263 sortedness-1.230712.1/src/sortedness/rank.py
--rw-r--r--   0        0        0     4707 2023-05-02 18:58:14.909747 sortedness-1.230712.1/src/sortedness/trustworthiness.py
--rw-r--r--   0        0        0     3518 2023-07-07 00:28:29.856946 sortedness-1.230712.1/src/sortedness/wtau/__init__.py
--rw-r--r--   0        0        0  1267818 2023-07-12 00:45:59.562335 sortedness-1.230712.1/src/sortedness/wtau/wtau.c
--rwxr-xr-x   0        0        0  1348408 2023-05-30 20:09:00.000000 sortedness-1.230712.1/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0        0        0   334715 2023-07-12 00:45:59.586335 sortedness-1.230712.1/src/sortedness/wtau/wtau.html
--rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-1.230712.1/src/sortedness/wtau/wtau.pyx
--rw-r--r--   0        0        0     8470 1970-01-01 00:00:00.000000 sortedness-1.230712.1/setup.py
--rw-r--r--   0        0        0     7856 1970-01-01 00:00:00.000000 sortedness-1.230712.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-1.230712.2/LICENSE
+-rw-r--r--   0        0        0     7314 2023-07-15 02:47:54.433362 sortedness-1.230712.2/README.md
+-rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-1.230712.2/build.py
+-rw-r--r--   0        0        0     1368 2023-07-15 02:47:56.001362 sortedness-1.230712.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-02 18:43:33.326749 sortedness-1.230712.2/src/sortedness/__init__.py
+-rw-r--r--   0        0        0     7224 2023-07-07 00:44:07.161305 sortedness-1.230712.2/src/sortedness/agnostic.py
+-rw-r--r--   0        0        0     1281 2023-05-02 18:58:14.909747 sortedness-1.230712.2/src/sortedness/config.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-1.230712.2/src/sortedness/evaluation/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-02 18:58:14.873747 sortedness-1.230712.2/src/sortedness/evaluation/plot.py
+-rw-r--r--   0        0        0     5145 2023-05-02 18:58:14.889747 sortedness-1.230712.2/src/sortedness/global_.py
+-rw-r--r--   0        0        0     3043 2023-07-07 00:44:07.169305 sortedness-1.230712.2/src/sortedness/gtau.py
+-rw-r--r--   0        0        0    32707 2023-07-15 02:47:38.881365 sortedness-1.230712.2/src/sortedness/local.py
+-rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-1.230712.2/src/sortedness/matrices.py
+-rw-r--r--   0        0        0     2983 2023-07-11 23:12:22.741346 sortedness-1.230712.2/src/sortedness/parallel.py
+-rw-r--r--   0        0        0     8399 2023-07-07 00:56:13.866263 sortedness-1.230712.2/src/sortedness/rank.py
+-rw-r--r--   0        0        0     4707 2023-05-02 18:58:14.909747 sortedness-1.230712.2/src/sortedness/trustworthiness.py
+-rw-r--r--   0        0        0     3518 2023-07-07 00:28:29.856946 sortedness-1.230712.2/src/sortedness/wtau/__init__.py
+-rw-r--r--   0        0        0  1267818 2023-07-12 16:04:40.593147 sortedness-1.230712.2/src/sortedness/wtau/wtau.c
+-rwxr-xr-x   0        0        0  1348408 2023-05-30 20:09:00.000000 sortedness-1.230712.2/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0   334715 2023-07-12 15:53:25.926317 sortedness-1.230712.2/src/sortedness/wtau/wtau.html
+-rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-1.230712.2/src/sortedness/wtau/wtau.pyx
+-rw-r--r--   0        0        0     8534 1970-01-01 00:00:00.000000 sortedness-1.230712.2/setup.py
+-rw-r--r--   0        0        0     7919 1970-01-01 00:00:00.000000 sortedness-1.230712.2/PKG-INFO
```

### Comparing `sortedness-1.230712.1/LICENSE` & `sortedness-1.230712.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/README.md` & `sortedness-1.230712.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 ![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)
 [![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)
 [![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sortedness)
 
 
 # sortedness
 
 `sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.
-This ia valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.
+This is valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.
 It is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.
 <br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 
 ## Overview
 Local variants return a value for each provided point. The global variant returns a single value for all points.
 Any local variant can be used as a global measure by taking the mean value.
```

#### html2text {}

```diff
@@ -3,20 +3,21 @@
 badge.svg)](https://codecov.io/gh/sortedness/sortedness) [github] ![Python
 version](https://img.shields.io/badge/python-3.8+-blue.svg) [![license: GPL v3]
 (https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)  [![API documentation](https://img.shields.io/badge/doc-
 API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness) [![DOI]
 (https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/
 513273889) [![Downloads](https://static.pepy.tech/badge/sortedness)](https://
-pepy.tech/project/sortedness) # sortedness `sortedness` is the level of
-agreement between two points regarding to how they rank all remaining points in
-a dataset. This ia valid even for points from different spaces, enabling the
-measurement of the quality of data transformation processes, often
-dimensionality reduction. It is less sensitive to irrelevant distortions, and
-return values in a more meaningful interval, than Kruskal stress formula I.
+pepy.tech/project/sortedness) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/sortedness) # sortedness `sortedness` is the level of agreement between two
+points regarding to how they rank all remaining points in a dataset. This is
+valid even for points from different spaces, enabling the measurement of the
+quality of data transformation processes, often dimensionality reduction. It is
+less sensitive to irrelevant distortions, and return values in a more
+meaningful interval, than Kruskal stress formula I.
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
 functions presented [here (paper unavailable until publication)](https://
 scholar.google.com/
 scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 ## Overview Local variants return a value for each provided point. The global
 variant returns a single value for all points. Any local variant can be used as
```

### Comparing `sortedness-1.230712.1/build.py` & `sortedness-1.230712.2/build.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/pyproject.toml` & `sortedness-1.230712.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortedness"
-version = "1.230712.1"
+version = "1.230712.2"
 description = "Measures of projection quality"
 authors = ["davips <dpsabc@gmail.com>", "tacito <tacito.neves@gmail.com>"]
 license = "GPLv3"
 build = "build.py"  # For Cython. apt-get package needed: python3-numpy
 readme = 'README.md'
 packages = [
     { include = "sortedness", from = "src" }
```

### Comparing `sortedness-1.230712.1/src/sortedness/agnostic.py` & `sortedness-1.230712.2/src/sortedness/agnostic.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/config.py` & `sortedness-1.230712.2/src/sortedness/config.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/evaluation/plot.py` & `sortedness-1.230712.2/src/sortedness/evaluation/plot.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/global_.py` & `sortedness-1.230712.2/src/sortedness/global_.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/gtau.py` & `sortedness-1.230712.2/src/sortedness/gtau.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/local.py` & `sortedness-1.230712.2/src/sortedness/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,18 @@
     array([1., 1., 1., 1., 1., 1., 1.])
     >>> projected = np.array([[0],[6],[5],[4],[3],[2],[1]])
     >>> sortedness(original, projected)
     array([-1.        ,  0.51956213,  0.81695345,  0.98180162,  0.98180162,
             0.81695345,  0.51956213])
     >>> sortedness(original, projected, 1)
     0.519562134793
+    >>> sortedness(original, projected, rank=True)[1]
+    0.519562134793
+    >>> sortedness(original, projected, rank=False)[1]
+    0.074070734162
     >>> sortedness(original, projected, 1, symmetric=False)
     0.422638894922
     >>> sortedness([[1,2,3,3],[1,2,7,3],[3,4,8,5],[1,8,3,5]], [[2,1,2,3],[3,1,2,3],[5,4,5,6],[9,7,6,3]], 1)
     0.181818181818
     """
     isweightedtau = False
     if hasattr(f, "isweightedtau") and f.isweightedtau:
@@ -233,15 +237,14 @@
             if "rank" in kwargs:  # pragma: no cover
                 raise Exception(f"Cannot set `symmetric=False` and provide `rank` at the same time.")
             kwargs["rank"] = None
     elif not symmetric:  # pragma: no cover
         raise Exception(f"`symmetric=False` not implemented for custom `f`")
     if parallel_kwargs is None:
         parallel_kwargs = {}
-    result, pvalues = [], []
     npoints = len(X)
 
     if i is not None:
         x = X[i] if isinstance(X, (ndarray, list)) else X.iloc[i].to_numpy()
         x_ = X_[i] if isinstance(X_, (ndarray, list)) else X_.iloc[i].to_numpy()
         X = np.delete(X, i, axis=0)
         X_ = np.delete(X_, i, axis=0)
@@ -249,44 +252,36 @@
         if distance_dependent:
             d = np.sum((X - x) ** 2, axis=1)
             scores_X, scores_X_ = (-d, -d_) if isweightedtau else (d, d_)
             corr, pvalue = f(scores_X, scores_X_, **kwargs)
             return (np.round(corr, 12), pvalue) if return_pvalues else np.round(corr, 12)
         else:  # pragma: no cover
             raise Exception(f"Not implemented yet; it is an open problem")
-            # D = abs(X - x).T
-            # scores_X, scores_x_ = (-D, -d_) if isweightedtau else (D, d_)
-            # for j in range(len(scores_X)):
-            #     corr, pvalue = f(scores_X[j], scores_x_, **kwargs)
-            #     result.append(round(corr, 12))
-            #     pvalues.append(round(pvalue, 12))
-            # return (mean(result), mean(pvalues)) if return_pvalues else mean(result)
 
     if distance_dependent:
+        def thread(a, b):
+            return f(a, b, **kwargs)
         tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
+        pmap = mp.ProcessingPool(**parallel_kwargs).imap if parallel and npoints > parallel_n_trigger else map
         sqdist_X, sqdist_X_ = tmap(lambda M: cdist(M, M, metric='sqeuclidean'), [X, X_])
         D = remove_diagonal(sqdist_X)
         D_ = remove_diagonal(sqdist_X_)
         scores_X, scores_X_ = (-D, -D_) if isweightedtau else (D, D_)
-        for i in range(len(X)):
-            corr, pvalue = f(scores_X[i], scores_X_[i], **kwargs)
-            result.append(round(corr, 12))
-            pvalues.append(round(pvalue, 12))
+        jobs = pmap(thread if kwargs else f, scores_X, scores_X_)
+        result, pvalues = [], []
+        for corr, pvalue in jobs:
+            result.append(corr)
+            pvalues.append(pvalue)
     else:  # pragma: no cover
         raise Exception(f"Not implemented yet; it is an open problem")
-        #     for i in range(len(X)):
-    #         corr, pvalue = sortedness(X, X_, i, f=f, distance_dependent=False, return_pvalues=True,
-    #                                   parallel=parallel, parallel_n_trigger=parallel_n_trigger, parallel_kwargs=parallel_kwargs, **kwargs)
-    #         result.append(round(corr, 12))
-    #         pvalues.append(round(pvalue, 12))
 
     result = np.array(result, dtype=float)
     if return_pvalues:
-        return np.array(list(zip(result, pvalues)))
-    return result
+        return np.round(np.array(list(zip(result, pvalues))), 12)
+    return np.round(result, 12)
 
 
 def pwsortedness(X, X_, i=None, symmetric=True, f=weightedtau, parallel=True, parallel_n_trigger=200, batches=10, debug=False, dist=None, cython=False, parallel_kwargs=None, **kwargs):
     """
     Local pairwise sortedness (Λ𝜏w) based on Sebastiano Vigna weighted Kendall's 𝜏
 
     Importance rankings are calculated internally based on proximity of each pair to the point of interest.
@@ -587,34 +582,23 @@
     R, R_ = (rank_alongcol(M, parallel=parallel) for M in [D, D_])
     scores_X, scores_X_ = tmap(lambda M: -remove_diagonal(M), [R, R_])  # For f=weightedtau: scores = -ranks.
 
     if hasattr(f, "isparwtau"):  # pragma: no cover
         raise Exception("TODO: Pairtau implementation disagree with scipy weightedtau")
         # return parwtau(scores_X, scores_X_, npoints, parallel=parallel, **kwargs)
 
-    def thread(l):
-        lst1 = []
-        lst2 = []
-        for i in l:
-            corr, pvalue = f(scores_X[i], scores_X_[i], **kwargs)
-            lst1.append(round(corr, 12))
-            lst2.append(round(pvalue, 12))
-        return lst1, lst2
-
-    result, pvalues = [], []
-    try:
-        from shelchemy.lazy import ichunks
-    except Exception as e:
-        print("please install shelchemy library.")
-        exit()
     if i is None:
-        jobs = pmap(thread, ichunks(range(npoints), 15, asgenerators=False))
-        for corrs, pvalues in jobs:
-            result.extend(corrs)
-            pvalues.extend(pvalues)
+        def thread(a, b):
+            return f(a, b, **kwargs)
+
+        jobs = pmap(thread if kwargs else f, scores_X, scores_X_)
+        result, pvalues = [], []
+        for corr, pvalue in jobs:
+            result.append(corr)
+            pvalues.append(pvalue)
 
         result = np.array(result, dtype=float)
         if return_pvalues:
             return np.array(list(zip(result, pvalues)))
         return result
 
     corr, pvalue = f(scores_X[i], scores_X_[i], **kwargs)
@@ -624,14 +608,35 @@
 
 
 def stress(X, X_, i=None, metric=True, parallel=True, parallel_size_trigger=10000, **parallel_kwargs):
     """
     Kruskal's "Stress Formula 1" normalized before comparing distances.
     default: Euclidean
 
+    Parameters
+    ----------
+    X
+        matrix with an instance by row in a given space (often the original one)
+    X_
+        matrix with an instance by row in another given space (often the projected one)
+    i
+        None:   calculate stress for all instances
+        `int`:  index of the instance of interest
+    metric
+        Stress formula version: metric or nonmetric
+    parallel
+        Parallelize processing when |X|>1000. Might use more memory.
+
+    Returns
+    -------
+    parallel_kwargs
+        Any extra argument to be provided to pathos parallelization
+    parallel_n_trigger
+        Threshold to disable parallelization for small n values
+
     >>> import numpy as np
     >>> from functools import partial
     >>> from scipy.stats import spearmanr, weightedtau
     >>> mean = (1, 12)
     >>> cov = eye(2)
     >>> rng = np.random.default_rng(seed=0)
     >>> original = rng.multivariate_normal(mean, cov, size=12)
@@ -670,29 +675,14 @@
     array([0.36599664, 0.39465927, 0.27349092, 0.25096851, 0.31476019,
            0.27612935, 0.3064739 , 0.26141414, 0.2635681 , 0.25811772,
            0.36113025, 0.29740821])
     >>> stress(original, projected, 1)
     0.316031007598
     >>> stress(original, projected, 1, metric=False)
     0.39465927169
-
-    Parameters
-    ----------
-    X
-        matrix with an instance by row in a given space (often the original one)
-    X_
-        matrix with an instance by row in another given space (often the projected one)
-    metric
-        Stress formula version: metric or nonmetric
-    parallel
-        Parallelize processing when |X|>1000. Might use more memory.
-
-    Returns
-    -------
-
     """
     tmap = mp.ThreadingPool(**parallel_kwargs).imap if parallel and X.size > parallel_size_trigger else map
     # TODO: parallelize cdist in slices?
     if metric:
         thread = (lambda M, m: cdist(M, M, metric=m)) if i is None else (lambda M, m: cdist(M[i:i + 1], M, metric=m))
         D, Dsq_ = tmap(thread, [X, X_], ["Euclidean", "sqeuclidean"])
         Dsq_ /= Dsq_.max(axis=1, keepdims=True)
@@ -702,15 +692,15 @@
         D, Dsq_ = tmap(thread, [X, X_], ["Euclidean", "sqeuclidean"])
         Dsq_ /= Dsq_.max(axis=1, keepdims=True)
         D_ = sqrt(Dsq_)
 
     D /= D.max(axis=1, keepdims=True)
     s = ((D - D_) ** 2).sum(axis=1) / 2
     result = np.round(np.sqrt(s / (Dsq_.sum(axis=1) / 2)), 12)
-    return result if i is None else result[0]
+    return result if i is None else result.flat[0]
 
 
 def hyperbolic(x):
     """
     >>> import numpy as np
     >>> np.round(list(map(hyperbolic, range(10))), 12).tolist()
     [1.0, 0.5, 0.333333333333, 0.25, 0.2, 0.166666666667, 0.142857142857, 0.125, 0.111111111111, 0.1]
```

### Comparing `sortedness-1.230712.1/src/sortedness/matrices.py` & `sortedness-1.230712.2/src/sortedness/matrices.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/parallel.py` & `sortedness-1.230712.2/src/sortedness/parallel.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/rank.py` & `sortedness-1.230712.2/src/sortedness/rank.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/trustworthiness.py` & `sortedness-1.230712.2/src/sortedness/trustworthiness.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/wtau/__init__.py` & `sortedness-1.230712.2/src/sortedness/wtau/__init__.py`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/wtau/wtau.c` & `sortedness-1.230712.2/src/sortedness/wtau/wtau.c`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so` & `sortedness-1.230712.2/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/wtau/wtau.html` & `sortedness-1.230712.2/src/sortedness/wtau/wtau.html`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/src/sortedness/wtau/wtau.pyx` & `sortedness-1.230712.2/src/sortedness/wtau/wtau.pyx`

 * *Files identical despite different names*

### Comparing `sortedness-1.230712.1/setup.py` & `sortedness-1.230712.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['lange>=1.230203.1,<2.0.0', 'pathos>=0.3.0,<0.4.0']
 
 extras_require = \
 {':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'sortedness',
-    'version': '1.230712.1',
+    'version': '1.230712.2',
     'description': 'Measures of projection quality',
-    'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n\n# sortedness\n\n`sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.\nThis ia valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n## Overview\nLocal variants return a value for each provided point. The global variant returns a single value for all points.\nAny local variant can be used as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant: `global_sortedness(X, X_)`.\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import sortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = sortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.393463224666 0.7565797804351666 0.944810120534\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.648305479567 -0.09539895194975 0.397019507592\n"""\n```\n\n```python3\n\n# Single point fast calculation.\ns = sortedness(original, projectedrnd, 2)\nprint(s)\n"""\n0.231079547491\n"""\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = pwsortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.649315577592 0.7534291438323333 0.834601601062\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.168611098044 -0.07988253899799999 0.14442446342\n"""\n```\n\n```python3\n\n# Single point fast calculation.\ns = pwsortedness(original, projectedrnd, 2)\nprint(s)\n"""\n0.036119718802\n"""\n```\n\n\n</p>\n</details>\n\n**Global pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import global_pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print measurement result and p-value.\ns = global_pwsortedness(original, original)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected2)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected1)\nprint(list(s))\n"""\n[0.7715617715617715, 5.240847664048334e-20]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projectedrnd)\nprint(list(s))\n"""\n[-0.06107226107226107, 0.46847188611226276]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**\n\n\n### TODO\nFuture work address handling large datasets: approximate sortedness value, and size-insensitive weighting scheme.\n\n## Reference\nPlease use the following reference to cite this work:\n```\n@inproceedings {10.2312:eurova.20231093,\nbooktitle = {EuroVis Workshop on Visual Analytics (EuroVA)},\neditor = {Angelini, Marco and El-Assady, Mennatallah},\ntitle = {{Nonparametric Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted Neighborhood}},\nauthor = {Pereira-Santos, Davi and Neves, Tácito Trindade Araújo Tiburtino and Carvalho, André C. P. L. F. de and Paulovich, Fernando V.},\nyear = {2023},\npublisher = {The Eurographics Association},\nISSN = {2664-4487},\nISBN = {978-3-03868-222-6},\nDOI = {10.2312/eurova.20231093}\n}\n```\n\n## Grants\nThis work was supported by Wellcome Leap 1kD Program; São\nPaulo Research Foundation (FAPESP) - grant 2020/09835-1; Cana-\ndian Institute for Health Research (CIHR) Canadian Research\nChairs (CRC) stipend [award number 1024586]; Canadian Foun-\ndation for Innovation (CFI) John R. Evans Leaders Fund (JELF)\n[grant number 38835]; Dalhousie Medical Research Fund (DMRF)\nCOVID-19 Research Grant [grant number 603082]; and the Cana-\ndian Institute for Health Research (CIHR) Project Grant [award\nnumber 177968].\n',
+    'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/sortedness)\n\n\n# sortedness\n\n`sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.\nThis is valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n## Overview\nLocal variants return a value for each provided point. The global variant returns a single value for all points.\nAny local variant can be used as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant: `global_sortedness(X, X_)`.\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import sortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = sortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.393463224666 0.7565797804351666 0.944810120534\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.648305479567 -0.09539895194975 0.397019507592\n"""\n```\n\n```python3\n\n# Single point fast calculation.\ns = sortedness(original, projectedrnd, 2)\nprint(s)\n"""\n0.231079547491\n"""\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print `min`, `mean`, and `max` values.\ns = pwsortedness(original, original)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n1.0 1.0 1.0\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n0.649315577592 0.7534291438323333 0.834601601062\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\nprint(min(s), sum(s) / len(s), max(s))\n"""\n-0.168611098044 -0.07988253899799999 0.14442446342\n"""\n```\n\n```python3\n\n# Single point fast calculation.\ns = pwsortedness(original, projectedrnd, 2)\nprint(s)\n"""\n0.036119718802\n"""\n```\n\n\n</p>\n</details>\n\n**Global pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness import global_pwsortedness\n\n# Some synthetic data.\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\n# Print measurement result and p-value.\ns = global_pwsortedness(original, original)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected2)\nprint(list(s))\n"""\n[1.0, 3.6741408919675163e-93]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projected1)\nprint(list(s))\n"""\n[0.7715617715617715, 5.240847664048334e-20]\n"""\n```\n\n```python3\n\ns = global_pwsortedness(original, projectedrnd)\nprint(list(s))\n"""\n[-0.06107226107226107, 0.46847188611226276]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2023. Davi Pereira dos Santos and Tacito Neves**\n\n\n### TODO\nFuture work address handling large datasets: approximate sortedness value, and size-insensitive weighting scheme.\n\n## Reference\nPlease use the following reference to cite this work:\n```\n@inproceedings {10.2312:eurova.20231093,\nbooktitle = {EuroVis Workshop on Visual Analytics (EuroVA)},\neditor = {Angelini, Marco and El-Assady, Mennatallah},\ntitle = {{Nonparametric Dimensionality Reduction Quality Assessment based on Sortedness of Unrestricted Neighborhood}},\nauthor = {Pereira-Santos, Davi and Neves, Tácito Trindade Araújo Tiburtino and Carvalho, André C. P. L. F. de and Paulovich, Fernando V.},\nyear = {2023},\npublisher = {The Eurographics Association},\nISSN = {2664-4487},\nISBN = {978-3-03868-222-6},\nDOI = {10.2312/eurova.20231093}\n}\n```\n\n## Grants\nThis work was supported by Wellcome Leap 1kD Program; São\nPaulo Research Foundation (FAPESP) - grant 2020/09835-1; Cana-\ndian Institute for Health Research (CIHR) Canadian Research\nChairs (CRC) stipend [award number 1024586]; Canadian Foun-\ndation for Innovation (CFI) John R. Evans Leaders Fund (JELF)\n[grant number 38835]; Dalhousie Medical Research Fund (DMRF)\nCOVID-19 Research Grant [grant number 603082]; and the Cana-\ndian Institute for Health Research (CIHR) Project Grant [award\nnumber 177968].\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['sortedness', 'sortedness.evaluation', 'sortedness.wtau']
 package_data = \ {'': ['*']} install_requires = \ ['lange>=1.230203.1,<2.0.0',
 'pathos>=0.3.0,<0.4.0'] extras_require = \ {':python_version >= "3.8" and
 python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']} setup_kwargs = { 'name':
-'sortedness', 'version': '1.230712.1', 'description': 'Measures of projection
+'sortedness', 'version': '1.230712.2', 'description': 'Measures of projection
 quality', 'long_description': '![test](https://github.com/sortedness/
 sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/
 sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/
 sortedness/sortedness)\n\n[github]\n\n![Python version](https://img.shields.io/
 badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/
 License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![API
 documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)]
 (https://sortedness.github.io/sortedness)\n[![DOI](https://zenodo.org/badge/
 513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)\n[![Downloads]
 (https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/
+sortedness)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/
 sortedness)\n\n\n# sortedness\n\n`sortedness` is the level of agreement between
 two points regarding to how they rank all remaining points in a dataset.\nThis
-ia valid even for points from different spaces, enabling the measurement of the
+is valid even for points from different spaces, enabling the measurement of the
 quality of data transformation processes, often dimensionality reduction.\nIt
 is less sensitive to irrelevant distortions, and return values in a more
 meaningful interval, than Kruskal stress formula I.\n
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
 functions presented [here (paper unavailable until publication)](https://
 scholar.google.com/
```

### Comparing `sortedness-1.230712.1/PKG-INFO` & `sortedness-1.230712.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortedness
-Version: 1.230712.1
+Version: 1.230712.2
 Summary: Measures of projection quality
 License: GPLv3
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -23,20 +23,21 @@
 ![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!-- [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)
 [![DOI](https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/513273889)
 [![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sortedness)
 
 
 # sortedness
 
 `sortedness` is the level of agreement between two points regarding to how they rank all remaining points in a dataset.
-This ia valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.
+This is valid even for points from different spaces, enabling the measurement of the quality of data transformation processes, often dimensionality reduction.
 It is less sensitive to irrelevant distortions, and return values in a more meaningful interval, than Kruskal stress formula I.
 <br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 
 ## Overview
 Local variants return a value for each provided point. The global variant returns a single value for all points.
 Any local variant can be used as a global measure by taking the mean value.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sortedness Version: 1.230712.1 Summary: Measures of
+Metadata-Version: 2.1 Name: sortedness Version: 1.230712.2 Summary: Measures of
 projection quality License: GPLv3 Author: davips Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lange (>=1.230203.1,<2.0.0) Requires-Dist: pathos
 (>=0.3.0,<0.4.0) Requires-Dist: scipy (>=1.10.1,<2.0.0) ; python_version >=
 "3.8" and python_version < "3.11" Description-Content-Type: text/markdown !
@@ -11,20 +11,21 @@
 badge.svg)](https://codecov.io/gh/sortedness/sortedness) [github] ![Python
 version](https://img.shields.io/badge/python-3.8+-blue.svg) [![license: GPL v3]
 (https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)  [![API documentation](https://img.shields.io/badge/doc-
 API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness) [![DOI]
 (https://zenodo.org/badge/513273889.svg)](https://zenodo.org/badge/latestdoi/
 513273889) [![Downloads](https://static.pepy.tech/badge/sortedness)](https://
-pepy.tech/project/sortedness) # sortedness `sortedness` is the level of
-agreement between two points regarding to how they rank all remaining points in
-a dataset. This ia valid even for points from different spaces, enabling the
-measurement of the quality of data transformation processes, often
-dimensionality reduction. It is less sensitive to irrelevant distortions, and
-return values in a more meaningful interval, than Kruskal stress formula I.
+pepy.tech/project/sortedness) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/sortedness) # sortedness `sortedness` is the level of agreement between two
+points regarding to how they rank all remaining points in a dataset. This is
+valid even for points from different spaces, enabling the measurement of the
+quality of data transformation processes, often dimensionality reduction. It is
+less sensitive to irrelevant distortions, and return values in a more
+meaningful interval, than Kruskal stress formula I.
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
 functions presented [here (paper unavailable until publication)](https://
 scholar.google.com/
 scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 ## Overview Local variants return a value for each provided point. The global
 variant returns a single value for all points. Any local variant can be used as
```

