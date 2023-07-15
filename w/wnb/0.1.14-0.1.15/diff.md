# Comparing `tmp/wnb-0.1.14.tar.gz` & `tmp/wnb-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnb-0.1.14.tar", last modified: Fri Jun  9 18:20:06 2023, max compression
+gzip compressed data, was "wnb-0.1.15.tar", last modified: Sat Jul 15 02:51:38 2023, max compression
```

## Comparing `wnb-0.1.14.tar` & `wnb-0.1.15.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.043672 wnb-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-09 18:20:06.043672 wnb-0.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-09 18:19:55.000000 wnb-0.1.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 18:20:06.043672 wnb-0.1.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-09 18:19:55.000000 wnb-0.1.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.035672 wnb-0.1.14/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-09 18:19:55.000000 wnb-0.1.14/tests/test_gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-09 18:19:55.000000 wnb-0.1.14/tests/test_gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.039672 wnb-0.1.14/wnb/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-06-09 18:19:55.000000 wnb-0.1.14/wnb/gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:20:06.039672 wnb-0.1.14/wnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 18:20:06.000000 wnb-0.1.14/wnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:51:38.418533 wnb-0.1.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-15 02:51:38.418533 wnb-0.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-15 02:51:26.000000 wnb-0.1.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:51:38.418533 wnb-0.1.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 02:51:26.000000 wnb-0.1.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:51:38.414533 wnb-0.1.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-07-15 02:51:26.000000 wnb-0.1.15/tests/test_gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-15 02:51:26.000000 wnb-0.1.15/tests/test_gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:51:38.418533 wnb-0.1.15/wnb/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 02:51:26.000000 wnb-0.1.15/wnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-15 02:51:26.000000 wnb-0.1.15/wnb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-15 02:51:26.000000 wnb-0.1.15/wnb/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-15 02:51:26.000000 wnb-0.1.15/wnb/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-15 02:51:26.000000 wnb-0.1.15/wnb/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-07-15 02:51:26.000000 wnb-0.1.15/wnb/gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:51:38.418533 wnb-0.1.15/wnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-15 02:51:38.000000 wnb-0.1.15/wnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-15 02:51:38.000000 wnb-0.1.15/wnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:51:38.000000 wnb-0.1.15/wnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 02:51:38.000000 wnb-0.1.15/wnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 02:51:38.000000 wnb-0.1.15/wnb.egg-info/top_level.txt
```

### Comparing `wnb-0.1.14/PKG-INFO` & `wnb-0.1.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.14
+Version: 0.1.15
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -14,26 +14,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.14-green)
+![](https://img.shields.io/badge/version-v0.1.15-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 ![](https://img.shields.io/pypi/dm/wnb)
 
 
 <p>
-<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
 Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
 This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
```

### Comparing `wnb-0.1.14/README.md` & `wnb-0.1.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.14-green)
+![](https://img.shields.io/badge/version-v0.1.15-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 ![](https://img.shields.io/pypi/dm/wnb)
 
 
 <p>
-<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
 Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
 This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
```

### Comparing `wnb-0.1.14/tests/test_gnb.py` & `wnb-0.1.15/tests/test_gnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.14/tests/test_gwnb.py` & `wnb-0.1.15/tests/test_gwnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.14/wnb/_base.py` & `wnb-0.1.15/wnb/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from abc import ABCMeta
-import inspect
 from functools import wraps
+import inspect
 from numbers import Number
 from typing import List, Tuple, Union
 import warnings
 
 import numpy as np
 
 from ._enums import Distribution
 
-__all__ = [
-    'ContinuousDistMixin',
-    'DiscreteDistMixin'
-]
+__all__ = ["ContinuousDistMixin", "DiscreteDistMixin"]
 
 
 def vectorize(otypes=None, excluded=None, signature=None):
     """
     Numpy vectorization wrapper that works with class methods.
     """
 
     def decorator(func):
-        vectorized = np.vectorize(func, otypes=otypes, excluded=excluded, signature=signature)
+        vectorized = np.vectorize(
+            func, otypes=otypes, excluded=excluded, signature=signature
+        )
 
         @wraps(func)
         def wrapper(*args):
             return vectorized(*args)
 
         return wrapper
 
@@ -37,16 +36,19 @@
     Mixin class for probability distributions in wnb.
     """
 
     name: Union[str, Distribution] = None
     _support: Union[List[float], Tuple[float, float]] = None
 
     @classmethod
-    def from_data(cls, data):
-        """Creates an instance of the class from given data. Distribution parameters will be estimated from the data.
+    def from_data(cls, data, **kwargs):
+        """Creates an instance of the class from given data. Distribution parameters will be estimated from data.
+
+        Args:
+            data: Input data from which distribution parameters will be estimated.
 
         Returns:
             self: An instance of the class.
         """
         pass
 
     @classmethod
@@ -89,36 +91,47 @@
             out[key] = value
         return out
 
     @property
     def support(self) -> Union[List[float], Tuple[float, float]]:
         """Returns the support of the probability distribution.
 
-        If support is a list, it represents a limited number of discrete values. If it is a tuple, it indicates a limited or unlimited range of continuous values.
+        If support is a list, it represents a limited number of discrete values.
+        If it is a tuple, it indicates a limited or unlimited range of continuous values.
 
         """
         return self._support
 
     def _check_support(self, x):
-        if (isinstance(self.support, list) and x not in self.support) or \
-           (isinstance(self.support, tuple) and (x < self.support[0] or x > self.support[1])):
-            warnings.warn("Value doesn't lie within the support of the distribution", RuntimeWarning)
+        if (isinstance(self.support, list) and x not in self.support) or (
+            isinstance(self.support, tuple)
+            and (x < self.support[0] or x > self.support[1])
+        ):
+            warnings.warn(
+                "Value doesn't lie within the support of the distribution",
+                RuntimeWarning,
+            )
         else:
             pass
 
     def __repr__(self) -> str:
-        return "".join([
-            "<",
-            self.__class__.__name__,
-            "(",
-            ", ".join(
-                [f"{k}={v:.4f}" if isinstance(v, Number) else f"{k}={v}" for k, v in self.get_params().items()]
-            ),
-            ")>"
-        ])
+        return "".join(
+            [
+                "<",
+                self.__class__.__name__,
+                "(",
+                ", ".join(
+                    [
+                        f"{k}={v:.4f}" if isinstance(v, Number) else f"{k}={v}"
+                        for k, v in self.get_params().items()
+                    ]
+                ),
+                ")>",
+            ]
+        )
 
 
 class ContinuousDistMixin(DistMixin, metaclass=ABCMeta):
     """
     Mixin class for all continuous probability distributions in wnb.
     """
```

### Comparing `wnb-0.1.14/wnb/dist.py` & `wnb-0.1.15/wnb/dist.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,75 +4,79 @@
 from scipy.special import gamma
 
 from ._base import ContinuousDistMixin, DiscreteDistMixin
 from ._enums import Distribution as D
 
 
 __all__ = [
-    'NormalDist',
-    'LognormalDist',
-    'ExponentialDist',
-    'UniformDist',
-    'ParetoDist',
-    'GammaDist',
-    'BernoulliDist',
-    'CategoricalDist',
+    "NormalDist",
+    "LognormalDist",
+    "ExponentialDist",
+    "UniformDist",
+    "ParetoDist",
+    "GammaDist",
+    "BernoulliDist",
+    "CategoricalDist",
     # 'MultinomialDist',
-    'GeometricDist',
-    'PoissonDist'
+    "GeometricDist",
+    "PoissonDist",
 ]
 
 
 class NormalDist(ContinuousDistMixin):
     name = D.NORMAL
     _support = (-np.inf, np.inf)
 
     def __init__(self, mu: float, sigma: float):
         self.mu = mu
         self.sigma = sigma
         super().__init__()
 
     @classmethod
-    def from_data(cls, data: np.ndarray):
+    def from_data(cls, data: np.ndarray, **kwargs):
         return cls(mu=np.average(data), sigma=np.std(data))
 
     def pdf(self, x: float) -> float:
-        return (1.0 / np.sqrt(2 * np.pi * self.sigma**2)) * np.exp(-0.5 * (((x - self.mu) / self.sigma)**2))
+        return (1.0 / np.sqrt(2 * np.pi * self.sigma ** 2)) * np.exp(
+            -0.5 * (((x - self.mu) / self.sigma) ** 2)
+        )
 
 
 class LognormalDist(ContinuousDistMixin):
     name = D.LOGNORMAL
     _support = (0, np.inf)
 
     def __init__(self, mu: float, sigma: float):
         self.mu = mu
         self.sigma = sigma
         super().__init__()
 
     @classmethod
-    def from_data(cls, data: np.ndarray):
+    def from_data(cls, data: np.ndarray, **kwargs):
         mu_hat = np.sum(np.log(data)) / len(data)
-        sigma_hat = np.sum((np.log(data) - mu_hat)**2) / len(data)
+        sigma_hat = np.sum((np.log(data) - mu_hat) ** 2) / len(data)
         return cls(mu=mu_hat, sigma=sigma_hat)
 
     def pdf(self, x: float) -> float:
-        return (1.0 / (x * np.sigma * np.sqrt(2 * np.pi))) * np.exp(-0.5 * ((np.log(x - self.mu) / self.sigma)**2))
+        return (1.0 / (x * np.sigma * np.sqrt(2 * np.pi))) * np.exp(
+            -0.5 * ((np.log(x - self.mu) / self.sigma) ** 2)
+        )
 
 
 class ExponentialDist(ContinuousDistMixin):
     name = D.EXPONENTIAL
     _support = (0, np.inf)
 
     def __init__(self, rate: float):
         self.rate = rate
         super().__init__()
 
     @classmethod
-    def from_data(cls, data: np.ndarray):
-        return cls(rate=(len(data)-2) / np.sum(data))
+    def from_data(cls, data: np.ndarray, **kwargs):
+        return cls(rate=(len(data) - 2) / np.sum(data))
 
     def pdf(self, x: float) -> float:
         return self.rate * np.exp(-self.rate * x) if x >= 0 else 0.0
 
 
 class UniformDist(ContinuousDistMixin):
     name = D.UNIFORM
@@ -80,15 +84,15 @@
     def __init__(self, a: float, b: float):
         self.a = a
         self.b = b
         self._support = (a, b)
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data, **kwargs):
         return cls(a=np.min(data), b=np.max(data))
 
     def pdf(self, x: float) -> float:
         return 1 / (self.b - self.a) if self.a <= x <= self.b else 0.0
 
 
 class ParetoDist(ContinuousDistMixin):
