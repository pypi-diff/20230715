# Comparing `tmp/spark_quality_rules_tools-0.6.5.tar.gz` & `tmp/spark_quality_rules_tools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.6.5.tar", last modified: Tue Jul 11 02:06:54 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.7.0.tar", last modified: Sat Jul 15 03:33:30 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.6.5.tar` & `spark_quality_rules_tools-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.5/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.6.5/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-11 02:06:38.000000 spark_quality_rules_tools-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.077172 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.108423 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    56738 2023-07-11 02:06:38.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.124050 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25809 2023-07-06 02:34:48.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-06 05:59:35.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.108423 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-11 02:06:54.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.179382 spark_quality_rules_tools-0.7.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-15 03:33:30.180382 spark_quality_rules_tools-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.7.0/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-15 03:33:30.181383 spark_quality_rules_tools-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-14 14:04:42.000000 spark_quality_rules_tools-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.130616 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.152103 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    56640 2023-07-14 14:06:25.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.169740 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.178382 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.151103 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.6.5/LICENSE` & `spark_quality_rules_tools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/PKG-INFO` & `spark_quality_rules_tools-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.6.5
+Version: 0.7.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.6.5/README.md` & `spark_quality_rules_tools-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/pyproject.toml` & `spark_quality_rules_tools-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/setup.py` & `spark_quality_rules_tools-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.6.5',
+    version='0.7.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
     cutoff_date = ""
     with open(dir_confs_filename) as f:
         txt_conf = f.read()
 
     txt_conf = txt_conf.replace(f'${{TEST_PATH}}', "")
     txt_conf = txt_conf.replace(f'${{COUNTRY}}', "pe")
     txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
-    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}',"http://artifactory-gdt.central-02.nextgen.igrupobbva")
+    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}', "http://artifactory-gdt.central-02.nextgen.igrupobbva")
     if is_prod:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-local")
     else:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-dev-local")
 
     for params_parameter_conf in tqdm(parameter_conf_list):
         for k, v in params_parameter_conf.items():
@@ -757,17 +757,14 @@
     url_conf_name = str(str(file_conf).split(".")[0])
     uuaa_name = str(uuaa).upper()
 
     now = datetime.now()
     current_datetime = now.strftime("%Y-%m-%d %H:%M:%S")
     current_datetime_str = now.strftime("%Y%m%d%H%M")
 
-    id_split = str(rules_id).split("_")
-    table_name = "_".join(id_split[2:-2])
-
     dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
     dir_confs_filename_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS-{url_conf_name}.json")
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_ruleid_generated.conf")
 
     if is_windows:
         dir_confs_filename = dir_confs_filename.replace("\\", "/")
         dir_confs_filename_parameters = dir_confs_filename_parameters.replace("\\", "/")
@@ -823,15 +820,15 @@
             dataframeinfo = info["dataFrameInfo"]
         if 'input' in info.keys():
             input = info["input"]
         if 'rules' in info.keys():
             rules = info["rules"]
             for rule in rules:
                 key_id_rule = rule.get("config").get("id", None)
-                if str(key_id_rule).strip() == str(rules_id).strip():
+                if str(key_id_rule).strip() in rules_id:
                     rule_list.append(rule)
         hamu_dict = dict(hammurabi=dict(dataFrameInfo=dataframeinfo, input=input, rules=rule_list))
     json_file2 = json.dumps(hamu_dict, indent=4)
     conf2 = ConfigFactory.parse_string(json_file2)
     hocons_file2 = HOCONConverter.convert(conf2, "hocon")
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file2)
```

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999906994047619%*

 * *Differences: {"'rules_config'": "{'consistence': {'ValueConciliationRule': {0: {'rules_columns': {0: "*

 * *                   "{'dataSystemId': {insert: [(1, 'False')], delete: [1]}}}}}}}"}*

```diff
@@ -898,15 +898,15 @@
                             "column": [
                                 "String",
                                 "True",
                                 ""
                             ],
                             "dataSystemId": [
                                 "String",
-                                "True",
+                                "False",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
                                 "True",
                                 ""
                             ],
```

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.6.5
+Version: 0.7.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

