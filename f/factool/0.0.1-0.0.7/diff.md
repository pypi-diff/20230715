# Comparing `tmp/factool-0.0.1.tar.gz` & `tmp/factool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factool-0.0.1.tar", last modified: Sat Jul 15 05:45:42 2023, max compression
+gzip compressed data, was "factool-0.0.7.tar", last modified: Sat Jul 15 07:27:32 2023, max compression
```

## Comparing `factool-0.0.1.tar` & `factool-0.0.7.tar`

### file list

```diff
@@ -1,59 +1,52 @@
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      143 2023-07-15 05:27:59.000000 factool-0.0.1/MANIFEST.in
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     8085 2023-07-15 05:45:42.446501 factool-0.0.1/PKG-INFO
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     7649 2023-07-15 05:33:08.000000 factool-0.0.1/README.md
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.442501 factool-0.0.1/factool/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)       35 2023-07-15 05:30:29.000000 factool-0.0.1/factool/__init__.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.442501 factool-0.0.1/factool/code/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/__init__.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.442501 factool-0.0.1/factool/code/helper/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/helper/__init__.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     7167 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/helper/_execution.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     1681 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/helper/execution.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      730 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/helper/io_utils.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     1384 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/helper/postprocess.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)    12238 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/pipeline.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/code/tool.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      664 2023-07-15 05:27:59.000000 factool-0.0.1/factool/env_config.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     3840 2023-07-15 05:27:59.000000 factool-0.0.1/factool/factool.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/knowledge_qa/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/knowledge_qa/__init__.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     4238 2023-07-15 05:27:59.000000 factool-0.0.1/factool/knowledge_qa/google_serper.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)    10147 2023-07-15 05:27:59.000000 factool-0.0.1/factool/knowledge_qa/pipeline.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      328 2023-07-15 05:27:59.000000 factool-0.0.1/factool/knowledge_qa/tool.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/math/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/math/__init__.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     9266 2023-07-15 05:27:59.000000 factool-0.0.1/factool/math/pipeline.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     1099 2023-07-15 05:27:59.000000 factool-0.0.1/factool/math/tool.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/scientific/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/scientific/__init__.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)    10933 2023-07-15 05:27:59.000000 factool-0.0.1/factool/scientific/pipeline.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      869 2023-07-15 05:27:59.000000 factool-0.0.1/factool/scientific/tool.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/utils/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/utils/__init_.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/utils/__pycache__/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      690 2023-07-15 03:19:53.000000 factool-0.0.1/factool/utils/__pycache__/CustomJSONEncoder.cpython-38.pyc
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     4335 2023-07-15 05:45:01.000000 factool-0.0.1/factool/utils/__pycache__/openai_wrapper.cpython-38.pyc
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      683 2023-07-15 05:45:01.000000 factool-0.0.1/factool/utils/__pycache__/utils_json.cpython-38.pyc
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/utils/base/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:27:59.000000 factool-0.0.1/factool/utils/base/__init__.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/utils/base/__pycache__/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      153 2023-07-15 05:45:01.000000 factool-0.0.1/factool/utils/base/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      925 2023-07-15 05:45:01.000000 factool-0.0.1/factool/utils/base/__pycache__/pipeline.cpython-38.pyc
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      647 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/base/pipeline.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     2834 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/claim_extractor.py
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     4393 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/openai_wrapper.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.446501 factool-0.0.1/factool/utils/prompts/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     2763 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/prompts/agreement_verification.yaml
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     5729 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/prompts/claim_extraction.yaml
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     5618 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/prompts/query_generation.yaml
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)    19390 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/prompts/self_check.yaml
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      378 2023-07-15 05:28:00.000000 factool-0.0.1/factool/utils/utils_json.py
-drwxrwxr-x   0 pliu3    (58062) pliu3    (58063)        0 2023-07-15 05:45:42.442501 factool-0.0.1/factool.egg-info/
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     8085 2023-07-15 05:45:41.000000 factool-0.0.1/factool.egg-info/PKG-INFO
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     1418 2023-07-15 05:45:42.000000 factool-0.0.1/factool.egg-info/SOURCES.txt
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        1 2023-07-15 05:45:41.000000 factool-0.0.1/factool.egg-info/dependency_links.txt
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)      143 2023-07-15 05:45:41.000000 factool-0.0.1/factool.egg-info/requires.txt
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)        8 2023-07-15 05:45:41.000000 factool-0.0.1/factool.egg-info/top_level.txt
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)     1293 2023-07-15 05:45:42.494502 factool-0.0.1/setup.cfg
--rw-rw-r--   0 pliu3    (58062) pliu3    (58063)       77 2023-07-15 05:41:52.000000 factool-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-15 07:26:53.000000 factool-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-15 07:27:32.729171 factool-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-15 07:26:53.000000 factool-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.725171 factool-0.0.7/factool/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 07:26:53.000000 factool-0.0.7/factool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/code/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/helper/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/code/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-15 07:26:53.000000 factool-0.0.7/factool/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-15 07:26:53.000000 factool-0.0.7/factool/factool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/knowledge_qa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/google_serper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 07:26:53.000000 factool-0.0.7/factool/knowledge_qa/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-15 07:26:53.000000 factool-0.0.7/factool/math/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 07:26:53.000000 factool-0.0.7/factool/math/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/scientific/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/scientific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-15 07:26:53.000000 factool-0.0.7/factool/scientific/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-15 07:26:53.000000 factool-0.0.7/factool/scientific/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/__init_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/utils/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/claim_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/openai_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.729171 factool-0.0.7/factool/utils/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/agreement_verification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/claim_extraction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/query_generation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/prompts/self_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 07:26:53.000000 factool-0.0.7/factool/utils/utils_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:27:32.725171 factool-0.0.7/factool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 07:27:32.000000 factool-0.0.7/factool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-15 07:27:32.729171 factool-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-15 07:26:53.000000 factool-0.0.7/setup.py
```

### Comparing `factool-0.0.1/factool/code/helper/_execution.py` & `factool-0.0.7/factool/code/helper/_execution.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-# Copyright (c) Microsoft Corporation.
-# Licensed under the MIT license.
-
-from typing import Optional, Dict
-import contextlib
-import faulthandler
-import io
-import os
-import multiprocessing
-import platform
-import signal
-import tempfile
-
-def test_case_against_solution(prompt: str, completion: str, test: str, timeout: float):
-    """
-    Get the output of a testcases against a solution
-    """
-
-    def unsafe_execute():
-
-        with create_tempdir():
-
-            # These system calls are needed when cleaning up tempdir.
-            import os
-            import shutil
-            rmtree = shutil.rmtree
-            rmdir = os.rmdir
-            chdir = os.chdir
-
-            # Disable functionalities that can make destructive changes to the test.
-            reliability_guard()
-
-            # Construct the check program and run it. VERY IMPORTANT!!!
-            import_packages_end_index = prompt.find("def")
-
-            # some HumanEval prompts contain helper function that has to be included. Patching.
-            helper_func = ""
-            helper_funcs_to_be_included = ["\n\ndef is_palindrome(string: str) -> bool:\n    \"\"\" Test if given string is a palindrome \"\"\"\n    return string == string[::-1]\n\n\n", "import math\n\n\ndef poly(xs: list, x: float):\n    \"\"\"\n    Evaluates polynomial with coefficients xs at point x.\n    return xs[0] + xs[1] * x + xs[1] * x^2 + .... xs[n] * x^n\n    \"\"\"\n    return sum([coeff * math.pow(x, i) for i, coeff in enumerate(xs)])\n\n\n", "\n\ndef encode_cyclic(s: str):\n    \"\"\"\n    returns encoded string by cycling groups of three characters.\n    \"\"\"\n    # split string to groups. Each of length 3.\n    groups = [s[(3 * i):min((3 * i + 3), len(s))] for i in range((len(s) + 2) // 3)]\n    # cycle elements in each group. Unless group has fewer elements than 3.\n    groups = [(group[1:] + group[0]) if len(group) == 3 else group for group in groups]\n    return \"\".join(groups)\n\n\n", "\n\ndef encode_shift(s: str):\n    \"\"\"\n    returns encoded string by shifting every character by 5 in the alphabet.\n    \"\"\"\n    return \"\".join([chr(((ord(ch) + 5 - ord(\"a\")) % 26) + ord(\"a\")) for ch in s])\n\n\n"]
-            for helper in helper_funcs_to_be_included:
-                if helper in prompt:
-                    helper_func = helper
-
-            check_program = (
-                prompt[:import_packages_end_index] + helper_func + completion + "\n" + f'result = {test}'
-            )
-
-            try:
-                exec_globals = {}
-                with swallow_io():
-                    with time_limit(timeout):
-                        exec(check_program, exec_globals)
-                        result.append(exec_globals['result'])
-            except TimeoutException:
-                result.append("FAILURE: timed out")
-            except BaseException as e:
-                error_type = type(e).__name__
-                result.append(f"FAILURE: {error_type}: {e}")
-
-            # Needed for cleaning up.
-            shutil.rmtree = rmtree
-            os.rmdir = rmdir
-            os.chdir = chdir
-
-    manager = multiprocessing.Manager()
-    result = manager.list()
-
-    p = multiprocessing.Process(target=unsafe_execute)
-    p.start()
-    p.join(timeout=timeout+1)
-    if p.is_alive():
-        p.kill()
-
-    if not result:
-        result.append("timed out")
-
-    return result[0]
-
-@contextlib.contextmanager
-def time_limit(seconds: float):
-    def signal_handler(signum, frame):
-        raise TimeoutException("Timed out!")
-    signal.setitimer(signal.ITIMER_REAL, seconds)
-    signal.signal(signal.SIGALRM, signal_handler)
-    try:
-        yield
-    finally:
-        signal.setitimer(signal.ITIMER_REAL, 0)
-
-
-@contextlib.contextmanager
-def swallow_io():
-    stream = WriteOnlyStringIO()
-    with contextlib.redirect_stdout(stream):
-        with contextlib.redirect_stderr(stream):
-            with redirect_stdin(stream):
-                yield
-
-
-@contextlib.contextmanager
-def create_tempdir():
-    with tempfile.TemporaryDirectory() as dirname:
-        with chdir(dirname):
-            yield dirname
-
-
-class TimeoutException(Exception):
-    pass
-
-
-class WriteOnlyStringIO(io.StringIO):
-    """ StringIO that throws an exception when it's read from """
-
-    def read(self, *args, **kwargs):
-        raise IOError
-
-    def readline(self, *args, **kwargs):
-        raise IOError
-
-    def readlines(self, *args, **kwargs):
-        raise IOError
-
-    def readable(self, *args, **kwargs):
-        """ Returns True if the IO object can be read. """
-        return False
-
-
-class redirect_stdin(contextlib._RedirectStream):  # type: ignore
-    _stream = 'stdin'
-
-
-@contextlib.contextmanager
-def chdir(root):
-    if root == ".":
-        yield
-        return
-    cwd = os.getcwd()
-    os.chdir(root)
-    try:
-        yield
-    except BaseException as exc:
-        raise exc
-    finally:
-        os.chdir(cwd)
-
-
-def reliability_guard(maximum_memory_bytes: Optional[int] = None):
-    """
-    This disables various destructive functions and prevents the generated code
-    from interfering with the test (e.g. fork bomb, killing other processes,
-    removing filesystem files, etc.)
-
-    WARNING
-    This function is NOT a security sandbox. Untrusted code, including, model-
-    generated code, should not be blindly executed outside of one. See the 
-    Codex paper for more information about OpenAI's code sandbox, and proceed
-    with caution.
-    """
-
-    if maximum_memory_bytes is not None:
-        import resource
-        resource.setrlimit(resource.RLIMIT_AS, (maximum_memory_bytes, maximum_memory_bytes))
-        resource.setrlimit(resource.RLIMIT_DATA, (maximum_memory_bytes, maximum_memory_bytes))
-        if not platform.uname().system == 'Darwin':
-            resource.setrlimit(resource.RLIMIT_STACK, (maximum_memory_bytes, maximum_memory_bytes))
-
-    faulthandler.disable()
-
-    import builtins
-    builtins.exit = None
-    builtins.quit = None
-
-    import os
-    os.environ['OMP_NUM_THREADS'] = '1'
-
-    os.kill = None
-    os.system = None
-    os.putenv = None
-    os.remove = None
-    os.removedirs = None
-    os.rmdir = None
-    os.fchdir = None
-    os.setuid = None
-    os.fork = None
-    os.forkpty = None
-    os.killpg = None
-    os.rename = None
-    os.renames = None
-    os.truncate = None
-    os.replace = None
-    os.unlink = None
-    os.fchmod = None
-    os.fchown = None
-    os.chmod = None
-    os.chown = None
-    os.chroot = None
-    os.fchdir = None
-    os.lchflags = None
-    os.lchmod = None
-    os.lchown = None
-    os.getcwd = None
-    os.chdir = None
-
-    import shutil
-    shutil.rmtree = None
-    shutil.move = None
-    shutil.chown = None
-
-    import subprocess
-    subprocess.Popen = None  # type: ignore
-
-    __builtins__['help'] = None
-
-    import sys
-    sys.modules['ipdb'] = None
-    sys.modules['joblib'] = None
-    sys.modules['resource'] = None
-    sys.modules['psutil'] = None
-    sys.modules['tkinter'] = None
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
+from typing import Optional, Dict
+import contextlib
+import faulthandler
+import io
+import os
+import multiprocessing
+import platform
+import signal
+import tempfile
+
+def test_case_against_solution(prompt: str, completion: str, test: str, timeout: float):
+    """
+    Get the output of a testcases against a solution
+    """
+
+    def unsafe_execute():
+
+        with create_tempdir():
+
+            # These system calls are needed when cleaning up tempdir.
+            import os
+            import shutil
+            rmtree = shutil.rmtree
+            rmdir = os.rmdir
+            chdir = os.chdir
+
+            # Disable functionalities that can make destructive changes to the test.
+            reliability_guard()
+
+            # Construct the check program and run it. VERY IMPORTANT!!!
+            import_packages_end_index = prompt.find("def")
+
+            # some HumanEval prompts contain helper function that has to be included. Patching.
+            helper_func = ""
+            helper_funcs_to_be_included = ["\n\ndef is_palindrome(string: str) -> bool:\n    \"\"\" Test if given string is a palindrome \"\"\"\n    return string == string[::-1]\n\n\n", "import math\n\n\ndef poly(xs: list, x: float):\n    \"\"\"\n    Evaluates polynomial with coefficients xs at point x.\n    return xs[0] + xs[1] * x + xs[1] * x^2 + .... xs[n] * x^n\n    \"\"\"\n    return sum([coeff * math.pow(x, i) for i, coeff in enumerate(xs)])\n\n\n", "\n\ndef encode_cyclic(s: str):\n    \"\"\"\n    returns encoded string by cycling groups of three characters.\n    \"\"\"\n    # split string to groups. Each of length 3.\n    groups = [s[(3 * i):min((3 * i + 3), len(s))] for i in range((len(s) + 2) // 3)]\n    # cycle elements in each group. Unless group has fewer elements than 3.\n    groups = [(group[1:] + group[0]) if len(group) == 3 else group for group in groups]\n    return \"\".join(groups)\n\n\n", "\n\ndef encode_shift(s: str):\n    \"\"\"\n    returns encoded string by shifting every character by 5 in the alphabet.\n    \"\"\"\n    return \"\".join([chr(((ord(ch) + 5 - ord(\"a\")) % 26) + ord(\"a\")) for ch in s])\n\n\n"]
+            for helper in helper_funcs_to_be_included:
+                if helper in prompt:
+                    helper_func = helper
+
+            check_program = (
+                prompt[:import_packages_end_index] + helper_func + completion + "\n" + f'result = {test}'
+            )
+
+            try:
+                exec_globals = {}
+                with swallow_io():
+                    with time_limit(timeout):
+                        exec(check_program, exec_globals)
+                        result.append(exec_globals['result'])
+            except TimeoutException:
+                result.append("FAILURE: timed out")
+            except BaseException as e:
+                error_type = type(e).__name__
+                result.append(f"FAILURE: {error_type}: {e}")
+
+            # Needed for cleaning up.
+            shutil.rmtree = rmtree
+            os.rmdir = rmdir
+            os.chdir = chdir
+
+    manager = multiprocessing.Manager()
+    result = manager.list()
+
+    p = multiprocessing.Process(target=unsafe_execute)
+    p.start()
+    p.join(timeout=timeout+1)
+    if p.is_alive():
+        p.kill()
+
+    if not result:
+        result.append("timed out")
+
+    return result[0]
+
+@contextlib.contextmanager
+def time_limit(seconds: float):
+    def signal_handler(signum, frame):
+        raise TimeoutException("Timed out!")
+    signal.setitimer(signal.ITIMER_REAL, seconds)
+    signal.signal(signal.SIGALRM, signal_handler)
+    try:
+        yield
+    finally:
+        signal.setitimer(signal.ITIMER_REAL, 0)
+
+
+@contextlib.contextmanager
+def swallow_io():
+    stream = WriteOnlyStringIO()
+    with contextlib.redirect_stdout(stream):
+        with contextlib.redirect_stderr(stream):
+            with redirect_stdin(stream):
+                yield
+
+
+@contextlib.contextmanager
+def create_tempdir():
+    with tempfile.TemporaryDirectory() as dirname:
+        with chdir(dirname):
+            yield dirname
+
+
+class TimeoutException(Exception):
+    pass
+
+
+class WriteOnlyStringIO(io.StringIO):
+    """ StringIO that throws an exception when it's read from """
+
+    def read(self, *args, **kwargs):
+        raise IOError
+
+    def readline(self, *args, **kwargs):
+        raise IOError
+
+    def readlines(self, *args, **kwargs):
+        raise IOError
+
+    def readable(self, *args, **kwargs):
+        """ Returns True if the IO object can be read. """
+        return False
+
+
+class redirect_stdin(contextlib._RedirectStream):  # type: ignore
+    _stream = 'stdin'
+
+
+@contextlib.contextmanager
+def chdir(root):
+    if root == ".":
+        yield
+        return
+    cwd = os.getcwd()
+    os.chdir(root)
+    try:
+        yield
+    except BaseException as exc:
+        raise exc
+    finally:
+        os.chdir(cwd)
+
+
+def reliability_guard(maximum_memory_bytes: Optional[int] = None):
+    """
+    This disables various destructive functions and prevents the generated code
+    from interfering with the test (e.g. fork bomb, killing other processes,
+    removing filesystem files, etc.)
+
+    WARNING
+    This function is NOT a security sandbox. Untrusted code, including, model-
+    generated code, should not be blindly executed outside of one. See the 
+    Codex paper for more information about OpenAI's code sandbox, and proceed
+    with caution.
+    """
+
+    if maximum_memory_bytes is not None:
+        import resource
+        resource.setrlimit(resource.RLIMIT_AS, (maximum_memory_bytes, maximum_memory_bytes))
+        resource.setrlimit(resource.RLIMIT_DATA, (maximum_memory_bytes, maximum_memory_bytes))
+        if not platform.uname().system == 'Darwin':
+            resource.setrlimit(resource.RLIMIT_STACK, (maximum_memory_bytes, maximum_memory_bytes))
+
+    faulthandler.disable()
+
+    import builtins
+    builtins.exit = None
+    builtins.quit = None
+
+    import os
+    os.environ['OMP_NUM_THREADS'] = '1'
+
+    os.kill = None
+    os.system = None
+    os.putenv = None
+    os.remove = None
+    os.removedirs = None
+    os.rmdir = None
+    os.fchdir = None
+    os.setuid = None
+    os.fork = None
+    os.forkpty = None
+    os.killpg = None
+    os.rename = None
+    os.renames = None
+    os.truncate = None
+    os.replace = None
+    os.unlink = None
+    os.fchmod = None
+    os.fchown = None
+    os.chmod = None
+    os.chown = None
+    os.chroot = None
+    os.fchdir = None
+    os.lchflags = None
+    os.lchmod = None
+    os.lchown = None
+    os.getcwd = None
+    os.chdir = None
+
+    import shutil
+    shutil.rmtree = None
+    shutil.move = None
+    shutil.chown = None
+
+    import subprocess
+    subprocess.Popen = None  # type: ignore
+
+    __builtins__['help'] = None
+
+    import sys
+    sys.modules['ipdb'] = None
+    sys.modules['joblib'] = None
+    sys.modules['resource'] = None
+    sys.modules['psutil'] = None
+    sys.modules['tkinter'] = None
```

### Comparing `factool-0.0.1/factool/code/helper/execution.py` & `factool-0.0.7/factool/code/helper/execution.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# Copyright (c) Microsoft Corporation.
-# Licensed under the MIT license.
-
-import ctypes
-# libgcc_s = ctypes.CDLL('libgcc_s.so.1')
-
-from collections import defaultdict
-from concurrent.futures import as_completed, ProcessPoolExecutor
-import logging
-
-from factool.code.helper._execution import test_case_against_solution
-
-logging.basicConfig(
-    format="SystemLog: [%(asctime)s][%(name)s][%(levelname)s] - %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S",
-    level=logging.INFO,
-)
-
-logger = logging.getLogger(__name__)
-
-def evaluate_test_cases_multi_solution(prompt, testcases_input, multi_solutions, timeout=0.1):
-    logger.info(f'Start evaluation with test code, timeout={timeout}')
-
-    with ProcessPoolExecutor() as executor:
-        futures = []
-        results = [[None for _ in multi_solutions] for _ in testcases_input]
-
-        for i, testcase in enumerate(testcases_input):
-            for j, solution in enumerate(multi_solutions):
-                args = (prompt, solution, testcase, timeout)
-                future = executor.submit(test_case_against_solution, *args)
-                futures.append((i, j, future))
-        logger.info(f'{len(futures)} execution requests are submitted')
-        
-        for completed_future in as_completed([f[2] for f in futures]):
-            for i, j, future in futures:
-                if future == completed_future:
-                    logger.info('[{}/{}] execution completed'.format(i * len(multi_solutions) + j + 1, len(futures)))
-                    result = completed_future.result()
-                    results[i][j] = result
-                    break
-
-    return results
-
-
-
-
-
-
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
+import ctypes
+# libgcc_s = ctypes.CDLL('libgcc_s.so.1')
+
+from collections import defaultdict
+from concurrent.futures import as_completed, ProcessPoolExecutor
+import logging
+
+from factool.code.helper._execution import test_case_against_solution
+
+logging.basicConfig(
+    format="SystemLog: [%(asctime)s][%(name)s][%(levelname)s] - %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+    level=logging.INFO,
+)
+
+logger = logging.getLogger(__name__)
+
+def evaluate_test_cases_multi_solution(prompt, testcases_input, multi_solutions, timeout=0.1):
+    logger.info(f'Start evaluation with test code, timeout={timeout}')
+
+    with ProcessPoolExecutor() as executor:
+        futures = []
+        results = [[None for _ in multi_solutions] for _ in testcases_input]
+
+        for i, testcase in enumerate(testcases_input):
+            for j, solution in enumerate(multi_solutions):
+                args = (prompt, solution, testcase, timeout)
+                future = executor.submit(test_case_against_solution, *args)
+                futures.append((i, j, future))
+        logger.info(f'{len(futures)} execution requests are submitted')
+        
+        for completed_future in as_completed([f[2] for f in futures]):
+            for i, j, future in futures:
+                if future == completed_future:
+                    logger.info('[{}/{}] execution completed'.format(i * len(multi_solutions) + j + 1, len(futures)))
+                    result = completed_future.result()
+                    results[i][j] = result
+                    break
+
+    return results
+
+
+
+
+
+
```

### Comparing `factool-0.0.1/factool/code/helper/io_utils.py` & `factool-0.0.7/factool/code/helper/io_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Copyright (c) Microsoft Corporation.
-# Licensed under the MIT license.
-
-import json
-
-class Tools:
-    @staticmethod
-    def load_jsonl(file_path):
-        json_objects = []
-        with open(file_path, 'r', encoding='utf8') as f:
-            for line in f:
-                json_objects.append(json.loads(line.strip()))
-        return json_objects
-    
-    @staticmethod
-    def load_tasks(task_path):
-        result = dict()
-        lines = Tools.load_jsonl(task_path)
-        for line in lines:
-            result[line['task_id']] = line
-        return result
-        
-    @staticmethod
-    def write_file(path, content):
-        with open(path, 'w', encoding='utf8') as f:
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT license.
+
+import json
+
+class Tools:
+    @staticmethod
+    def load_jsonl(file_path):
+        json_objects = []
+        with open(file_path, 'r', encoding='utf8') as f:
+            for line in f:
+                json_objects.append(json.loads(line.strip()))
+        return json_objects
+    
+    @staticmethod
+    def load_tasks(task_path):
+        result = dict()
+        lines = Tools.load_jsonl(task_path)
+        for line in lines:
+            result[line['task_id']] = line
+        return result
+        
+    @staticmethod
+    def write_file(path, content):
+        with open(path, 'w', encoding='utf8') as f:
             f.write(content)