@@ -97,71 +101,84 @@
     def __init__(self, x_m: float, alpha: float):
         self.x_m = x_m
         self.alpha = alpha
         self._support = (self.x_m, np.inf)
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data, **kwargs):
         x_m = np.min(data)
         return cls(x_m=x_m, alpha=len(data) / np.sum(np.log(data / x_m)))
 
     def pdf(self, x: float) -> float:
-        return (self.alpha * self.x_m**self.alpha) / x**(self.alpha + 1) if x >= self.x_m else 0.0
+        return (
+            (self.alpha * self.x_m ** self.alpha) / x ** (self.alpha + 1)
+            if x >= self.x_m
+            else 0.0
+        )
 
 
 class GammaDist(ContinuousDistMixin):
     name = D.GAMMA
     _support = (0, np.inf)
 
     def __init__(self, k: float, theta: float):
         self.k = k
         self.theta = theta
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data, **kwargs):
         n = len(data)
         return cls(
-            k=n * np.sum(data) / (n * np.sum(data * np.log(data)) - np.sum(data * np.sum(np.log(data)))),
-            theta=(n * np.sum(data * np.log(data)) - np.sum(data * np.sum(np.log(data)))) / n**2
+            k=n
+            * np.sum(data)
+            / (n * np.sum(data * np.log(data)) - np.sum(data * np.sum(np.log(data)))),
+            theta=(
+                n * np.sum(data * np.log(data)) - np.sum(data * np.sum(np.log(data)))
+            )
+            / n ** 2,
         )
 
     def pdf(self, x: float) -> float:
