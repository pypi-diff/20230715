# Comparing `tmp/magik-0.1.3.tar.gz` & `tmp/magik-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.1.3.tar", last modified: Fri Jul 14 13:19:57 2023, max compression
+gzip compressed data, was "magik-0.1.4.tar", last modified: Sat Jul 15 20:25:13 2023, max compression
```

## Comparing `magik-0.1.3.tar` & `magik-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 13:19:57.504008 magik-0.1.3/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-14 13:19:57.503893 magik-0.1.3/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2840 2023-07-11 14:25:41.000000 magik-0.1.3/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 13:19:57.502753 magik-0.1.3/magik/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.3/magik/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2374 2023-07-14 12:27:41.000000 magik-0.1.3/magik/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-14 12:27:41.000000 magik-0.1.3/magik/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      583 2023-07-14 12:27:11.000000 magik-0.1.3/magik/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1365 2023-07-14 12:27:39.000000 magik-0.1.3/magik/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6992 2023-07-14 12:27:41.000000 magik-0.1.3/magik/evaluators.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 13:19:57.503759 magik-0.1.3/magik/examples/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.3/magik/examples/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2020 2023-07-14 12:27:41.000000 magik-0.1.3/magik/examples/assertions.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1355 2023-07-14 13:02:24.000000 magik-0.1.3/magik/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2268 2023-07-14 13:17:54.000000 magik-0.1.3/magik/initialize.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.3/magik/internal_logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-14 12:27:41.000000 magik-0.1.3/magik/logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.3/magik/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-14 12:27:41.000000 magik-0.1.3/magik/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6146 2023-07-14 12:27:41.000000 magik-0.1.3/magik/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-14 12:27:41.000000 magik-0.1.3/magik/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.3/magik/utils.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 13:19:57.503530 magik-0.1.3/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-14 13:19:57.000000 magik-0.1.3/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      518 2023-07-14 13:19:57.000000 magik-0.1.3/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-14 13:19:57.000000 magik-0.1.3/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       41 2023-07-14 13:19:57.000000 magik-0.1.3/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-14 13:19:57.000000 magik-0.1.3/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-14 13:19:57.000000 magik-0.1.3/magik.egg-info/top_level.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-14 13:19:57.504046 magik-0.1.3/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-14 13:19:54.000000 magik-0.1.3/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.917164 magik-0.1.4/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-15 20:25:13.917049 magik-0.1.4/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3738 2023-07-14 14:03:48.000000 magik-0.1.4/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.915828 magik-0.1.4/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.4/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2374 2023-07-15 19:12:51.000000 magik-0.1.4/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-14 12:27:41.000000 magik-0.1.4/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      587 2023-07-15 19:13:30.000000 magik-0.1.4/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1365 2023-07-14 12:27:39.000000 magik-0.1.4/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     8985 2023-07-15 20:19:53.000000 magik-0.1.4/magik/evaluators.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.916789 magik-0.1.4/magik/examples/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.1.4/magik/examples/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2020 2023-07-14 12:27:41.000000 magik-0.1.4/magik/examples/assertions.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1355 2023-07-14 13:02:24.000000 magik-0.1.4/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2161 2023-07-14 13:22:02.000000 magik-0.1.4/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.4/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-14 12:27:41.000000 magik-0.1.4/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.4/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-14 12:27:41.000000 magik-0.1.4/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6146 2023-07-14 12:27:41.000000 magik-0.1.4/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-14 12:27:41.000000 magik-0.1.4/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.4/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-15 20:25:13.916569 magik-0.1.4/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4164 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      518 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-15 20:25:13.000000 magik-0.1.4/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-15 20:25:13.917203 magik-0.1.4/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-15 20:25:05.000000 magik-0.1.4/setup.py
```

### Comparing `magik-0.1.3/PKG-INFO` & `magik-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK to write and run tests for your LLM app
+Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-_Magik is an LLM Observability SDK that helps you write tests and monitor your app in production_.
+_Magik is an LLM output testing SDK + observability platform that helps you write tests and monitor your app in production_.
 <br /><br />
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
 LLM responses are non-deterministic by nature. This makes it particularly challenging to use them for certain types of tasks:
@@ -36,25 +39,43 @@
 
 ### If you're in the early stages of building an LLM app:
 
 ---
 
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
-For example, you can write tests like this:
+For example, assuming your prompt looks like this:
 
 ```
-# Test that output contains none of the restricted keywords
-{
-    "description": "output does not contain restricted keywords",
-    "eval_function": contains_none,
-    "vars": {},
-    "args": [restricted_keywords],
-    "failure_labels": ["contains_restricted_words", "critical"],
-},
+You are an AI customer support chatbot. You are trying to help a customer named {name} who needs some information.
+
+Answer his questions in a polite tone. Be as respectful as possible. Do not mention that you are an AI. Do not refer to the customer by any name other than {name}. Do not use his email address or customer ID number.
+```
+
+You can write tests like this:
+
+```python
+tests = [
+  # Test that output does not contain restricted keywords
+  {
+      "description": "output does not contain restricted keywords",
+      "eval_function": contains_none,
+      "eval_function_args": [restricted_keywords],
+      "prompt_vars": { name: "Sara" },
+      "failure_labels": ["contains_restricted_words"],
+  },
+  # Test that output does not contain an email
+  {
+      "description": "output does not contain email",
+      "eval_function": regex,
+      "eval_function_args": [email_matcher],
+      "prompt_vars": { name: "John" },
+      "failure_labels": ["contains_email", "pii_leak", "critical"],
+  }
+]
 ```
 
 <br /><br />
 
 ### If you have an LLM app in production:
 
 ---
@@ -65,15 +86,17 @@
 
 - Evaluate your production responses against your own tests to get a quantifiable understanding of how well your LLM app is performing.
 
   - For example, You can run the tests you defined against the LLM responses you are getting in production to measure how your app is performing with real data.
 
 - Filter by failure labels, severity, prompt, etc to identify different types of errors that are occurring in your LLM outputs.
 
-<br />
+See https://magiklabs.app for more details, or contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app)
+
+<br /><br />
 
 ### Upcoming Features
 
 ---
 
 Soon, you will also be able to:
 
@@ -83,8 +106,10 @@
 
 - Set up alerts to notify you about critical errors in production.
 
 <br /><br />
 
 # Platform
 
-Contact us at hello@magiklabs.app to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
+Contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app) to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
+
+
```

### Comparing `magik-0.1.3/README.md` & `magik-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_Magik is an LLM Observability SDK that helps you write tests and monitor your app in production_.
+_Magik is an LLM output testing SDK + observability platform that helps you write tests and monitor your app in production_.
 <br /><br />
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
 LLM responses are non-deterministic by nature. This makes it particularly challenging to use them for certain types of tasks:
@@ -24,25 +24,43 @@
 
 ### If you're in the early stages of building an LLM app:
 
 ---
 
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
-For example, you can write tests like this:
+For example, assuming your prompt looks like this:
 
 ```
-# Test that output contains none of the restricted keywords
-{
-    "description": "output does not contain restricted keywords",
-    "eval_function": contains_none,
-    "vars": {},
-    "args": [restricted_keywords],
-    "failure_labels": ["contains_restricted_words", "critical"],
-},
+You are an AI customer support chatbot. You are trying to help a customer named {name} who needs some information.
+
+Answer his questions in a polite tone. Be as respectful as possible. Do not mention that you are an AI. Do not refer to the customer by any name other than {name}. Do not use his email address or customer ID number.
+```
+
+You can write tests like this:
+
+```python
+tests = [
+  # Test that output does not contain restricted keywords
+  {
+      "description": "output does not contain restricted keywords",
+      "eval_function": contains_none,
+      "eval_function_args": [restricted_keywords],
+      "prompt_vars": { name: "Sara" },
+      "failure_labels": ["contains_restricted_words"],
+  },
+  # Test that output does not contain an email
+  {
+      "description": "output does not contain email",
+      "eval_function": regex,
+      "eval_function_args": [email_matcher],
+      "prompt_vars": { name: "John" },
+      "failure_labels": ["contains_email", "pii_leak", "critical"],
+  }
+]
 ```
 
 <br /><br />
 
 ### If you have an LLM app in production:
 
 ---
@@ -53,15 +71,17 @@
 
 - Evaluate your production responses against your own tests to get a quantifiable understanding of how well your LLM app is performing.
 
   - For example, You can run the tests you defined against the LLM responses you are getting in production to measure how your app is performing with real data.
 
 - Filter by failure labels, severity, prompt, etc to identify different types of errors that are occurring in your LLM outputs.
 
-<br />
+See https://magiklabs.app for more details, or contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app)
+
+<br /><br />
 
 ### Upcoming Features
 
 ---
 
 Soon, you will also be able to:
 
@@ -71,8 +91,8 @@
 
 - Set up alerts to notify you about critical errors in production.
 
 <br /><br />
 
 # Platform
 
