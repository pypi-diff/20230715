# Comparing `tmp/threemystic_common-0.1.14.tar.gz` & `tmp/threemystic_common-0.1.15.tar.gz`

## Comparing `threemystic_common-0.1.14.tar` & `threemystic_common-0.1.15.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/__version__.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/common.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/base.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/base_common.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/base_general.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/base_provider.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/base_script_options.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/generate_data/generate_data_handlers.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/base_class/generate_data/handlers/base.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/cli/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/app_monitoring/common.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/app_monitoring/performance.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/cmdb/aws.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/cmdb/azure.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/cmdb/common.py
--rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/cmdb/base_class/base.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/encryption/common.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/encryption/hash.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/exception/argument.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/exception/common.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/exception/function.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/exception/generic.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/exception/base_class/base.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/generate_data/generate.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/graph/common.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/graph/msgraph.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/graph/base_class/base.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/graph/config/msgraph.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/hashicorp/common.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/hashicorp/vault.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/app.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/config.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/currency.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/json.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/parallel_processing.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/path.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/yaml.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/bool.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/common.py
--rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/datetime.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/dictionary.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/general.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/int.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/list.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/logging.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/openpyxl.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/regex.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/requests.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/domain/helpers/type/string.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/threemystic_common/exceptions/generate_data/quit.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/LICENSE
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/hatch.toml
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/pyproject.toml
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 threemystic_common-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/__version__.py
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/common.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/base.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/base_common.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/base_general.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/base_provider.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/base_script_options.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/generate_data/generate_data_handlers.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/base_class/generate_data/handlers/base.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/cli/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/app_monitoring/common.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/app_monitoring/performance.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/cmdb/aws.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/cmdb/azure.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/cmdb/common.py
+-rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/cmdb/base_class/base.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/encryption/common.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/encryption/hash.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/exception/argument.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/exception/common.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/exception/function.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/exception/generic.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/exception/base_class/base.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/generate_data/generate.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/graph/common.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/graph/msgraph.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/graph/base_class/base.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/graph/config/msgraph.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/hashicorp/common.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/hashicorp/vault.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/app.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/config.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/currency.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/json.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/parallel_processing.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/path.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/yaml.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/bool.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/common.py
+-rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/datetime.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/dictionary.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/general.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/int.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/list.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/logging.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/openpyxl.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/regex.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/requests.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/domain/helpers/type/string.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/threemystic_common/exceptions/generate_data/quit.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/LICENSE
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/hatch.toml
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 threemystic_common-0.1.15/PKG-INFO
```

### Comparing `threemystic_common-0.1.14/threemystic_common/common.py` & `threemystic_common-0.1.15/threemystic_common/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/base_class/base.py` & `threemystic_common-0.1.15/threemystic_common/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/base_class/base_provider.py` & `threemystic_common-0.1.15/threemystic_common/base_class/base_provider.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/base_class/base_script_options.py` & `threemystic_common-0.1.15/threemystic_common/base_class/base_script_options.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/base_class/generate_data/handlers/base.py` & `threemystic_common-0.1.15/threemystic_common/base_class/generate_data/handlers/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/app_monitoring/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/app_monitoring/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/app_monitoring/performance.py` & `threemystic_common-0.1.15/threemystic_common/domain/app_monitoring/performance.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/cmdb/aws.py` & `threemystic_common-0.1.15/threemystic_common/domain/cmdb/aws.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/cmdb/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/cmdb/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/cmdb/base_class/base.py` & `threemystic_common-0.1.15/threemystic_common/domain/cmdb/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/encryption/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/encryption/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/encryption/hash.py` & `threemystic_common-0.1.15/threemystic_common/domain/encryption/hash.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/exception/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/exception/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/exception/base_class/base.py` & `threemystic_common-0.1.15/threemystic_common/domain/exception/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/generate_data/generate.py` & `threemystic_common-0.1.15/threemystic_common/domain/generate_data/generate.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/graph/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/graph/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/graph/msgraph.py` & `threemystic_common-0.1.15/threemystic_common/domain/graph/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/graph/base_class/base.py` & `threemystic_common-0.1.15/threemystic_common/domain/graph/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/graph/config/msgraph.py` & `threemystic_common-0.1.15/threemystic_common/domain/graph/config/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/hashicorp/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/hashicorp/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/app.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/app.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/config.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/config.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/currency.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/currency.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/json.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/json.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/parallel_processing.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/parallel_processing.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/path.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/path.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/yaml.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/bool.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/bool.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/common.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/datetime.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/datetime.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/dictionary.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/dictionary.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/general.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/general.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/list.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/list.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/logging.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/logging.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/regex.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/regex.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/requests.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/requests.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/threemystic_common/domain/helpers/type/string.py` & `threemystic_common-0.1.15/threemystic_common/domain/helpers/type/string.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/.gitignore` & `threemystic_common-0.1.15/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/LICENSE` & `threemystic_common-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/hatch.toml` & `threemystic_common-0.1.15/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/pyproject.toml` & `threemystic_common-0.1.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.14/PKG-INFO` & `threemystic_common-0.1.15/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-common
-Version: 0.1.14
+Version: 0.1.15
 Summary: Common Library for for various tool sets
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_common
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_common/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -29,33 +29,42 @@
 Requires-Dist: ruamel-yaml>=0.17.31
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_common
 A set of common files that are used for the various projects under 3 Mystic Apes
 
+This project is currently in beta, along with the other projects. Once the other projects come out of beta this one will as well. However, this is also, the most stable of the project. I am trying not to change things that would break from version to version. So if you would like to use something here, it should be relatively safe. I will try to call out breaking changes.
+
 # Install
 
 ## pip
 
-This project is currently designed to be installed via pip <br/>
-pip install https://github.com/3MysticApes/3mystic_common
+The latest version of this project is currently being pushed to
+https://pypi.org/project/threemystic-common/
 
-Once installed you will get the following command:
-3mystic_common
+pip install threemystic-common
 
-The above command currently just lets you know the scripts have been installed and are usable for reference. It also will let you know what version of the toolset is installed.
+If you would prefer to install directly from GitHub you need to install Hatch.
+Please refer to the section below for that.
 
+Once hatch is installed you can use pip
 
-# Contribute
+pip install https://github.com/3MysticApes/3mystic_common
 
+
+
+## Hatch
 This project is packaged using Hatch. If you need to install Hatch please refer to their documentation
 https://hatch.pypa.io/latest/install/
 
+# Contribute
+You need to install Hatch. Please see the previous Hatch section under install.
 
+Once you download the project you can do the following
 You should be able to run the following command in the root directory for a general status
 hatch status
 
 Then from the root directory you can run
 pip install ./
 
 I would suggest while you are debugging issues to install it with the command below. Once you are done with your development you can uninstall. This allows you to make edits and test easier.
```