-        return (x ** (self.k-1) * np.exp(-x / self.theta)) / (gamma(self.k) * self.theta ** self.k)
+        return (x ** (self.k - 1) * np.exp(-x / self.theta)) / (
+            gamma(self.k) * self.theta ** self.k
+        )
 
 
 class BernoulliDist(DiscreteDistMixin):
     name = D.BERNOULLI
     _support = [0, 1]
 
     def __init__(self, p: float):
         self.p = p
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
-        return cls(p=((np.array(data) == 1).sum() + 1e-10) / len(data))  # TODO: use alpha instead of 1e-10
+    def from_data(cls, data, **kwargs):
+        alpha = kwargs.get("alpha", 1e-10)
+        return cls(p=((np.array(data) == 1).sum() + alpha) / len(data))
 
     def pmf(self, x: int) -> float:
         return 0.0 if x not in self._support else self.p if x == 1 else 1 - self.p
 
 
 class CategoricalDist(DiscreteDistMixin):
     name = D.CATEGORICAL
 
     def __init__(self, prob: Mapping[Any, float]):
         self.prob = prob
         self._support = list(self.prob.keys())
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data, **kwargs):
+        alpha = kwargs.get("alpha", 1e-10)
         values, counts = np.unique(data, return_counts=True)
-        return cls(prob={v: (c + 1e-10)/len(data) for v, c in zip(values, counts)})  # TODO: use alpha instead of 1e-10
+        return cls(prob={v: (c + alpha) / len(data) for v, c in zip(values, counts)})
 
     def pmf(self, x: Any) -> float:
         return self.prob.get(x, 0.0)
 
 
 # class MultinomialDist(DiscreteDistMixin):
 #     name = D.MULTINOMIAL
@@ -169,15 +186,15 @@
 #     def __init__(self, n: int, prob: Mapping[int, float]):
 #         self.n = n
 #         self.prob = prob
 #         self._support = [i for i in range(self.n+1)]
 #         super().__init__()
 #
 #     @classmethod
-#     def from_data(cls, data: Sequence[int]):
+#     def from_data(cls, data: Sequence[int], **kwargs):
 #         values, counts = np.unique(data, return_counts=True)
 #         return cls(n=int(np.sum(values)), prob={v: c / len(data) for v, c in zip(values, counts)})
 #
 #     def pmf(self, x: Sequence[int]) -> float:
 #         if sum(x) != self.n:
 #             return 0.0
 #         else:
@@ -190,37 +207,36 @@
     _support = (1, np.inf)
 
     def __init__(self, p: float):
         self.p = p
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data, **kwargs):
         return cls(p=len(data) / np.sum(data))
 
     def pmf(self, x: int) -> float:
-        return self.p * (1 - self.p)**(x-1) if x >= 1 else 0.0
+        return self.p * (1 - self.p) ** (x - 1) if x >= 1 else 0.0
 
 
 class PoissonDist(DiscreteDistMixin):
     name = D.POISSON
     _support = (0, np.inf)
 
     def __init__(self, rate: float):
         self.rate = rate
         super().__init__()
 
     @classmethod
-    def from_data(cls, data):
-        return cls(rate=np.sum(data)/len(data))
+    def from_data(cls, data, **kwargs):
+        return cls(rate=np.sum(data) / len(data))
 
     def pmf(self, x: int) -> float:
-        return (np.exp(-self.rate) * self.rate**x) / np.math.factorial(x)
+        return (np.exp(-self.rate) * self.rate ** x) / np.math.factorial(x)
 
 
-AllDistributions = {
-    eval(cls).name: eval(cls)
-    for cls in __all__
-}
+AllDistributions = {eval(cls).name: eval(cls) for cls in __all__}
 
 
-NonNumericDistributions = [D.CATEGORICAL, ]
+NonNumericDistributions = [
+    D.CATEGORICAL,
+]
```

### Comparing `wnb-0.1.14/wnb/gnb.py` & `wnb-0.1.15/wnb/gnb.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,111 +17,133 @@
 
 
 class GeneralNB(ClassifierMixin, BaseEstimator, metaclass=ABCMeta):
     """
     A general Naive Bayes classifier that allows you to specify the likelihood distribution for each feature.
     """
 
