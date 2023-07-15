# Comparing `tmp/factool-0.0.7.tar.gz` & `tmp/factool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factool-0.0.7.tar", last modified: Sat Jul 15 07:27:32 2023, max compression
+gzip compressed data, was "factool-0.0.8.tar", last modified: Sat Jul 15 08:05:51 2023, max compression
```

## Comparing `factool-0.0.7.tar` & `factool-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-15 07:26:53.000000 factool-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-15 07:27:32.729171 factool-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-15 07:26:53.000000 factool-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.725171 factool-0.0.7/factool/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 07:26:53.000000 factool-0.0.7/factool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/code/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-15 07:26:53.000000 factool-0.0.7/factool/env_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-15 07:26:53.000000 factool-0.0.7/factool/factool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/knowledge_qa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/google_serper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-15 07:26:53.000000 factool-0.0.7/factool/math/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 07:26:53.000000 factool-0.0.7/factool/math/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/scientific/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/scientific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-15 07:26:53.000000 factool-0.0.7/factool/scientific/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-15 07:26:53.000000 factool-0.0.7/factool/scientific/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/__init_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/utils/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/claim_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/openai_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/utils/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/agreement_verification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/claim_extraction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/query_generation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/self_check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/utils_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.725171 factool-0.0.7/factool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-15 07:27:32.729171 factool-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-15 07:26:53.000000 factool-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-15 08:05:10.000000 factool-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-15 08:05:51.091860 factool-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-15 08:05:10.000000 factool-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 08:05:10.000000 factool-0.0.8/factool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/code/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/helper/_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/helper/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/helper/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/helper/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/code/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-15 08:05:10.000000 factool-0.0.8/factool/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-15 08:05:10.000000 factool-0.0.8/factool/factool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/knowledge_qa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/knowledge_qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-15 08:05:10.000000 factool-0.0.8/factool/knowledge_qa/google_serper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-15 08:05:10.000000 factool-0.0.8/factool/knowledge_qa/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 08:05:10.000000 factool-0.0.8/factool/knowledge_qa/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-15 08:05:10.000000 factool-0.0.8/factool/math/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 08:05:10.000000 factool-0.0.8/factool/math/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/scientific/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/scientific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-15 08:05:10.000000 factool-0.0.8/factool/scientific/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-15 08:05:10.000000 factool-0.0.8/factool/scientific/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/__init_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/utils/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/claim_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/openai_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool/utils/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/prompts/agreement_verification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/prompts/claim_extraction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/prompts/query_generation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/prompts/self_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 08:05:10.000000 factool-0.0.8/factool/utils/utils_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:05:51.091860 factool-0.0.8/factool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-15 08:05:51.000000 factool-0.0.8/factool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-15 08:05:51.000000 factool-0.0.8/factool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 08:05:51.000000 factool-0.0.8/factool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 08:05:51.000000 factool-0.0.8/factool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 08:05:51.000000 factool-0.0.8/factool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-15 08:05:51.095860 factool-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-15 08:05:10.000000 factool-0.0.8/setup.py
```

### Comparing `factool-0.0.7/factool/code/helper/_execution.py` & `factool-0.0.8/factool/code/helper/_execution.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,23 +29,56 @@
 
             # Disable functionalities that can make destructive changes to the test.
             reliability_guard()
 
             # Construct the check program and run it. VERY IMPORTANT!!!
             import_packages_end_index = prompt.find("def")
 
-            # some HumanEval prompts contain helper function that has to be included. Patching.
+            # some HumanEval prompts contain helper function that has
+            # to be included. Patching.
             helper_func = ""