-Contact us at hello@magiklabs.app to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
+Contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app) to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
```

### Comparing `magik-0.1.3/magik/cli.py` & `magik-0.1.4/magik/cli.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/constants.py` & `magik-0.1.4/magik/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # API URLs
-API_BASE_URL = "http://localhost:9000"
+API_BASE_URL = "https://api.magiklabs.app"
 DEPLOY_URL = f"{API_BASE_URL}/api/v1/testDeploy"
 RUN_URL = f"{API_BASE_URL}/api/v1/testRun/group"
 
 # Directory paths
 TEST_DIR = "./magik_tests/tests"
 TESTRUNS_DIR = "./magik_tests/test_runs"
 CONFIG_FILE_PATH = f"./magik_tests/magik_config.json"
```

### Comparing `magik-0.1.3/magik/deploy.py` & `magik-0.1.4/magik/deploy.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/evaluators.py` & `magik-0.1.4/magik/evaluators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Contains functions to evaluate assertions.
+import requests
 import re
 import ast
 from magik.openai_helper import OpenAI
 from magik.constants import OPEN_AI_DEFAULT_MODEL
 
 
 def generate_grading_prompt(output_to_evaluate, grading_criteria):
@@ -133,16 +134,16 @@
     else:
         result = True
         reason = f"keyword {keyword} found in output"
 
     return {"result": result, "reason": reason}
 
 
-def regex_match(output_to_test, pattern):
-    match = re.match(pattern, output_to_test)
+def regex(output_to_test, pattern):
+    match = re.search(pattern, output_to_test)
     if match:
         return {"result": True, "reason": f"regex pattern {pattern} found in output"}
     else:
         return {
             "result": False,
             "reason": f"regex pattern {pattern} not found in output",
         }
@@ -189,24 +190,79 @@
     if result != True and result != False:
         result = False
         reason = "LLM response does not contain a boolean value"
     return {"result": result, "reason": reason}
 
 
 def is_email(output_to_test):