-    def __init__(self, *,
-                 priors: Optional[Union[Sequence[float], np.ndarray]] = None,
-                 distributions: Optional[Sequence[Union[
-                     str, Distribution, Type[ContinuousDistMixin], Type[DiscreteDistMixin]]]
-                 ] = None) -> None:
-        """Initializes an object of the class.
+    def __init__(
+        self,
+        *,
+        priors: Optional[Union[Sequence[float], np.ndarray]] = None,
+        distributions: Optional[
+            Sequence[
+                Union[
+                    str,
+                    Distribution,
+                    Type[ContinuousDistMixin],
+                    Type[DiscreteDistMixin],
+                ]
+            ]
+        ] = None,
+        alpha: float = 1e-10,
+    ) -> None:
+        """Initializes an instance of the GeneralNB class.
 
         Args:
             priors (Optional[Union[list, np.ndarray]]): Prior probabilities. Defaults to None.
-            distributions: Names of the distributions to be used for features' likelihoods. A sequence with same length
+            distributions: Probability distributions to be used for features' likelihoods. A sequence with same length
                            of the number of features. If not specified, all likelihood will be considered Gaussian.
                            Defaults to None.
+            alpha (float): Additive (Laplace/Lidstone) smoothing parameter (set alpha=0 for no smoothing). Defaults to 1e-10.
 
         """
         self.priors = priors
         self.distributions = distributions
+        self.alpha = alpha
 
     def _more_tags(self):
-        return {
-            'multilabel': True,
-            'requires_y': True
-        }
+        return {"multilabel": True, "requires_y": True}
 
     def _get_distributions(self):
         try:
             if self.distributions_ is not None:
                 return self.distributions_
         except:
-            return self.distributions if self.distributions is not None else []
+            return self.distributions or []
 
     def _check_inputs(self, X, y):
         # Check if only one class is present in label vector
         if self.n_classes_ == 1:
             raise ValueError("Classifier can't train when only one class is present")
 
         X = check_array(
             array=X,
             accept_sparse=False,
             accept_large_sparse=False,
-            dtype=None if any(d in self._get_distributions() for d in NonNumericDistributions) else 'numeric',
+            dtype=None
+            if any(d in self._get_distributions() for d in NonNumericDistributions)
+            else "numeric",
             force_all_finite=True,
             ensure_2d=True,
             ensure_min_samples=1,
             ensure_min_features=1,
-            estimator=self
+            estimator=self,
         )
 
         # Check if X contains complex values
         if np.iscomplex(X).any() or np.iscomplex(y).any():
             raise ValueError("Complex data not supported")
 
         # Check that the number of samples and labels are compatible
         if self.__n_samples != y.shape[0]:
             raise ValueError(
-                "X.shape[0]=%d and y.shape[0]=%d are incompatible." % (X.shape[0], y.shape[0])
+                "X.shape[0]=%d and y.shape[0]=%d are incompatible."
+                % (X.shape[0], y.shape[0])
             )
 
     def _prepare_X_y(self, X=None, y=None):
         if X is not None:
             # Convert to NumPy array if X is Pandas DataFrame
             if isinstance(X, pd.DataFrame):
                 X = X.values
-            X = X if any(d in self._get_distributions() for d in NonNumericDistributions) else as_float_array(X)
+            X = (
+                X
+                if any(d in self._get_distributions() for d in NonNumericDistributions)
+                else as_float_array(X)
+            )
 
         if y is not None:
             # Convert to a NumPy array
             if isinstance(y, pd.DataFrame) or isinstance(y, pd.Series):
                 y = y.values
             else:
                 y = np.array(y)
 
             # Warning in case of y being 2d
             if y.ndim > 1:
-                warnings.warn("A column-vector y was passed when a 1d array was expected.", DataConversionWarning)
+                warnings.warn(
+                    "A column-vector y was passed when a 1d array was expected.",
+                    DataConversionWarning,
+                )
 
             y = y.flatten()
 
         output = tuple(item for item in [X, y] if item is not None)
         output = output[0] if len(output) == 1 else output
         return output
 
     def _prepare_parameters(self, X, y):
         # Set priors if not specified
         if self.priors is None:
             _, class_count_ = np.unique(y, return_counts=True)
-            self.class_prior_ = class_count_ / class_count_.sum()  # Calculate empirical prior probabilities
+            self.class_prior_ = (
+                class_count_ / class_count_.sum()
+            )  # Calculate empirical prior probabilities
 
         else:
             # Check that the provided priors match the number of classes
             if len(self.priors) != self.n_classes_:
-                raise ValueError('Number of priors must match the number of classes.')
+                raise ValueError("Number of priors must match the number of classes.")
             # Check that the sum of priors is 1
             if not np.isclose(self.priors.sum(), 1.0):
-                raise ValueError('The sum of the priors should be 1.')
+                raise ValueError("The sum of the priors should be 1.")
             # Check that the priors are non-negative
             if (self.priors < 0).any():
-                raise ValueError('Priors must be non-negative.')
+                raise ValueError("Priors must be non-negative.")
 
             self.class_prior_ = self.priors
 
         # Convert to NumPy array if input priors is in a list
         if type(self.class_prior_) is list:
             self.class_prior_ = np.array(self.class_prior_)
 
@@ -136,52 +158,63 @@
                     "Number of specified distributions must match the number of features."
                     f"({len(self.distributions)} != {self.n_features_in_})"
                 )
 
             # Check that all specified distributions are supported
             for dist in self.distributions:
                 if not (
-                        isinstance(dist, Distribution) or
-                        dist in Distribution.__members__.values() or
-                        (hasattr(dist, 'from_data') and hasattr(dist, '__call__'))
+                    isinstance(dist, Distribution)
+                    or dist in Distribution.__members__.values()
+                    or (hasattr(dist, "from_data") and hasattr(dist, "__call__"))
                 ):
-                    raise ValueError(f"Distribution '{dist}' is not supported")
+                    raise ValueError(f"Distribution '{dist}' is not supported.")
 
             self.distributions_ = self.distributions
 
-    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: Union[np.ndarray, pd.DataFrame, pd.Series]):
-        """Fits general Naive Bayes classifier according to X and y.
+    def fit(
+        self,
+        X: Union[np.ndarray, pd.DataFrame],
+        y: Union[np.ndarray, pd.DataFrame, pd.Series],
+    ):
+        """Fits general Naive Bayes classifier to X and y.
 
         Args:
             X (Union[np.ndarray, pd.DataFrame]): Array-like of shape (n_samples, n_features).
                                                  Training vectors, where `n_samples` is the number of samples
                                                  and `n_features` is the number of features.
             y (Union[np.ndarray, pd.DataFrame, pd.Series]): Array-like of shape (n_samples,). Target values.
 
         Returns:
             self: The instance itself.
         """