-            helper_funcs_to_be_included = ["\n\ndef is_palindrome(string: str) -> bool:\n    \"\"\" Test if given string is a palindrome \"\"\"\n    return string == string[::-1]\n\n\n", "import math\n\n\ndef poly(xs: list, x: float):\n    \"\"\"\n    Evaluates polynomial with coefficients xs at point x.\n    return xs[0] + xs[1] * x + xs[1] * x^2 + .... xs[n] * x^n\n    \"\"\"\n    return sum([coeff * math.pow(x, i) for i, coeff in enumerate(xs)])\n\n\n", "\n\ndef encode_cyclic(s: str):\n    \"\"\"\n    returns encoded string by cycling groups of three characters.\n    \"\"\"\n    # split string to groups. Each of length 3.\n    groups = [s[(3 * i):min((3 * i + 3), len(s))] for i in range((len(s) + 2) // 3)]\n    # cycle elements in each group. Unless group has fewer elements than 3.\n    groups = [(group[1:] + group[0]) if len(group) == 3 else group for group in groups]\n    return \"\".join(groups)\n\n\n", "\n\ndef encode_shift(s: str):\n    \"\"\"\n    returns encoded string by shifting every character by 5 in the alphabet.\n    \"\"\"\n    return \"\".join([chr(((ord(ch) + 5 - ord(\"a\")) % 26) + ord(\"a\")) for ch in s])\n\n\n"]
+            helper_funcs_to_be_included = \
+                ["\n\ndef is_palindrome(string: str) -> bool:\n"
+                 "    \"\"\" Test if given string is a palindrome \"\"\"\n"
+                 "    return string == string[::-1]\n\n\n",
+                 "import math\n\n\ndef poly(xs: list, x: float):\n"
+                 "    \"\"\"\n    Evaluates polynomial with"
+                 " coefficients xs at point x.\n"
+                 "    return xs[0] + xs[1] * x + xs[1] * x^2 + .... xs[n] * x^n\n"
+                 "    \"\"\"\n    return sum([coeff * math.pow(x, i) for i,"
+                 " coeff in enumerate(xs)])\n\n\n", "\n\ndef encode_cyclic(s: str):\n"
+                                                    "    \"\"\"\n    returns encoded"
+                                                    " string by cycling groups of three"
+                                                    " characters.\n    \"\"\"\n"
+                                                    "    # split string to groups."
+                                                    " Each of length 3.\n"
+                                                    "    groups"
+                                                    " = [s[(3 * i):min((3 * i + 3),"
+                                                    " len(s))] for"
+                                                    " i in range((len(s) + 2) // 3)]\n"
+                                                    "    # cycle elements in each"
+                                                    " group. Unless group has fewer"
+                                                    " elements than 3.\n    "
+                                                    "groups = [(group[1:] + group[0])"
+                                                    " if len(group) == 3 "
+                                                    "else group for group in groups]\n"
+                                                    "    "
+                                                    "return \"\".join(groups)\n\n\n",
+                 "\n\ndef encode_shift(s: str):\n    \"\"\"\n"
+                 "    returns encoded string by shifting every"
+                 " character by 5 in the alphabet.\n    \"\"\"\n"
+                 "    return \"\".join([chr(((ord(ch)"
+                 " + 5 - ord(\"a\")) % 26) + ord(\"a\")) for ch in s])\n\n\n"]
             for helper in helper_funcs_to_be_included:
                 if helper in prompt:
                     helper_func = helper
 
             check_program = (
-                prompt[:import_packages_end_index] + helper_func + completion + "\n" + f'result = {test}'
+                prompt[:import_packages_end_index]
+                + helper_func + completion + "\n" + f'result = {test}'
             )
 
             try:
                 exec_globals = {}
                 with swallow_io():
                     with time_limit(timeout):
                         exec(check_program, exec_globals)
