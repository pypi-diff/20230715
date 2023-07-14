# Comparing `tmp/pytheus-0.1.0.tar.gz` & `tmp/pytheus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.1.0.tar", last modified: Fri Jun 16 22:09:15 2023, max compression
+gzip compressed data, was "pytheus-0.2.0.tar", last modified: Fri Jul 14 22:11:19 2023, max compression
```

## Comparing `pytheus-0.1.0.tar` & `pytheus-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.494112 pytheus-0.1.0/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.1.0/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)    13832 2023-06-16 22:09:15.493921 pytheus-0.1.0/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)    13187 2023-06-11 21:57:42.000000 pytheus-0.1.0/README.md
--rw-r--r--   0 llandy     (501) staff       (20)     1325 2023-06-16 22:08:06.000000 pytheus-0.1.0/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.490759 pytheus-0.1.0/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.1.0/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.492094 pytheus-0.1.0/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.1.0/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4254 2023-06-10 22:34:13.000000 pytheus-0.1.0/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     6255 2023-06-03 01:35:21.000000 pytheus-0.1.0/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.1.0/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     3282 2023-06-03 01:35:21.000000 pytheus-0.1.0/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    22725 2023-06-16 22:06:24.000000 pytheus-0.1.0/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     4391 2023-06-16 22:06:24.000000 pytheus-0.1.0/pytheus/middleware.py
--rw-r--r--   0 llandy     (501) staff       (20)     3076 2023-06-03 01:35:21.000000 pytheus-0.1.0/pytheus/registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      568 2023-05-14 22:26:37.000000 pytheus-0.1.0/pytheus/utils.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.491515 pytheus-0.1.0/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)    13832 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      507 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)      217 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2023-06-16 22:09:15.000000 pytheus-0.1.0/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2023-06-16 22:09:15.494146 pytheus-0.1.0/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.1.0/setup.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-06-16 22:09:15.493529 pytheus-0.1.0/tests/
--rw-r--r--   0 llandy     (501) staff       (20)     7264 2023-06-02 00:02:13.000000 pytheus-0.1.0/tests/test_exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    29297 2023-06-11 21:57:42.000000 pytheus-0.1.0/tests/test_metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.1.0/tests/test_registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      349 2023-04-13 22:40:07.000000 pytheus-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-07-14 22:11:19.065726 pytheus-0.2.0/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.2.0/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    14169 2023-07-14 22:11:19.065566 pytheus-0.2.0/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    13524 2023-07-14 21:50:01.000000 pytheus-0.2.0/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1325 2023-07-14 21:50:23.000000 pytheus-0.2.0/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-07-14 22:11:19.062730 pytheus-0.2.0/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.2.0/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-07-14 22:11:19.064131 pytheus-0.2.0/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.2.0/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4254 2023-06-10 22:34:13.000000 pytheus-0.2.0/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     6255 2023-06-03 01:35:21.000000 pytheus-0.2.0/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.2.0/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3282 2023-06-03 01:35:21.000000 pytheus-0.2.0/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    23030 2023-07-14 21:50:01.000000 pytheus-0.2.0/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4391 2023-06-16 22:06:24.000000 pytheus-0.2.0/pytheus/middleware.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3076 2023-06-03 01:35:21.000000 pytheus-0.2.0/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      568 2023-05-14 22:26:37.000000 pytheus-0.2.0/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-07-14 22:11:19.063576 pytheus-0.2.0/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    14169 2023-07-14 22:11:19.000000 pytheus-0.2.0/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      507 2023-07-14 22:11:19.000000 pytheus-0.2.0/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-07-14 22:11:19.000000 pytheus-0.2.0/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      217 2023-07-14 22:11:19.000000 pytheus-0.2.0/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-07-14 22:11:19.000000 pytheus-0.2.0/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-07-14 22:11:19.065758 pytheus-0.2.0/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.2.0/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-07-14 22:11:19.065167 pytheus-0.2.0/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     7264 2023-07-14 20:34:10.000000 pytheus-0.2.0/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    30007 2023-07-14 21:50:01.000000 pytheus-0.2.0/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.2.0/tests/test_registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      349 2023-04-13 22:40:07.000000 pytheus-0.2.0/tests/test_utils.py
```

### Comparing `pytheus-0.1.0/LICENSE` & `pytheus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/PKG-INFO` & `pytheus-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.1.0
+Version: 0.2.0
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -38,14 +38,15 @@
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
 
 Some of the features are:
 
   - multiple multiprocess support:
     - redis backend ✅