-        self.classes_, y_ = np.unique(y, return_inverse=True)  # Unique class labels and their indices
+        self.classes_, y_ = np.unique(
+            y, return_inverse=True
+        )  # Unique class labels and their indices
         self.n_classes_ = len(self.classes_)  # Number of classes
 
         X, y = self._prepare_X_y(X, y)
 
-        self.__n_samples, self.n_features_in_ = X.shape  # Number of samples and features
+        (
+            self.__n_samples,
+            self.n_features_in_,
+        ) = X.shape  # Number of samples and features
 
         self._check_inputs(X, y)
 
         y = y_
         self._prepare_parameters(X, y)
 
         self.likelihood_params_ = {
             c: [
-                AllDistributions[self.distributions_[i]].from_data(X[y == c, i])
-                if isinstance(self.distributions_[i], Distribution) or
-                   self.distributions_[i] in Distribution.__members__.values() else
-                self.distributions_[i].from_data(X[y == c, i])
+                AllDistributions[self.distributions_[i]].from_data(
+                    X[y == c, i], alpha=self.alpha
+                )
+                if isinstance(self.distributions_[i], Distribution)
+                or self.distributions_[i] in Distribution.__members__.values()
+                else self.distributions_[i].from_data(X[y == c, i], alpha=self.alpha)
                 for i in range(self.n_features_in_)
             ]
             for c in range(self.n_classes_)
         }
 
         return self
 
