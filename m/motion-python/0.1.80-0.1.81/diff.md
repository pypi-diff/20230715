# Comparing `tmp/motion_python-0.1.80.tar.gz` & `tmp/motion_python-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.80.tar", max compression
+gzip compressed data, was "motion_python-0.1.81.tar", max compression
```

## Comparing `motion_python-0.1.80.tar` & `motion_python-0.1.81.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-11 22:32:47.862080 motion_python-0.1.80/README.md
--rw-r--r--   0        0        0      344 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/cli.py
--rw-r--r--   0        0        0    23989 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/dicts.py
--rw-r--r--   0        0        0    17368 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/execute.py
--rw-r--r--   0        0        0    13507 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/instance.py
--rw-r--r--   0        0        0     4882 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/route.py
--rw-r--r--   0        0        0     4953 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/server/update_task.py
--rw-r--r--   0        0        0     8661 2023-07-11 22:32:47.866080 motion_python-0.1.80/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-11 22:33:13.239630 motion_python-0.1.80/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.80/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-14 23:09:36.657246 motion_python-0.1.81/README.md
+-rw-r--r--   0        0        0      344 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/cli.py
+-rw-r--r--   0        0        0    24251 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/dicts.py
+-rw-r--r--   0        0        0    17368 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/execute.py
+-rw-r--r--   0        0        0    13681 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/instance.py
+-rw-r--r--   0        0        0     4882 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/route.py
+-rw-r--r--   0        0        0     4953 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/server/update_task.py
+-rw-r--r--   0        0        0     8661 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-14 23:10:02.405441 motion_python-0.1.81/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.81/PKG-INFO
```

### Comparing `motion_python-0.1.80/README.md` & `motion_python-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/cli.py` & `motion_python-0.1.81/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/component.py` & `motion_python-0.1.81/motion/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,14 +495,22 @@
 
         # Creates instance of MyComponent
         if __name__ == "__main__":
             c_instance = MyComponent(init_state_params={"starting_val": 3})
             c_instance.run(..)
         ```
 
+        You can also use component instances as context managers:
+        ```python
+        ...
+        if __name__ == "__main__":
+            with MyComponent(init_state_params={"starting_val": 3}) as c_instance:
+                c_instance.run(..)
+        ```
+
         Args:
             instance_id (str, optional):
                 id of the component instance. Defaults to "" which will
                 generate a random id.
             init_state_params (Dict[str, Any], optional):
                 Parameters to pass into the init_state function. Defaults to {}.
             logging_level (str, optional):
```

### Comparing `motion_python-0.1.80/motion/dicts.py` & `motion_python-0.1.81/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/execute.py` & `motion_python-0.1.81/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/instance.py` & `motion_python-0.1.81/motion/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,20 @@
             load_state_func=load_state_func,
             serve_routes=serve_routes,
             update_routes=update_routes,
             disabled=self.disabled,
         )
         self.running = True
 
+    def __enter__(self) -> "ComponentInstance":
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:  # type: ignore
+        self.shutdown()
+
     @property
     def instance_name(self) -> str:
         """Component name with a random phrase to represent
         the name of this instance.
         In the form of componentname__randomphrase.
         """
         return self._instance_name
```

### Comparing `motion_python-0.1.80/motion/migrate.py` & `motion_python-0.1.81/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.81/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/route.py` & `motion_python-0.1.81/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/server/update_task.py` & `motion_python-0.1.81/motion/server/update_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/motion/utils.py` & `motion_python-0.1.81/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.80/pyproject.toml` & `motion_python-0.1.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.80"
+version = "0.1.81"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.80/PKG-INFO` & `motion_python-0.1.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.80
+Version: 0.1.81
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