+    - Rust powered backend 🧪
     - bring your own ✅
   - support for default labels value ✅
   - partial labels value (built in an incremental way) ✅
   - customizable registry support ✅
   - registry prefix support ✅
 
 ---
@@ -60,14 +61,16 @@
 - High flexibility with an high degree of `labels` control and customization.
 
 ---
 ## Requirements
 
 - Python 3.8+
 - redis >= 4.0.0 (**optional**: for multiprocessing)
+- pytheus-backend-rs (**optional**: for Rust powered multiprocessing 🦀)
+
 
 ---
 
 **Architecture**
 
 A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
 
@@ -82,14 +85,19 @@
 Optionally if you want to use the Redis backend (for multiprocess support) you will need the redis library:
 ```python
 pip install redis
 # or
 pip install pytheus[redis]
 ```
 
+If you want to try the Rust based backend (for multiprocess support):
+```python
+pip install pytheus-backend-rs
+```
+
 ---
 
 **Partial labels support:**
 
 ```python
 from pytheus.metrics import Counter
 
@@ -101,14 +109,17 @@
 my_metric = Counter('metric_name', 'desc', required_labels=['req1', 'req2'])
 
 my_metric.labels({'req1': '1', 'req2': '2'}).inc()  # you can pass all the labels at once
 partial_my_metric = my_metric.labels({'req1': '1'})  # a cacheable object with one of the required labels already set
 observable_my_metric = partial_my_metric.labels({'req2': '2'})  # finish setting the remaining values before observing
 observable_my_metric.inc()
 
+# alternatively to using a `dict` you can use `kwargs` (keyword arguments)
+my_metric.labels(req1='1', req2='2')
+
 ```
 
 ---
 
 **Default labels support:**
 
 ```python
```

### Comparing `pytheus-0.1.0/README.md` & `pytheus-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
 
 Some of the features are:
 
   - multiple multiprocess support:
     - redis backend ✅
+    - Rust powered backend 🧪
     - bring your own ✅
   - support for default labels value ✅
   - partial labels value (built in an incremental way) ✅
   - customizable registry support ✅
   - registry prefix support ✅
 
 ---
@@ -41,14 +42,16 @@
 - High flexibility with an high degree of `labels` control and customization.
 
 ---
 ## Requirements
 
 - Python 3.8+
 - redis >= 4.0.0 (**optional**: for multiprocessing)
+- pytheus-backend-rs (**optional**: for Rust powered multiprocessing 🦀)
+
 
 ---
 
 **Architecture**
 
 A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
 
@@ -63,14 +66,19 @@
 Optionally if you want to use the Redis backend (for multiprocess support) you will need the redis library:
 ```python
 pip install redis
 # or
 pip install pytheus[redis]
 ```
 
+If you want to try the Rust based backend (for multiprocess support):
+```python
+pip install pytheus-backend-rs
+```
+
 ---
 
 **Partial labels support:**
 
 ```python
 from pytheus.metrics import Counter
 
@@ -82,14 +90,17 @@
 my_metric = Counter('metric_name', 'desc', required_labels=['req1', 'req2'])
 
 my_metric.labels({'req1': '1', 'req2': '2'}).inc()  # you can pass all the labels at once
 partial_my_metric = my_metric.labels({'req1': '1'})  # a cacheable object with one of the required labels already set
 observable_my_metric = partial_my_metric.labels({'req2': '2'})  # finish setting the remaining values before observing
 observable_my_metric.inc()
 
+# alternatively to using a `dict` you can use `kwargs` (keyword arguments)
+my_metric.labels(req1='1', req2='2')
+
 ```
 
 ---
 
 **Default labels support:**
 
 ```python
```