@@ -217,40 +250,45 @@
         check_is_fitted(self)
 
         # Input validation
         X = check_array(
             array=X,
             accept_large_sparse=False,
             force_all_finite=True,
-            dtype=None if any(d in self._get_distributions() for d in NonNumericDistributions) else 'numeric',
-            estimator=self
+            dtype=None
+            if any(d in self._get_distributions() for d in NonNumericDistributions)
+            else "numeric",
+            estimator=self,
         )
 
         # Check if the number of input features matches the data seen during fit
         if not X.shape[1] == self.n_features_in_:
             raise ValueError(
-                "Expected input with %d features, got %d instead." % (self.n_features_in_, X.shape[1])
+                "Expected input with %d features, got %d instead."
+                % (self.n_features_in_, X.shape[1])
             )
 
         n_samples = X.shape[0]
 
         X = self._prepare_X_y(X=X)
 
         log_joint = np.zeros((n_samples, self.n_classes_))
         for c in range(self.n_classes_):
             log_joint[:, c] = np.log(self.class_prior_[c]) + np.sum(
-                (
+                [
                     np.log(likelihood(X[:, i]))
                     for i, likelihood in enumerate(self.likelihood_params_[c])
-                ),
-                axis=0
+                ],
+                axis=0,
             )
 
         log_proba = log_joint - np.transpose(
-            np.repeat(logsumexp(log_joint, axis=1).reshape(1, -1), self.n_classes_, axis=0)
+            np.repeat(
+                logsumexp(log_joint, axis=1).reshape(1, -1), self.n_classes_, axis=0
+            )
         )
         return log_proba
 
     def predict_proba(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
         """Returns probability estimates for the test vector X.
 
         Args:
```

### Comparing `wnb-0.1.14/wnb/gwnb.py` & `wnb-0.1.15/wnb/gwnb.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,121 +16,123 @@
 
 
 class GaussianWNB(ClassifierMixin, BaseEstimator, metaclass=ABCMeta):
     """
     Binary Gaussian Minimum Log-likelihood Difference Weighted Naive Bayes (MLD-WNB) Classifier
     """
 
-    def __init__(self, *,
-                 priors: Optional[Union[Sequence[float], np.ndarray]] = None,
-                 error_weights: Optional[np.ndarray] = None,
-                 max_iter: int = 25,
-                 step_size: float = 1e-4,
-                 penalty: str = 'l2',
-                 C: float = 1.0,
-                 learning_hist: bool = False) -> None:
-        """Initializes an object of the class.
+    def __init__(
+        self,
+        *,
+        priors: Optional[Union[Sequence[float], np.ndarray]] = None,
+        error_weights: Optional[np.ndarray] = None,
+        max_iter: int = 25,
+        step_size: float = 1e-4,
+        penalty: str = "l2",
+        C: float = 1.0,
+        learning_hist: bool = False
+    ) -> None:
+        """Initializes an instance of the GaussianWNB class.
 
         Args:
             priors (Optional[Union[Sequence[float], np.ndarray]]): Prior probabilities. Defaults to None.
             error_weights (Optional[np.ndarray]): Matrix of error weights (n_classes * n_classes). Defaults to None.
             max_iter (int): Maximum number of gradient descent iterations. Defaults to 25.
             step_size (float): Step size of weight update (i.e., learning rate). Defaults to 1e-4.
             penalty (str): Regularization term; must be either 'l1' or 'l2'. Defaults to 'l2'.
             C (float): Regularization strength; must be a positive float. Defaults to 1.0.
             learning_hist (bool): Whether to record the learning history, i.e., the value of cost function in each
                                   learning iteration.
 
         """
-        self.priors = priors  # Prior probabilities of classes (n_classes x 1)
-        self.error_weights = error_weights  # Matrix of error weights (n_features x n_features)
-        self.max_iter = max_iter  # Maximum number of iterations of the learning algorithm
-        self.step_size = step_size  # Learning rate
-        self.penalty = penalty  # Regularization type ('l1' or 'l2')
-        self.C = C  # Regularization parameter
+        self.priors = priors
+        self.error_weights = error_weights
+        self.max_iter = max_iter
+        self.step_size = step_size
+        self.penalty = penalty
+        self.C = C
         self.learning_hist = learning_hist
 
     def _more_tags(self):
-        return {
-            'binary_only': True,
-            'requires_y': True
-        }
+        return {"binary_only": True, "requires_y": True}
 
     def _check_inputs(self, X, y):
         # Check that the dataset has only two unique labels
-        if type_of_target(y) != 'binary':
-            warnings.warn('This version of MLD-WNB only supports binary classification.')
-            raise ValueError('Unknown label type: non-binary')
+        if type_of_target(y) != "binary":
+            warnings.warn(
+                "This version of MLD-WNB only supports binary classification."
+            )
+            raise ValueError("Unknown label type: non-binary")
 
         # Check if only one class is present in label vector
         if self.n_classes_ == 1:
-            raise ValueError("Classifier can't train when only one class is present")
+            raise ValueError("Classifier can't train when only one class is present.")
 
         X = check_array(
             array=X,
             accept_sparse=False,
             accept_large_sparse=False,
-            dtype='numeric',
+            dtype="numeric",
             force_all_finite=True,
             ensure_2d=True,
             ensure_min_samples=1,
             ensure_min_features=1,
-            estimator=self
+            estimator=self,
         )
 
         # Check if X contains complex values
         if np.iscomplex(X).any() or np.iscomplex(y).any():
             raise ValueError("Complex data not supported")
 
         # Check that the number of samples and labels are compatible
         if self.__n_samples != y.shape[0]:
             raise ValueError(
-                "X.shape[0]=%d and y.shape[0]=%d are incompatible." % (X.shape[0], y.shape[0])
+                "X.shape[0]=%d and y.shape[0]=%d are incompatible."
+                % (X.shape[0], y.shape[0])
             )
 
         if self.priors is not None:
             # Check that the provided priors match the number of classes
             if len(self.priors) != self.n_classes_:
-                raise ValueError('Number of priors must match the number of classes.')
+                raise ValueError("Number of priors must match the number of classes.")
             # Check that the sum of priors is 1
             if not np.isclose(self.priors.sum(), 1.0):
-                raise ValueError('The sum of the priors should be 1.')
+                raise ValueError("The sum of the priors should be 1.")
             # Check that the priors are non-negative
             if (self.priors < 0).any():
-                raise ValueError('Priors must be non-negative.')
+                raise ValueError("Priors must be non-negative.")
 
         if self.error_weights is not None:
             # Check that the size of error weights matrix matches number of classes
             if self.error_weights.shape != (self.n_classes_, self.n_classes_):
                 raise ValueError(
-                    'The shape of error weights matrix does not match the number of classes, '
-                    'must be (n_classes, n_classes).'
+                    "The shape of error weights matrix does not match the number of classes, "
+                    "must be (n_classes, n_classes)."
                 )
 
         # Check that the regularization type is either 'l1' or 'l2'
-        if self.penalty not in ['l1', 'l2']:
+        if self.penalty not in ["l1", "l2"]:
             raise ValueError("Regularization type must be either 'l1' or 'l2'.")
 
         # Check that the regularization parameter is a positive integer
         if not isinstance(self.C, numbers.Number) or self.C < 0:
             raise ValueError(
-                "Regularization parameter must be positive; got (C=%r)"
-                % self.C
+                "Regularization parameter must be positive; got (C=%r)" % self.C
             )
 
         # Check that the maximum number of iterations is a positive integer
         if not isinstance(self.max_iter, numbers.Number) or self.max_iter < 0:
             raise ValueError(
-                "Maximum number of iteration must be a positive integer; got (max_iter=%r)"
+                "Maximum number of iteration must be a positive integer; got (max_iter=%r)."
                 % self.max_iter
             )
 
     def _prepare_X_y(self, X=None, y=None, from_fit=False):
         if from_fit and y is None:
-            raise ValueError("requires y to be passed, but the target y is None")
+            raise ValueError("requires y to be passed, but the target y is None.")
 
         if X is not None:
             # Convert to NumPy array if X is Pandas DataFrame
             if isinstance(X, pd.DataFrame):
                 X = X.values
             X = as_float_array(X)
 
@@ -139,89 +141,117 @@
             if isinstance(y, pd.DataFrame) or isinstance(y, pd.Series):
                 y = y.values
             else:
                 y = np.array(y)
 
             # Warning in case of y being 2d
             if y.ndim > 1:
-                warnings.warn("A column-vector y was passed when a 1d array was expected.", DataConversionWarning)
+                warnings.warn(
+                    "A column-vector y was passed when a 1d array was expected.",
+                    DataConversionWarning,
+                )
 
             y = y.flatten()
 
         output = tuple(item for item in [X, y] if item is not None)
         output = output[0] if len(output) == 1 else output
         return output
 
     def _prepare_parameters(self, X, y):
         # Calculate mean and standard deviation of features for each class
         for c in range(self.n_classes_):
-            self.mu_[:, c] = np.mean(X[y == c, :], axis=0)  # Calculate mean of features for class c
-            self.std_[:, c] = np.std(X[y == c, :], axis=0)  # Calculate std of features for class c
+            self.mu_[:, c] = np.mean(
+                X[y == c, :], axis=0
+            )  # Calculate mean of features for class c
+            self.std_[:, c] = np.std(
+                X[y == c, :], axis=0
+            )  # Calculate std of features for class c
 
         # Update if no priors is provided
         if self.priors is None:
             _, class_count_ = np.unique(y, return_counts=True)
-            self.class_prior_ = class_count_ / class_count_.sum()  # Calculate empirical prior probabilities
+            self.class_prior_ = (
+                class_count_ / class_count_.sum()
+            )  # Calculate empirical prior probabilities
         else:
             self.class_prior_ = self.priors
 
         # Convert to NumPy array if input priors is in a list
         if type(self.class_prior_) is list:
             self.class_prior_ = np.array(self.class_prior_)
 
         # Update if no error weights is provided
         if self.error_weights is None:
             self.error_weights_ = np.array([[0, 1], [-1, 0]])
         else:
             self.error_weights_ = self.error_weights
 
-    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: Union[np.ndarray, pd.DataFrame, pd.Series]):
-        """Fits Gaussian Binary MLD-WNB according to X and y.
+    def fit(
+        self,
+        X: Union[np.ndarray, pd.DataFrame],
+        y: Union[np.ndarray, pd.DataFrame, pd.Series],
+    ):
+        """Fits Gaussian Binary MLD-WNB to X and y.
 
         Args:
             X (Union[np.ndarray, pd.DataFrame]): Array-like of shape (n_samples, n_features).
                                                  Training vectors, where `n_samples` is the number of samples
                                                  and `n_features` is the number of features.
             y (Union[np.ndarray, pd.DataFrame, pd.Series]): Array-like of shape (n_samples,). Target values.
 
         Returns:
             self: The instance itself.
         """
         X, y = self._prepare_X_y(X, y, from_fit=True)
 
-        self.classes_, y_ = np.unique(y, return_inverse=True)  # Unique class labels and their indices
+        self.classes_, y_ = np.unique(
+            y, return_inverse=True
+        )  # Unique class labels and their indices
         self.n_classes_ = len(self.classes_)  # Number of classes
-        self.__n_samples, self.n_features_in_ = X.shape  # Number of samples and features
+        (
+            self.__n_samples,
+            self.n_features_in_,
+        ) = X.shape  # Number of samples and features
 
         self._check_inputs(X, y)
         y = y_
 
-        self.mu_ = np.zeros((self.n_features_in_, self.n_classes_))  # Mean of features (n_features x 1)
-        self.std_ = np.zeros((self.n_features_in_, self.n_classes_))  # Standard deviation of features (n_features x 1)
-        self.coef_ = np.ones((self.n_features_in_,))  # WNB coefficients (n_features x 1)
-        self.cost_hist_ = np.array([np.nan for _ in range(self.max_iter)])  # To store cost value in each iteration
+        self.mu_ = np.zeros(
+            (self.n_features_in_, self.n_classes_)
+        )  # Mean of features (n_features x 1)
+        self.std_ = np.zeros(
+            (self.n_features_in_, self.n_classes_)
+        )  # Standard deviation of features (n_features x 1)
+        self.coef_ = np.ones(
+            (self.n_features_in_,)
+        )  # WNB coefficients (n_features x 1)
+        self.cost_hist_ = np.array(
+            [np.nan for _ in range(self.max_iter)]
+        )  # To store cost value in each iteration
 
         self._prepare_parameters(X, y)
 
         # Learn the weights using gradient descent
         self.n_iter_ = 0
         for self.n_iter_ in range(self.max_iter):
             # Predict on X
             y_hat = self.__predict(X)
 
             # Calculate cost
-            self.cost_hist_[self.n_iter_], _lambda = self._calculate_cost(X, y, y_hat, self.learning_hist)
+            self.cost_hist_[self.n_iter_], _lambda = self._calculate_cost(
+                X, y, y_hat, self.learning_hist
+            )
 
             # Calculate gradients (most time-consuming)
             _grad = self._calculate_grad(X, _lambda)
 
             # Add regularization
-            if self.penalty == 'l1':
+            if self.penalty == "l1":
                 _grad += self.C * np.sign(self.coef_)
-            elif self.penalty == 'l2':
+            elif self.penalty == "l2":
                 _grad += 2 * self.C * self.coef_
 
             # Update weights
             self.coef_ = self.coef_ - self.step_size * _grad
 
         self.cost_hist_ = None if not self.learning_hist else self.cost_hist_
 
@@ -233,43 +263,65 @@
         if learning_hist:
             # Calculate cost
             _cost = 0
             for i in range(self.__n_samples):
                 _sum = np.log(self.class_prior_[1] / self.class_prior_[0])
                 x = X[i, :]
                 for j in range(self.n_features_in_):
-                    _sum += self.coef_[j] * (np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 1], self.std_[j, 1]))
-                                             - np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 0], self.std_[j, 0])))
+                    _sum += self.coef_[j] * (
+                        np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 1], self.std_[j, 1]))
+                        - np.log(
+                            1e-20 + norm.pdf(x[j], self.mu_[j, 0], self.std_[j, 0])
+                        )
+                    )
                 _cost += _lambda[i] * _sum
         else:
             _cost = np.nan
 
         return _cost, _lambda
 
     def _calculate_grad(self, X, _lambda):
-        _grad = np.repeat(np.log(self.std_[:, 0] / self.std_[:, 1]).reshape(1, -1), self.__n_samples, axis=0)
-        _grad += 0.5 * ((X - np.repeat(self.mu_[:, 0].reshape(1, -1), self.__n_samples, axis=0)) /
-                        (np.repeat(self.std_[:, 0].reshape(1, -1), self.__n_samples, axis=0))) ** 2
-        _grad -= 0.5 * ((X - np.repeat(self.mu_[:, 1].reshape(1, -1), self.__n_samples, axis=0)) /
-                        (np.repeat(self.std_[:, 1].reshape(1, -1), self.__n_samples, axis=0))) ** 2
-        _grad *= np.transpose(np.repeat(np.array(_lambda).reshape(1, -1), self.n_features_in_, axis=0))
+        _grad = np.repeat(
+            np.log(self.std_[:, 0] / self.std_[:, 1]).reshape(1, -1),
+            self.__n_samples,
+            axis=0,
+        )
+        _grad += (
+            0.5
+            * (
+                (X - np.repeat(self.mu_[:, 0].reshape(1, -1), self.__n_samples, axis=0))
+                / (np.repeat(self.std_[:, 0].reshape(1, -1), self.__n_samples, axis=0))
+            )
+            ** 2
+        )
+        _grad -= (
+            0.5
+            * (
+                (X - np.repeat(self.mu_[:, 1].reshape(1, -1), self.__n_samples, axis=0))
+                / (np.repeat(self.std_[:, 1].reshape(1, -1), self.__n_samples, axis=0))
+            )
+            ** 2
+        )
+        _grad *= np.transpose(
+            np.repeat(np.array(_lambda).reshape(1, -1), self.n_features_in_, axis=0)
+        )
         _grad = np.sum(_grad, axis=0)
 
         return _grad
 
     @deprecated()
     def _calculate_grad_slow(self, X, _lambda):
         _grad = np.zeros((self.n_features_in_,))
         for i in range(self.__n_samples):
             x = X[i, :]
             _log_p = np.array(
                 [
-                    np.log(self.std_[j, 0] / self.std_[j, 1]) +
-                    0.5*((x[j] - self.mu_[j, 0]) / self.std_[j, 0])**2 -
-                    0.5*((x[j] - self.mu_[j, 1]) / self.std_[j, 1])**2
+                    np.log(self.std_[j, 0] / self.std_[j, 1])
+                    + 0.5 * ((x[j] - self.mu_[j, 0]) / self.std_[j, 0]) ** 2
+                    - 0.5 * ((x[j] - self.mu_[j, 1]) / self.std_[j, 1]) ** 2
                     for j in range(self.n_features_in_)
                 ]
             )
             _grad += _lambda[i] * _log_p
         return _grad
 
     def __predict(self, X):
@@ -300,36 +352,46 @@
                         The log-probability of the samples for each class in the model.
                         The columns correspond to the classes in sorted order, as they appear in the attribute `classes_`.
         """
         # Check is fit had been called
         check_is_fitted(self)
 
         # Input validation
