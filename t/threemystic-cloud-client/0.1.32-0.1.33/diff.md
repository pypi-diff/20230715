# Comparing `tmp/threemystic_cloud_client-0.1.32.tar.gz` & `tmp/threemystic_cloud_client-0.1.33.tar.gz`

## Comparing `threemystic_cloud_client-0.1.32.tar` & `threemystic_cloud_client-0.1.33.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/action_generate/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    23700 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/pyproject.toml
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/action_generate/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0    32978 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.33/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/action_generate/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/action_generate/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 class cloud_client_aws_client_auto(base):
   def __init__(self, *args, **kwargs):
     super().__init__(logger_name= "cloud_client_aws_auto", *args, **kwargs)
 
     self.__set_profile(*args, **kwargs)
   
+  def get_resource_group_from_resource(self, account, *args, **kwargs):
+    pass
   
   def get_profile(self, *args, **kwargs):
     if(not hasattr(self, "_profile")):
       raise self.get_common().exception().exception(
           exception_type = "generic"
         ).type_error(
           logger = self.get_common().get_logger(),
```

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,112 @@
+from threemystic_cloud_client.cloud_providers.base_class.base import cloud_client_provider_base as base
 import os
-from abc import abstractmethod
-from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
 from botocore import session as botocore_session, credentials as botocore_credentials
 from botocore.config import Config as botocore_config_config
 from boto3 import Session as boto_session
 from botocore.exceptions import ClientError
 from polling2 import TimeoutException, poll as poll2
 import time
 from random import randint
 
-class cloud_client_aws_client_base(base):
+
+class cloud_client_provider_aws_base(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(*args, **kwargs)
+    # https://github.com/boto/botocore/issues/2705 
+    # This update should be temporary until boto version 1.28 is released
+    os.environ["BOTO_DISABLE_COMMONNAME"] = "true" 
+
+    super().__init__(provider= "aws", *args, **kwargs)   
+    self.links = {
+      "cli_doc_link": "https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html",
+      "ssm_doc_link": "https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html",
+      "saml2aws_doc_link": "https://github.com/Versent/saml2aws"
+    }
 
-    self.__set_profile(*args, **kwargs)
-  
-  @abstractmethod
-  def _session_expired(self, refresh = False, *args, **kwargs):
-    pass
+  def get_account_name(self, account):
+    if account is None:
+      return None
+    if self.get_common().helper_type().general().is_type(obj= account, type_check= str):
+      return account.strip()
+
+    if account.get("Name"):
+      return account["Name"].strip()
+    
+    if account.get("accountName"):
+      self.get_common().get_logger().warning("accountName will be depreciated use Name")
+      return account["accountName"].strip()
+    
+    raise self.get_common().exception().exception(
+      exception_type = "generic"
+    ).not_implemented(
+      logger = self.get_common().get_logger(),
+      name = "account",
+      message = f"Unknown account object: {account}."
+    )
+
+  def get_account_id(self, account):
+    if account is None:
+      return None
+    if self.get_common().helper_type().general().is_type(obj= account, type_check= str):
+      return self.get_common().helper_type().string().trim(string_value=self.get_common().helper_type().string().set_case(string_value= account, case= "lower"))
+    
+    if account.get("Id"):
+      return self.get_common().helper_type().string().trim(string_value=self.get_common().helper_type().string().set_case(string_value= account["Id"], case= "lower"))
+
+    if account.get("accountId"):
+      self.get_common().get_logger().warning("accountId will be depreciated use Id")
+      return self.get_common().helper_type().string().trim(string_value=self.get_common().helper_type().string().set_case(string_value= account["accountId"], case= "lower"))
+    
+    raise self.get_common().exception().exception(
+      exception_type = "generic"
+    ).not_implemented(
+      logger = self.get_common().get_logger(),
+      name = "account",
+      message = f"Unknown account object: {account}."
+    )
   
+  def make_account(self, **kwargs):    
+    account = {}
+    if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= kwargs.get("accountId")):
+      self.get_common().get_logger().warning("accountId will be depreciated use Id")
+      account["accountId"] = self.get_common().helper_type().string().trim(string_value=self.get_common().helper_type().string().set_case(string_value= kwargs.get("accountId"), case= "lower"))
+      account["Id"] = self.get_common().helper_type().string().trim(string_value=self.get_common().helper_type().string().set_case(string_value= kwargs.get("accountId"), case= "lower"))
+
+    if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= kwargs.get("Id")):
+      account["Id"] = self.get_common().helper_type().string().trim(string_value=self.get_common().helper_type().string().set_case(string_value= kwargs.get("Id"), case= "lower"))
+
+    if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= kwargs.get("accountName")):
+      self.get_common().get_logger().warning("accountName will be depreciated use Name")
+      account["accountName"] = self.get_common().helper_type().string().trim(string_value=kwargs.get("accountName"))
+      account["Name"] = self.get_common().helper_type().string().trim(string_value=kwargs.get("accountName"))
+
+    if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= kwargs.get("Name")):
+      account["Name"] = self.get_common().helper_type().string().trim(string_value=kwargs.get("Name"))
+    
+    return account
+  
+  @property
+  def default_region_resources(self):
+    if hasattr(self, "_default_region_resources"):
+      return self._default_region_resources
+    
+    return ["us-east-1"]
+  
+  @default_region_resources.setter
+  def _set_default_region_resources(self, value):
+    self._default_region_resources = value
+
   def get_resource_general_arn(cls, resource_type = None, resource_type_sub = None, account_id = None, region = None, id = None, data_item = None, **kwargs ):
     if data_item is not None:
       lower_keys = [key.lower() for key in data_item.keys()]
       if "arn" in lower_keys:
         arn_key = list(data_item.keys())[lower_keys.index("arn")]
-        return data_item[arn_key]
+        return self.get_common().helper_type().string().set_case(string_value= data_item[arn_key], case= "lower")
 
-    return f'arn:aws:{resource_type}:{region}:{account_id}:{resource_type_sub}/{id}'
+    return self.get_common().helper_type().string().set_case(string_value= f'arn:aws:{resource_type}:{region}:{account_id}:{resource_type_sub}/{id}', case= "lower")
   
   def _get_boto_client_key(self, client, account = None, region = None, *args, **kwargs):
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region):
       region = self.get_default_region()
 
     if account is None or (self.get_common().helper_type().general().is_type(obj= account, type_check= str) and self.get_common().helper_type().string().is_null_or_whitespace(string_value= account)):
@@ -106,50 +182,15 @@
   
   def __set_profile(self, profile_data = None, *args, **kwargs):
     if profile_data is None:
       self._profile = self.get_default_profile()
       return
       
     self._profile = profile_data
-
-  def _post_init(self, *args, **kwargs):
-    self._load_base_configs()
   
-  @abstractmethod
-  def _load_base_configs(self):
-    pass
-  
-  @abstractmethod
-  def get_main_account_id(self, *args, **kwargs):
-    pass
-
-  @abstractmethod
-  def get_organization_account_id(self, *args, **kwargs):
-    pass
-  
-  @abstractmethod
-  def _assume_role(self, *args, **kwargs):    
-    pass
-  
-  @abstractmethod
-  def get_default_rolename(self, *args, **kwargs):
-    pass
-  
-  @abstractmethod
-  def get_default_region(self, *args, **kwargs):
-    pass
-  
-  @abstractmethod
-  def get_default_account(self, *args, **kwargs):
-    pass
-  
-  @abstractmethod
-  def authenticate_session(self, *args, **kwargs):
-    pass
-
   async def async_general_boto_call_array(self, *args, **kwargs):
     return self.general_boto_call_array(*args, **kwargs)
   
   async def async_general_boto_call_single(self, *args, **kwargs):
     return self.general_boto_call_single(*args, **kwargs)
   
   def general_boto_call_single(self, *args, **kwargs):
@@ -472,14 +513,101 @@
 
     session._credentials = credentials 
     session.set_config_variable("region", region)
       
     self._get_created_boto_sessions()[cache_key] = boto_session(botocore_session= session)
     return self.get_boto_session(account=account, role = role, region = region, profile = profile, *args, **kwargs)
   
+  def _get_account_regions_costexplorer(self, account, services = None, *args, **kwargs ):
+    
+    ce_client = self.get_boto_client(
+      client= "ce",
+      account=account
+    )
+
+    filter = {}
+    granularity = "DAILY"
+    
+    utc_now = self.get_common().helper_type().datetime().get()
+    time_period = {
+      "Start":(self.get_common().helper_type().datetime().datetime_as_string(
+        dt= (utc_now + self.get_common().helper_type().datetime().time_delta(monts= -1, dt= utc_now)),
+        dt_format= "%Y-%m-%d"
+      )),
+      "End": (self.get_common().helper_type().datetime().datetime_as_string(
+        dt= utc_now,
+        dt_format= "%Y-%m-%d"
+      ))
+    }   
+    metrics = ["NET_UNBLENDED_COST"]
+    group_by= [{"Type":"DIMENSION", "Key":"REGION"}]
+
+    get_cost_usage_params = {
+      "Granularity":granularity,
+      "TimePeriod": time_period,
+      "Metrics": metrics,
+      "GroupBy": group_by
+    }
+
+    if not services is None:
+      filter["Dimensions"] = {
+        "Key": "SERVICE",
+        "Values": services,
+        "MatchOptions": ["EQUALS", "CASE_SENSITIVE"]
+      }
+      get_cost_usage_params["Filter"] = filter
+
+
+    try:
+      discovered_resultsbytime = self.general_boto_call_array(
+        boto_call = lambda item: ce_client.get_cost_and_usage(**item),
+        boto_params = get_cost_usage_params,
+        boto_nextkey = "NextToken",
+        boto_key="ResultsByTime"
+      )
+
+      regions = []
+
+      for itemTime in discovered_resultsbytime:
+        for itemGroup in itemTime["Groups"]:
+          for item in itemGroup["Keys"]:
+            if self.get_common().helper_type().string().set_case(string_value= item, case= "lower") == "noregion":
+              continue
+            if not item in regions:
+              regions.append(item)
+      return regions
+    except Exception as err:
+      self.get_common().get_logger().exception(msg=f"Could not pull regions dynamically: {err}", exc_info= err)
+      return self.default_region_resources
+    
+  def get_accounts_regions_costexplorer(self, accounts, services, role= None):     
+    if role is None:
+      role = self.get_default_rolename()
+    regions = { }
+    
+    for account in accounts:      
+      regions[self.get_account_id(account)] = self.get_account_regions_costexplorer(
+        account=account,
+        role=role,
+        services= services
+      )
+
+    return regions
+
+  def get_account_regions_costexplorer(self, account, role, services):     
+    # to get a list of all services for an account
+    # aws ce get-dimension-values --time-period "Start=2022-09-01,End=2022-09-11" --dimension SERVICE
+    regions = { }
+
+    return self._get_account_regions_costexplorer(
+      account= account, 
+      role= role,
+      services= services
+    )
+  
   def _get_accounts(self, refresh = False, include_suspended = False):
     
     if hasattr(self, "_account_list") and not refresh:
       return_list = "active" if not include_suspended else "all"
       if self._account_list is not None and len(self._account_list) > 0:
         if return_list in self._account_list:
           return self._account_list[return_list]
@@ -540,9 +668,95 @@
     search_accounts = [ self.get_account_id(account= acct) for acct in account if not self.get_account_id(account= acct) .startswith("ou-") and not self.get_account_id(account= acct) .startswith("-") ]
     search_accounts_ous = [ self.get_account_id(account= acct)  for acct in account if self.get_account_id(account= acct) .startswith("ou-") ]
     exclude_accounts_ous = [ self.get_account_id(account= acct)  for acct in account if self.get_account_id(account= acct) .startswith("-ou-") ]
     exclude_accounts = [ self.get_account_id(account= acct)  for acct in account if self.get_account_id(account= acct).startswith("-") and not self.get_account_id(account= acct).startswith("-ou-") ]
     account = list(dict.fromkeys(search_accounts + self.get_accountids_by_ou(org_ou= search_accounts_ous, exclude_ous= exclude_accounts_ous)))
 
     return [ acct for acct in all_accounts if f'-{self.get_account_id(account= acct) }' not in exclude_accounts and  (len(account) < 1 or self.get_common().helper_type().list().find_item(data= account, filter= lambda item: self.get_account_id(account= item)  == self.get_account_id(account= acct)) is not None) ]
+  
+  def get_resource_groups(self, account, region, filters = [], rg_client = None):
+    if rg_client is None:
+      rg_client = self.get_boto_client(
+        client= 'resource-groups', 
+        account= account,
+        role = None,
+        region = region
+      )
+
+    boto_params = {}
+    if len(filters) > 0:
+      boto_params["Filters"] = filters
+
+    return self.general_boto_call_array(
+      boto_call=lambda item: rg_client.list_groups(**item),
+      boto_params= boto_params,
+      boto_nextkey = "NextToken",
+      boto_key="GroupIdentifiers"
+    )
+  
+  def get_resource_group_from_resource(self, account, region, filters_rg = [], filters_resource = [], aws_client = None, rg_client = None, resource_groups = None, treat_badfilter_err_as_empty = True):
+    if rg_client is None:
+      rg_client = self.get_boto_client(
+        client= 'resource-groups', 
+        account= account,
+        role = None,
+        region = region
+      )
+      
+    if resource_groups is None or (resource_groups is not None and len(resource_groups)<1):
+      resource_groups = self.get_resource_groups(account=account, region= region,filters=filters_rg, rg_client= rg_client)
+
+    if resource_groups is None or (resource_groups is not None and len(resource_groups)<1):
+      return {}
+
+    resources = {} 
+    boto_params = {}
+    if len(filters_resource) > 0:
+      boto_params["Filters"] = filters_resource
+    
+    boto_nextkey = "NextToken"
+    for rg in resource_groups:
+      boto_params["Group"] = rg["GroupArn"]
+      if boto_nextkey in boto_params:
+        boto_params.pop(boto_nextkey)
+      try:
+        for resource in self.general_boto_call_array(
+            boto_call=lambda item: rg_client.list_group_resources(**item),
+            boto_params= boto_params,
+            boto_nextkey = boto_nextkey,
+            boto_key="Resources",
+            error_codes_raise = ["BadRequestException"]
+          ):
+        
+          if resource.get("Identifier").get("ResourceArn").lower() not in resources:
+            resources[resource.get("Identifier").get("ResourceArn").lower()] = []
+          
+          resources[resource.get("Identifier").get("ResourceArn").lower()].append(rg["GroupName"])
+          
+      except ClientError as err:
+        if treat_badfilter_err_as_empty and "filters not valid" in str(err).lower():
+          continue
+        raise err
+      except Exception as err:
+        raise err
+
+    return resources
+  
+def get_resource_tags_as_dictionary(self, resource, *args, **kwargs):
+    if resource is None:
+      return None
+
+    tags = None
+    if not self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      if hasattr(resource, "tags"):
+        tags = resource.tags
+        
+    elif self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      tags = resource.get("tags")
+
+    if tags is None:
+      tags = {}
     
-    
+    if self.get_common().helper_type().general().is_type(obj= tags, type_check= list ):
+        tags = {tag["Key"]:tag["Value"] for tag in tags}
+
+    return tags
```

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.33/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,26 @@
   @abstractmethod
   def get_account_id(self, account, *args, **kwargs):
     pass
 
   @abstractmethod
   def make_account(self, account, *args, **kwargs):
     pass  
+  
+  @abstractmethod
+  def get_resource_group_from_resource(self, account, *args, **kwargs):
+    pass
 
+  def get_resource_location(self, resource, *args, **kwargs):
+    if resource is None:
+      return None
+    
+  def serialize_resource(self, *args, **kwargs):    
+    return None
+    
   def __load_config(self, *args, **kwargs):
     config_data = self.get_common().helper_config().load(
       path= self.config_path(),
       config_type= "yaml"
     )
     if config_data is not None:
       return config_data
```

### Comparing `threemystic_cloud_client-0.1.32/.gitignore` & `threemystic_cloud_client-0.1.33/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/LICENSE` & `threemystic_cloud_client-0.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/README.md` & `threemystic_cloud_client-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/hatch.toml` & `threemystic_cloud_client-0.1.33/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.32/pyproject.toml` & `threemystic_cloud_client-0.1.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.12",
+  "threemystic-common >= 0.1.14",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "pyopenssl >= 22.1.0",
   "PyJWT >= 2.7.0",
   "cryptography >= 41.0.1",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
```

### Comparing `threemystic_cloud_client-0.1.32/PKG-INFO` & `threemystic_cloud_client-0.1.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.32
+Version: 0.1.33
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
 Requires-Dist: pyjwt>=2.7.0
 Requires-Dist: pyopenssl>=22.1.0
-Requires-Dist: threemystic-common>=0.1.12
+Requires-Dist: threemystic-common>=0.1.14
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