### Comparing `pytheus-0.1.0/pyproject.toml` & `pytheus-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytheus"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Llandy Riveron Del Risco", email="llandy3d@gmail.com" },
 ]
 description = "playing with metrics"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytheus-0.1.0/pytheus/backends/base.py` & `pytheus-0.2.0/pytheus/backends/base.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/pytheus/backends/redis.py` & `pytheus-0.2.0/pytheus/backends/redis.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/pytheus/exposition.py` & `pytheus-0.2.0/pytheus/exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/pytheus/metrics.py` & `pytheus-0.2.0/pytheus/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,21 +198,27 @@
         return True
 
     def _raise_if_cannot_observe(self) -> None:
         """Raise if the metric cannot be observed, for example if labels values are missing."""
         if not self._can_observe:
             raise UnobservableMetricException
 
-    def labels(self, labels_: Labels) -> "_Metric":
+    def labels(self, pytheus_labels_: Optional[Labels] = None, **kwargs: str) -> "_Metric":
         """
         If no labels is passed to the call returns itself.
         If there are already present labels, they will be updated with the passed labels_ and if
         it's not observable will just return the new child instance. Otherwise it will also add
         the instance to the labeled_metrics on the collector.
         """
+        if pytheus_labels_ and kwargs:
+            raise LabelValidationException("Please use either a dict or kwargs, not both.")
+
+        # if we got labels as kwargs, we use that directly
+        labels_ = kwargs if pytheus_labels_ is None else pytheus_labels_
+
         if not labels_:
             return self
 
         self._collector._validate_labels(labels_)
 
         if self._labels:
             new_labels = self._labels.copy()
```

### Comparing `pytheus-0.1.0/pytheus/middleware.py` & `pytheus-0.2.0/pytheus/middleware.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/pytheus/registry.py` & `pytheus-0.2.0/pytheus/registry.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/pytheus/utils.py` & `pytheus-0.2.0/pytheus/utils.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/pytheus.egg-info/PKG-INFO` & `pytheus-0.2.0/pytheus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.1.0
+Version: 0.2.0
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -38,14 +38,15 @@
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
 
 Some of the features are:
 
   - multiple multiprocess support:
     - redis backend ✅
+    - Rust powered backend 🧪
     - bring your own ✅
   - support for default labels value ✅
   - partial labels value (built in an incremental way) ✅
   - customizable registry support ✅
   - registry prefix support ✅
 
 ---
@@ -60,14 +61,16 @@
 - High flexibility with an high degree of `labels` control and customization.
 
 ---
 ## Requirements
 
 - Python 3.8+
 - redis >= 4.0.0 (**optional**: for multiprocessing)
+- pytheus-backend-rs (**optional**: for Rust powered multiprocessing 🦀)
+
 
 ---
 
 **Architecture**
 
 A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
 
@@ -82,14 +85,19 @@
 Optionally if you want to use the Redis backend (for multiprocess support) you will need the redis library:
 ```python
 pip install redis
 # or
 pip install pytheus[redis]
 ```
 
+If you want to try the Rust based backend (for multiprocess support):
+```python
+pip install pytheus-backend-rs
+```
+
 ---
 
 **Partial labels support:**
 
 ```python
 from pytheus.metrics import Counter
 
@@ -101,14 +109,17 @@
 my_metric = Counter('metric_name', 'desc', required_labels=['req1', 'req2'])
 
 my_metric.labels({'req1': '1', 'req2': '2'}).inc()  # you can pass all the labels at once
 partial_my_metric = my_metric.labels({'req1': '1'})  # a cacheable object with one of the required labels already set
 observable_my_metric = partial_my_metric.labels({'req2': '2'})  # finish setting the remaining values before observing
 observable_my_metric.inc()
 
+# alternatively to using a `dict` you can use `kwargs` (keyword arguments)
+my_metric.labels(req1='1', req2='2')
+
 ```
 
 ---
 
 **Default labels support:**
 
 ```python
```

### Comparing `pytheus-0.1.0/tests/test_exposition.py` & `pytheus-0.2.0/tests/test_exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.1.0/tests/test_metrics.py` & `pytheus-0.2.0/tests/test_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,26 +95,26 @@
         samples = counter._collector.collect()
         samples = list(samples)
         assert len(samples) == 1
         assert "a" in samples[0].labels
         assert 1 == samples[0].labels["a"]
 
     def test_collect_with_labels_and_default_labels(self):