-        X = check_array(array=X, accept_large_sparse=False, force_all_finite=True, estimator=self)
+        X = check_array(
+            array=X, accept_large_sparse=False, force_all_finite=True, estimator=self
+        )
 
         # Check if the number of input features matches the data seen during fit
         if not X.shape[1] == self.n_features_in_:
             raise ValueError(
-                "Expected input with %d features, got %d instead." % (self.n_features_in_, X.shape[1])
+                "Expected input with %d features, got %d instead."
+                % (self.n_features_in_, X.shape[1])
             )
 
         n_samples = X.shape[0]
 
         X = self._prepare_X_y(X=X)
 
         log_priors = np.tile(np.log(self.class_prior_), (n_samples, 1))
         w_reshaped = np.tile(self.coef_.reshape(-1, 1), (1, self.n_classes_))
         term1 = np.sum(np.multiply(w_reshaped, -np.log(np.sqrt(2 * np.pi) * self.std_)))
-        var_inv = np.multiply(w_reshaped, 1.0/np.multiply(self.std_, self.std_))
+        var_inv = np.multiply(w_reshaped, 1.0 / np.multiply(self.std_, self.std_))
         mu_by_var = np.multiply(self.mu_, var_inv)
-        term2 = -0.5*(np.matmul(np.multiply(X, X), var_inv) - 2.0*np.matmul(X, mu_by_var)
-                      + np.sum(self.mu_.conj()*mu_by_var, axis=0))
+        term2 = -0.5 * (
+            np.matmul(np.multiply(X, X), var_inv)
+            - 2.0 * np.matmul(X, mu_by_var)
+            + np.sum(self.mu_.conj() * mu_by_var, axis=0)
+        )
         log_proba = log_priors + term1 + term2
 
-        log_proba -= np.transpose(np.repeat(logsumexp(log_proba, axis=1).reshape(1, -1), self.n_classes_, axis=0))
+        log_proba -= np.transpose(
+            np.repeat(
+                logsumexp(log_proba, axis=1).reshape(1, -1), self.n_classes_, axis=0
+            )
+        )
         return log_proba
 
     def predict_proba(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
         """Returns probability estimates for the test vector X.
 
         Args:
             X (Union[np.ndarray, pd.DataFrame]): Array-like of shape (n_samples, n_features). The input samples.
```

### Comparing `wnb-0.1.14/wnb.egg-info/PKG-INFO` & `wnb-0.1.15/wnb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.14
+Version: 0.1.15
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -14,26 +14,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.14-green)
+![](https://img.shields.io/badge/version-v0.1.15-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 ![](https://img.shields.io/pypi/dm/wnb)
 
 
 <p>
-<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
 <br>
 </p>
 
 ## Introduction
 Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
 This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
```