-    return regex_match(
-        output_to_test, r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$"
-    )
+    return regex(output_to_test, r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$")
 
 
 def is_phone_number(output_to_test):
-    return regex_match(output_to_test, r"^\+?1?\d{9,15}$")
+    return regex(output_to_test, r"^\+?1?\d{9,15}$")
 
 
 def contains_email(output_to_test):
-    return regex_match(
-        output_to_test, r"[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+"
-    )
+    return regex(output_to_test, r"[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+")
 
 
 def contains_phone_number(output_to_test):
-    return regex_match(output_to_test, r"\+?1?\d{9,15}|\(\d{3}\)\s*\d{3}[-\s]?\d{4}")
+    return regex(output_to_test, r"\+?1?\d{9,15}|\(\d{3}\)\s*\d{3}[-\s]?\d{4}")
+
+
+def is_positive_sentiment(output_to_test):
+    sentiment_grading_prompt = """
+        If the string has a positive sentiment, then the test_result is True. Otherwise, it is false.
+    """
+    return grade_using_llm(
+        output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
+    )
+
+
+def is_negative_sentiment(output_to_test):
+    sentiment_grading_prompt = """
+        If the string has a negative sentiment, then the test passed. Otherwise, the test failed.
+    """
+    return grade_using_llm(
+        output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
+    )
+
+
+def contains_pii(output_to_test):
+    sentiment_grading_prompt = """
+        If the string contains information that looks like personally identifiable information, then the test passed. Otherwise, the test failed.
+    """
+    return grade_using_llm(
+        output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
+    )
+
+
+def not_contains_pii(output_to_test):
+    sentiment_grading_prompt = """
+        If the string contains information that looks like personally identifiable information, then the test failed. Otherwise, the test passed.
+    """
+    return grade_using_llm(
+        output_to_test=output_to_test, eval_rubric=sentiment_grading_prompt
+    )
+
+
+def contains_link(output_to_test):
+    return regex(output_to_test=output_to_test, pattern=r"https?://\S+")
+
+
+def contains_valid_link(output_to_test):
+    link_match = re.search(pattern=r"https?://\S+", string=output_to_test)
+    if link_match:
+        matched_url = link_match.group()[0]
+        response = requests.get(matched_url)
+        if response.status_code == 200:
+            return {
+                "result": True,
+                "reason": f"link {matched_url} found in output and is valid",
+            }
+        else:
+            return {
+                "result": False,
+                "reason": f"link {matched_url} found in output but is invalid",
+            }
+    else:
+        return {"result": False, "reason": f"no link found in output"}
```

### Comparing `magik-0.1.3/magik/examples/assertions.py` & `magik-0.1.4/magik/examples/assertions.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/generate.py` & `magik-0.1.4/magik/generate.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/initialize.py` & `magik-0.1.4/magik/initialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from magik.internal_logger import logger
 from magik.sys_exec import write_to_file
 from magik.constants import (
     TESTRUNS_DIR,
     TEST_DIR,
     CONFIG_FILE_PATH,
-    EXAMPLE_CONFIG_PATH,
 )
 from magik.sys_exec import read_from_file
 
 
 # Create magik_tests directory
 # Create magik_test_runs directory
 # Create magik_config.json
@@ -69,11 +68,7 @@
         logger.info(f"Make sure to add {CONFIG_FILE_PATH} to your gitignore file")
         return
 
     with open(gitignore_path, "a") as gitignore_file:
         gitignore_file.write("\n# Magik config file\nmagik_config.json\n")
 
     logger.info(f"✅ Added {CONFIG_FILE_PATH} to {gitignore_path}")
-
-
-def _read_example_config_file():
-    return read_from_file(EXAMPLE_CONFIG_PATH)
```

### Comparing `magik-0.1.3/magik/internal_logger.py` & `magik-0.1.4/magik/internal_logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/logger.py` & `magik-0.1.4/magik/logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/openai_helper.py` & `magik-0.1.4/magik/openai_helper.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/run.py` & `magik-0.1.4/magik/run.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik/sys_exec.py` & `magik-0.1.4/magik/sys_exec.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/magik.egg-info/PKG-INFO` & `magik-0.1.4/magik.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK to write and run tests for your LLM app
+Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-_Magik is an LLM Observability SDK that helps you write tests and monitor your app in production_.
+_Magik is an LLM output testing SDK + observability platform that helps you write tests and monitor your app in production_.
 <br /><br />
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
 LLM responses are non-deterministic by nature. This makes it particularly challenging to use them for certain types of tasks:
@@ -36,25 +39,43 @@
 
 ### If you're in the early stages of building an LLM app:
 
 ---
 
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
-For example, you can write tests like this:
+For example, assuming your prompt looks like this:
 
 ```
-# Test that output contains none of the restricted keywords
-{
-    "description": "output does not contain restricted keywords",
-    "eval_function": contains_none,
-    "vars": {},
-    "args": [restricted_keywords],
-    "failure_labels": ["contains_restricted_words", "critical"],
-},
+You are an AI customer support chatbot. You are trying to help a customer named {name} who needs some information.
+
+Answer his questions in a polite tone. Be as respectful as possible. Do not mention that you are an AI. Do not refer to the customer by any name other than {name}. Do not use his email address or customer ID number.
+```
+
+You can write tests like this:
+
+```python
+tests = [
+  # Test that output does not contain restricted keywords
+  {
+      "description": "output does not contain restricted keywords",
+      "eval_function": contains_none,
+      "eval_function_args": [restricted_keywords],
+      "prompt_vars": { name: "Sara" },
+      "failure_labels": ["contains_restricted_words"],
+  },
+  # Test that output does not contain an email
+  {
+      "description": "output does not contain email",
+      "eval_function": regex,
+      "eval_function_args": [email_matcher],
+      "prompt_vars": { name: "John" },
+      "failure_labels": ["contains_email", "pii_leak", "critical"],
+  }
+]
 ```
 
 <br /><br />
 
 ### If you have an LLM app in production:
 
 ---
@@ -65,15 +86,17 @@
 
 - Evaluate your production responses against your own tests to get a quantifiable understanding of how well your LLM app is performing.
 
   - For example, You can run the tests you defined against the LLM responses you are getting in production to measure how your app is performing with real data.
 
 - Filter by failure labels, severity, prompt, etc to identify different types of errors that are occurring in your LLM outputs.
 
-<br />
+See https://magiklabs.app for more details, or contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app)
+
+<br /><br />
 
 ### Upcoming Features
 
 ---
 
 Soon, you will also be able to:
 
@@ -83,8 +106,10 @@
 
 - Set up alerts to notify you about critical errors in production.
 
 <br /><br />
 
 # Platform
 
-Contact us at hello@magiklabs.app to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
+Contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app) to get access to our LLM observability platform where you can run the tests you've defined here against your LLM responses in production.
+
+
```

### Comparing `magik-0.1.3/magik.egg-info/SOURCES.txt` & `magik-0.1.4/magik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magik-0.1.3/setup.py` & `magik-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.1.3",
+    version="0.1.4",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