-        default_labels = {"a": 3}
+        default_labels = {"a": "3"}
         counter = Counter("name", "desc", required_labels=["a", "b"], default_labels=default_labels)
         counter_a = counter.labels({"a": "1", "b": "2"})  # noqa: F841
         counter_b = counter.labels({"a": "7", "b": "8"})  # noqa: F841
         counter_c = counter.labels({"a": "6"})  # this should not be creating a sample  # noqa: F841
         counter_d = counter.labels({"b": "5"})  # noqa: F841
         samples = counter._collector.collect()
         samples = list(samples)
         assert len(samples) == 3
         assert samples[0].labels["a"] == "1"
         assert samples[1].labels["a"] == "7"
-        assert samples[2].labels["a"] == 3
+        assert samples[2].labels["a"] == "3"
 
     def test_collector_created_on_metric_creation(self):
         counter = Counter("name", "desc", required_labels=["a", "b"])
         assert counter._collector.name == "name"
         assert counter._collector.description == "desc"
         assert counter._collector._required_labels == {"a", "b"}
 
@@ -141,101 +141,122 @@
         required_labels = ["bob", "cat"]
         metric = _Metric("name", "desc", required_labels=required_labels)
         assert metric._collector._required_labels == set(required_labels)
 
     def test_create_metric_raises_with_labels(self):
         # only default labels are allowed to be set on creation
         with pytest.raises(LabelValidationException):
-            _Metric("name", "desc", required_labels=["a"], labels={"a": 1})
+            _Metric("name", "desc", required_labels=["a"], labels={"a": "1"})
 
     def test_check_can_observe_without_required_labels(self):
         metric = _Metric("name", "desc")
         assert metric._check_can_observe() is True
 
     def test_check_can_observe_with_required_labels_without_labels(self):
         metric = _Metric("name", "desc", required_labels=["bob", "cat"])
         assert metric._check_can_observe() is False
 
     def test_check_can_observe_with_required_labels_with_partial_labels(self):
         metric = _Metric("name", "desc", required_labels=["bob", "cat"])
-        metric = metric.labels({"bob": 2})
+        metric = metric.labels({"bob": "2"})
         assert metric._check_can_observe() is False
 
     def test_check_can_observe_with_required_labels_with_labels(self):
         metric = _Metric("name", "desc", required_labels=["bob", "cat"])
-        metric = metric.labels({"bob": 1, "cat": 2})
+        metric = metric.labels({"bob": "1", "cat": "2"})
         assert metric._check_can_observe() is True
 
     def test_raises_if_cannot_be_observed_observable(self):
         metric = _Metric("name", "desc", required_labels=["bob", "cat"])
-        metric = metric.labels({"bob": 1, "cat": 2})
+        metric = metric.labels({"bob": "1", "cat": "2"})
         metric._raise_if_cannot_observe()
 
     def test_raises_if_cannot_be_observed_unobservable(self):
         metric = _Metric("name", "desc", required_labels=["bob", "cat"])
-        metric = metric.labels({"bob": 1})
+        metric = metric.labels({"bob": "1"})
         with pytest.raises(UnobservableMetricException):
             metric._raise_if_cannot_observe()
 
     def test_check_can_observe_with_default_labels(self):
         metric = _Metric(
             "name",
             "desc",
             required_labels=["bob", "cat"],
-            default_labels={"bob": 1, "cat": 2},
+            default_labels={"bob": "1", "cat": "2"},
         )
         assert metric._check_can_observe() is True
 
     def test_check_can_observe_with_default_labels_partial_uncomplete(self):
-        metric = _Metric("name", "desc", required_labels=["bob", "cat"], default_labels={"bob": 1})
+        metric = _Metric(
+            "name", "desc", required_labels=["bob", "cat"], default_labels={"bob": "1"}
+        )
         assert metric._check_can_observe() is False
 
     def test_check_can_observe_with_default_labels_partial_complete(self):
-        metric = _Metric("name", "desc", required_labels=["bob", "cat"], default_labels={"bob": 1})
-        metric = metric.labels({"cat": 2})
+        metric = _Metric(
+            "name", "desc", required_labels=["bob", "cat"], default_labels={"bob": "1"}
+        )
+        metric = metric.labels({"cat": "2"})
         assert metric._check_can_observe() is True
 
     def test_check_can_observe_with_default_labels_partial_overriden_label(self):
