# Comparing `tmp/pysigma_backend_carbonblack-0.1.3.tar.gz` & `tmp/pysigma_backend_carbonblack-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_carbonblack-0.1.3.tar", max compression
+gzip compressed data, was "pysigma_backend_carbonblack-0.1.4.tar", max compression
```

## Comparing `pysigma_backend_carbonblack-0.1.3.tar` & `pysigma_backend_carbonblack-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/LICENSE
--rw-r--r--   0        0        0      575 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      371 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/backends/carbonblack/__init__.py
--rw-r--r--   0        0        0     6915 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/backends/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      315 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/pipelines/carbonblack/__init__.py
--rw-r--r--   0        0        0    13828 2023-07-11 18:59:31.492613 pysigma_backend_carbonblack-0.1.3/sigma/pipelines/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-15 19:45:01.275062 pysigma_backend_carbonblack-0.1.4/LICENSE
+-rw-r--r--   0        0        0      575 2023-07-15 19:45:01.275062 pysigma_backend_carbonblack-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-07-15 19:45:01.275062 pysigma_backend_carbonblack-0.1.4/sigma/backends/carbonblack/__init__.py
+-rw-r--r--   0        0        0     7937 2023-07-15 19:45:01.275062 pysigma_backend_carbonblack-0.1.4/sigma/backends/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      315 2023-07-15 19:45:01.275062 pysigma_backend_carbonblack-0.1.4/sigma/pipelines/carbonblack/__init__.py
+-rw-r--r--   0        0        0    13828 2023-07-15 19:45:01.275062 pysigma_backend_carbonblack-0.1.4/sigma/pipelines/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.4/PKG-INFO
```

### Comparing `pysigma_backend_carbonblack-0.1.3/LICENSE` & `pysigma_backend_carbonblack-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.3/pyproject.toml` & `pysigma_backend_carbonblack-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-carbonblack"
-version = "0.1.3"
+version = "0.1.4"
 description = "pySigma carbonblack backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-carbonblack"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_carbonblack-0.1.3/sigma/backends/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.4/sigma/backends/carbonblack/carbonblack.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,14 +93,36 @@
             value = f'[{cond.value.number} TO *]'
 
         return self.compare_op_expression.format(
             field=self.escape_and_quote_field(cond.field),
             value = value
         )
 
+    def convert_condition_not(self, cond: ConditionNOT, state: ConversionState) -> Union[str, DeferredQueryExpression]:
+        """
+        Conversion of NOT conditions.
+        CarbonBlack is unique in that the NOT operator cannot have a space
+        """
+        arg = cond.args[0]
+        try:
+            if arg.__class__ in self.precedence:  # group if AND or OR condition is negated
+                return (
+                    self.not_token + self.convert_condition_group(arg, state)
+                )
+            else:
+                expr = self.convert_condition(arg, state)
+                if isinstance(
+                    expr, DeferredQueryExpression
+                ):  # negate deferred expression and pass it to parent
+                    return expr.negate()
+                else:  # convert negated expression to string
+                    return self.not_token + expr
+        except TypeError:  # pragma: no cover
+            raise NotImplementedError("Operator 'not' not supported by the backend")
+
     def finalize_query_default(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Any:
         return query
 
     def finalize_output_default(self, queries: List[str]) -> Any:
         return queries
     
     def finalize_query_json(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> Any:
```

### Comparing `pysigma_backend_carbonblack-0.1.3/sigma/pipelines/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.4/sigma/pipelines/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.3/PKG-INFO` & `pysigma_backend_carbonblack-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-carbonblack
-Version: 0.1.3
+Version: 0.1.4
 Summary: pySigma carbonblack backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-carbonblack
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

