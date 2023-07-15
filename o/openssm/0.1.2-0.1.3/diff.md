# Comparing `tmp/openssm-0.1.2.tar.gz` & `tmp/openssm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssm-0.1.2.tar", max compression
+gzip compressed data, was "openssm-0.1.3.tar", max compression
```

## Comparing `openssm-0.1.2.tar` & `openssm-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     6946 2023-07-14 16:35:00.896701 openssm-0.1.2/README.md
--rw-r--r--   0        0        0       79 2023-07-07 18:20:26.251547 openssm-0.1.2/openssm/Makefile
--rw-r--r--   0        0        0     2553 2023-07-10 09:13:36.452086 openssm-0.1.2/openssm/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.796606 openssm-0.1.2/openssm/__init__.py
--rw-r--r--   0        0        0      899 2023-07-12 04:07:00.397143 openssm-0.1.2/openssm/config.py
--rw-r--r--   0        0        0      754 2023-07-12 04:07:00.397716 openssm-0.1.2/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
--rw-r--r--   0        0        0      789 2023-07-12 04:07:00.397936 openssm-0.1.2/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
--rw-r--r--   0        0        0     1010 2023-07-12 04:07:00.398136 openssm-0.1.2/openssm/contrib/ssms/mri_operator_ssm/__init__.py
--rw-r--r--   0        0        0     1610 2023-07-12 04:07:00.398292 openssm-0.1.2/openssm/contrib/ssms/semiconductor_ssm/__init__.py
--rw-r--r--   0        0        0       19 2023-06-30 08:00:20.798353 openssm-0.1.2/openssm/core/__init__.py
--rw-r--r--   0        0        0     2203 2023-07-14 05:15:42.916155 openssm-0.1.2/openssm/core/adapter/abstract_adapter.py
--rw-r--r--   0        0        0     3399 2023-07-14 16:15:33.092368 openssm-0.1.2/openssm/core/adapter/base_adapter.py
--rw-r--r--   0        0        0     2926 2023-07-14 02:34:13.823441 openssm-0.1.2/openssm/core/adapter/llama_index_adapter.py
--rw-r--r--   0        0        0     1159 2023-07-14 02:34:13.823890 openssm-0.1.2/openssm/core/backend/abstract_backend.py
--rw-r--r--   0        0        0     1595 2023-07-14 15:59:33.058040 openssm-0.1.2/openssm/core/backend/base_backend.py
--rw-r--r--   0        0        0     1658 2023-07-14 02:34:13.824322 openssm-0.1.2/openssm/core/backend/text_backend.py
--rw-r--r--   0        0        0      720 2023-07-10 18:00:54.628456 openssm-0.1.2/openssm/core/inferencer/abstract_inferencer.py
--rw-r--r--   0        0        0      458 2023-07-12 04:07:00.400091 openssm-0.1.2/openssm/core/inferencer/base_inferencer.py
--rw-r--r--   0        0        0      885 2023-07-12 04:07:00.400461 openssm-0.1.2/openssm/core/slm/abstract_slm.py
--rw-r--r--   0        0        0     1626 2023-07-12 04:07:00.400690 openssm-0.1.2/openssm/core/slm/base_slm.py
--rw-r--r--   0        0        0     6760 2023-07-14 02:34:13.824686 openssm-0.1.2/openssm/core/slm/huggingface_slm.py
--rw-r--r--   0        0        0      417 2023-07-07 18:30:35.408067 openssm-0.1.2/openssm/core/slm/memory/conversation_db.py
--rw-r--r--   0        0        0     1620 2023-07-12 04:07:00.401194 openssm-0.1.2/openssm/core/slm/memory/sqlite_conversation_db.py
--rw-r--r--   0        0        0     2053 2023-07-12 04:07:00.401379 openssm-0.1.2/openssm/core/slm/openai_slm.py
--rw-r--r--   0        0        0     2307 2023-07-12 04:07:00.401590 openssm-0.1.2/openssm/core/ssm/abstract_ssm.py
--rw-r--r--   0        0        0     3037 2023-07-12 04:07:00.401769 openssm-0.1.2/openssm/core/ssm/base_ssm.py
--rw-r--r--   0        0        0      454 2023-07-14 02:34:13.824917 openssm-0.1.2/openssm/core/ssm/gpt3_llama_index_ssm.py
--rw-r--r--   0        0        0      747 2023-07-12 04:07:00.402181 openssm-0.1.2/openssm/core/ssm/huggingface_ssm.py
--rw-r--r--   0        0        0      770 2023-07-14 02:34:13.825086 openssm-0.1.2/openssm/core/ssm/openai_ssm.py
--rw-r--r--   0        0        0       58 2023-06-30 08:00:20.803155 openssm-0.1.2/openssm/industrial/interpretability/README.md
--rw-r--r--   0        0        0       60 2023-06-30 08:00:20.803373 openssm-0.1.2/openssm/industrial/monitoring/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803462 openssm-0.1.2/openssm/industrial/security/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803611 openssm-0.1.2/openssm/industrial/security/audit/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803745 openssm-0.1.2/openssm/industrial/security/best_practices/README.md
--rw-r--r--   0        0        0       63 2023-06-30 08:00:20.803985 openssm-0.1.2/openssm/integration/README.md
--rw-r--r--   0        0        0     3574 2023-06-30 08:00:20.804216 openssm-0.1.2/openssm/integration/llamaindex/README.md
--rw-r--r--   0        0        0       34 2023-06-30 08:00:20.804401 openssm-0.1.2/openssm/integration/testing_tools/README.md
--rw-r--r--   0        0        0      688 2023-07-15 00:47:49.708064 openssm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7709 1970-01-01 00:00:00.000000 openssm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     6946 2023-07-14 16:35:00.896701 openssm-0.1.3/README.md
+-rw-r--r--   0        0        0       79 2023-07-07 18:20:26.251547 openssm-0.1.3/openssm/Makefile
+-rw-r--r--   0        0        0     2553 2023-07-10 09:13:36.452086 openssm-0.1.3/openssm/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.796606 openssm-0.1.3/openssm/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-12 04:07:00.397143 openssm-0.1.3/openssm/config.py
+-rw-r--r--   0        0        0      754 2023-07-12 04:07:00.397716 openssm-0.1.3/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-12 04:07:00.397936 openssm-0.1.3/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
+-rw-r--r--   0        0        0     1010 2023-07-12 04:07:00.398136 openssm-0.1.3/openssm/contrib/ssms/mri_operator_ssm/__init__.py
+-rw-r--r--   0        0        0     1610 2023-07-12 04:07:00.398292 openssm-0.1.3/openssm/contrib/ssms/semiconductor_ssm/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-30 08:00:20.798353 openssm-0.1.3/openssm/core/__init__.py
+-rw-r--r--   0        0        0     2203 2023-07-14 05:15:42.916155 openssm-0.1.3/openssm/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0     3399 2023-07-14 16:15:33.092368 openssm-0.1.3/openssm/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     2926 2023-07-14 02:34:13.823441 openssm-0.1.3/openssm/core/adapter/llama_index_adapter.py
+-rw-r--r--   0        0        0     1159 2023-07-14 02:34:13.823890 openssm-0.1.3/openssm/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0     1595 2023-07-14 15:59:33.058040 openssm-0.1.3/openssm/core/backend/base_backend.py
+-rw-r--r--   0        0        0     1658 2023-07-14 02:34:13.824322 openssm-0.1.3/openssm/core/backend/text_backend.py
+-rw-r--r--   0        0        0      720 2023-07-10 18:00:54.628456 openssm-0.1.3/openssm/core/inferencer/abstract_inferencer.py
+-rw-r--r--   0        0        0      458 2023-07-12 04:07:00.400091 openssm-0.1.3/openssm/core/inferencer/base_inferencer.py
+-rw-r--r--   0        0        0      885 2023-07-12 04:07:00.400461 openssm-0.1.3/openssm/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0     1626 2023-07-12 04:07:00.400690 openssm-0.1.3/openssm/core/slm/base_slm.py
+-rw-r--r--   0        0        0     6760 2023-07-14 02:34:13.824686 openssm-0.1.3/openssm/core/slm/huggingface_slm.py
+-rw-r--r--   0        0        0      417 2023-07-07 18:30:35.408067 openssm-0.1.3/openssm/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     1620 2023-07-12 04:07:00.401194 openssm-0.1.3/openssm/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     2053 2023-07-12 04:07:00.401379 openssm-0.1.3/openssm/core/slm/openai_slm.py
+-rw-r--r--   0        0        0     2307 2023-07-12 04:07:00.401590 openssm-0.1.3/openssm/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     3037 2023-07-12 04:07:00.401769 openssm-0.1.3/openssm/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0      454 2023-07-14 02:34:13.824917 openssm-0.1.3/openssm/core/ssm/gpt3_llama_index_ssm.py
+-rw-r--r--   0        0        0      747 2023-07-12 04:07:00.402181 openssm-0.1.3/openssm/core/ssm/huggingface_ssm.py
+-rw-r--r--   0        0        0      770 2023-07-14 02:34:13.825086 openssm-0.1.3/openssm/core/ssm/openai_ssm.py
+-rw-r--r--   0        0        0       58 2023-06-30 08:00:20.803155 openssm-0.1.3/openssm/industrial/interpretability/README.md
+-rw-r--r--   0        0        0       60 2023-06-30 08:00:20.803373 openssm-0.1.3/openssm/industrial/monitoring/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803462 openssm-0.1.3/openssm/industrial/security/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803611 openssm-0.1.3/openssm/industrial/security/audit/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803745 openssm-0.1.3/openssm/industrial/security/best_practices/README.md
+-rw-r--r--   0        0        0       63 2023-06-30 08:00:20.803985 openssm-0.1.3/openssm/integration/README.md
+-rw-r--r--   0        0        0     3574 2023-06-30 08:00:20.804216 openssm-0.1.3/openssm/integration/llamaindex/README.md
+-rw-r--r--   0        0        0       34 2023-06-30 08:00:20.804401 openssm-0.1.3/openssm/integration/testing_tools/README.md
+-rw-r--r--   0        0        0      690 2023-07-15 04:41:43.824823 openssm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7703 1970-01-01 00:00:00.000000 openssm-0.1.3/PKG-INFO
```

### Comparing `openssm-0.1.2/LICENSE.md` & `openssm-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/README.md` & `openssm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/README.md` & `openssm-0.1.3/openssm/README.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/config.py` & `openssm-0.1.3/openssm/config.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py` & `openssm-0.1.3/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py` & `openssm-0.1.3/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/contrib/ssms/mri_operator_ssm/__init__.py` & `openssm-0.1.3/openssm/contrib/ssms/mri_operator_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/contrib/ssms/semiconductor_ssm/__init__.py` & `openssm-0.1.3/openssm/contrib/ssms/semiconductor_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/adapter/abstract_adapter.py` & `openssm-0.1.3/openssm/core/adapter/abstract_adapter.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/adapter/base_adapter.py` & `openssm-0.1.3/openssm/core/adapter/base_adapter.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/adapter/llama_index_adapter.py` & `openssm-0.1.3/openssm/core/adapter/llama_index_adapter.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/backend/abstract_backend.py` & `openssm-0.1.3/openssm/core/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/backend/base_backend.py` & `openssm-0.1.3/openssm/core/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/backend/text_backend.py` & `openssm-0.1.3/openssm/core/backend/text_backend.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/inferencer/abstract_inferencer.py` & `openssm-0.1.3/openssm/core/inferencer/abstract_inferencer.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/slm/abstract_slm.py` & `openssm-0.1.3/openssm/core/slm/abstract_slm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/slm/base_slm.py` & `openssm-0.1.3/openssm/core/slm/base_slm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/slm/huggingface_slm.py` & `openssm-0.1.3/openssm/core/slm/huggingface_slm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/slm/memory/sqlite_conversation_db.py` & `openssm-0.1.3/openssm/core/slm/memory/sqlite_conversation_db.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/slm/openai_slm.py` & `openssm-0.1.3/openssm/core/slm/openai_slm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/ssm/abstract_ssm.py` & `openssm-0.1.3/openssm/core/ssm/abstract_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/ssm/base_ssm.py` & `openssm-0.1.3/openssm/core/ssm/base_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/ssm/huggingface_ssm.py` & `openssm-0.1.3/openssm/core/ssm/huggingface_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/core/ssm/openai_ssm.py` & `openssm-0.1.3/openssm/core/ssm/openai_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/openssm/integration/llamaindex/README.md` & `openssm-0.1.3/openssm/integration/llamaindex/README.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.2/pyproject.toml` & `openssm-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Aitomatic Engineering <engineering@aitomatic.com>"]
 description = "OpenSSM – 'Small Specialist Models' for Industrial AI"
 name = "openssm"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