-        metric = _Metric("name", "desc", required_labels=["bob", "cat"], default_labels={"bob": 1})
-        metric = metric.labels({"cat": 2, "bob": 2})
+        metric = _Metric(
+            "name", "desc", required_labels=["bob", "cat"], default_labels={"bob": "1"}
+        )
+        metric = metric.labels({"cat": "2", "bob": "2"})
         assert metric._check_can_observe() is True
 
     # labels
 
+    def test_labels_with_dict(self):
+        metric = _Metric("name", "desc", required_labels=["a"])
+        new = metric.labels({"a": "1"})
+        assert new._labels == {"a": "1"}
+
+    def test_labels_with_kwargs(self):
+        metric = _Metric("name", "desc", required_labels=["a"])
+        new = metric.labels(a="1")
+        assert new._labels == {"a": "1"}
+
+    def test_labels_with_dict_and_kwargs_raises(self):
+        metric = _Metric("name", "desc", required_labels=["a"])
+        with pytest.raises(LabelValidationException):
+            metric.labels({"a": "1"}, a="1")
+
     def test_labels_without_labels_return_itself(self):
         metric = _Metric("name", "desc")
         new = metric.labels({})
         assert new is metric
 
     def test_labels_without_required_labels_raises(self):
         metric = _Metric("name", "desc")
         with pytest.raises(LabelValidationException):
-            metric.labels({"a": 1})
+            metric.labels({"a": "1"})
 
     def test_labels_unobservable(self):
         metric = _Metric("name", "desc", required_labels=["a", "b"])
-        metric = metric.labels({"a": 1})
+        metric = metric.labels({"a": "1"})
         assert metric not in metric._collector._labeled_metrics.values()
 
     def test_labels_observable(self):
         metric = _Metric("name", "desc", required_labels=["a", "b"])
-        metric = metric.labels({"a": 1, "b": 2})
+        metric = metric.labels({"a": "1", "b": "2"})
         assert metric in metric._collector._labeled_metrics.values()
 
     def test_labels_observable_returns_existing_child(self):
         metric = _Metric("name", "desc", required_labels=["a", "b"])
-        metric_a = metric.labels({"a": 1, "b": 2})
-        metric_b = metric.labels({"a": 1, "b": 2})
+        metric_a = metric.labels({"a": "1", "b": "2"})
+        metric_b = metric.labels({"a": "1", "b": "2"})
         assert len(metric._collector._labeled_metrics) == 1
         assert metric_a is metric_b
 
     def test_labels_with_unknown_label(self):
         metric = _Metric("name", "desc", required_labels=["a", "b"])
         with pytest.raises(LabelValidationException):
-            metric.labels({"a": 1, "c": 2})
+            metric.labels({"a": "1", "c": "2"})
 
     # default_labels
 
     def test_metric_with_default_labels(self):
         default_labels = {"bob": "bobvalue"}
         metric = _Metric("name", "desc", required_labels=["bob"], default_labels=default_labels)
         assert metric._collector._default_labels == default_labels
@@ -271,31 +292,31 @@
         default_labels = {"bob": "bobvalue"}
         metric = _Metric(
             "name",
             "desc",
             required_labels=["bob", "cat"],
             default_labels=default_labels,
         )
-        metric = metric.labels({"cat": 2})
+        metric = metric.labels({"cat": "2"})
         sample = metric._get_sample()
 
-        assert sample.labels == {"bob": "bobvalue", "cat": 2}
+        assert sample.labels == {"bob": "bobvalue", "cat": "2"}
 
     def test_add_default_labels_to_sample_does_not_ovveride_provided_labels(self):
         default_labels = {"bob": "bobvalue"}
         metric = _Metric(
             "name",
             "desc",
             required_labels=["bob", "cat"],
             default_labels=default_labels,
         )
-        metric = metric.labels({"cat": 2, "bob": "newvalue"})
+        metric = metric.labels({"cat": "2", "bob": "newvalue"})
         sample = metric._get_sample()
 
-        assert sample.labels == {"bob": "newvalue", "cat": 2}
+        assert sample.labels == {"bob": "newvalue", "cat": "2"}
 
 
 class TestCounter:
     @pytest.fixture
     def counter(self):
         return Counter("name", "desc")
```

### Comparing `pytheus-0.1.0/tests/test_registry.py` & `pytheus-0.2.0/tests/test_registry.py`

 * *Files identical despite different names*