@@ -154,18 +187,21 @@
     generated code, should not be blindly executed outside of one. See the 
     Codex paper for more information about OpenAI's code sandbox, and proceed
     with caution.
     """
 
     if maximum_memory_bytes is not None:
         import resource
-        resource.setrlimit(resource.RLIMIT_AS, (maximum_memory_bytes, maximum_memory_bytes))
-        resource.setrlimit(resource.RLIMIT_DATA, (maximum_memory_bytes, maximum_memory_bytes))
+        resource.setrlimit(resource.RLIMIT_AS,
+                           (maximum_memory_bytes, maximum_memory_bytes))
+        resource.setrlimit(resource.RLIMIT_DATA,
+                           (maximum_memory_bytes, maximum_memory_bytes))
         if not platform.uname().system == 'Darwin':
-            resource.setrlimit(resource.RLIMIT_STACK, (maximum_memory_bytes, maximum_memory_bytes))
+            resource.setrlimit(resource.RLIMIT_STACK,
+                               (maximum_memory_bytes, maximum_memory_bytes))
 
     faulthandler.disable()
 
     import builtins
     builtins.exit = None
     builtins.quit = None
```

### Comparing `factool-0.0.7/factool/code/helper/execution.py` & `factool-0.0.8/factool/code/helper/execution.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     format="SystemLog: [%(asctime)s][%(name)s][%(levelname)s] - %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     level=logging.INFO,
 )
 
 logger = logging.getLogger(__name__)
 
-def evaluate_test_cases_multi_solution(prompt, testcases_input, multi_solutions, timeout=0.1):
+def evaluate_test_cases_multi_solution(prompt, testcases_input,
+                                       multi_solutions, timeout=0.1):
     logger.info(f'Start evaluation with test code, timeout={timeout}')
 
     with ProcessPoolExecutor() as executor:
         futures = []
         results = [[None for _ in multi_solutions] for _ in testcases_input]
 
         for i, testcase in enumerate(testcases_input):
@@ -31,15 +32,16 @@
                 future = executor.submit(test_case_against_solution, *args)
                 futures.append((i, j, future))
         logger.info(f'{len(futures)} execution requests are submitted')
         
         for completed_future in as_completed([f[2] for f in futures]):
             for i, j, future in futures:
                 if future == completed_future:
-                    logger.info('[{}/{}] execution completed'.format(i * len(multi_solutions) + j + 1, len(futures)))
+                    logger.info('[{}/{}] execution completed'.format(
+                        i * len(multi_solutions) + j + 1, len(futures)))
                     result = completed_future.result()
                     results[i][j] = result
                     break
 
     return results
```

### Comparing `factool-0.0.7/factool/code/helper/io_utils.py` & `factool-0.0.8/factool/code/helper/io_utils.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/code/helper/postprocess.py` & `factool-0.0.8/factool/code/helper/postprocess.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/code/pipeline.py` & `factool-0.0.8/factool/code/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,85 +27,118 @@
 
     async def _testcases_input_generation(self, batch, testcases_input_cnt):
         messages_list = []
         if self.company == 'openai':
             messages_list = [
                 [
                     {"role": "system", "content": self.query_generation_prompt['system']},
-                    {"role": "user", "content": self.query_generation_prompt['user_testcases_' + str(testcases_input_cnt)].format(input_question=sample['prompt'], entry_point=sample['entry_point'])},
+                    {"role": "user",
+                     "content":
+                         self.query_generation_prompt[
+                             'user_testcases_' + str(testcases_input_cnt)
+                             ].format(input_question=sample['prompt'],
+                                      entry_point=sample['entry_point'])
+                     },
                 ]
                 for sample in batch
             ]
         elif self.company == 'anthropic':
-            messages_list = [self.query_generation_prompt['user_testcases_' + str(testcases_input_cnt)].format(input_question=sample['prompt'], entry_point=sample['entry_point']) for sample in batch]
+            messages_list = [self.query_generation_prompt[
+                                 'user_testcases_' + str(testcases_input_cnt)
+                                 ].format(input_question=sample['prompt'],
+                                          entry_point=sample['entry_point'])
+                             for sample in batch]
         return await self.chat.async_run(messages_list, Dict)
     
     async def _multi_solution_generation(self, batch, multi_solution_cnt):
         bsize = 15
         messages_list = [
             [
                 {"role": "system", "content": self.query_generation_prompt['system']},
-                {"role": "user", "content": self.query_generation_prompt['user_solutions'].format(input_question=sample['prompt'], entry_point=sample['entry_point'])},
+                {"role": "user", "content": self.query_generation_prompt[
+                    'user_solutions'].format(input_question=sample['prompt'],
+                                             entry_point=sample['entry_point'])},
             ]
             for sample in batch
         ]
 
-        final_messages_list = [copy.deepcopy(messages) for messages in messages_list for _ in range(multi_solution_cnt)]
+        final_messages_list = [copy.deepcopy(messages)
+                               for messages in messages_list
+                               for _ in range(multi_solution_cnt)
+                               ]
 
         responses = []
         for i in range(0, len(final_messages_list), bsize):
             batch = final_messages_list[i:i + bsize]
             responses += await self.chat.async_run(batch, Dict)
         
         # Split the list into lists of length of multi_solution_cnt
-        responses_split = [responses[i:i + multi_solution_cnt] for i in range(0, len(responses),  multi_solution_cnt)]
+        responses_split = [responses[i:i + multi_solution_cnt]
+                           for i in range(0, len(responses),
+                                          multi_solution_cnt)]
 
         # Transform each element in each list
         multi_solutions = []
         for solutions in responses_split:
-            key_names = [f"python_solution_{i}" for i in range(1, multi_solution_cnt + 1)]
-            new_element = {key: solutions[i]['python_solution'] if solutions[i] != None else "None" for i, key in enumerate(key_names)}
+            key_names = [f"python_solution_{i}"
+                         for i in range(1, multi_solution_cnt + 1)]
+            new_element = {key: solutions[i]['python_solution']
+            if solutions[i] != None else "None" for i, key in enumerate(key_names)}
             multi_solutions.append(new_element)
 
         return multi_solutions
     
     async def run_with_tool_live(self, batch, batch_size):
         testcases_input = await self._testcases_input_generation(batch, self.testcases_input_cnt)
         multi_solutions = await self._multi_solution_generation(batch, self.multi_solution_cnt)
 
         if testcases_input == None or multi_solutions == None:
             return None
         
         responses = []
         for i in range(batch_size):
-            response = {'testcases_input': [], 'multi_solutions': [], 'with_tool_classification': "None"}
+            response = {'testcases_input': [],
+                        'multi_solutions': [], 'with_tool_classification': "None"}
             try:
                 response['testcases_input'] = list(testcases_input[i].values())
-                # Append the solution to be verified to the LAST element of multi_solutions
-                response['multi_solutions'] = [multi_solutions[i][f'python_solution_{j}'] for j in range(1, self.multi_solution_cnt + 1)] + [batch[i]['completion']]
+                # Append the solution to be verified to the LAST element
+                # of multi_solutions
+                response['multi_solutions']\
+                    = [multi_solutions[i][f'python_solution_{j}']
+                       for j in range(1, self.multi_solution_cnt + 1)] +\
+                      [batch[i]['completion']]
             except:
                 response['testcases_input'] = ["None"] * self.testcases_input_cnt
                 response['multi_solutions'] = ["None"] * (self.multi_solution_cnt + 1)
             
-            exec_result = evaluate_test_cases_multi_solution(batch[i]['prompt'], response['testcases_input'], response['multi_solutions'], timeout=0.1)
+            exec_result = evaluate_test_cases_multi_solution(
+                batch[i]['prompt'], response['testcases_input'],
+                response['multi_solutions'], timeout=0.1)
             response['exec_result'] = exec_result
             
             response['with_tool_classification'] = True
             # must pass all testcases to be classified as "True"
             for testcase_result in exec_result:
                 # syntax or timeout error happening on the potential solution
-                if isinstance(testcase_result[-1], str) and testcase_result[-1].startswith('FAILURE'):
+                if isinstance(testcase_result[-1], str) \
+                        and testcase_result[-1].startswith('FAILURE'):
                     response['with_tool_classification'] = False
-                # majority voting. Note that the last element is the solution to be verified. Also, multi solutions that return "FAILURE" are not counted and removed.
+                # majority voting. Note that the last element
+                # is the solution to be verified. Also, multi solutions that return "FAILURE" are not counted and removed.
                 else:
-                    failure_indices = [i for i, res in enumerate(testcase_result[:-1]) if isinstance(res, str) and res.startswith('FAILURE')]
-                    testcase_result = [res for i, res in enumerate(testcase_result) if i not in failure_indices]
+                    failure_indices = [
+                        i for i, res in enumerate(testcase_result[:-1])
+                        if isinstance(res, str) and res.startswith('FAILURE')]
+                    testcase_result = [
+                        res for i, res in enumerate(testcase_result)
+                        if i not in failure_indices]
 
                     try:
-                        if testcase_result[:-1].count(testcase_result[-1]) < math.ceil(len(testcase_result) / 2):
+                        if testcase_result[:-1].count(testcase_result[-1]) \
+                                < math.ceil(len(testcase_result) / 2):
                             response['with_tool_classification'] = False
                     # sometimes numpy array is included in testcase_result, so this error will be raised
                     except:
                         response['with_tool_classification'] = False
             
             responses.append(response)
 
@@ -130,15 +163,20 @@
                     claims.append("")
             else:
                 claims.append(response)
 
         batch_size = 5
         num_batches = math.ceil(len(prompts) / batch_size)
 
-        self.sample_list = [{"prompt": prompt, "response": response, "entry_point": entry_point, "completion": claim, "category": 'code'} for prompt, response, entry_point, claim in zip(prompts, responses, entry_points, claims)]
+        self.sample_list = [
+            {"prompt": prompt, "response": response,
+             "entry_point": entry_point, "completion": claim,
+             "category": 'code'}
+            for prompt, response, entry_point, claim
+            in zip(prompts, responses, entry_points, claims)]
 
         for i in range(num_batches):
             print(i)
             batch_start = i * batch_size
             batch_end = min((i + 1) * batch_size, len(responses))
 
             responses_returned = await self.run_with_tool_live(self.sample_list[batch_start: batch_end], batch_end - batch_start)
```

### Comparing `factool-0.0.7/factool/env_config.py` & `factool-0.0.8/factool/env_config.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/factool.py` & `factool-0.0.8/factool/factool.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/knowledge_qa/google_serper.py` & `factool-0.0.8/factool/knowledge_qa/google_serper.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/knowledge_qa/pipeline.py` & `factool-0.0.8/factool/knowledge_qa/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/math/pipeline.py` & `factool-0.0.8/factool/math/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/math/tool.py` & `factool-0.0.8/factool/math/tool.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/scientific/pipeline.py` & `factool-0.0.8/factool/scientific/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/scientific/tool.py` & `factool-0.0.8/factool/scientific/tool.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/base/pipeline.py` & `factool-0.0.8/factool/utils/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/claim_extractor.py` & `factool-0.0.8/factool/utils/claim_extractor.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/openai_wrapper.py` & `factool-0.0.8/factool/utils/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/prompts/agreement_verification.yaml` & `factool-0.0.8/factool/utils/prompts/agreement_verification.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/prompts/claim_extraction.yaml` & `factool-0.0.8/factool/utils/prompts/claim_extraction.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/prompts/query_generation.yaml` & `factool-0.0.8/factool/utils/prompts/query_generation.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool/utils/prompts/self_check.yaml` & `factool-0.0.8/factool/utils/prompts/self_check.yaml`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/factool.egg-info/SOURCES.txt` & `factool-0.0.8/factool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `factool-0.0.7/setup.cfg` & `factool-0.0.8/setup.cfg`

 * *Files identical despite different names*