@@ -16,11 +16,11 @@
 llama-index = ">=0.6.33"
 # misc / other
 accelerate = "^0.20.3"
 einops = "^0.6.1"
 pypdf = ">=3.11.0"
 pytest = ">=7.0.0"
 transformers = "^4.30.2"
-torch = "^2.0.1"
+torch = ">=1.13.1"
 #torch = ">=1.13.1"
 #xformers = ">=0.0.16"	# don’t include this. It fails on GitHub actions. Support in Makefile.
 #xformers = ">=0.0.20"
```

### Comparing `openssm-0.1.2/PKG-INFO` & `openssm-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openssm
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenSSM – 'Small Specialist Models' for Industrial AI
 Author: Aitomatic Engineering
 Author-email: engineering@aitomatic.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: einops (>=0.6.1,<0.7.0)
 Requires-Dist: llama-hub (>=0.0.4)
 Requires-Dist: llama-index (>=0.6.33)
 Requires-Dist: pypdf (>=3.11.0)
 Requires-Dist: pytest (>=7.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torch (>=1.13.1)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenSSM – “Small Specialist Models” for Industrial AI
 
 OpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing trust, reliability, and safety in Industrial-AI applications.  Harnessing the power of domain expertise, SSMs operate either alone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving capabilities.
```