```

### Comparing `factool-0.0.1/factool/code/pipeline.py` & `factool-0.0.7/factool/code/pipeline.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-import logging
-import copy
-import pdb
-import math
-import os
-import json
-import yaml
-import time
-import re
-from typing import List, Dict
-
-from factool.utils.base.pipeline import pipeline
-from factool.code.helper.postprocess import PostProcessor
-from factool.code.helper.execution import evaluate_test_cases_multi_solution
-from factool.utils.utils_json import CustomJSONEncoder
-
-class code_pipeline(pipeline):
-    def __init__(self, foundation_model, multi_solution_cnt, testcases_input_cnt):
-        super().__init__('code', foundation_model)
-
-        self.multi_solution_cnt = multi_solution_cnt
-        self.testcases_input_cnt = testcases_input_cnt
-
-        with open(os.path.join(self.prompts_path, "query_generation.yaml"), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.query_generation_prompt = data['code']
-
-    async def _testcases_input_generation(self, batch, testcases_input_cnt):
-        messages_list = []
-        if self.company == 'openai':
-            messages_list = [
-                [
-                    {"role": "system", "content": self.query_generation_prompt['system']},
-                    {"role": "user", "content": self.query_generation_prompt['user_testcases_' + str(testcases_input_cnt)].format(input_question=sample['prompt'], entry_point=sample['entry_point'])},
-                ]
-                for sample in batch
-            ]
-        elif self.company == 'anthropic':
-            messages_list = [self.query_generation_prompt['user_testcases_' + str(testcases_input_cnt)].format(input_question=sample['prompt'], entry_point=sample['entry_point']) for sample in batch]
-        return await self.chat.async_run(messages_list, Dict)
-    
-    async def _multi_solution_generation(self, batch, multi_solution_cnt):
-        bsize = 15
-        messages_list = [
-            [
-                {"role": "system", "content": self.query_generation_prompt['system']},
-                {"role": "user", "content": self.query_generation_prompt['user_solutions'].format(input_question=sample['prompt'], entry_point=sample['entry_point'])},
-            ]
-            for sample in batch
-        ]
-
-        final_messages_list = [copy.deepcopy(messages) for messages in messages_list for _ in range(multi_solution_cnt)]
-
-        responses = []
-        for i in range(0, len(final_messages_list), bsize):
-            batch = final_messages_list[i:i + bsize]
-            responses += await self.chat.async_run(batch, Dict)
-        
-        # Split the list into lists of length of multi_solution_cnt
-        responses_split = [responses[i:i + multi_solution_cnt] for i in range(0, len(responses),  multi_solution_cnt)]
-
-        # Transform each element in each list
-        multi_solutions = []
-        for solutions in responses_split:
-            key_names = [f"python_solution_{i}" for i in range(1, multi_solution_cnt + 1)]
-            new_element = {key: solutions[i]['python_solution'] if solutions[i] != None else "None" for i, key in enumerate(key_names)}
-            multi_solutions.append(new_element)
-
-        return multi_solutions
-    
-    async def run_with_tool_live(self, batch, batch_size):
-        testcases_input = await self._testcases_input_generation(batch, self.testcases_input_cnt)
-        multi_solutions = await self._multi_solution_generation(batch, self.multi_solution_cnt)
-
-        if testcases_input == None or multi_solutions == None:
-            return None
-        
-        responses = []
-        for i in range(batch_size):
-            response = {'testcases_input': [], 'multi_solutions': [], 'with_tool_classification': "None"}
-            try:
-                response['testcases_input'] = list(testcases_input[i].values())
-                # Append the solution to be verified to the LAST element of multi_solutions
-                response['multi_solutions'] = [multi_solutions[i][f'python_solution_{j}'] for j in range(1, self.multi_solution_cnt + 1)] + [batch[i]['completion']]
-            except:
-                response['testcases_input'] = ["None"] * self.testcases_input_cnt
-                response['multi_solutions'] = ["None"] * (self.multi_solution_cnt + 1)
-            
-            exec_result = evaluate_test_cases_multi_solution(batch[i]['prompt'], response['testcases_input'], response['multi_solutions'], timeout=0.1)
-            response['exec_result'] = exec_result
-            
-            response['with_tool_classification'] = True
-            # must pass all testcases to be classified as "True"
-            for testcase_result in exec_result:
-                # syntax or timeout error happening on the potential solution
-                if isinstance(testcase_result[-1], str) and testcase_result[-1].startswith('FAILURE'):
-                    response['with_tool_classification'] = False
-                # majority voting. Note that the last element is the solution to be verified. Also, multi solutions that return "FAILURE" are not counted and removed.
-                else:
-                    failure_indices = [i for i, res in enumerate(testcase_result[:-1]) if isinstance(res, str) and res.startswith('FAILURE')]
-                    testcase_result = [res for i, res in enumerate(testcase_result) if i not in failure_indices]
-
-                    try:
-                        if testcase_result[:-1].count(testcase_result[-1]) < math.ceil(len(testcase_result) / 2):
-                            response['with_tool_classification'] = False
-                    # sometimes numpy array is included in testcase_result, so this error will be raised
-                    except:
-                        response['with_tool_classification'] = False
-            
-            responses.append(response)
-
-        return responses
-
-    async def run_with_tool_api_call(self, prompts, responses, entry_points):
-
-        # response preprocessing to extract the code snippet:
-        claims = []
-        for i, response in enumerate(responses):
-            if "```python" in response:
-                match = re.search(r"```python\n(.*?)\n```", response, re.DOTALL)
-                if match:
-                    claims.append(match.group(1))
-                else:
-                    claims.append("")
-            elif "```" in response:
-                match = re.search(r"```\n(.*?)\n```", response, re.DOTALL)
-                if match:
-                    claims.append(match.group(1))
-                else:
-                    claims.append("")
-            else:
-                claims.append(response)
-
-        batch_size = 5
-        num_batches = math.ceil(len(prompts) / batch_size)
-
-        self.sample_list = [{"prompt": prompt, "response": response, "entry_point": entry_point, "completion": claim, "category": 'code'} for prompt, response, entry_point, claim in zip(prompts, responses, entry_points, claims)]
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(responses))
-
-            responses_returned = await self.run_with_tool_live(self.sample_list[batch_start: batch_end], batch_end - batch_start)
-
-            for j, response_returned in enumerate(responses_returned):
-                index = batch_start + j
-                self.sample_list[index].update({
-                    'claim': self.sample_list[index]['completion'],
-                    'testcases_queries': response_returned['testcases_input'],
-                    'potential_solutions_queries': response_returned['multi_solutions'],
-                    'exec_results': response_returned['exec_result'],
-                    'claim_level_factuality': response_returned['with_tool_classification'],
-                    'response_level_factuality': response_returned['with_tool_classification']
-                })
-                del self.sample_list[index]["completion"]
-
-        return self.sample_list
-        
-    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
-        data_path = with_tool_classified_dataset_path if rerun else annotated_dataset_path
-        with open(data_path, 'r') as f:
-            data = [json.loads(line) for line in f]
-        self.sample_list = data
-        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 5
-        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(rerun_elements))
-
-            responses = await self.run_with_tool_live(rerun_elements[batch_start:batch_end], batch_end - batch_start)
-
-            for j, response in enumerate(responses):
-                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
-                self.sample_list[index]['with_tool_classification'] = response['with_tool_classification'] if response is not None else 'None'
-                if response is not None:
-                    self.sample_list[index].update({
-                        'testcases_input': response['testcases_input'],
-                        'multi_solutions': response['multi_solutions'],
-                        'exec_result': response['exec_result']
-                    })
-        
-            # save everything after each batch to prevent data loss
-            with open(with_tool_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    try:
-                        json_str = json.dumps(item, cls=CustomJSONEncoder)
-                    except:
-                        continue
-                    f.write(json_str + '\n')
-    
-    async def run_self_check_live(self, fewshot, batch):
-        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
-        messages_list = [
-            [
-                {"role": "system", "content": self.self_check_prompt['system']},
-                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(input_question=response['prompt'], input_solution=response['completion'])},
-            ]
-            for response in batch
-        ]
-        return await self.chat.async_run(messages_list, Dict)
-
-    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
-        if rerun == False:
-            with open(annotated_dataset_path, 'r') as f:
-                self.sample_list = [json.loads(line) for line in f]
-            rerun_elements = self.sample_list
-        else:
-            with open(self_check_classified_dataset_path, 'r') as f:
-                self.sample_list = [json.loads(line) for line in f]
-            rerun_elements = [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 5
-        num_batches = math.ceil(len(rerun_elements) / batch_size)
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = (i + 1) * batch_size
-            batch = rerun_elements[batch_start:batch_end]
-
-            responses = await self.run_self_check_live(fewshot, batch)
-            for j, response in enumerate(responses):
-                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
-                self.sample_list[index]['self_check_classification'] = response.get('factuality', 'None') if response is not None else 'None'
-                self.sample_list[index]['self_check_reasoning'] = response.get('reasoning', 'None') if response is not None else 'None'
-        
-            # save everything after each batch to prevent data loss
-            with open(self_check_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    json_str = json.dumps(item)
+import logging
+import copy
+import pdb
+import math
+import os
+import json
+import yaml
+import time
+import re
+from typing import List, Dict
+
+from factool.utils.base.pipeline import pipeline
+from factool.code.helper.postprocess import PostProcessor
+from factool.code.helper.execution import evaluate_test_cases_multi_solution
+from factool.utils.utils_json import CustomJSONEncoder
+
+class code_pipeline(pipeline):
+    def __init__(self, foundation_model, multi_solution_cnt, testcases_input_cnt):
+        super().__init__('code', foundation_model)
+
+        self.multi_solution_cnt = multi_solution_cnt
+        self.testcases_input_cnt = testcases_input_cnt
+
+        with open(os.path.join(self.prompts_path, "query_generation.yaml"), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.query_generation_prompt = data['code']
+
+    async def _testcases_input_generation(self, batch, testcases_input_cnt):
+        messages_list = []
+        if self.company == 'openai':
+            messages_list = [
+                [
+                    {"role": "system", "content": self.query_generation_prompt['system']},
+                    {"role": "user", "content": self.query_generation_prompt['user_testcases_' + str(testcases_input_cnt)].format(input_question=sample['prompt'], entry_point=sample['entry_point'])},
+                ]
+                for sample in batch
+            ]
+        elif self.company == 'anthropic':
+            messages_list = [self.query_generation_prompt['user_testcases_' + str(testcases_input_cnt)].format(input_question=sample['prompt'], entry_point=sample['entry_point']) for sample in batch]
+        return await self.chat.async_run(messages_list, Dict)
+    
+    async def _multi_solution_generation(self, batch, multi_solution_cnt):
+        bsize = 15
+        messages_list = [
+            [
+                {"role": "system", "content": self.query_generation_prompt['system']},
+                {"role": "user", "content": self.query_generation_prompt['user_solutions'].format(input_question=sample['prompt'], entry_point=sample['entry_point'])},
+            ]
+            for sample in batch
+        ]
+
+        final_messages_list = [copy.deepcopy(messages) for messages in messages_list for _ in range(multi_solution_cnt)]
+
+        responses = []
+        for i in range(0, len(final_messages_list), bsize):
+            batch = final_messages_list[i:i + bsize]
+            responses += await self.chat.async_run(batch, Dict)
+        
+        # Split the list into lists of length of multi_solution_cnt
+        responses_split = [responses[i:i + multi_solution_cnt] for i in range(0, len(responses),  multi_solution_cnt)]
+
+        # Transform each element in each list
+        multi_solutions = []
+        for solutions in responses_split:
+            key_names = [f"python_solution_{i}" for i in range(1, multi_solution_cnt + 1)]
+            new_element = {key: solutions[i]['python_solution'] if solutions[i] != None else "None" for i, key in enumerate(key_names)}
+            multi_solutions.append(new_element)
+
+        return multi_solutions
+    
+    async def run_with_tool_live(self, batch, batch_size):
+        testcases_input = await self._testcases_input_generation(batch, self.testcases_input_cnt)
+        multi_solutions = await self._multi_solution_generation(batch, self.multi_solution_cnt)
+
+        if testcases_input == None or multi_solutions == None:
+            return None
+        
+        responses = []
+        for i in range(batch_size):
+            response = {'testcases_input': [], 'multi_solutions': [], 'with_tool_classification': "None"}
+            try:
+                response['testcases_input'] = list(testcases_input[i].values())
+                # Append the solution to be verified to the LAST element of multi_solutions
+                response['multi_solutions'] = [multi_solutions[i][f'python_solution_{j}'] for j in range(1, self.multi_solution_cnt + 1)] + [batch[i]['completion']]
+            except:
+                response['testcases_input'] = ["None"] * self.testcases_input_cnt
+                response['multi_solutions'] = ["None"] * (self.multi_solution_cnt + 1)
+            
+            exec_result = evaluate_test_cases_multi_solution(batch[i]['prompt'], response['testcases_input'], response['multi_solutions'], timeout=0.1)
+            response['exec_result'] = exec_result
+            
+            response['with_tool_classification'] = True
+            # must pass all testcases to be classified as "True"
+            for testcase_result in exec_result:
+                # syntax or timeout error happening on the potential solution
+                if isinstance(testcase_result[-1], str) and testcase_result[-1].startswith('FAILURE'):
+                    response['with_tool_classification'] = False
+                # majority voting. Note that the last element is the solution to be verified. Also, multi solutions that return "FAILURE" are not counted and removed.
+                else:
+                    failure_indices = [i for i, res in enumerate(testcase_result[:-1]) if isinstance(res, str) and res.startswith('FAILURE')]
+                    testcase_result = [res for i, res in enumerate(testcase_result) if i not in failure_indices]
+
+                    try:
+                        if testcase_result[:-1].count(testcase_result[-1]) < math.ceil(len(testcase_result) / 2):
+                            response['with_tool_classification'] = False
+                    # sometimes numpy array is included in testcase_result, so this error will be raised
+                    except:
+                        response['with_tool_classification'] = False
+            
+            responses.append(response)
+
+        return responses
+
+    async def run_with_tool_api_call(self, prompts, responses, entry_points):
+
+        # response preprocessing to extract the code snippet:
+        claims = []
+        for i, response in enumerate(responses):
+            if "```python" in response:
+                match = re.search(r"```python\n(.*?)\n```", response, re.DOTALL)
+                if match:
+                    claims.append(match.group(1))
+                else:
+                    claims.append("")
+            elif "```" in response:
+                match = re.search(r"```\n(.*?)\n```", response, re.DOTALL)
+                if match:
+                    claims.append(match.group(1))
+                else:
+                    claims.append("")
+            else:
+                claims.append(response)
+
+        batch_size = 5
+        num_batches = math.ceil(len(prompts) / batch_size)
+
+        self.sample_list = [{"prompt": prompt, "response": response, "entry_point": entry_point, "completion": claim, "category": 'code'} for prompt, response, entry_point, claim in zip(prompts, responses, entry_points, claims)]
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(responses))
+
+            responses_returned = await self.run_with_tool_live(self.sample_list[batch_start: batch_end], batch_end - batch_start)
+
+            for j, response_returned in enumerate(responses_returned):
+                index = batch_start + j
+                self.sample_list[index].update({
+                    'claim': self.sample_list[index]['completion'],
+                    'testcases_queries': response_returned['testcases_input'],
+                    'potential_solutions_queries': response_returned['multi_solutions'],
+                    'exec_results': response_returned['exec_result'],
+                    'claim_level_factuality': response_returned['with_tool_classification'],
+                    'response_level_factuality': response_returned['with_tool_classification']
+                })
+                del self.sample_list[index]["completion"]
+
+        return self.sample_list
+        
+    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
+        data_path = with_tool_classified_dataset_path if rerun else annotated_dataset_path
+        with open(data_path, 'r') as f:
+            data = [json.loads(line) for line in f]
+        self.sample_list = data
+        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 5
+        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(rerun_elements))
+
+            responses = await self.run_with_tool_live(rerun_elements[batch_start:batch_end], batch_end - batch_start)
+
+            for j, response in enumerate(responses):
+                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
+                self.sample_list[index]['with_tool_classification'] = response['with_tool_classification'] if response is not None else 'None'
+                if response is not None:
+                    self.sample_list[index].update({
+                        'testcases_input': response['testcases_input'],
+                        'multi_solutions': response['multi_solutions'],
+                        'exec_result': response['exec_result']
+                    })
+        
+            # save everything after each batch to prevent data loss
+            with open(with_tool_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    try:
+                        json_str = json.dumps(item, cls=CustomJSONEncoder)
+                    except:
+                        continue
+                    f.write(json_str + '\n')
+    
+    async def run_self_check_live(self, fewshot, batch):
+        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
+        messages_list = [
+            [
+                {"role": "system", "content": self.self_check_prompt['system']},
+                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(input_question=response['prompt'], input_solution=response['completion'])},
+            ]
+            for response in batch
+        ]
+        return await self.chat.async_run(messages_list, Dict)
+
+    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
+        if rerun == False:
+            with open(annotated_dataset_path, 'r') as f:
+                self.sample_list = [json.loads(line) for line in f]
+            rerun_elements = self.sample_list
+        else:
+            with open(self_check_classified_dataset_path, 'r') as f:
+                self.sample_list = [json.loads(line) for line in f]
+            rerun_elements = [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 5
+        num_batches = math.ceil(len(rerun_elements) / batch_size)
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = (i + 1) * batch_size
+            batch = rerun_elements[batch_start:batch_end]
+
+            responses = await self.run_self_check_live(fewshot, batch)
+            for j, response in enumerate(responses):
+                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
+                self.sample_list[index]['self_check_classification'] = response.get('factuality', 'None') if response is not None else 'None'
+                self.sample_list[index]['self_check_reasoning'] = response.get('reasoning', 'None') if response is not None else 'None'
+        
+            # save everything after each batch to prevent data loss
+            with open(self_check_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    json_str = json.dumps(item)
                     f.write(json_str + '\n')
```

### Comparing `factool-0.0.1/factool/factool.py` & `factool-0.0.7/factool/factool.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import asyncio
-import copy
-
-from factool.knowledge_qa.pipeline import knowledge_qa_pipeline
-from factool.code.pipeline import code_pipeline
-from factool.math.pipeline import math_pipeline
-from factool.scientific.pipeline import scientific_pipeline
-
-class Factool():
-    def __init__(self, foundation_model):
-        self.pipelines = {
-                            "kbqa": knowledge_qa_pipeline(
-                                foundation_model, 10
-                            ),
-                            "code": code_pipeline(
-                                foundation_model, 3, 3
-                            ),
-                            "math": math_pipeline(
-                                foundation_model
-                            ),
-                            "scientific": scientific_pipeline(
-                                foundation_model
-                            ),
-                        }
-
-    def run(self, inputs):
-        outputs = copy.deepcopy(inputs)
-
-        batches = []
-        current_category = inputs[0]['category']
-        current_batch = []
-
-        for input in inputs:
-            if input['category'] == current_category:
-                current_batch.append(input)
-            else:
-                batches.append(current_batch)
-                current_batch = [input]
-                current_category = input['category']
-                    
-        batches.append(current_batch)  # append the last batch
-
-        index = 0
-        for batch in batches:
-            category = batch[0]['category']
-            if category == 'code':
-                batch_results = asyncio.run(
-                    self.pipelines[category].run_with_tool_api_call(
-                        [sample['prompt'] for sample in batch],
-                        [sample['response'] for sample in batch],
-                        [sample['entry_point'] for sample in batch]
-                    )
-                )
-            else:
-                batch_results = asyncio.run(
-                    self.pipelines[category].run_with_tool_api_call(
-                        [sample['prompt'] for sample in batch],
-                        [sample['response'] for sample in batch]
-                    )
-                )
-            for result in batch_results:
-                outputs[index].update(result)
-                index += 1
-        
-        return outputs
-
-    async def run_for_plugin(self, inputs):
-        outputs = copy.deepcopy(inputs)
-
-        batches = []
-        current_category = inputs[0]['category']
-        current_batch = []
-
-        for input in inputs:
-            if input['category'] == current_category:
-                current_batch.append(input)
-            else:
-                batches.append(current_batch)
-                current_batch = [input]
-                current_category = input['category']
-                    
-        batches.append(current_batch)  # append the last batch
-
-        index = 0
-        for batch in batches:
-            category = batch[0]['category']
-            if category == 'code':
-                batch_results = await self.pipelines[category].run_with_tool_api_call(
-                    [sample['prompt'] for sample in batch],
-                    [sample['response'] for sample in batch],
-                    [sample['entry_point'] for sample in batch],
-                )
-            else:
-                batch_results = await self.pipelines[category].run_with_tool_api_call(
-                    [sample['prompt'] for sample in batch],
-                    [sample['response'] for sample in batch],
-                )
-            for result in batch_results:
-                outputs[index].update(result)
-                index += 1
-        
+import asyncio
+import copy
+
+from factool.knowledge_qa.pipeline import knowledge_qa_pipeline
+from factool.code.pipeline import code_pipeline
+from factool.math.pipeline import math_pipeline
+from factool.scientific.pipeline import scientific_pipeline
+
+class Factool():
+    def __init__(self, foundation_model):
+        self.pipelines = {
+                            "kbqa": knowledge_qa_pipeline(
+                                foundation_model, 10
+                            ),
+                            "code": code_pipeline(
+                                foundation_model, 3, 3
+                            ),
+                            "math": math_pipeline(
+                                foundation_model
+                            ),
+                            "scientific": scientific_pipeline(
+                                foundation_model
+                            ),
+                        }
+
+    def run(self, inputs):
+        outputs = copy.deepcopy(inputs)
+
+        batches = []
+        current_category = inputs[0]['category']
+        current_batch = []
+
+        for input in inputs:
+            if input['category'] == current_category:
+                current_batch.append(input)
+            else:
+                batches.append(current_batch)
+                current_batch = [input]
+                current_category = input['category']
+                    
+        batches.append(current_batch)  # append the last batch
+
+        index = 0
+        for batch in batches:
+            category = batch[0]['category']
+            if category == 'code':
+                batch_results = asyncio.run(
+                    self.pipelines[category].run_with_tool_api_call(
+                        [sample['prompt'] for sample in batch],
+                        [sample['response'] for sample in batch],
+                        [sample['entry_point'] for sample in batch]
+                    )
+                )
+            else:
+                batch_results = asyncio.run(
+                    self.pipelines[category].run_with_tool_api_call(
+                        [sample['prompt'] for sample in batch],
+                        [sample['response'] for sample in batch]
+                    )
+                )
+            for result in batch_results:
+                outputs[index].update(result)
+                index += 1
+        
+        return outputs
+
+    async def run_for_plugin(self, inputs):
+        outputs = copy.deepcopy(inputs)
+
+        batches = []
+        current_category = inputs[0]['category']
+        current_batch = []
+
+        for input in inputs:
+            if input['category'] == current_category:
+                current_batch.append(input)
+            else:
+                batches.append(current_batch)
+                current_batch = [input]
+                current_category = input['category']
+                    
+        batches.append(current_batch)  # append the last batch
+
+        index = 0
+        for batch in batches:
+            category = batch[0]['category']
+            if category == 'code':
+                batch_results = await self.pipelines[category].run_with_tool_api_call(
+                    [sample['prompt'] for sample in batch],
+                    [sample['response'] for sample in batch],
+                    [sample['entry_point'] for sample in batch],
+                )
+            else:
+                batch_results = await self.pipelines[category].run_with_tool_api_call(
+                    [sample['prompt'] for sample in batch],
+                    [sample['response'] for sample in batch],
+                )
+            for result in batch_results:
+                outputs[index].update(result)
+                index += 1
+        
         return outputs
```

### Comparing `factool-0.0.1/factool/knowledge_qa/google_serper.py` & `factool-0.0.7/factool/knowledge_qa/google_serper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# The following code was adapted from https://github.com/hwchase17/langchain/blob/master/langchain/utilities/google_serper.py
-
-"""Util that calls Google Search using the Serper.dev API."""
-import pdb
-import requests
-import asyncio
-import aiohttp
-import yaml
-
-from factool.env_config import factool_env_config
-
-# env
-serper_api_key = factool_env_config.serper_api_key
-
-
-class GoogleSerperAPIWrapper():
-    """Wrapper around the Serper.dev Google Search API.
-    You can create a free API key at https://serper.dev.
-    To use, you should have the environment variable ``SERPER_API_KEY``
-    set with your API key, or pass `serper_api_key` as a named parameter
-    to the constructor.
-    Example:
-        .. code-block:: python
-            from langchain import GoogleSerperAPIWrapper
-            google_serper = GoogleSerperAPIWrapper()
-    """
-    def __init__(self, snippet_cnt = 10) -> None:
-        self.k = snippet_cnt
-        self.gl = "us"
-        self.hl = "en"
-        self.serper_api_key = serper_api_key
-
-    async def _google_serper_search_results(self, session, search_term: str, gl: str, hl: str) -> dict:
-        headers = {
-            "X-API-KEY": self.serper_api_key or "",
-            "Content-Type": "application/json",
-        }
-        params = {"q": search_term, "gl": gl, "hl": hl}
-        async with session.post(
-            "https://google.serper.dev/search", headers=headers, params=params, raise_for_status=True
-        ) as response:
-            return await response.json()
-    
-    def _parse_results(self, results):
-        snippets = []
-
-        if results.get("answerBox"):
-            answer_box = results.get("answerBox", {})
-            if answer_box.get("answer"):
-                return [answer_box.get("answer")]
-            elif answer_box.get("snippet"):
-                return [answer_box.get("snippet").replace("\n", " ")]
-            elif answer_box.get("snippetHighlighted"):
-                return answer_box.get("snippetHighlighted")
-            
-        if results.get("knowledgeGraph"):
-            kg = results.get("knowledgeGraph", {})
-            title = kg.get("title")
-            entity_type = kg.get("type")
-            if entity_type:
-                snippets.append(f"{title}: {entity_type}.")
-            description = kg.get("description")
-            if description:
-                snippets.append(description)
-            for attribute, value in kg.get("attributes", {}).items():
-                snippets.append(f"{title} {attribute}: {value}.")
-
-        for result in results["organic"][: self.k]:
-            if "snippet" in result:
-                snippets.append(result["snippet"])
-            for attribute, value in result.get("attributes", {}).items():
-                snippets.append(f"{attribute}: {value}.")
-
-        if len(snippets) == 0:
-            return ["No good Google Search Result was found"]
-        
-        # keep only the first k snippets
-        snippets = snippets[:int(self.k / 2)]
-
-        return snippets
-    
-    async def parallel_searches(self, search_queries, gl, hl):
-        async with aiohttp.ClientSession() as session:
-            tasks = [self._google_serper_search_results(session, query, gl, hl) for query in search_queries]
-            search_results = await asyncio.gather(*tasks, return_exceptions=True)
-            return search_results
-
-    async def run(self, queries):
-        """Run query through GoogleSearch and parse result."""
-        flattened_queries = []
-
-        for sublist in queries:
-            if sublist is None:
-                sublist = ['None', 'None']
-            for item in sublist:
-                flattened_queries.append(item)
-
-        results = await self.parallel_searches(flattened_queries, gl=self.gl, hl=self.hl)
-        snippets = []
-        for i in range(len(results)):
-            snippets.append(self._parse_results(results[i]))
-        snippets_split = [snippets[i] + snippets[i+1] for i in range(0, len(snippets), 2)]
-        return snippets_split
-    
-if __name__ == "__main__":
-    search = GoogleSerperAPIWrapper()
+# The following code was adapted from https://github.com/hwchase17/langchain/blob/master/langchain/utilities/google_serper.py
+
+"""Util that calls Google Search using the Serper.dev API."""
+import pdb
+import requests
+import asyncio
+import aiohttp
+import yaml
+
+from factool.env_config import factool_env_config
+
+# env
+serper_api_key = factool_env_config.serper_api_key
+
+
+class GoogleSerperAPIWrapper():
+    """Wrapper around the Serper.dev Google Search API.
+    You can create a free API key at https://serper.dev.
+    To use, you should have the environment variable ``SERPER_API_KEY``
+    set with your API key, or pass `serper_api_key` as a named parameter
+    to the constructor.
+    Example:
+        .. code-block:: python
+            from langchain import GoogleSerperAPIWrapper
+            google_serper = GoogleSerperAPIWrapper()
+    """
+    def __init__(self, snippet_cnt = 10) -> None:
+        self.k = snippet_cnt
+        self.gl = "us"
+        self.hl = "en"
+        self.serper_api_key = serper_api_key
+
+    async def _google_serper_search_results(self, session, search_term: str, gl: str, hl: str) -> dict:
+        headers = {
+            "X-API-KEY": self.serper_api_key or "",
+            "Content-Type": "application/json",
+        }
+        params = {"q": search_term, "gl": gl, "hl": hl}
+        async with session.post(
+            "https://google.serper.dev/search", headers=headers, params=params, raise_for_status=True
+        ) as response:
+            return await response.json()
+    
+    def _parse_results(self, results):
+        snippets = []
+
+        if results.get("answerBox"):
+            answer_box = results.get("answerBox", {})
+            if answer_box.get("answer"):
+                return [answer_box.get("answer")]
+            elif answer_box.get("snippet"):
+                return [answer_box.get("snippet").replace("\n", " ")]
+            elif answer_box.get("snippetHighlighted"):
+                return answer_box.get("snippetHighlighted")
+            
+        if results.get("knowledgeGraph"):
+            kg = results.get("knowledgeGraph", {})
+            title = kg.get("title")
+            entity_type = kg.get("type")
+            if entity_type:
+                snippets.append(f"{title}: {entity_type}.")
+            description = kg.get("description")
+            if description:
+                snippets.append(description)
+            for attribute, value in kg.get("attributes", {}).items():
+                snippets.append(f"{title} {attribute}: {value}.")
+
+        for result in results["organic"][: self.k]:
+            if "snippet" in result:
+                snippets.append(result["snippet"])
+            for attribute, value in result.get("attributes", {}).items():
+                snippets.append(f"{attribute}: {value}.")
+
+        if len(snippets) == 0:
+            return ["No good Google Search Result was found"]
+        
+        # keep only the first k snippets
+        snippets = snippets[:int(self.k / 2)]
+
+        return snippets
+    
+    async def parallel_searches(self, search_queries, gl, hl):
+        async with aiohttp.ClientSession() as session:
+            tasks = [self._google_serper_search_results(session, query, gl, hl) for query in search_queries]
+            search_results = await asyncio.gather(*tasks, return_exceptions=True)
+            return search_results
+
+    async def run(self, queries):
+        """Run query through GoogleSearch and parse result."""
+        flattened_queries = []
+
+        for sublist in queries:
+            if sublist is None:
+                sublist = ['None', 'None']
+            for item in sublist:
+                flattened_queries.append(item)
+
+        results = await self.parallel_searches(flattened_queries, gl=self.gl, hl=self.hl)
+        snippets = []
+        for i in range(len(results)):
+            snippets.append(self._parse_results(results[i]))
+        snippets_split = [snippets[i] + snippets[i+1] for i in range(0, len(snippets), 2)]
+        return snippets_split
+    
+if __name__ == "__main__":
+    search = GoogleSerperAPIWrapper()
     print(search.run("What is the capital of the United States?"))
```

### Comparing `factool-0.0.1/factool/knowledge_qa/pipeline.py` & `factool-0.0.7/factool/knowledge_qa/pipeline.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-import json
-import yaml
-import os
-import time
-import math
-import pdb
-from typing import List, Dict
-
-from factool.knowledge_qa.tool import google_search
-from factool.utils.base.pipeline import pipeline
-
-class knowledge_qa_pipeline(pipeline):
-    def __init__(self, foundation_model, snippet_cnt):
-        super().__init__('knowledge_qa', foundation_model)
-
-        self.tool = google_search(snippet_cnt = snippet_cnt)
-
-        with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.claim_prompt = data['knowledge_qa']
-
-        with open(os.path.join(self.prompts_path, 'query_generation.yaml'), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.query_prompt = data['knowledge_qa']
-
-        with open(os.path.join(self.prompts_path, 'agreement_verification.yaml'), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.verification_prompt = data['knowledge_qa']
-    
-    async def _claim_extraction(self, responses):
-        messages_list = [
-            [
-                {"role": "system", "content": self.claim_prompt['system']},
-                {"role": "user", "content": self.claim_prompt['user'].format(input=response)},
-            ]
-            for response in responses
-        ]
-        return await self.chat.async_run(messages_list, List)
-    
-    async def _query_generation(self, claims):
-        if claims == None:
-            return ['None']
-        messages_list = [
-            [
-                {"role": "system", "content": self.query_prompt['system']},
-                {"role": "user", "content": self.query_prompt['user'].format(input=claim['claim'] if 'claim' in claim else '')},
-            ]
-            for claim in claims
-        ]
-        return await self.chat.async_run(messages_list, List)
-
-    async def _verification(self, claims, evidences):
-        messages_list = [
-            [
-                {"role": "system", "content": self.verification_prompt['system']},
-                {"role": "user", "content": self.verification_prompt['user'].format(claim=claim['claim'], evidence=str(evidence))},
-            ]
-            for claim, evidence in zip(claims, evidences)
-        ]
-        return await self.chat.async_run(messages_list, Dict)
-    
-    async def run_with_tool_live(self, responses):
-        claims_in_responses = await self._claim_extraction(responses)
-        queries_in_responses = []
-        evidences_in_responses = []
-        verifications_in_responses = []
-        for claims_in_response in claims_in_responses:
-            queries = await self._query_generation(claims_in_response)
-            queries_in_responses.append(queries)
-            evidences = await self.tool.run(queries)
-            evidences_in_responses.append(evidences)
-            verifications = await self._verification(claims_in_response, evidences)
-            verifications_in_responses.append(verifications)
-
-        return claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses
-    
-    async def run_with_tool_live_without_claim_extraction(self, claims):
-        queries = await self._query_generation(claims)
-        evidences = await self.tool.run(queries)
-
-        final_response = await self._verification(claims, evidences)
-        for i in range(len(final_response)):
-            if final_response[i] != None:
-                final_response[i]['queries'] = queries[i]
-                final_response[i]['evidences'] = evidences[i]
-
-        return final_response
-    
-    async def run_with_tool_api_call(self, prompts, responses):
-        batch_size = 5
-        num_batches = math.ceil(len(prompts) / batch_size)
-
-        self.sample_list = [{"prompt": prompt, "response": response, "category": 'kbqa'} for prompt, response in zip(prompts, responses)]
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(responses))
-
-            claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses = await self.run_with_tool_live(responses[batch_start:batch_end])
-
-            for j, (claims_in_response, queries_in_response, evidences_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses)):
-                index = batch_start + j
-                
-                if claims_in_response != None:
-                    for k, claim in enumerate(claims_in_response):
-                        if verifications_in_response[k] != None:
-                            if claim != None:
-                                verifications_in_response[k].update({'claim': claim['claim']})
-                            else:
-                                verifications_in_response[k].update({'claim': 'None'})
-
-                self.sample_list[index].update({
-                    'claims': claims_in_response,
-                    'queries': queries_in_response,
-                    'evidences': evidences_in_response,
-                    'claim_level_factuality': verifications_in_response,
-                    'response_level_factuality': all([verification['factuality'] if verification != None else True for verification in verifications_in_response])
-                })
-
-        return self.sample_list
-    
-    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
-        data_path = with_tool_classified_dataset_path if rerun else annotated_dataset_path
-        with open(data_path, 'r') as f:
-            data = [json.loads(line) for line in f]
-        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
-        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 4
-        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
-        
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(rerun_elements))
-
-            responses = await self.run_with_tool_live_without_claim_extraction(rerun_elements[batch_start:batch_end])
-
-            for j, response in enumerate(responses):
-                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
-                if response is None:
-                    self.sample_list[index].update({
-                        'with_tool_classification': 'None',
-                        'with_tool_reasoning': 'None',
-                        'queries': 'None',
-                        'evidences': 'None'
-                    })
-                else:
-                    self.sample_list[index].update({
-                        'with_tool_classification': response.get('factuality', 'None'),
-                        'with_tool_reasoning': response.get('reasoning', 'None'),
-                        'queries': response.get('queries', 'None'),
-                        'evidences': response.get('evidences', 'None')
-                    })
-        
-            # save everything after each batch to prevent data loss
-            with open(with_tool_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    json_str = json.dumps(item)
-                    f.write(json_str + '\n')
-
-    async def run_self_check_live(self, fewshot, batch):
-        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
-        messages_list = [
-            [
-                {"role": "system", "content": self.self_check_prompt['system']},
-                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(claim=response['claim'])},
-            ]
-            for response in batch
-        ]
-        return await self.chat.async_run(messages_list, Dict)
-
-    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
-        data_path = annotated_dataset_path if not rerun else self_check_classified_dataset_path
-        with open(data_path, 'r') as f:
-            data = [json.loads(line) for line in f]
-        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
-        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 10
-        num_batches = math.ceil(len(rerun_elements) / batch_size)
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(rerun_elements))
-            batch = rerun_elements[batch_start:batch_end]
-
-            responses = await self.run_self_check_live(fewshot, batch)
-            for j, response in enumerate(responses):
-                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
-                if response is None:
-                    self.sample_list[index].update({
-                        'self_check_classification': 'None',
-                        'self_check_reasoning': 'None'
-                    })
-                else:
-                    self.sample_list[index].update({
-                        'self_check_classification': response.get('factuality', 'None'),
-                        'self_check_reasoning': response.get('reasoning', 'None')
-                    })
-
-            # save everything after each batch to prevent data loss
-            with open(self_check_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    json_str = json.dumps(item)
+import json
+import yaml
+import os
+import time
+import math
+import pdb
+from typing import List, Dict
+
+from factool.knowledge_qa.tool import google_search
+from factool.utils.base.pipeline import pipeline
+
+class knowledge_qa_pipeline(pipeline):
+    def __init__(self, foundation_model, snippet_cnt):
+        super().__init__('knowledge_qa', foundation_model)
+
+        self.tool = google_search(snippet_cnt = snippet_cnt)
+
+        with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.claim_prompt = data['knowledge_qa']
+
+        with open(os.path.join(self.prompts_path, 'query_generation.yaml'), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.query_prompt = data['knowledge_qa']
+
+        with open(os.path.join(self.prompts_path, 'agreement_verification.yaml'), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.verification_prompt = data['knowledge_qa']
+    
+    async def _claim_extraction(self, responses):
+        messages_list = [
+            [
+                {"role": "system", "content": self.claim_prompt['system']},
+                {"role": "user", "content": self.claim_prompt['user'].format(input=response)},
+            ]
+            for response in responses
+        ]
+        return await self.chat.async_run(messages_list, List)
+    
+    async def _query_generation(self, claims):
+        if claims == None:
+            return ['None']
+        messages_list = [
+            [
+                {"role": "system", "content": self.query_prompt['system']},
+                {"role": "user", "content": self.query_prompt['user'].format(input=claim['claim'] if 'claim' in claim else '')},
+            ]
+            for claim in claims
+        ]
+        return await self.chat.async_run(messages_list, List)
+
+    async def _verification(self, claims, evidences):
+        messages_list = [
+            [
+                {"role": "system", "content": self.verification_prompt['system']},
+                {"role": "user", "content": self.verification_prompt['user'].format(claim=claim['claim'], evidence=str(evidence))},
+            ]
+            for claim, evidence in zip(claims, evidences)
+        ]
+        return await self.chat.async_run(messages_list, Dict)
+    
+    async def run_with_tool_live(self, responses):
+        claims_in_responses = await self._claim_extraction(responses)
+        queries_in_responses = []
+        evidences_in_responses = []
+        verifications_in_responses = []
+        for claims_in_response in claims_in_responses:
+            queries = await self._query_generation(claims_in_response)
+            queries_in_responses.append(queries)
+            evidences = await self.tool.run(queries)
+            evidences_in_responses.append(evidences)
+            verifications = await self._verification(claims_in_response, evidences)
+            verifications_in_responses.append(verifications)
+
+        return claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses
+    
+    async def run_with_tool_live_without_claim_extraction(self, claims):
+        queries = await self._query_generation(claims)
+        evidences = await self.tool.run(queries)
+
+        final_response = await self._verification(claims, evidences)
+        for i in range(len(final_response)):
+            if final_response[i] != None:
+                final_response[i]['queries'] = queries[i]
+                final_response[i]['evidences'] = evidences[i]
+
+        return final_response
+    
+    async def run_with_tool_api_call(self, prompts, responses):
+        batch_size = 5
+        num_batches = math.ceil(len(prompts) / batch_size)
+
+        self.sample_list = [{"prompt": prompt, "response": response, "category": 'kbqa'} for prompt, response in zip(prompts, responses)]
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(responses))
+
+            claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses = await self.run_with_tool_live(responses[batch_start:batch_end])
+
+            for j, (claims_in_response, queries_in_response, evidences_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses)):
+                index = batch_start + j
+                
+                if claims_in_response != None:
+                    for k, claim in enumerate(claims_in_response):
+                        if verifications_in_response[k] != None:
+                            if claim != None:
+                                verifications_in_response[k].update({'claim': claim['claim']})
+                            else:
+                                verifications_in_response[k].update({'claim': 'None'})
+
+                self.sample_list[index].update({
+                    'claims': claims_in_response,
+                    'queries': queries_in_response,
+                    'evidences': evidences_in_response,
+                    'claim_level_factuality': verifications_in_response,
+                    'response_level_factuality': all([verification['factuality'] if verification != None else True for verification in verifications_in_response])
+                })
+
+        return self.sample_list
+    
+    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
+        data_path = with_tool_classified_dataset_path if rerun else annotated_dataset_path
+        with open(data_path, 'r') as f:
+            data = [json.loads(line) for line in f]
+        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
+        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 4
+        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
+        
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(rerun_elements))
+
+            responses = await self.run_with_tool_live_without_claim_extraction(rerun_elements[batch_start:batch_end])
+
+            for j, response in enumerate(responses):
+                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
+                if response is None:
+                    self.sample_list[index].update({
+                        'with_tool_classification': 'None',
+                        'with_tool_reasoning': 'None',
+                        'queries': 'None',
+                        'evidences': 'None'
+                    })
+                else:
+                    self.sample_list[index].update({
+                        'with_tool_classification': response.get('factuality', 'None'),
+                        'with_tool_reasoning': response.get('reasoning', 'None'),
+                        'queries': response.get('queries', 'None'),
+                        'evidences': response.get('evidences', 'None')
+                    })
+        
+            # save everything after each batch to prevent data loss
+            with open(with_tool_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    json_str = json.dumps(item)
+                    f.write(json_str + '\n')
+
+    async def run_self_check_live(self, fewshot, batch):
+        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
+        messages_list = [
+            [
+                {"role": "system", "content": self.self_check_prompt['system']},
+                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(claim=response['claim'])},
+            ]
+            for response in batch
+        ]
+        return await self.chat.async_run(messages_list, Dict)
+
+    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
+        data_path = annotated_dataset_path if not rerun else self_check_classified_dataset_path
+        with open(data_path, 'r') as f:
+            data = [json.loads(line) for line in f]
+        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
+        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 10
+        num_batches = math.ceil(len(rerun_elements) / batch_size)
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(rerun_elements))
+            batch = rerun_elements[batch_start:batch_end]
+
+            responses = await self.run_self_check_live(fewshot, batch)
+            for j, response in enumerate(responses):
+                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
+                if response is None:
+                    self.sample_list[index].update({
+                        'self_check_classification': 'None',
+                        'self_check_reasoning': 'None'
+                    })
+                else:
+                    self.sample_list[index].update({
+                        'self_check_classification': response.get('factuality', 'None'),
+                        'self_check_reasoning': response.get('reasoning', 'None')
+                    })
+
+            # save everything after each batch to prevent data loss
+            with open(self_check_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    json_str = json.dumps(item)
                     f.write(json_str + '\n')
```

### Comparing `factool-0.0.1/factool/math/pipeline.py` & `factool-0.0.7/factool/math/pipeline.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-import json
-import math
-import os
-from typing import List, Dict
-import yaml
-import pdb
-
-from factool.math.tool import python_executor
-from factool.utils.base.pipeline import pipeline
-
-class math_pipeline(pipeline):
-    def __init__(self, foundation_model):
-        super().__init__('math', foundation_model)
-
-        self.tool = python_executor()
-
-        with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.claim_prompt = data['math']
-
-        with open(os.path.join(self.prompts_path, 'query_generation.yaml'), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.query_prompt = data['math']
-
-    def _verification(self, exec_results):
-        classification_results = [True for _ in range(len(exec_results))]
-        for i in range(len(exec_results)):
-            if exec_results[i] is not None and 'False' in exec_results[i]:
-                classification_results[i] = False
-        
-        return classification_results
-
-    async def _claim_extraction(self, samples):
-        messages_list = [
-            [
-                {"role": "system", "content": self.claim_prompt['system']},
-                {"role": "user", "content": self.claim_prompt['user'].format(input_question=sample['prompt'], input_solution=sample['response'])},
-            ]
-            for sample in samples
-        ]
-        return await self.chat.async_run(messages_list, List)
-    
-    async def _query_generation(self, claims):
-        messages_list = [
-            [
-                {"role": "system", "content": self.query_prompt['system']},
-                {"role": "user", "content": self.query_prompt['user'].format(math_calculation=claim['math_calculation'], calculated_answer=claim['calculated_answer'])},
-            ]
-            for claim in claims
-        ]
-        return await self.chat.async_run(messages_list, Dict)
-    
-    async def run_with_tool_live(self, samples):
-        claims_in_responses = await self._claim_extraction(samples)
-        queries_in_responses = []
-        exec_results_in_responses = []
-        verifications_in_responses = []
-        for claims_in_response in claims_in_responses:
-            queries = await self._query_generation(claims_in_response)
-            queries_in_responses.append(queries)
-            exec_results = []
-            for query in queries:
-                try:
-                    exec_results.append(self.tool.run(query['python_snippet']))
-                except:
-                    exec_results.append('None')
-            exec_results_in_responses.append(exec_results)
-            verifications = self._verification(exec_results)
-            verifications_in_responses.append(verifications)
-
-        return claims_in_responses, queries_in_responses, exec_results_in_responses, verifications_in_responses
-    
-    async def run_with_tool_live_without_claim_extraction(self, claims):
-        queries = await self._query_generation(claims)
-
-        exec_results = []
-        for query in queries:
-            try:
-                exec_results.append(self.tool.run(query['python_snippet']))
-            except:
-                exec_results.append(None)
-        classification_results = self._verification(exec_results)
-        return queries, exec_results, classification_results
-    
-    async def run_with_tool_api_call(self, prompts, responses):
-        batch_size = 5
-        num_batches = math.ceil(len(prompts) / batch_size)
-
-        self.sample_list = [{"prompt": prompt, "response": response, "category": 'math'} for prompt, response in zip(prompts, responses)]
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(responses))
-
-            claims_in_responses, queries_in_responses, exec_results_in_response, verifications_in_responses = await self.run_with_tool_live(self.sample_list[batch_start: batch_end])
-
-            for j, (claims_in_response, queries_in_response, exec_results_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, exec_results_in_response, verifications_in_responses)):
-                index = batch_start + j
-
-                self.sample_list[index].update({
-                    'claims': claims_in_response,
-                    'queries': queries_in_response,
-                    'execution_results': exec_results_in_response,
-                    'claim_level_factuality': verifications_in_response,
-                    'response_level_factuality': all([verification if verification != None else True for verification in verifications_in_response])
-                })
-
-        return self.sample_list
-
-    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
-        data_path = annotated_dataset_path if not rerun else with_tool_classified_dataset_path
-        with open(data_path, 'r') as f:
-            data = [json.loads(line) for line in f]
-        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
-        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 10
-        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
-
-        for i in range(num_batches):
-            print("test1")
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(rerun_elements))
-            batch = rerun_elements[batch_start:batch_end]
-
-            queries, exec_results, classification_results = await self.run_with_tool_live_without_claim_extraction(batch)
-
-            for j, (query, exec_result, classification_result) in enumerate(zip(queries, exec_results, classification_results)):
-                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
-                self.sample_list[index].update({
-                    'query': query,
-                    'exec_result': exec_result,
-                    'with_tool_classification': classification_result,
-                })
-        
-            # save everything after each batch to prevent data loss
-            with open(with_tool_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    try:
-                        json_str = json.dumps(item)
-                    except:
-                        continue
-                    f.write(json_str + '\n')
-
-    async def run_self_check_live(self, fewshot, batch):
-        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
-        messages_list = [
-            [
-                {"role": "system", "content": self.self_check_prompt['system']},
-                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(input_calculation=response['math_calculation'], input_calculated_answer=response['calculated_answer'])},
-            ]
-            for response in batch
-        ]
-        return await self.chat.async_run(messages_list, Dict)
-
-    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
-        data_path = annotated_dataset_path if not rerun else self_check_classified_dataset_path
-        with open(data_path, 'r') as f:
-            data = [json.loads(line) for line in f]
-        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
-        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 10
-        num_batches = math.ceil(len(rerun_elements) / batch_size)
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(rerun_elements))
-            batch = rerun_elements[batch_start:batch_end]
-
-            responses = await self.run_self_check_live(fewshot, batch)
-            for j, response in enumerate(responses):
-                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
-                if response is None:
-                    self.sample_list[index].update({
-                        'self_check_classification': 'None',
-                        'self_check_reasoning': 'None'
-                    })
-                else:
-                    self.sample_list[index].update({
-                        'self_check_classification': response.get('factuality', 'None'),
-                        'self_check_reasoning': response.get('reasoning', 'None')
-                    })
-
-            # save everything after each batch to prevent data loss
-            with open(self_check_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    json_str = json.dumps(item)
+import json
+import math
+import os
+from typing import List, Dict
+import yaml
+import pdb
+
+from factool.math.tool import python_executor
+from factool.utils.base.pipeline import pipeline
+
+class math_pipeline(pipeline):
+    def __init__(self, foundation_model):
+        super().__init__('math', foundation_model)
+
+        self.tool = python_executor()
+
+        with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.claim_prompt = data['math']
+
+        with open(os.path.join(self.prompts_path, 'query_generation.yaml'), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.query_prompt = data['math']
+
+    def _verification(self, exec_results):
+        classification_results = [True for _ in range(len(exec_results))]
+        for i in range(len(exec_results)):
+            if exec_results[i] is not None and 'False' in exec_results[i]:
+                classification_results[i] = False
+        
+        return classification_results
+
+    async def _claim_extraction(self, samples):
+        messages_list = [
+            [
+                {"role": "system", "content": self.claim_prompt['system']},
+                {"role": "user", "content": self.claim_prompt['user'].format(input_question=sample['prompt'], input_solution=sample['response'])},
+            ]
+            for sample in samples
+        ]
+        return await self.chat.async_run(messages_list, List)
+    
+    async def _query_generation(self, claims):
+        messages_list = [
+            [
+                {"role": "system", "content": self.query_prompt['system']},
+                {"role": "user", "content": self.query_prompt['user'].format(math_calculation=claim['math_calculation'], calculated_answer=claim['calculated_answer'])},
+            ]
+            for claim in claims
+        ]
+        return await self.chat.async_run(messages_list, Dict)
+    
+    async def run_with_tool_live(self, samples):
+        claims_in_responses = await self._claim_extraction(samples)
+        queries_in_responses = []
+        exec_results_in_responses = []
+        verifications_in_responses = []
+        for claims_in_response in claims_in_responses:
+            queries = await self._query_generation(claims_in_response)
+            queries_in_responses.append(queries)
+            exec_results = []
+            for query in queries:
+                try:
+                    exec_results.append(self.tool.run(query['python_snippet']))
+                except:
+                    exec_results.append('None')
+            exec_results_in_responses.append(exec_results)
+            verifications = self._verification(exec_results)
+            verifications_in_responses.append(verifications)
+
+        return claims_in_responses, queries_in_responses, exec_results_in_responses, verifications_in_responses
+    
+    async def run_with_tool_live_without_claim_extraction(self, claims):
+        queries = await self._query_generation(claims)
+
+        exec_results = []
+        for query in queries:
+            try:
+                exec_results.append(self.tool.run(query['python_snippet']))
+            except:
+                exec_results.append(None)
+        classification_results = self._verification(exec_results)
+        return queries, exec_results, classification_results
+    
+    async def run_with_tool_api_call(self, prompts, responses):
+        batch_size = 5
+        num_batches = math.ceil(len(prompts) / batch_size)
+
+        self.sample_list = [{"prompt": prompt, "response": response, "category": 'math'} for prompt, response in zip(prompts, responses)]
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(responses))
+
+            claims_in_responses, queries_in_responses, exec_results_in_response, verifications_in_responses = await self.run_with_tool_live(self.sample_list[batch_start: batch_end])
+
+            for j, (claims_in_response, queries_in_response, exec_results_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, exec_results_in_response, verifications_in_responses)):
+                index = batch_start + j
+
+                self.sample_list[index].update({
+                    'claims': claims_in_response,
+                    'queries': queries_in_response,
+                    'execution_results': exec_results_in_response,
+                    'claim_level_factuality': verifications_in_response,
+                    'response_level_factuality': all([verification if verification != None else True for verification in verifications_in_response])
+                })
+
+        return self.sample_list
+
+    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
+        data_path = annotated_dataset_path if not rerun else with_tool_classified_dataset_path
+        with open(data_path, 'r') as f:
+            data = [json.loads(line) for line in f]
+        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
+        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 10
+        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
+
+        for i in range(num_batches):
+            print("test1")
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(rerun_elements))
+            batch = rerun_elements[batch_start:batch_end]
+
+            queries, exec_results, classification_results = await self.run_with_tool_live_without_claim_extraction(batch)
+
+            for j, (query, exec_result, classification_result) in enumerate(zip(queries, exec_results, classification_results)):
+                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
+                self.sample_list[index].update({
+                    'query': query,
+                    'exec_result': exec_result,
+                    'with_tool_classification': classification_result,
+                })
+        
+            # save everything after each batch to prevent data loss
+            with open(with_tool_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    try:
+                        json_str = json.dumps(item)
+                    except:
+                        continue
+                    f.write(json_str + '\n')
+
+    async def run_self_check_live(self, fewshot, batch):
+        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
+        messages_list = [
+            [
+                {"role": "system", "content": self.self_check_prompt['system']},
+                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(input_calculation=response['math_calculation'], input_calculated_answer=response['calculated_answer'])},
+            ]
+            for response in batch
+        ]
+        return await self.chat.async_run(messages_list, Dict)
+
+    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
+        data_path = annotated_dataset_path if not rerun else self_check_classified_dataset_path
+        with open(data_path, 'r') as f:
+            data = [json.loads(line) for line in f]
+        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
+        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 10
+        num_batches = math.ceil(len(rerun_elements) / batch_size)
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(rerun_elements))
+            batch = rerun_elements[batch_start:batch_end]
+
+            responses = await self.run_self_check_live(fewshot, batch)
+            for j, response in enumerate(responses):
+                index = batch_start + j if not rerun else rerun_indices[batch_start + j]
+                if response is None:
+                    self.sample_list[index].update({
+                        'self_check_classification': 'None',
+                        'self_check_reasoning': 'None'
+                    })
+                else:
+                    self.sample_list[index].update({
+                        'self_check_classification': response.get('factuality', 'None'),
+                        'self_check_reasoning': response.get('reasoning', 'None')
+                    })
+
+            # save everything after each batch to prevent data loss
+            with open(self_check_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    json_str = json.dumps(item)
                     f.write(json_str + '\n')
```

### Comparing `factool-0.0.1/factool/math/tool.py` & `factool-0.0.7/factool/math/tool.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import sys
-import io
-import yaml
-import pdb
-
-class python_executor:
-    def __init__(self):
-        pass
-
-    def run_single(self, program):
-        buffer = io.StringIO() # Create an in-memory buffer for the output
-        stdout = sys.stdout # Save the original standard output
-        sys.stdout = buffer # Redirect the standard output to the buffer
-        try:
-            exec(program)
-        except Exception as e:
-            # Handle the error here
-            error_message = str(e)
-            sys.stdout = stdout  # Restore the original standard output
-            return error_message
-
-        exec(program)
-        sys.stdout = stdout # Restore the original standard output
-        output = buffer.getvalue() # Get the output from the buffer
-        return output
-
-    def run(self, snippet):
-        if snippet == None:
-            return None
-        exec_result = self.run_single(snippet)
-        if exec_result and 'False' in exec_result:
-            exec_result = 'False'
-        else:
-            exec_result = 'True'
+import sys
+import io
+import yaml
+import pdb
+
+class python_executor:
+    def __init__(self):
+        pass
+
+    def run_single(self, program):
+        buffer = io.StringIO() # Create an in-memory buffer for the output
+        stdout = sys.stdout # Save the original standard output
+        sys.stdout = buffer # Redirect the standard output to the buffer
+        try:
+            exec(program)
+        except Exception as e:
+            # Handle the error here
+            error_message = str(e)
+            sys.stdout = stdout  # Restore the original standard output
+            return error_message
+
+        exec(program)
+        sys.stdout = stdout # Restore the original standard output
+        output = buffer.getvalue() # Get the output from the buffer
+        return output
+
+    def run(self, snippet):
+        if snippet == None:
+            return None
+        exec_result = self.run_single(snippet)
+        if exec_result and 'False' in exec_result:
+            exec_result = 'False'
+        else:
+            exec_result = 'True'
         return exec_result
```

### Comparing `factool-0.0.1/factool/scientific/pipeline.py` & `factool-0.0.7/factool/scientific/pipeline.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import time
-import json
-import math
-import os
-import yaml
-from typing import Dict, List
-
-from factool.scientific.tool import google_scholar
-from factool.utils.base.pipeline import pipeline
-
-class scientific_pipeline(pipeline):
-    def __init__(self, foundation_model):
-        super().__init__('scientific', foundation_model)
-
-        self.tool = google_scholar()
-
-        with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.claim_prompt = data['scientific']
-
-        with open(os.path.join(self.prompts_path, 'agreement_verification.yaml'), 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        self.verification_prompt = data['scientific']
-
-    async def _claim_extraction(self, responses):
-        messages_list = [
-            [
-                {"role": "system", "content": self.claim_prompt['system']},
-                {"role": "user", "content": self.claim_prompt['user'].format(input=response)},
-            ]
-            for response in responses
-        ]
-        return await self.chat.async_run(messages_list, List)
-    
-    async def _check_authors(self, authors):
-        messages_list = [
-            [
-                {"role": "system", "content": self.verification_prompt['system']},
-                {"role": "user", "content": self.verification_prompt['user'].format(string1=claim_author, list2=real_author)},
-            ]
-            for claim_author, real_author in authors
-        ]
-
-        return await self.chat.async_run(messages_list, Dict)
-
-    async def _verification(self, claims, responses):
-        authors = [(claim['paper_author(s)'], response['author']) for claim, response in zip(claims, responses)]
-        check_authors_results = await self._check_authors(authors)
-        final_responses = []
-        for i, (claim, response) in enumerate(zip(claims, responses)):
-            final_response = {
-                'generated_paper_title': claim['paper_title'],
-                'generated_paper_author(s)': claim['paper_author(s)'],
-                'generated_paper_pub_year': claim['paper_pub_year'],
-                'actual_paper_title': response['title'],
-                'actual_paper_author(s)': response['author'],
-                'actual_paper_pub_year': response['pub_year'],
-            }
-
-            errors = []
-            if final_response['generated_paper_title'].lower() != final_response['actual_paper_title'].lower() and final_response['generated_paper_title'].lower() not in final_response['actual_paper_title'].lower() and final_response['actual_paper_title'].lower() not in final_response['generated_paper_title'].lower() :
-                errors.append('wrong_paper_title')
-            if check_authors_results[i]['factuality'] == False:
-                errors.append('wrong_paper_author(s)')
-            if final_response['generated_paper_pub_year'] != final_response['actual_paper_pub_year']:
-                errors.append('wrong_paper_pub_year')
-
-            final_response['error'] = errors
-            final_response['factuality'] = len(errors) == 0
-
-            final_responses.append(final_response)
-
-        return final_responses
-
-    async def run_with_tool_live(self, samples):
-        claims_in_responses = await self._claim_extraction(samples)
-        queries_in_responses = []
-        evidences_in_responses = []
-        verifications_in_responses = []
-        for claims_in_response in claims_in_responses:
-            queries = [claim['paper_title'] for claim in claims_in_response]
-            queries_in_responses.append(queries)
-            evidences = [self.tool.run(paper_title) for paper_title in queries]
-            evidences_in_responses.append(evidences)
-            verifications = await self._verification(claims_in_response, evidences)
-            verifications_in_responses.append(verifications)
-
-        return claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses
-        
-    async def run_with_tool_live_without_claim_extraction(self, claims):
-        # claims = [{"paper_title": "A Survey of Modern Authorship Attribution Methods", "paper_author(s)": "Stamatatos, Efstathios", "paper_pub_year": "2013"}, {"paper_title": "BERT", "paper_author(s)": "John Smith", "paper_pub_year": "2020"}]
-        papers_titles = [claim['paper_title'] for claim in claims]
-        responses = [self.tool.run(paper_title) for paper_title in papers_titles]
-        final_response = await self._verification(claims, responses)
-        return final_response
-
-    async def run_with_tool_api_call(self, prompts, responses):
-        batch_size = 5
-        num_batches = math.ceil(len(prompts) / batch_size)
-
-        self.sample_list = [{"prompt": prompt, "response": response, "category": 'scientific'} for prompt, response in zip(prompts, responses)]
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(responses))
-
-            claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses = await self.run_with_tool_live(responses[batch_start:batch_end])
-
-            for j, (claims_in_response, queries_in_response, evidences_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses)):
-                index = batch_start + j
-
-                self.sample_list[index].update({
-                    'claims': claims_in_response,
-                    'queries': queries_in_response,
-                    'evidences': evidences_in_response,
-                    'claim_level_factuality': verifications_in_response,
-                    'response_level_factuality': all([verification['factuality'] if verification != None else True for verification in verifications_in_response])
-                })
-        return self.sample_list
-
-    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
-        # Example of a line: 
-        # {"paper_title": "A Survey of Modern Authorship Attribution Methods", "paper_author(s)": "Stamatatos, Efstathios", "paper_pub_year": "2013", "label": True / False}
-        if rerun == False:
-            with open(annotated_dataset_path, 'r') as f:
-                data = [json.loads(line) for line in f]
-            self.sample_list = [claim for sample in data for claim in sample['claims']]
-            rerun_elements = self.sample_list
-        else:
-            with open(with_tool_classified_dataset_path, 'r') as f:
-                data = [json.loads(line) for line in f]
-            self.sample_list = data
-            rerun_elements = [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 5
-        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = (i + 1) * batch_size if (i + 1) * batch_size < len(rerun_elements) else len(rerun_elements)
-
-            responses = await self.run_with_tool_live_without_claim_extraction(rerun_elements[batch_start:batch_end])
-            for j, response in enumerate(responses):
-                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
-                if response == None:
-                    self.sample_list[index]['with_tool_classification'] = 'None'
-                    self.sample_list[index]['error'] = 'None'
-                else:
-                    self.sample_list[index]['with_tool_classification'] = response.get('factuality', 'None')
-                    self.sample_list[index]['error'] = response.get('error', 'None')
-        
-            # save everything after each batch to prevent data loss
-            with open(with_tool_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    json_str = json.dumps(item)
-                    f.write(json_str + '\n')
-
-    async def run_self_check_live(self, fewshot, batch):
-        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
-        messages_list = [
-            [
-                {"role": "system", "content": self.self_check_prompt['system']},
-                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(scientific_literature=response)}
-            ]
-            for response in batch
-        ]
-        return await self.chat.async_run(messages_list, Dict)
-
-    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
-        # Example of a line: 
-        # {"paper_title": "A Survey of Modern Authorship Attribution Methods", "paper_author(s)": "Stamatatos, Efstathios", "paper_pub_year": "2013", "annotation": True / False}
-        data_path = annotated_dataset_path if not rerun else self_check_classified_dataset_path
-        with open(data_path, 'r') as f:
-            data = [json.loads(line) for line in f]
-        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
-        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
-
-        batch_size = 5
-        num_batches = math.ceil(len(rerun_elements) / batch_size)
-
-        for i in range(num_batches):
-            print(i)
-            batch_start = i * batch_size
-            batch_end = (i + 1) * batch_size
-            batch = rerun_elements[batch_start:batch_end]
-            batch = [{k:v for k,v in d.items() if k != "label"} for d in batch]
-
-            responses = await self.run_self_check_live(fewshot, batch)
-            for j, response in enumerate(responses):
-                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
-                if response == None:
-                    self.sample_list[index]['self_check_classification'] = 'None'
-                    self.sample_list[index]['self_check_reasoning'] = 'None'
-                else:
-                    self.sample_list[index]['self_check_classification'] = response.get('factuality', 'None')
-                    self.sample_list[index]['self_check_reasoning'] = response.get('reasoning', 'None')
-        
-            # save everything after each batch to prevent data loss
-            with open(self_check_classified_dataset_path, 'w') as f:
-                for item in self.sample_list:
-                    json_str = json.dumps(item)
+import time
+import json
+import math
+import os
+import yaml
+from typing import Dict, List
+
+from factool.scientific.tool import google_scholar
+from factool.utils.base.pipeline import pipeline
+
+class scientific_pipeline(pipeline):
+    def __init__(self, foundation_model):
+        super().__init__('scientific', foundation_model)
+
+        self.tool = google_scholar()
+
+        with open(os.path.join(self.prompts_path, "claim_extraction.yaml"), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.claim_prompt = data['scientific']
+
+        with open(os.path.join(self.prompts_path, 'agreement_verification.yaml'), 'r') as file:
+            data = yaml.load(file, Loader=yaml.FullLoader)
+        self.verification_prompt = data['scientific']
+
+    async def _claim_extraction(self, responses):
+        messages_list = [
+            [
+                {"role": "system", "content": self.claim_prompt['system']},
+                {"role": "user", "content": self.claim_prompt['user'].format(input=response)},
+            ]
+            for response in responses
+        ]
+        return await self.chat.async_run(messages_list, List)
+    
+    async def _check_authors(self, authors):
+        messages_list = [
+            [
+                {"role": "system", "content": self.verification_prompt['system']},
+                {"role": "user", "content": self.verification_prompt['user'].format(string1=claim_author, list2=real_author)},
+            ]
+            for claim_author, real_author in authors
+        ]
+
+        return await self.chat.async_run(messages_list, Dict)
+
+    async def _verification(self, claims, responses):
+        authors = [(claim['paper_author(s)'], response['author']) for claim, response in zip(claims, responses)]
+        check_authors_results = await self._check_authors(authors)
+        final_responses = []
+        for i, (claim, response) in enumerate(zip(claims, responses)):
+            final_response = {
+                'generated_paper_title': claim['paper_title'],
+                'generated_paper_author(s)': claim['paper_author(s)'],
+                'generated_paper_pub_year': claim['paper_pub_year'],
+                'actual_paper_title': response['title'],
+                'actual_paper_author(s)': response['author'],
+                'actual_paper_pub_year': response['pub_year'],
+            }
+
+            errors = []
+            if final_response['generated_paper_title'].lower() != final_response['actual_paper_title'].lower() and final_response['generated_paper_title'].lower() not in final_response['actual_paper_title'].lower() and final_response['actual_paper_title'].lower() not in final_response['generated_paper_title'].lower() :
+                errors.append('wrong_paper_title')
+            if check_authors_results[i]['factuality'] == False:
+                errors.append('wrong_paper_author(s)')
+            if final_response['generated_paper_pub_year'] != final_response['actual_paper_pub_year']:
+                errors.append('wrong_paper_pub_year')
+
+            final_response['error'] = errors
+            final_response['factuality'] = len(errors) == 0
+
+            final_responses.append(final_response)
+
+        return final_responses
+
+    async def run_with_tool_live(self, samples):
+        claims_in_responses = await self._claim_extraction(samples)
+        queries_in_responses = []
+        evidences_in_responses = []
+        verifications_in_responses = []
+        for claims_in_response in claims_in_responses:
+            queries = [claim['paper_title'] for claim in claims_in_response]
+            queries_in_responses.append(queries)
+            evidences = [self.tool.run(paper_title) for paper_title in queries]
+            evidences_in_responses.append(evidences)
+            verifications = await self._verification(claims_in_response, evidences)
+            verifications_in_responses.append(verifications)
+
+        return claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses
+        
+    async def run_with_tool_live_without_claim_extraction(self, claims):
+        # claims = [{"paper_title": "A Survey of Modern Authorship Attribution Methods", "paper_author(s)": "Stamatatos, Efstathios", "paper_pub_year": "2013"}, {"paper_title": "BERT", "paper_author(s)": "John Smith", "paper_pub_year": "2020"}]
+        papers_titles = [claim['paper_title'] for claim in claims]
+        responses = [self.tool.run(paper_title) for paper_title in papers_titles]
+        final_response = await self._verification(claims, responses)
+        return final_response
+
+    async def run_with_tool_api_call(self, prompts, responses):
+        batch_size = 5
+        num_batches = math.ceil(len(prompts) / batch_size)
+
+        self.sample_list = [{"prompt": prompt, "response": response, "category": 'scientific'} for prompt, response in zip(prompts, responses)]
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(responses))
+
+            claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses = await self.run_with_tool_live(responses[batch_start:batch_end])
+
+            for j, (claims_in_response, queries_in_response, evidences_in_response, verifications_in_response) in enumerate(zip(claims_in_responses, queries_in_responses, evidences_in_responses, verifications_in_responses)):
+                index = batch_start + j
+
+                self.sample_list[index].update({
+                    'claims': claims_in_response,
+                    'queries': queries_in_response,
+                    'evidences': evidences_in_response,
+                    'claim_level_factuality': verifications_in_response,
+                    'response_level_factuality': all([verification['factuality'] if verification != None else True for verification in verifications_in_response])
+                })
+        return self.sample_list
+
+    async def run_with_tool_dataset(self, annotated_dataset_path: str, with_tool_classified_dataset_path: str, rerun: bool = False, rerun_indices: list = []):
+        # Example of a line: 
+        # {"paper_title": "A Survey of Modern Authorship Attribution Methods", "paper_author(s)": "Stamatatos, Efstathios", "paper_pub_year": "2013", "label": True / False}
+        if rerun == False:
+            with open(annotated_dataset_path, 'r') as f:
+                data = [json.loads(line) for line in f]
+            self.sample_list = [claim for sample in data for claim in sample['claims']]
+            rerun_elements = self.sample_list
+        else:
+            with open(with_tool_classified_dataset_path, 'r') as f:
+                data = [json.loads(line) for line in f]
+            self.sample_list = data
+            rerun_elements = [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 5
+        num_batches = math.ceil(len(rerun_elements) / batch_size) # 5
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = (i + 1) * batch_size if (i + 1) * batch_size < len(rerun_elements) else len(rerun_elements)
+
+            responses = await self.run_with_tool_live_without_claim_extraction(rerun_elements[batch_start:batch_end])
+            for j, response in enumerate(responses):
+                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
+                if response == None:
+                    self.sample_list[index]['with_tool_classification'] = 'None'
+                    self.sample_list[index]['error'] = 'None'
+                else:
+                    self.sample_list[index]['with_tool_classification'] = response.get('factuality', 'None')
+                    self.sample_list[index]['error'] = response.get('error', 'None')
+        
+            # save everything after each batch to prevent data loss
+            with open(with_tool_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    json_str = json.dumps(item)
+                    f.write(json_str + '\n')
+
+    async def run_self_check_live(self, fewshot, batch):
+        user_prompt_key = 'user_3_shot_CoT' if fewshot else 'user_zero_shot_CoT'
+        messages_list = [
+            [
+                {"role": "system", "content": self.self_check_prompt['system']},
+                {"role": "user", "content": self.self_check_prompt[user_prompt_key].format(scientific_literature=response)}
+            ]
+            for response in batch
+        ]
+        return await self.chat.async_run(messages_list, Dict)
+
+    async def run_self_check_dataset(self, annotated_dataset_path: str, self_check_classified_dataset_path: str, fewshot: bool = False, rerun: bool = False, rerun_indices: list = []):
+        # Example of a line: 
+        # {"paper_title": "A Survey of Modern Authorship Attribution Methods", "paper_author(s)": "Stamatatos, Efstathios", "paper_pub_year": "2013", "annotation": True / False}
+        data_path = annotated_dataset_path if not rerun else self_check_classified_dataset_path
+        with open(data_path, 'r') as f:
+            data = [json.loads(line) for line in f]
+        self.sample_list = data if rerun else [claim for sample in data for claim in sample['claims']]
+        rerun_elements = self.sample_list if not rerun else [self.sample_list[i] for i in rerun_indices]
+
+        batch_size = 5
+        num_batches = math.ceil(len(rerun_elements) / batch_size)
+
+        for i in range(num_batches):
+            print(i)
+            batch_start = i * batch_size
+            batch_end = (i + 1) * batch_size
+            batch = rerun_elements[batch_start:batch_end]
+            batch = [{k:v for k,v in d.items() if k != "label"} for d in batch]
+
+            responses = await self.run_self_check_live(fewshot, batch)
+            for j, response in enumerate(responses):
+                index = batch_start + j if rerun == False else rerun_indices[batch_start + j]
+                if response == None:
+                    self.sample_list[index]['self_check_classification'] = 'None'
+                    self.sample_list[index]['self_check_reasoning'] = 'None'
+                else:
+                    self.sample_list[index]['self_check_classification'] = response.get('factuality', 'None')
+                    self.sample_list[index]['self_check_reasoning'] = response.get('reasoning', 'None')
+        
+            # save everything after each batch to prevent data loss
+            with open(self_check_classified_dataset_path, 'w') as f:
+                for item in self.sample_list:
+                    json_str = json.dumps(item)
                     f.write(json_str + '\n')
```

### Comparing `factool-0.0.1/factool/scientific/tool.py` & `factool-0.0.7/factool/scientific/tool.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,22 @@
-import yaml
-
-from scholarly import scholarly
-from scholarly import ProxyGenerator
-
-from factool.env_config import factool_env_config
-
-# env
-scraper_api_key = factool_env_config.scraper_api_key
-
-class google_scholar():
-    def __init__(self):
-        pg = ProxyGenerator()
-
-        success = pg.ScraperAPI(scraper_api_key)
-        scholarly.use_proxy(pg)
-
-    def run(self, query):
-        results = scholarly.search_pubs(query)
-        paper_info = next(results)
-        paper_info_subset = {key: paper_info['bib'][key] for key in ['title', 'author', 'pub_year']}
-        return paper_info_subset
-
-# Example Usage  
-if __name__ == "__main__":
-    tool = google_scholar()
-    query = "Quantum approximate optimization algorithm: Performance, mechanism, and implementation on near-term devices"
-    results = tool.run(query)
-    print(results)
+import yaml
+
+from scholarly import scholarly
+from scholarly import ProxyGenerator
+
+from factool.env_config import factool_env_config
+
+# env
+scraper_api_key = factool_env_config.scraper_api_key
+
+class google_scholar():
+    def __init__(self):
+        pg = ProxyGenerator()
+        if scraper_api_key is not None:
+            success = pg.ScraperAPI(scraper_api_key)
+            scholarly.use_proxy(pg)
+
+    def run(self, query):
+        results = scholarly.search_pubs(query)
+        paper_info = next(results)
+        paper_info_subset = {key: paper_info['bib'][key] for key in ['title', 'author', 'pub_year']}
+        return paper_info_subset
```

### Comparing `factool-0.0.1/factool/utils/claim_extractor.py` & `factool-0.0.7/factool/utils/claim_extractor.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import os
-import pathlib
-import openai
-import yaml
-import json
-import asyncio
-from tqdm import tqdm
-from factool.env_config import factool_env_config
-
-
-# env
-openai.api_key = factool_env_config.openai_api_key
-
-
-config = {
-    'model_name': 'gpt-3.5-turbo',
-    'max_tokens': 2000,
-    'temperature': 0.0,
-    'top_p': 1,
-    'frequency_penalty': 0.0,
-    'presence_penalty': 0.0,
-    'n': 1
-}
-
-
-# Make api calls asynchronously
-async def run_api(messages):
-    async def single_run(message):
-        output = openai.ChatCompletion.create(
-            model=config['model_name'],
-            messages=message,
-            max_tokens=config['max_tokens'],
-            temperature=config['temperature'],
-            top_p=config['top_p'],
-            frequency_penalty=config['frequency_penalty'],
-            presence_penalty=config['presence_penalty'],
-            n=config['n'],
-        )
-        return output.choices[0].message.content.strip()
-
-    responses = [single_run(messages[index]) for index in range(len(messages))]
-    return await asyncio.gather(*responses)
-
-
-
-# Import data from scientific.json
-scientific_list = []
-with open("../datasets/scientific/scientific.json", "r") as f:
-    data = json.load(f)
-    for dict_data in data:
-        cur_dict = {'dataset_name': 'scientific',
-                    'question': dict_data["question"],
-                    'factual_response': dict_data['factual_response']}
-        scientific_list.append(cur_dict)
-
-# Apply template prompt
-with open("./prompts/claim_extraction.yaml") as f:
-    data = yaml.load(f, Loader=yaml.FullLoader)
-prompt = data['scientific']
-messages_list = [
-    [
-        {"role": "system", "content": prompt['system']},
-        {"role": "user", "content": prompt['user'].format(input=sample['factual_response'])},
-    ]
-    for sample in scientific_list
-]
-
-assert len(messages_list) == len(scientific_list), "The data length is different"
-
-# Run the API to get the output
-print("begin claims extraction...")
-results = asyncio.run(run_api(messages_list))
-for i in range(len(scientific_list)):
-    scientific_list[i]["claims"] = results[i]
-
-with open('../datasets/scientific/scientific_claims.json', 'w') as f:
-    json.dump(scientific_list, f, indent=4)
-
-
-"""
-The scientific_claims.json file saved by the above code may have format problems, here are some adjustments
-"""
-with open("../datasets/scientific/scientific_claims.json", "r") as f:
-    data = json.load(f)
-    for data_i in tqdm(data, total=len(data)):
-        try:
-            data_i["claims"] = json.loads(data_i["claims"].strip())
-        except:
-            print(data_i["claims"])
-            continue
-with open("../datasets/scientific/scientific_claims.json", "w") as f:
-    json.dump(data, f, indent=4)
+import os
+import pathlib
+import openai
+import yaml
+import json
+import asyncio
+from tqdm import tqdm
+from factool.env_config import factool_env_config
+
+
+# env
+openai.api_key = factool_env_config.openai_api_key
+
+
+config = {
+    'model_name': 'gpt-3.5-turbo',
+    'max_tokens': 2000,
+    'temperature': 0.0,
+    'top_p': 1,
+    'frequency_penalty': 0.0,
+    'presence_penalty': 0.0,
+    'n': 1
+}
+
+
+# Make api calls asynchronously
+async def run_api(messages):
+    async def single_run(message):
+        output = openai.ChatCompletion.create(
+            model=config['model_name'],
+            messages=message,
+            max_tokens=config['max_tokens'],
+            temperature=config['temperature'],
+            top_p=config['top_p'],
+            frequency_penalty=config['frequency_penalty'],
+            presence_penalty=config['presence_penalty'],
+            n=config['n'],
+        )
+        return output.choices[0].message.content.strip()
+
+    responses = [single_run(messages[index]) for index in range(len(messages))]
+    return await asyncio.gather(*responses)
+
+
+
+# Import data from scientific.json
+scientific_list = []
+with open("../datasets/scientific/scientific.json", "r") as f:
+    data = json.load(f)
+    for dict_data in data:
+        cur_dict = {'dataset_name': 'scientific',
+                    'question': dict_data["question"],
+                    'factual_response': dict_data['factual_response']}
+        scientific_list.append(cur_dict)
+
+# Apply template prompt
+with open("./prompts/claim_extraction.yaml") as f:
+    data = yaml.load(f, Loader=yaml.FullLoader)
+prompt = data['scientific']
+messages_list = [
+    [
+        {"role": "system", "content": prompt['system']},
+        {"role": "user", "content": prompt['user'].format(input=sample['factual_response'])},
+    ]
+    for sample in scientific_list
+]
+
+assert len(messages_list) == len(scientific_list), "The data length is different"
+
+# Run the API to get the output
+print("begin claims extraction...")
+results = asyncio.run(run_api(messages_list))
+for i in range(len(scientific_list)):
+    scientific_list[i]["claims"] = results[i]
+
+with open('../datasets/scientific/scientific_claims.json', 'w') as f:
+    json.dump(scientific_list, f, indent=4)
+
+
+"""
+The scientific_claims.json file saved by the above code may have format problems, here are some adjustments
+"""
+with open("../datasets/scientific/scientific_claims.json", "r") as f:
+    data = json.load(f)
+    for data_i in tqdm(data, total=len(data)):
+        try:
+            data_i["claims"] = json.loads(data_i["claims"].strip())
+        except:
+            print(data_i["claims"])
+            continue
+with open("../datasets/scientific/scientific_claims.json", "w") as f:
+    json.dump(data, f, indent=4)
```

### Comparing `factool-0.0.1/factool/utils/openai_wrapper.py` & `factool-0.0.7/factool/utils/openai_wrapper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-# the async version is adapted from https://gist.github.com/neubig/80de662fb3e225c18172ec218be4917a
-
-from __future__ import annotations
-
-import os
-import yaml
-import openai
-import ast
-import pdb
-import asyncio
-from typing import Any, List
-import os
-import pathlib
-
-
-from factool.env_config import factool_env_config
-
-# env
-openai.api_key = factool_env_config.openai_api_key
-
-class OpenAIChat():
-    def __init__(self, model_name='gpt-3.5-turbo', max_tokens=2500, temperature=0.5, top_p=1, request_timeout=60):
-        self.config = {'model_name': model_name, 'max_tokens': max_tokens, 'temperature': temperature, 'top_p': top_p, 'request_timeout': request_timeout}
-
-    
-    def _boolean_fix(self, output):
-        return output.replace("true", "True").replace("false", "False")
-
-    def _type_check(self, output, expected_type):
-        try:
-            output_eval = ast.literal_eval(output)
-            if not isinstance(output_eval, expected_type):
-                return None
-            return output_eval
-        except:
-            return None
-
-    async def dispatch_openai_requests(
-        self,
-        messages_list,
-    ) -> list[str]:
-        """Dispatches requests to OpenAI API asynchronously.
-        
-        Args:
-            messages_list: List of messages to be sent to OpenAI ChatCompletion API.
-        Returns:
-            List of responses from OpenAI API.
-        """
-        async def _request_with_retry(messages, retry=3):
-            for _ in range(retry):
-                try:
-                    response = await openai.ChatCompletion.acreate(
-                        model=self.config['model_name'],
-                        messages=messages,
-                        max_tokens=self.config['max_tokens'],
-                        temperature=self.config['temperature'],
-                        top_p=self.config['top_p'],
-                        request_timeout=self.config['request_timeout'],
-                    )
-                    return response
-                except openai.error.RateLimitError:
-                    print('Rate limit error, waiting for 40 second...')
-                    await asyncio.sleep(40)
-                except openai.error.APIError:
-                    print('API error, waiting for 1 second...')
-                    await asyncio.sleep(1)
-                except openai.error.Timeout:
-                    print('Timeout error, waiting for 1 second...')
-                    await asyncio.sleep(1)
-                except openai.error.ServiceUnavailableError:
-                    print('Service unavailable error, waiting for 3 second...')
-                    await asyncio.sleep(3)
-            return None
-
-        async_responses = [
-            _request_with_retry(messages)
-            for messages in messages_list
-        ]
-
-        return await asyncio.gather(*async_responses)
-    
-    async def async_run(self, messages_list, expected_type):
-        retry = 1
-        responses = [None for _ in range(len(messages_list))]
-        messages_list_cur_index = [i for i in range(len(messages_list))]
-
-        while retry > 0 and len(messages_list_cur_index) > 0:
-            print(f'{retry} retry left...')
-            messages_list_cur = [messages_list[i] for i in messages_list_cur_index]
-            
-            predictions = await self.dispatch_openai_requests(
-                messages_list=messages_list_cur,
-            )
-
-            preds = [self._type_check(self._boolean_fix(prediction['choices'][0]['message']['content']), expected_type) if prediction is not None else None for prediction in predictions]
-
-            finised_index = []
-            for i, pred in enumerate(preds):
-                if pred is not None:
-                    responses[messages_list_cur_index[i]] = pred
-                    finised_index.append(messages_list_cur_index[i])
-            
-            messages_list_cur_index = [i for i in messages_list_cur_index if i not in finised_index]
-            
-            retry -= 1
-        
-        return responses
-
-if __name__ == "__main__":
-    chat = OpenAIChat()
-
-    predictions = chat.async_run(
-        messages_list=[
-            [{"role": "user", "content": "show either 'ab' or '['a']'. Do not do anything else."}],
-        ] * 20,
-        expected_type=List,
+# the async version is adapted from https://gist.github.com/neubig/80de662fb3e225c18172ec218be4917a
+
+from __future__ import annotations
+
+import os
+import yaml
+import openai
+import ast
+import pdb
+import asyncio
+from typing import Any, List
+import os
+import pathlib
+
+
+from factool.env_config import factool_env_config
+
+# env
+openai.api_key = factool_env_config.openai_api_key
+
+class OpenAIChat():
+    def __init__(self, model_name='gpt-3.5-turbo', max_tokens=2500, temperature=0.5, top_p=1, request_timeout=60):
+        self.config = {'model_name': model_name, 'max_tokens': max_tokens, 'temperature': temperature, 'top_p': top_p, 'request_timeout': request_timeout}
+
+    
+    def _boolean_fix(self, output):
+        return output.replace("true", "True").replace("false", "False")
+
+    def _type_check(self, output, expected_type):
+        try:
+            output_eval = ast.literal_eval(output)
+            if not isinstance(output_eval, expected_type):
+                return None
+            return output_eval
+        except:
+            return None
+
+    async def dispatch_openai_requests(
+        self,
+        messages_list,
+    ) -> list[str]:
+        """Dispatches requests to OpenAI API asynchronously.
+        
+        Args:
+            messages_list: List of messages to be sent to OpenAI ChatCompletion API.
+        Returns:
+            List of responses from OpenAI API.
+        """
+        async def _request_with_retry(messages, retry=3):
+            for _ in range(retry):
+                try:
+                    response = await openai.ChatCompletion.acreate(
+                        model=self.config['model_name'],
+                        messages=messages,
+                        max_tokens=self.config['max_tokens'],
+                        temperature=self.config['temperature'],
+                        top_p=self.config['top_p'],
+                        request_timeout=self.config['request_timeout'],
+                    )
+                    return response
+                except openai.error.RateLimitError:
+                    print('Rate limit error, waiting for 40 second...')
+                    await asyncio.sleep(40)
+                except openai.error.APIError:
+                    print('API error, waiting for 1 second...')
+                    await asyncio.sleep(1)
+                except openai.error.Timeout:
+                    print('Timeout error, waiting for 1 second...')
+                    await asyncio.sleep(1)
+                except openai.error.ServiceUnavailableError:
+                    print('Service unavailable error, waiting for 3 second...')
+                    await asyncio.sleep(3)
+            return None
+
+        async_responses = [
+            _request_with_retry(messages)
+            for messages in messages_list
+        ]
+
+        return await asyncio.gather(*async_responses)
+    
+    async def async_run(self, messages_list, expected_type):
+        retry = 1
+        responses = [None for _ in range(len(messages_list))]
+        messages_list_cur_index = [i for i in range(len(messages_list))]
+
+        while retry > 0 and len(messages_list_cur_index) > 0:
+            print(f'{retry} retry left...')
+            messages_list_cur = [messages_list[i] for i in messages_list_cur_index]
+            
+            predictions = await self.dispatch_openai_requests(
+                messages_list=messages_list_cur,
+            )
+
+            preds = [self._type_check(self._boolean_fix(prediction['choices'][0]['message']['content']), expected_type) if prediction is not None else None for prediction in predictions]
+
+            finised_index = []
+            for i, pred in enumerate(preds):
+                if pred is not None:
+                    responses[messages_list_cur_index[i]] = pred
+                    finised_index.append(messages_list_cur_index[i])
+            
+            messages_list_cur_index = [i for i in messages_list_cur_index if i not in finised_index]
+            
+            retry -= 1
+        
+        return responses
+
+if __name__ == "__main__":
+    chat = OpenAIChat()
+
+    predictions = chat.async_run(
+        messages_list=[
+            [{"role": "user", "content": "show either 'ab' or '['a']'. Do not do anything else."}],
+        ] * 20,
+        expected_type=List,
     )
```

### Comparing `factool-0.0.1/factool/utils/prompts/agreement_verification.yaml` & `factool-0.0.7/factool/utils/prompts/agreement_verification.yaml`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-knowledge_qa:
-  system: |-
-    You are a brilliant assistant.
-  user: |-
-    You are given a piece of text. Your task is to identify whether there are any factual errors within the text.
-    When you are judging the factuality of the given text, you could reference the provided evidences if needed. The provided evidences may be helpful. Some evidences may contradict to each other. You must be careful when using the evidences to judge the factuality of the given text.
-    When 
-    The response should be a dictionary with three keys - "reasoning", "factuality", "error", and "correction", which correspond to the reasoning, whether the given text is factual or not (Boolean - True or False), the factual error present in the text, and the corrected text.
-    The following is the given text
-    [text]: {claim}
-    The following is the provided evidences
-    [evidences]: {evidence}
-    You should only respond in format as described below. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Why is the given text factual or non-factual? Be careful when you said something is non-factual. When you said something is non-factual, you must provide mulitple evidences to support your decision.",
-      "error": "None if the text is factual; otherwise, describe the error.",
-      "correction": "The corrected text if there is an error.",
-      "factuality": True if the given text is factual, False otherwise.
-    }}
-
-scientific:
-  system: |-
-    You are a brilliant assistant.
-  user: |-
-    You are provided with two inputs, a string (string1) containing several names, and a list (list1) also containing names. Your task is to assess whether all the last names mentioned in string1 are included in list1.
-    
-    You should only respond in format as described below. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Explanation on whether all the last names in string1 are found within list1",
-      "factuality": This will be True if all last names from string1 are present in list1, and False otherwise.
-    }}
-
-    Example 1: 
-    [string1]: "J. Devlin and M. Chang"
-    [list1]: ["Devlin", "M Chang", "Kristina Toutanova"]
-    [response]: {{"reasoning": "string1 contains 2 last names 'Devlin' and 'Chang'. Both of these last names are present in list1.", "factuality": True}}
-
-    Example 2: 
-    [string1]: "Tom Brown et. al"
-    [list1]: ["Y. Lecun", "G. Hinton"]
-    [response]: {{"reasoning": "string 1 contains 1 last name 'Brown'. Brown is not present in list1.", "factuality": False}}
-
-    Complete the following:
-    [string1]: {string1}
-    [list1]: {list2}
+knowledge_qa:
+  system: |-
+    You are a brilliant assistant.
+  user: |-
+    You are given a piece of text. Your task is to identify whether there are any factual errors within the text.
+    When you are judging the factuality of the given text, you could reference the provided evidences if needed. The provided evidences may be helpful. Some evidences may contradict to each other. You must be careful when using the evidences to judge the factuality of the given text.
+    When 
+    The response should be a dictionary with three keys - "reasoning", "factuality", "error", and "correction", which correspond to the reasoning, whether the given text is factual or not (Boolean - True or False), the factual error present in the text, and the corrected text.
+    The following is the given text
+    [text]: {claim}
+    The following is the provided evidences
+    [evidences]: {evidence}
+    You should only respond in format as described below. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Why is the given text factual or non-factual? Be careful when you said something is non-factual. When you said something is non-factual, you must provide mulitple evidences to support your decision.",
+      "error": "None if the text is factual; otherwise, describe the error.",
+      "correction": "The corrected text if there is an error.",
+      "factuality": True if the given text is factual, False otherwise.
+    }}
+
+scientific:
+  system: |-
+    You are a brilliant assistant.
+  user: |-
+    You are provided with two inputs, a string (string1) containing several names, and a list (list1) also containing names. Your task is to assess whether all the last names mentioned in string1 are included in list1.
+    
+    You should only respond in format as described below. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Explanation on whether all the last names in string1 are found within list1",
+      "factuality": This will be True if all last names from string1 are present in list1, and False otherwise.
+    }}
+
+    Example 1: 
+    [string1]: "J. Devlin and M. Chang"
+    [list1]: ["Devlin", "M Chang", "Kristina Toutanova"]
+    [response]: {{"reasoning": "string1 contains 2 last names 'Devlin' and 'Chang'. Both of these last names are present in list1.", "factuality": True}}
+
+    Example 2: 
+    [string1]: "Tom Brown et. al"
+    [list1]: ["Y. Lecun", "G. Hinton"]
+    [response]: {{"reasoning": "string 1 contains 1 last name 'Brown'. Brown is not present in list1.", "factuality": False}}
+
+    Complete the following:
+    [string1]: {string1}
+    [list1]: {list2}
     [response]:
```

### Comparing `factool-0.0.1/factool/utils/prompts/claim_extraction.yaml` & `factool-0.0.7/factool/utils/prompts/claim_extraction.yaml`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-knowledge_qa:
-  system: |-
-    You are a brilliant assistant.
-  user: |-
-    You are given a piece of text that includes knowledge claims. A claim is a statement that asserts something as true or false, which can be verified by humans. Your task is to accurately identify and extract every claim stated in the provided text. Then, resolve any coreference (pronouns or other referring expressions) in the claim for clarity. Each claim should be concise (less than 15 words) and self-contained.
-    Your response MUST be a list of dictionaries. Each dictionary should contains the key "claim", which correspond to the extracted claim (with all coreferences resolved).
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '['.
-    [response format]: 
-    [
-      {{
-        "claim": "Ensure that the claim is fewer than 15 words and conveys a complete idea. Resolve any coreference (pronouns or other referring expressions) in the claim for clarity",
-      }},
-      ...
-    ]
-
-    Here are two examples:
-    [text]: Tomas Berdych defeated Gael Monfis 6-1, 6-4 on Saturday. The sixth-seed reaches Monte Carlo Masters final for the first time . Berdych will face either Rafael Nadal or Novak Djokovic in the final.
-    [response]: [{{"claim": "Tomas Berdych defeated Gael Monfis 6-1, 6-4"}}, {{"claim": "Tomas Berdych defeated Gael Monfis 6-1, 6-4 on Saturday"}}, {{"claim": "Tomas Berdych reaches Monte Carlo Masters final"}}, {{"claim": "Tomas Berdych is the sixth-seed"}}, {{"claim": "Tomas Berdych reaches Monte Carlo Masters final for the first time"}}, {{"claim": "Berdych will face either Rafael Nadal or Novak Djokovic"}}, {{"claim": "Berdych will face either Rafael Nadal or Novak Djokovic in the final"}}]
-
-    [text]: Tinder only displays the last 34 photos - but users can easily see more. Firm also said it had improved its mutual friends feature.
-    [response]: [{{"claim": "Tinder only displays the last photos"}}, {{"claim": "Tinder only displays the last 34 photos"}}, {{"claim": "Tinder users can easily see more photos"}}, {{"claim": "Tinder said it had improved its feature"}}, {{"claim": "Tinder said it had improved its mutual friends feature"}}]
-
-    Now complete the following:
-    [text]: {input}
-    [response]: 
-
-math:
-  system: |-
-    You are a helpful assistant.
-  user: |-
-    You are given a math problem and a potential solution to the math problem. Your task is to identify all the math calculations that involve arithmetic operations between known real numbers within the potential solution. However, do not include math calculations that contains variable(s).
-    Your response MUST be a list of dictionaries. Each dictionary should contains 2 key - "math_calculation" and "calculated_answer", which correspond to the extracted math calculation, and the calculated answer within the potential solution.
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '['.
-    [response format]: 
-    [
-      {{
-        "math_calculation": "Extracted math calculation involving real numbers within the potential solution. Do not include math calculataions that contains variable(s). Do not include units such as $, %, etc.",
-        "calculated_answer": "The calculated answer for the extracted math calculation."
-      }},
-      ...
-    ]
-
-    Here are two examples:
-    [math problem]: What is the area of a circle with a diameter of 10 inches?
-    [potential solution]: To find the area, we first calculate the radius as the diameter divided by 2, so the radius is 10/2 = 5 inches. Then, we use the formula for the area of a circle, which is πr^2. Plugging in the radius we get, Area = π*5^2 = 78.54 square inches.
-    [response]: [{{"math_calculation": "10 / 2", "calculated_answer": "5"}}, {{"math_calculation": "π * 5^2", "calculated_answer": "78.54"}}]
-
-    [math problem]: A store originally sold a shirt for $45. They are offering a 20% discount on the shirt. How much will the shirt cost now?
-    [potential solution]: The discount on the shirt is calculated as 20% of $45, which is 0.20 * 45 = $9. The new price of the shirt after the discount is $45 - $9 = $36.
-    [response]: [{{"math_calculation": "0.20 * 45", "calculated_answer": "9"}}, {{"math_calculation": "45 - 9","calculated_answer": "36"}}]
-
-    Now complete the following:
-    [math problem]: {input_question}
-    [potential solution]: {input_solution}
-    [response]: 
-
-scientific:
-  system: |-
-    You are a brilliant assistant.
-  user: |-
-    You are given a piece of text that mentions some scientific literature. Your task is to accurately find all papers mentioned in the text and identify the title, author(s), and publication year for each paper.
-    The response should be a list of dictionaries, with each dictionary having keys "paper_title", "paper_author(s)", and "paper_pub_year", which correspond to the title of the paper, the authors of the paper, and the publication year of the paper.
-    The following is the given text
-    [text]: {input}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '['.
-    [response format]: 
-    [
-      {{
-        "paper_title": "Title of the paper.",
-        "paper_author(s)": "Author(s) of the paper.",
-        "paper_pub_year": "Year of the paper published."
-      }},
-      ...
+knowledge_qa:
+  system: |-
+    You are a brilliant assistant.
+  user: |-
+    You are given a piece of text that includes knowledge claims. A claim is a statement that asserts something as true or false, which can be verified by humans. Your task is to accurately identify and extract every claim stated in the provided text. Then, resolve any coreference (pronouns or other referring expressions) in the claim for clarity. Each claim should be concise (less than 15 words) and self-contained.
+    Your response MUST be a list of dictionaries. Each dictionary should contains the key "claim", which correspond to the extracted claim (with all coreferences resolved).
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '['.
+    [response format]: 
+    [
+      {{
+        "claim": "Ensure that the claim is fewer than 15 words and conveys a complete idea. Resolve any coreference (pronouns or other referring expressions) in the claim for clarity",
+      }},
+      ...
+    ]
+
+    Here are two examples:
+    [text]: Tomas Berdych defeated Gael Monfis 6-1, 6-4 on Saturday. The sixth-seed reaches Monte Carlo Masters final for the first time . Berdych will face either Rafael Nadal or Novak Djokovic in the final.
+    [response]: [{{"claim": "Tomas Berdych defeated Gael Monfis 6-1, 6-4"}}, {{"claim": "Tomas Berdych defeated Gael Monfis 6-1, 6-4 on Saturday"}}, {{"claim": "Tomas Berdych reaches Monte Carlo Masters final"}}, {{"claim": "Tomas Berdych is the sixth-seed"}}, {{"claim": "Tomas Berdych reaches Monte Carlo Masters final for the first time"}}, {{"claim": "Berdych will face either Rafael Nadal or Novak Djokovic"}}, {{"claim": "Berdych will face either Rafael Nadal or Novak Djokovic in the final"}}]
+
+    [text]: Tinder only displays the last 34 photos - but users can easily see more. Firm also said it had improved its mutual friends feature.
+    [response]: [{{"claim": "Tinder only displays the last photos"}}, {{"claim": "Tinder only displays the last 34 photos"}}, {{"claim": "Tinder users can easily see more photos"}}, {{"claim": "Tinder said it had improved its feature"}}, {{"claim": "Tinder said it had improved its mutual friends feature"}}]
+
+    Now complete the following:
+    [text]: {input}
+    [response]: 
+
+math:
+  system: |-
+    You are a helpful assistant.
+  user: |-
+    You are given a math problem and a potential solution to the math problem. Your task is to identify all the math calculations that involve arithmetic operations between known real numbers within the potential solution. However, do not include math calculations that contains variable(s).
+    Your response MUST be a list of dictionaries. Each dictionary should contains 2 key - "math_calculation" and "calculated_answer", which correspond to the extracted math calculation, and the calculated answer within the potential solution.
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '['.
+    [response format]: 
+    [
+      {{
+        "math_calculation": "Extracted math calculation involving real numbers within the potential solution. Do not include math calculataions that contains variable(s). Do not include units such as $, %, etc.",
+        "calculated_answer": "The calculated answer for the extracted math calculation."
+      }},
+      ...
+    ]
+
+    Here are two examples:
+    [math problem]: What is the area of a circle with a diameter of 10 inches?
+    [potential solution]: To find the area, we first calculate the radius as the diameter divided by 2, so the radius is 10/2 = 5 inches. Then, we use the formula for the area of a circle, which is πr^2. Plugging in the radius we get, Area = π*5^2 = 78.54 square inches.
+    [response]: [{{"math_calculation": "10 / 2", "calculated_answer": "5"}}, {{"math_calculation": "π * 5^2", "calculated_answer": "78.54"}}]
+
+    [math problem]: A store originally sold a shirt for $45. They are offering a 20% discount on the shirt. How much will the shirt cost now?
+    [potential solution]: The discount on the shirt is calculated as 20% of $45, which is 0.20 * 45 = $9. The new price of the shirt after the discount is $45 - $9 = $36.
+    [response]: [{{"math_calculation": "0.20 * 45", "calculated_answer": "9"}}, {{"math_calculation": "45 - 9","calculated_answer": "36"}}]
+
+    Now complete the following:
+    [math problem]: {input_question}
+    [potential solution]: {input_solution}
+    [response]: 
+
+scientific:
+  system: |-
+    You are a brilliant assistant.
+  user: |-
+    You are given a piece of text that mentions some scientific literature. Your task is to accurately find all papers mentioned in the text and identify the title, author(s), and publication year for each paper.
+    The response should be a list of dictionaries, with each dictionary having keys "paper_title", "paper_author(s)", and "paper_pub_year", which correspond to the title of the paper, the authors of the paper, and the publication year of the paper.
+    The following is the given text
+    [text]: {input}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '['.
+    [response format]: 
+    [
+      {{
+        "paper_title": "Title of the paper.",
+        "paper_author(s)": "Author(s) of the paper.",
+        "paper_pub_year": "Year of the paper published."
+      }},
+      ...
     ]
```

### Comparing `factool-0.0.1/factool/utils/prompts/query_generation.yaml` & `factool-0.0.7/factool/utils/prompts/query_generation.yaml`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-knowledge_qa:
-  system: |-
-    You are a query generator that generates effective and concise search engine queries to verify a given claim.
-  user: |-
-    You are a query generator designed to help users verify a given claim using search engines. Your primary task is to generate a Python list of two effective and skeptical search engine queries. These queries should assist users in critically evaluating the factuality of a provided claim using search engines.
-    You should only respond in format as described below (a Python list of queries). PLEASE STRICTLY FOLLOW THE FORMAT. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '['.
-    [response format]: ['query1', 'query2']
-
-    Here are 3 examples:
-    [claim]: The CEO of twitter is Bill Gates.
-    [response]: ["Who is the CEO of twitter?", "CEO Twitter"]
-
-    [claim]: Michael Phelps is the most decorated Olympian of all time.
-    [response]: ["Who is the most decorated Olympian of all time?", "Michael Phelps"]
-
-    [claim]: ChatGPT is created by Google.
-    [response]: ["Who created ChatGPT?", "ChatGPT"]
-
-    Now complete the following:
-    [claim]: {input}
-    [response]: 
-
-code:
-  system: |-
-    You are a brilliant assistant.
-  user_testcases_3: |-
-    Please generate 3 distinct function calls for the given coding question to test the functionality of the function {entry_point} that attempts to solve the provided coding question.
-    Your response must be a dictionary with 3 keys - "function_call_1", "function_call_2", "function_call_3", which correspond to the 3 distinct function calls for function {entry_point}.
-    The following is the given coding question - 
-    [coding question]: {input_question}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "function_call_1": "First function call for function {entry_point}. Do not include anything else.",
-      "function_call_2": "Second function call for function {entry_point}. Do not include anything else.",
-      "function_call_3": "Third function call for function {entry_point}. Do not include anything else."
-    }}
-  user_testcases_5: |-
-    Please generate 5 distinct function calls for the given coding question to test the functionality of the function {entry_point} that attempts to solve the provided coding question.
-    Your response must be a dictionary with 5 keys - "function_call_1", "function_call_2", "function_call_3", "function_call_4", "function_call_5", which correspond to the 5 distinct function calls for function {entry_point}.
-    The following is the given coding question - 
-    [coding question]: {input_question}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "function_call_1": "First function call for function {entry_point}. Do not include anything else.",
-      "function_call_2": "Second function call for function {entry_point}. Do not include anything else.",
-      "function_call_3": "Third function call for function {entry_point}. Do not include anything else.",
-      "function_call_4": "Fourth function call for function {entry_point}. Do not include anything else.",
-      "function_call_5": "Fifth function call for function {entry_point}. Do not include anything else."
-    }}
-  user_solutions: |-
-    Please solve the given coding question. Make sure that the solution is optimized and correct. You MUST use Python to solve the coding question.
-    Your response MUST be a dictionary with keys "reasoning" and "python_solution", which correspond to the reasoning and Python implementations of the function {entry_point}.
-    The following is the given coding question - 
-    [coding question]: {input_question}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]:
-    {{
-      "reasoning": "Reasoning for solution.",  
-      "python_solution": "Python implementation of the function {entry_point}. Include only the implementation of the function itself. Ensure the output of the function aligns with its specified return type."
-    }}
-
-math:
-    system: |-
-      You are a brilliant assistant.
-    user: |-
-      You are given a math calculation and its corresponding calculated answer. Your task is to write an executable Python snippet that validate the accuracy of the math calculation against the calculated answer. The Python snippet should print 'True' if the calculated answer is correct, and 'False' otherwise.
-      Your response MUST be a dictionary with key "python_snippet", which correspond to the executable python snippet.
-      [math calculation]: {math_calculation}
-      [calculated answer]: {calculated_answer}
-      You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-      [response format]: 
-      {{
-        "python_snippet": "An executable Python snippet that validates the accuracy of the math calculation against the calculated answer. The Python snippet should print 'True' if the calculated answer is correct, and 'False' otherwise."
+knowledge_qa:
+  system: |-
+    You are a query generator that generates effective and concise search engine queries to verify a given claim.
+  user: |-
+    You are a query generator designed to help users verify a given claim using search engines. Your primary task is to generate a Python list of two effective and skeptical search engine queries. These queries should assist users in critically evaluating the factuality of a provided claim using search engines.
+    You should only respond in format as described below (a Python list of queries). PLEASE STRICTLY FOLLOW THE FORMAT. DO NOT RETURN ANYTHING ELSE. START YOUR RESPONSE WITH '['.
+    [response format]: ['query1', 'query2']
+
+    Here are 3 examples:
+    [claim]: The CEO of twitter is Bill Gates.
+    [response]: ["Who is the CEO of twitter?", "CEO Twitter"]
+
+    [claim]: Michael Phelps is the most decorated Olympian of all time.
+    [response]: ["Who is the most decorated Olympian of all time?", "Michael Phelps"]
+
+    [claim]: ChatGPT is created by Google.
+    [response]: ["Who created ChatGPT?", "ChatGPT"]
+
+    Now complete the following:
+    [claim]: {input}
+    [response]: 
+
+code:
+  system: |-
+    You are a brilliant assistant.
+  user_testcases_3: |-
+    Please generate 3 distinct function calls for the given coding question to test the functionality of the function {entry_point} that attempts to solve the provided coding question.
+    Your response must be a dictionary with 3 keys - "function_call_1", "function_call_2", "function_call_3", which correspond to the 3 distinct function calls for function {entry_point}.
+    The following is the given coding question - 
+    [coding question]: {input_question}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "function_call_1": "First function call for function {entry_point}. Do not include anything else.",
+      "function_call_2": "Second function call for function {entry_point}. Do not include anything else.",
+      "function_call_3": "Third function call for function {entry_point}. Do not include anything else."
+    }}
+  user_testcases_5: |-
+    Please generate 5 distinct function calls for the given coding question to test the functionality of the function {entry_point} that attempts to solve the provided coding question.
+    Your response must be a dictionary with 5 keys - "function_call_1", "function_call_2", "function_call_3", "function_call_4", "function_call_5", which correspond to the 5 distinct function calls for function {entry_point}.
+    The following is the given coding question - 
+    [coding question]: {input_question}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "function_call_1": "First function call for function {entry_point}. Do not include anything else.",
+      "function_call_2": "Second function call for function {entry_point}. Do not include anything else.",
+      "function_call_3": "Third function call for function {entry_point}. Do not include anything else.",
+      "function_call_4": "Fourth function call for function {entry_point}. Do not include anything else.",
+      "function_call_5": "Fifth function call for function {entry_point}. Do not include anything else."
+    }}
+  user_solutions: |-
+    Please solve the given coding question. Make sure that the solution is optimized and correct. You MUST use Python to solve the coding question.
+    Your response MUST be a dictionary with keys "reasoning" and "python_solution", which correspond to the reasoning and Python implementations of the function {entry_point}.
+    The following is the given coding question - 
+    [coding question]: {input_question}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]:
+    {{
+      "reasoning": "Reasoning for solution.",  
+      "python_solution": "Python implementation of the function {entry_point}. Include only the implementation of the function itself. Ensure the output of the function aligns with its specified return type."
+    }}
+
+math:
+    system: |-
+      You are a brilliant assistant.
+    user: |-
+      You are given a math calculation and its corresponding calculated answer. Your task is to write an executable Python snippet that validate the accuracy of the math calculation against the calculated answer. The Python snippet should print 'True' if the calculated answer is correct, and 'False' otherwise.
+      Your response MUST be a dictionary with key "python_snippet", which correspond to the executable python snippet.
+      [math calculation]: {math_calculation}
+      [calculated answer]: {calculated_answer}
+      You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+      [response format]: 
+      {{
+        "python_snippet": "An executable Python snippet that validates the accuracy of the math calculation against the calculated answer. The Python snippet should print 'True' if the calculated answer is correct, and 'False' otherwise."
       }}
```

### Comparing `factool-0.0.1/factool/utils/prompts/self_check.yaml` & `factool-0.0.7/factool/utils/prompts/self_check.yaml`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-knowledge_qa:
-  system: |-
-    You are a brilliant assistant.
-  user_zero_shot_CoT: |-
-    You are given a claim. Your task is to identify whether there are any factual errors within the claim.
-    The response must be a dictionary with 4 keys - "reasoning", "error", "corrected_claim", and "factuality", which correspond to the reasoning about whether the claim is factual, the factual error present in the claim (if any), the corrected claim (if needed), and whether the claim is factual or not (Boolean - True or False).
-    The following is the given claim - 
-    [claim]: {claim}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Reason about whether the claim is factual. Think step by step.",
-      "error": "None if the claim is factual; otherwise, describe the error.",
-      "corrected_claim": "None if the claim is factual; otherwise, write the corrected claim.",
-      "factuality": "True if the claim is factual, False otherwise."
-    }}
-  user_3_shot_CoT: |-
-    You are given a claim. Your task is to identify whether there are any factual errors within the claim.
-    The response must be a dictionary with 4 keys - "reasoning", "error", "corrected_claim", and "factuality", which correspond to the reasoning about whether the claim is factual, the factual error present in the claim (if any), the corrected claim (if needed), and whether the claim is factual or not (Boolean - True or False).
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Reason about whether the claim is factual. Think step by step.",
-      "error": "None if the claim is factual; otherwise, describe the error.",
-      "corrected_claim": "None if the claim is factual; otherwise, write the corrected claim.",
-      "factuality": "True if the claim is factual, False otherwise."
-    }}
-
-    Here are three examples:
-    [claim]: Albert Einstein was awarded the Nobel Prize in Physics in 1921 for his theory of relativity.
-    [response]: {{"reasoning": "Although Albert Einstein was indeed awarded the Nobel Prize in Physics in 1921, it was not for his theory of relativity, but rather for his discovery of the law of the photoelectric effect.", "error": "The claim incorrectly states that Einstein won the Nobel Prize for his theory of relativity.", "corrected_claim": "Albert Einstein was awarded the Nobel Prize in Physics in 1921 for his discovery of the law of the photoelectric effect.", "factuality": False}}
-
-    [claim]: The Titanic sank on its maiden voyage in 1912 after hitting an iceberg.
-    [response]: {{"reasoning": "This claim is accurate. The RMS Titanic, a British luxury passenger liner, did indeed sink during its maiden voyage in 1912 after colliding with an iceberg in the North Atlantic Ocean.", "error": "None", "corrected_claim": "None", "factuality": True}}
-
-    [claim]: The capital of Australia is Sydney.
-    [response]: {{"reasoning": "Despite Sydney being one of the most recognized and populated cities in Australia, it is not the capital. The capital of Australia is Canberra.", "error": "The claim incorrectly states that Sydney is the capital of Australia.", "corrected_claim": "The capital of Australia is Canberra.", "factuality": False}}
-
-    Now complete the following:
-    [claim]: {claim}
-    [response]: 
-
-code:
-  system: |-
-    You are a brilliant assistant.
-  user_zero_shot_CoT: |-
-    You are given a coding question and a potential solution to the coding question. Your task is to identify whether the potential solution solves the coding question correctly or not. You should check the potential solution line-by-line to see if the solution includes errors, such as syntax, logic, or runtime errors.
-    Your response must be a dictionary with four keys - "reasoning", "error", "corrected_solution", and "factuality", which correspond to the line-by-line reasoning about whether the potential solution contains errors, the coding error present in the potential solution (if any), the corrected solution (if necessary), and whether the potential solution solves the coding question correctly or not (a Boolean value of True or False).
-    The following is the given coding question and potential solution - 
-    [coding question]: {input_question}
-    [potential solution]: {input_solution}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "line-by-line reasoning about whether the potential solution contains errors.",
-      "error": "None if the potential solution correctly solves the coding question; otherwise, describe the error.",
-      "corrected_solution": "None if the potential solution is correct; otherwise, write the correct solution that correctly solves the coding question.",
-      "factuality": "True if the potential solution is correct, False otherwise."
-    }}
-  user_3_shot_CoT: |-
-    You are given a coding question and a potential solution to the coding question. Your task is to identify whether the potential solution solves the coding question correctly or not. You should check the potential solution line-by-line to see if the solution includes errors, such as syntax, logic, or runtime errors.
-    Your response must be a dictionary with four keys - "reasoning", "error", "corrected_solution", and "factuality", which correspond to the line-by-line reasoning about whether the potential solution contains errors, the coding error present in the potential solution (if any), the corrected solution (if necessary), and whether the potential solution solves the coding question correctly or not (a Boolean value of True or False).
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "line-by-line reasoning about whether the potential solution contains errors.",
-      "error": "None if the potential solution correctly solves the coding question; otherwise, describe the error.",
-      "corrected_solution": "None if the potential solution is correct; otherwise, write the correct solution that correctly solves the coding question.",
-      "factuality": "True if the potential solution is correct, False otherwise."
-    }}
-
-    Here are three examples:
-    [coding question]: Write a Python function that takes a list of integers as input and returns the sum of all the elements in the list.
-    [potential solution]: "def sum_list(input_list):\n    sum = 0\n    for i in input_list:\n        sum += i\n    return sum"
-    [response]: {{"reasoning": "The function correctly iterates over each element in the list and adds it to a running sum, which is then returned.", "error": "None", "corrected_solution": "None", "factuality": True}}
-
-    [coding question]: Write a Python function that checks if a given string is a palindrome or not. A palindrome is a word, phrase, number, or other sequence of characters that reads the same forward or backward, allowing for adjustments to punctuation and spaces.
-    [potential solution]: "def is_palindrome(input_string):\n    reversed_string = input_string[::-1]\n    if input_string == reversed_string:\n        return True\n    else:\n        return False"
-    [response]: {{"reasoning": "The function correctly reverses the input string and compares it with the original string to check if it's a palindrome. However, it doesn't account for possible spaces and punctuation, which are supposed to be ignored while checking for palindromes.", "error": "The function does not ignore spaces and punctuation while checking for palindromes.", "corrected_solution": "def is_palindrome(input_string):\n    input_string = ''.join(c for c in input_string if c.isalnum()).lower()\n    reversed_string = input_string[::-1]\n    if input_string == reversed_string:\n        return True\n    else:\n        return False", "factuality": False}}
-
-    [coding question]: Write a Python function that takes a list of integers as input and returns the average of all the elements in the list.
-    [potential solution]: "def average(input_list):\n    sum = 0\n    for i in input_list:\n        sum += i\n    return sum"
-    [response]: {{"reasoning": "The function correctly calculates the sum of all elements in the list, but it does not divide this sum by the number of elements in the list, which is necessary for finding the average.", "error": "The function does not calculate the average correctly because it does not divide the sum by the number of elements.", "corrected_solution": "def average(input_list):\n    sum = 0\n    for i in input_list:\n        sum += i\n    return sum / len(input_list)", "factuality": False}}
-
-    Now complete the following:
-    [coding question]: {input_question}
-    [potential solution]: {input_solution}
-    [response]: 
-
-math:
-  system: |-
-    You are a brilliant assistant.
-  user_zero_shot_CoT: |-
-    You are given a math calculation and a proposed calculated answer to this calculation. Your task is to verify whether the calculated answer solves the math calculation correctly or not.
-    Your response must be a dictionary with three keys - "reasoning", "corrected_answer", and "factuality", which correspond to the reasoning about whether the calculated answer is correct, the corrected calculated answer (if necessary), and whether the calculated answer correctly solves the math calculation or not (a Boolean value of True or False).
-    The following is the given math calculation and proposed calculated answer - 
-    [math calculation]: {input_calculation}
-    [proposed calculated answer]: {input_calculated_answer}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS PROHIBITED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Reason about whether the calculated answer is correct.",
-      "corrected_answer": "None if the calculated answer is correct; otherwise, write the corrected answer that correctly solves the math problem.",
-      "factuality": "True if the calculated answer is correct, False otherwise."
-    }}
-  user_3_shot_CoT: |-
-    You are given a math calculation and a proposed calculated answer to this calculation. Your task is to verify whether the calculated answer solves the math calculation correctly or not.
-    Your response must be a dictionary with three keys - "reasoning", "corrected_answer", and "factuality", which correspond to the reasoning about whether the calculated answer is correct, the corrected calculated answer (if necessary), and whether the calculated answer correctly solves the math calculation or not (a Boolean value of True or False).
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS PROHIBITED. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Reason about whether the calculated answer is correct.",
-      "corrected_answer": "None if the calculated answer is correct; otherwise, write the corrected answer that correctly solves the math problem.",
-      "factuality": "True if the calculated answer is correct, False otherwise."
-    }}
-
-    Here are three examples:
-    [math calculation]: 8 * 9
-    [proposed calculated answer]: 72
-    [response]: {{"reasoning": "The calculation involves a multiplication operation of 8 and 9. The correct answer of this operation is indeed 72.", "corrected_answer": "None", "factuality": True}}
-
-    [math calculation]: 15 / 5
-    [proposed calculated answer]: 5
-    [response]: {{"reasoning": "The calculation involves a division operation of 15 by 5. The correct answer should be 3, not 5.", "corrected_answer": 3, "factuality": False}}
-
-    [math calculation]: 45 - 20
-    [proposed calculated answer]: 30
-    [response]: {{"reasoning": "The calculation involves a subtraction operation of 45 minus 20. The correct answer should be 25, not 30.", "corrected_answer": 25, "factuality": False}}
-
-    Now complete the following:
-    [math calculation]: {input_calculation}
-    [proposed calculated answer]: {input_calculated_answer}
-    [response]: 
-
-scientific:
-  system: |-
-    You are a brilliant assistant.
-  user_zero_shot_CoT: |-
-    You are provided with a dictionary that contains details of a specific scientific literature. The dictionary contains three keys - 'paper_title', 'paper_author(s)', and 'paper_pub_year'. Your task is to use your own knowledge base to validate the following:
-    (1) Confirm if the paper actually exists and whether its title is accurate. The provided paper name should exactly matched the actual paper name.
-    (2) Compare the provided list of authors to that of the original paper, ensuring the provided authors are indeed a subset of the actual authors.
-    (3) Verify the accuracy of the year of publication.
-    Your response must be a dictionary with four keys - "reasoning", "error", "correction", and "factuality", which correspond to your logical process in verifying the dictionary's data integrity, the detection of any errors within the dictionary, rectifying any misinformation (if present), and finally confirming the factuality of the dictionary (Boolean - True or False).
-    The following is the given dictionary that contains details of a scientific literature - 
-    [scientific literature]: {scientific_literature}
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Your process of assessing the data integrity of the scientific literature details in the dictionary. Use your own knowledge base to verify the data integrity of the scientific literature details in the dictionary. You do not have access to an external database for this verification.",
-      "error": "None if the provided information of the scientific literature is correct; otherwise, describe the error.",
-      "correction": "None if the provided information of the scientific literature is correct; otherwise, correct the information.",
-      "factuality": "True if the provided information is factual, False otherwise.",
-    }}
-  user_3_shot_CoT: |-
-    You are provided with a dictionary that contains details of a specific scientific literature. The dictionary contains three keys - 'paper_title', 'paper_author(s)', and 'paper_pub_year'. Your task is to use your own knowledge base to validate the following:
-    (1) Confirm if the paper actually exists and whether its title is accurate. The provided paper name should exactly matched the actual paper name.
-    (2) Compare the provided list of authors to that of the original paper, ensuring the provided authors are indeed a subset of the actual authors.
-    (3) Verify the accuracy of the year of publication.
-    Your response must be a dictionary with four keys - "reasoning", "error", "correction", and "factuality", which correspond to your logical process in verifying the dictionary's data integrity, the detection of any errors within the dictionary, rectifying any misinformation (if present), and finally confirming the factuality of the dictionary (Boolean - True or False).
-    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
-    [response format]: 
-    {{
-      "reasoning": "Your process of assessing the data integrity of the scientific literature details in the dictionary. Use your own knowledge base to verify the data integrity of the scientific literature details in the dictionary. You do not have access to an external database for this verification.",
-      "error": "None if the provided information of the scientific literature is correct; otherwise, describe the error.",
-      "correction": "None if the provided information of the scientific literature is correct; otherwise, correct the information.",
-      "factuality": "True if the provided information is factual, False otherwise.",
-    }}
-
-    Here are three examples:
-    [scientific literature]: {{"paper_title": "A Brief History of Time", "paper_author(s)": "Albert Einstein", "paper_pub_year": "1987"}}
-    [response]: {{"reasoning": "While 'A Brief History of Time' is a well-recognized scientific literature, it was not written by Albert Einstein as indicated in the provided dictionary. The actual author of this book is Stephen Hawking. Also, the publication year of 1987 is incorrect. The actual publication year should be 1988.", "error": "The author of 'A Brief History of Time' is incorrectly listed as Albert Einstein. Also, the publication year is incorrect.", "correction": {{"paper_title": "A Brief History of Time", "paper_author(s)": ["Stephen Hawking"], "paper_pub_year": "1988"}}, "factuality": False}}
-
-    [scientific literature]: {{"paper_title": "BART: Pre-training of Deep Bidirectional Transformers for Language Understanding", "paper_author(s)": "Devlin et al.", "paper_pub_year": "1960"}}
-    [response]: {{"reasoning": "The paper_title 'BART: Pre-training of Deep Bidirectional Transformers for Language Understanding' is incorrect. The actual paper title should be 'BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding'. The paper_author seems correct since Jacob Devlin is indeed in the author list of the BERT paper. Moreover, the year of publication is not consistent with the timeline of the development of such advanced AI models. The BERT paper was published in 2018, not 1960.", "error": "The 'paper_title' is incorrect and the 'paper_pub_year' is incorrect.", "correction": "{{"paper_title": "BART: Pre-training of Deep Bidirectional Transformers for Language Understanding", "paper_author(s)": ["Devlin et al."], "paper_pub_year": "2018"}}", "factuality": False}}
-
-    [scientific literature]: {{"paper_title": "Deep Learning", "paper_author(s)": "Yoshua Bengio, Ian Goodfellow, and Aaron Courville", "paper_pub_year": "2016"}}
-    [response]: {{"reasoning": "Upon reviewing the dictionary details with my knowledge base, I confirm that the title 'Deep Learning' is a well-known scientific literature in the field of artificial intelligence. Moreover, the authors listed, Yoshua Bengio, Ian Goodfellow, and Aaron Courville, are indeed the authors of this book. Lastly, this book was indeed published in the year 2016. Thus, the provided information is accurate.", "error": "None", "correction": "None", "factuality": True}}
-
-    Now complete the following:
-    [scientific literature]: {scientific_literature}
-    [response]: 
-
-
-
-
-
-
-
-
-
+knowledge_qa:
+  system: |-
+    You are a brilliant assistant.
+  user_zero_shot_CoT: |-
+    You are given a claim. Your task is to identify whether there are any factual errors within the claim.
+    The response must be a dictionary with 4 keys - "reasoning", "error", "corrected_claim", and "factuality", which correspond to the reasoning about whether the claim is factual, the factual error present in the claim (if any), the corrected claim (if needed), and whether the claim is factual or not (Boolean - True or False).
+    The following is the given claim - 
+    [claim]: {claim}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Reason about whether the claim is factual. Think step by step.",
+      "error": "None if the claim is factual; otherwise, describe the error.",
+      "corrected_claim": "None if the claim is factual; otherwise, write the corrected claim.",
+      "factuality": "True if the claim is factual, False otherwise."
+    }}
+  user_3_shot_CoT: |-
+    You are given a claim. Your task is to identify whether there are any factual errors within the claim.
+    The response must be a dictionary with 4 keys - "reasoning", "error", "corrected_claim", and "factuality", which correspond to the reasoning about whether the claim is factual, the factual error present in the claim (if any), the corrected claim (if needed), and whether the claim is factual or not (Boolean - True or False).
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Reason about whether the claim is factual. Think step by step.",
+      "error": "None if the claim is factual; otherwise, describe the error.",
+      "corrected_claim": "None if the claim is factual; otherwise, write the corrected claim.",
+      "factuality": "True if the claim is factual, False otherwise."
+    }}
+
+    Here are three examples:
+    [claim]: Albert Einstein was awarded the Nobel Prize in Physics in 1921 for his theory of relativity.
+    [response]: {{"reasoning": "Although Albert Einstein was indeed awarded the Nobel Prize in Physics in 1921, it was not for his theory of relativity, but rather for his discovery of the law of the photoelectric effect.", "error": "The claim incorrectly states that Einstein won the Nobel Prize for his theory of relativity.", "corrected_claim": "Albert Einstein was awarded the Nobel Prize in Physics in 1921 for his discovery of the law of the photoelectric effect.", "factuality": False}}
+
+    [claim]: The Titanic sank on its maiden voyage in 1912 after hitting an iceberg.
+    [response]: {{"reasoning": "This claim is accurate. The RMS Titanic, a British luxury passenger liner, did indeed sink during its maiden voyage in 1912 after colliding with an iceberg in the North Atlantic Ocean.", "error": "None", "corrected_claim": "None", "factuality": True}}
+
+    [claim]: The capital of Australia is Sydney.
+    [response]: {{"reasoning": "Despite Sydney being one of the most recognized and populated cities in Australia, it is not the capital. The capital of Australia is Canberra.", "error": "The claim incorrectly states that Sydney is the capital of Australia.", "corrected_claim": "The capital of Australia is Canberra.", "factuality": False}}
+
+    Now complete the following:
+    [claim]: {claim}
+    [response]: 
+
+code:
+  system: |-
+    You are a brilliant assistant.
+  user_zero_shot_CoT: |-
+    You are given a coding question and a potential solution to the coding question. Your task is to identify whether the potential solution solves the coding question correctly or not. You should check the potential solution line-by-line to see if the solution includes errors, such as syntax, logic, or runtime errors.
+    Your response must be a dictionary with four keys - "reasoning", "error", "corrected_solution", and "factuality", which correspond to the line-by-line reasoning about whether the potential solution contains errors, the coding error present in the potential solution (if any), the corrected solution (if necessary), and whether the potential solution solves the coding question correctly or not (a Boolean value of True or False).
+    The following is the given coding question and potential solution - 
+    [coding question]: {input_question}
+    [potential solution]: {input_solution}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "line-by-line reasoning about whether the potential solution contains errors.",
+      "error": "None if the potential solution correctly solves the coding question; otherwise, describe the error.",
+      "corrected_solution": "None if the potential solution is correct; otherwise, write the correct solution that correctly solves the coding question.",
+      "factuality": "True if the potential solution is correct, False otherwise."
+    }}
+  user_3_shot_CoT: |-
+    You are given a coding question and a potential solution to the coding question. Your task is to identify whether the potential solution solves the coding question correctly or not. You should check the potential solution line-by-line to see if the solution includes errors, such as syntax, logic, or runtime errors.
+    Your response must be a dictionary with four keys - "reasoning", "error", "corrected_solution", and "factuality", which correspond to the line-by-line reasoning about whether the potential solution contains errors, the coding error present in the potential solution (if any), the corrected solution (if necessary), and whether the potential solution solves the coding question correctly or not (a Boolean value of True or False).
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS BANNED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "line-by-line reasoning about whether the potential solution contains errors.",
+      "error": "None if the potential solution correctly solves the coding question; otherwise, describe the error.",
+      "corrected_solution": "None if the potential solution is correct; otherwise, write the correct solution that correctly solves the coding question.",
+      "factuality": "True if the potential solution is correct, False otherwise."
+    }}
+
+    Here are three examples:
+    [coding question]: Write a Python function that takes a list of integers as input and returns the sum of all the elements in the list.
+    [potential solution]: "def sum_list(input_list):\n    sum = 0\n    for i in input_list:\n        sum += i\n    return sum"
+    [response]: {{"reasoning": "The function correctly iterates over each element in the list and adds it to a running sum, which is then returned.", "error": "None", "corrected_solution": "None", "factuality": True}}
+
+    [coding question]: Write a Python function that checks if a given string is a palindrome or not. A palindrome is a word, phrase, number, or other sequence of characters that reads the same forward or backward, allowing for adjustments to punctuation and spaces.
+    [potential solution]: "def is_palindrome(input_string):\n    reversed_string = input_string[::-1]\n    if input_string == reversed_string:\n        return True\n    else:\n        return False"
+    [response]: {{"reasoning": "The function correctly reverses the input string and compares it with the original string to check if it's a palindrome. However, it doesn't account for possible spaces and punctuation, which are supposed to be ignored while checking for palindromes.", "error": "The function does not ignore spaces and punctuation while checking for palindromes.", "corrected_solution": "def is_palindrome(input_string):\n    input_string = ''.join(c for c in input_string if c.isalnum()).lower()\n    reversed_string = input_string[::-1]\n    if input_string == reversed_string:\n        return True\n    else:\n        return False", "factuality": False}}
+
+    [coding question]: Write a Python function that takes a list of integers as input and returns the average of all the elements in the list.
+    [potential solution]: "def average(input_list):\n    sum = 0\n    for i in input_list:\n        sum += i\n    return sum"
+    [response]: {{"reasoning": "The function correctly calculates the sum of all elements in the list, but it does not divide this sum by the number of elements in the list, which is necessary for finding the average.", "error": "The function does not calculate the average correctly because it does not divide the sum by the number of elements.", "corrected_solution": "def average(input_list):\n    sum = 0\n    for i in input_list:\n        sum += i\n    return sum / len(input_list)", "factuality": False}}
+
+    Now complete the following:
+    [coding question]: {input_question}
+    [potential solution]: {input_solution}
+    [response]: 
+
+math:
+  system: |-
+    You are a brilliant assistant.
+  user_zero_shot_CoT: |-
+    You are given a math calculation and a proposed calculated answer to this calculation. Your task is to verify whether the calculated answer solves the math calculation correctly or not.
+    Your response must be a dictionary with three keys - "reasoning", "corrected_answer", and "factuality", which correspond to the reasoning about whether the calculated answer is correct, the corrected calculated answer (if necessary), and whether the calculated answer correctly solves the math calculation or not (a Boolean value of True or False).
+    The following is the given math calculation and proposed calculated answer - 
+    [math calculation]: {input_calculation}
+    [proposed calculated answer]: {input_calculated_answer}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS PROHIBITED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Reason about whether the calculated answer is correct.",
+      "corrected_answer": "None if the calculated answer is correct; otherwise, write the corrected answer that correctly solves the math problem.",
+      "factuality": "True if the calculated answer is correct, False otherwise."
+    }}
+  user_3_shot_CoT: |-
+    You are given a math calculation and a proposed calculated answer to this calculation. Your task is to verify whether the calculated answer solves the math calculation correctly or not.
+    Your response must be a dictionary with three keys - "reasoning", "corrected_answer", and "factuality", which correspond to the reasoning about whether the calculated answer is correct, the corrected calculated answer (if necessary), and whether the calculated answer correctly solves the math calculation or not (a Boolean value of True or False).
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. ADDING ANY OTHER EXTRA NOTES THAT VIOLATE THE RESPONSE FORMAT IS PROHIBITED. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Reason about whether the calculated answer is correct.",
+      "corrected_answer": "None if the calculated answer is correct; otherwise, write the corrected answer that correctly solves the math problem.",
+      "factuality": "True if the calculated answer is correct, False otherwise."
+    }}
+
+    Here are three examples:
+    [math calculation]: 8 * 9
+    [proposed calculated answer]: 72
+    [response]: {{"reasoning": "The calculation involves a multiplication operation of 8 and 9. The correct answer of this operation is indeed 72.", "corrected_answer": "None", "factuality": True}}
+
+    [math calculation]: 15 / 5
+    [proposed calculated answer]: 5
+    [response]: {{"reasoning": "The calculation involves a division operation of 15 by 5. The correct answer should be 3, not 5.", "corrected_answer": 3, "factuality": False}}
+
+    [math calculation]: 45 - 20
+    [proposed calculated answer]: 30
+    [response]: {{"reasoning": "The calculation involves a subtraction operation of 45 minus 20. The correct answer should be 25, not 30.", "corrected_answer": 25, "factuality": False}}
+
+    Now complete the following:
+    [math calculation]: {input_calculation}
+    [proposed calculated answer]: {input_calculated_answer}
+    [response]: 
+
+scientific:
+  system: |-
+    You are a brilliant assistant.
+  user_zero_shot_CoT: |-
+    You are provided with a dictionary that contains details of a specific scientific literature. The dictionary contains three keys - 'paper_title', 'paper_author(s)', and 'paper_pub_year'. Your task is to use your own knowledge base to validate the following:
+    (1) Confirm if the paper actually exists and whether its title is accurate. The provided paper name should exactly matched the actual paper name.
+    (2) Compare the provided list of authors to that of the original paper, ensuring the provided authors are indeed a subset of the actual authors.
+    (3) Verify the accuracy of the year of publication.
+    Your response must be a dictionary with four keys - "reasoning", "error", "correction", and "factuality", which correspond to your logical process in verifying the dictionary's data integrity, the detection of any errors within the dictionary, rectifying any misinformation (if present), and finally confirming the factuality of the dictionary (Boolean - True or False).
+    The following is the given dictionary that contains details of a scientific literature - 
+    [scientific literature]: {scientific_literature}
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Your process of assessing the data integrity of the scientific literature details in the dictionary. Use your own knowledge base to verify the data integrity of the scientific literature details in the dictionary. You do not have access to an external database for this verification.",
+      "error": "None if the provided information of the scientific literature is correct; otherwise, describe the error.",
+      "correction": "None if the provided information of the scientific literature is correct; otherwise, correct the information.",
+      "factuality": "True if the provided information is factual, False otherwise.",
+    }}
+  user_3_shot_CoT: |-
+    You are provided with a dictionary that contains details of a specific scientific literature. The dictionary contains three keys - 'paper_title', 'paper_author(s)', and 'paper_pub_year'. Your task is to use your own knowledge base to validate the following:
+    (1) Confirm if the paper actually exists and whether its title is accurate. The provided paper name should exactly matched the actual paper name.
+    (2) Compare the provided list of authors to that of the original paper, ensuring the provided authors are indeed a subset of the actual authors.
+    (3) Verify the accuracy of the year of publication.
+    Your response must be a dictionary with four keys - "reasoning", "error", "correction", and "factuality", which correspond to your logical process in verifying the dictionary's data integrity, the detection of any errors within the dictionary, rectifying any misinformation (if present), and finally confirming the factuality of the dictionary (Boolean - True or False).
+    You MUST only respond in the format as described below. DO NOT RESPOND WITH ANYTHING ELSE. START YOUR RESPONSE WITH '{{'.
+    [response format]: 
+    {{
+      "reasoning": "Your process of assessing the data integrity of the scientific literature details in the dictionary. Use your own knowledge base to verify the data integrity of the scientific literature details in the dictionary. You do not have access to an external database for this verification.",
+      "error": "None if the provided information of the scientific literature is correct; otherwise, describe the error.",
+      "correction": "None if the provided information of the scientific literature is correct; otherwise, correct the information.",
+      "factuality": "True if the provided information is factual, False otherwise.",
+    }}
+
+    Here are three examples:
+    [scientific literature]: {{"paper_title": "A Brief History of Time", "paper_author(s)": "Albert Einstein", "paper_pub_year": "1987"}}
+    [response]: {{"reasoning": "While 'A Brief History of Time' is a well-recognized scientific literature, it was not written by Albert Einstein as indicated in the provided dictionary. The actual author of this book is Stephen Hawking. Also, the publication year of 1987 is incorrect. The actual publication year should be 1988.", "error": "The author of 'A Brief History of Time' is incorrectly listed as Albert Einstein. Also, the publication year is incorrect.", "correction": {{"paper_title": "A Brief History of Time", "paper_author(s)": ["Stephen Hawking"], "paper_pub_year": "1988"}}, "factuality": False}}
+
+    [scientific literature]: {{"paper_title": "BART: Pre-training of Deep Bidirectional Transformers for Language Understanding", "paper_author(s)": "Devlin et al.", "paper_pub_year": "1960"}}
+    [response]: {{"reasoning": "The paper_title 'BART: Pre-training of Deep Bidirectional Transformers for Language Understanding' is incorrect. The actual paper title should be 'BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding'. The paper_author seems correct since Jacob Devlin is indeed in the author list of the BERT paper. Moreover, the year of publication is not consistent with the timeline of the development of such advanced AI models. The BERT paper was published in 2018, not 1960.", "error": "The 'paper_title' is incorrect and the 'paper_pub_year' is incorrect.", "correction": "{{"paper_title": "BART: Pre-training of Deep Bidirectional Transformers for Language Understanding", "paper_author(s)": ["Devlin et al."], "paper_pub_year": "2018"}}", "factuality": False}}
+
+    [scientific literature]: {{"paper_title": "Deep Learning", "paper_author(s)": "Yoshua Bengio, Ian Goodfellow, and Aaron Courville", "paper_pub_year": "2016"}}
+    [response]: {{"reasoning": "Upon reviewing the dictionary details with my knowledge base, I confirm that the title 'Deep Learning' is a well-known scientific literature in the field of artificial intelligence. Moreover, the authors listed, Yoshua Bengio, Ian Goodfellow, and Aaron Courville, are indeed the authors of this book. Lastly, this book was indeed published in the year 2016. Thus, the provided information is accurate.", "error": "None", "correction": "None", "factuality": True}}
+
+    Now complete the following:
+    [scientific literature]: {scientific_literature}
+    [response]: 
+
+
+
+
+
+
+
+
+
```

### Comparing `factool-0.0.1/factool.egg-info/SOURCES.txt` & `factool-0.0.7/factool.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,18 +28,13 @@
 factool/scientific/__init__.py
 factool/scientific/pipeline.py
 factool/scientific/tool.py
 factool/utils/__init_.py
 factool/utils/claim_extractor.py
 factool/utils/openai_wrapper.py
 factool/utils/utils_json.py
-factool/utils/__pycache__/CustomJSONEncoder.cpython-38.pyc
-factool/utils/__pycache__/openai_wrapper.cpython-38.pyc
-factool/utils/__pycache__/utils_json.cpython-38.pyc
 factool/utils/base/__init__.py
 factool/utils/base/pipeline.py
-factool/utils/base/__pycache__/__init__.cpython-38.pyc
-factool/utils/base/__pycache__/pipeline.cpython-38.pyc
 factool/utils/prompts/agreement_verification.yaml
 factool/utils/prompts/claim_extraction.yaml
 factool/utils/prompts/query_generation.yaml
 factool/utils/prompts/self_check.yaml
```

### Comparing `factool-0.0.1/setup.cfg` & `factool-0.0.7/setup.cfg`

 * *Files identical despite different names*

