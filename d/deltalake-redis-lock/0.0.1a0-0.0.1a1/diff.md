# Comparing `tmp/deltalake-redis-lock-0.0.1a0.tar.gz` & `tmp/deltalake-redis-lock-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake-redis-lock-0.0.1a0.tar", max compression
+gzip compressed data, was "deltalake-redis-lock-0.0.1a1.tar", max compression
```

## Comparing `deltalake-redis-lock-0.0.1a0.tar` & `deltalake-redis-lock-0.0.1a1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-14 15:51:34.636636 deltalake-redis-lock-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     2821 2023-07-15 09:12:56.597064 deltalake-redis-lock-0.0.1a0/README.md
--rw-r--r--   0        0        0      600 2023-07-15 09:24:58.420668 deltalake-redis-lock-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 15:52:45.562904 deltalake-redis-lock-0.0.1a0/src/__init__.py
--rw-r--r--   0        0        0     3055 2023-07-15 09:11:21.381111 deltalake-redis-lock-0.0.1a0/src/deltalake_redis_lock.py
--rw-r--r--   0        0        0      126 2023-07-14 20:40:43.341578 deltalake-redis-lock-0.0.1a0/src/global_lock.py
--rw-r--r--   0        0        0     2135 2023-07-15 08:43:49.675864 deltalake-redis-lock-0.0.1a0/src/redis_lock_object_store.py
--rw-r--r--   0        0        0     3737 2023-07-15 14:27:59.875343 deltalake-redis-lock-0.0.1a0/setup.py
--rw-r--r--   0        0        0     3450 2023-07-15 14:27:59.875647 deltalake-redis-lock-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-14 15:51:34.636636 deltalake-redis-lock-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0     2674 2023-07-15 14:32:46.206990 deltalake-redis-lock-0.0.1a1/README.md
+-rw-r--r--   0        0        0      578 2023-07-15 14:33:04.828141 deltalake-redis-lock-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 15:52:45.562904 deltalake-redis-lock-0.0.1a1/src/__init__.py
+-rw-r--r--   0        0        0     1638 2023-07-15 14:28:46.575777 deltalake-redis-lock-0.0.1a1/src/delta_lock.py
+-rw-r--r--   0        0        0     4045 2023-07-15 14:28:46.576300 deltalake-redis-lock-0.0.1a1/src/delta_rs.py
+-rw-r--r--   0        0        0     3055 2023-07-15 14:28:54.444862 deltalake-redis-lock-0.0.1a1/src/deltalake_redis_lock.py
+-rw-r--r--   0        0        0      126 2023-07-15 14:28:54.445676 deltalake-redis-lock-0.0.1a1/src/global_lock.py
+-rw-r--r--   0        0        0     2135 2023-07-15 14:28:54.446711 deltalake-redis-lock-0.0.1a1/src/redis_lock_object_store.py
+-rw-r--r--   0        0        0     3587 2023-07-15 14:35:52.918476 deltalake-redis-lock-0.0.1a1/setup.py
+-rw-r--r--   0        0        0     3303 2023-07-15 14:35:52.918776 deltalake-redis-lock-0.0.1a1/PKG-INFO
```

### Comparing `deltalake-redis-lock-0.0.1a0/LICENSE` & `deltalake-redis-lock-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `deltalake-redis-lock-0.0.1a0/README.md` & `deltalake-redis-lock-0.0.1a1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # deltalake-redis-lock
 
 ![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/merge.yaml/badge.svg)
 ![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/pr.yaml/badge.svg)
-![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/wily.yaml/badge.svg)
 
 A library creating an interface for a write lock for [delta-rs](https://pypi.org/project/deltalake/).
 
 ## Library Usage
 
 When using this client, it can be used from multiple hosts. Below follow a minimal example
 to mimic this behaviour.
@@ -23,15 +22,15 @@
 ### Concurrent Write Example
 ```python
 # run.py
 import logging
 import os
 import string
 from random import choices
-from multiprocessing import Pool, freeze_support
+from multiprocessing import Pool
 
 from pandas import DataFrame
 
 from src.delta_rs import write_redis_lock_deltalake
 
 
 def fake_worker(args):
@@ -65,16 +64,14 @@
 
 
 def generate_random_string(length):
     return "".join(choices(string.ascii_lowercase, k=length))
 
 
 if __name__ == '__main__':
-    freeze_support()
-
     random_string = generate_random_string(3)
     table_name = f"test_run_{random_string}"
 
     define_datasets(_table_name=table_name)
 ```
 
 This can be exeucted with something like:
@@ -83,15 +80,15 @@
 seq 2 | xargs -I{} -P 2 poetry run python run.py
 ```
 
 ## Setup From Scratch
 
 ### Requirement
 
-* ^python3.8
+* ^python3.9
 * poetry 1.1.13
 * make (GNU Make 3.81)
 
 ### Setup
 
 ```bash
 make setup-environment
```

### Comparing `deltalake-redis-lock-0.0.1a0/pyproject.toml` & `deltalake-redis-lock-0.0.1a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltalake-redis-lock"
-version = "0.0.1-alpha.0"
+version = "0.0.1-alpha.1"
 description = "deltalake-redis-lock"
 authors = ["Simon Thelin"]
 readme = "README.md"
 homepage = "https://github.com/wrapbytes/deltalake-redis-lock"
 repository = "https://github.com/wrapbytes/deltalake-redis-lock"
 packages = [
     { include = "**/*.*", from="src"}
@@ -18,9 +18,7 @@
 pandas= "2.0.3"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.3.3"
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 pytest-env = "^0.8.2"
-fakeredis = "2.16.0"
-
```

### Comparing `deltalake-redis-lock-0.0.1a0/src/deltalake_redis_lock.py` & `deltalake-redis-lock-0.0.1a1/src/deltalake_redis_lock.py`

 * *Files identical despite different names*

### Comparing `deltalake-redis-lock-0.0.1a0/src/redis_lock_object_store.py` & `deltalake-redis-lock-0.0.1a1/src/redis_lock_object_store.py`

 * *Files identical despite different names*

### Comparing `deltalake-redis-lock-0.0.1a0/setup.py` & `deltalake-redis-lock-0.0.1a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['deltalake>=0.10.0,<0.11.0',
  'pandas==2.0.3',
  'pyarrow>=12.0.1,<13.0.0',
  'redis>=4.6.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'deltalake-redis-lock',
-    'version': '0.0.1a0',
+    'version': '0.0.1a1',
     'description': 'deltalake-redis-lock',
-    'long_description': '# deltalake-redis-lock\n\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/merge.yaml/badge.svg)\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/pr.yaml/badge.svg)\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/wily.yaml/badge.svg)\n\nA library creating an interface for a write lock for [delta-rs](https://pypi.org/project/deltalake/).\n\n## Library Usage\n\nWhen using this client, it can be used from multiple hosts. Below follow a minimal example\nto mimic this behaviour.\n\n### Redis Env Variables\n\nMake sure to set these `envs` before executing code.\n```bash\nREDIS_HOST=<host>\nREDIS_PORT=<port>  # default 6739\nREDIS_DB=<0>  # default 0\n```\n\n### Concurrent Write Example\n```python\n# run.py\nimport logging\nimport os\nimport string\nfrom random import choices\nfrom multiprocessing import Pool, freeze_support\n\nfrom pandas import DataFrame\n\nfrom src.delta_rs import write_redis_lock_deltalake\n\n\ndef fake_worker(args):\n    df, table_name = args\n\n    logging.basicConfig(\n        level=logging.INFO,\n        format=\'%(asctime)s [%(levelname)s] %(message)s\',\n        datefmt=\'%Y-%m-%d %H:%M:%S\'\n    )\n\n    write_redis_lock_deltalake(\n        table_or_uri=f"{os.getcwd()}/{table_name}",\n        lock_table_name=table_name,\n        mode="append",\n        data=df,\n        overwrite_schema=True,\n    )\n\n\ndef define_datasets(_table_name: str) -> None:\n    df1 = DataFrame({"id": [1]})\n    df2 = DataFrame({"id": [2]})\n    df3 = DataFrame({"id": [3]})\n    df4 = DataFrame({"id": [4]})\n\n    datasets = [(df1, table_name), (df2, table_name), (df3, table_name), (df4, table_name)]\n\n    with Pool() as pool:\n        pool.map(fake_worker, datasets)\n\n\ndef generate_random_string(length):\n    return "".join(choices(string.ascii_lowercase, k=length))\n\n\nif __name__ == \'__main__\':\n    freeze_support()\n\n    random_string = generate_random_string(3)\n    table_name = f"test_run_{random_string}"\n\n    define_datasets(_table_name=table_name)\n```\n\nThis can be exeucted with something like:\n\n```bash\nseq 2 | xargs -I{} -P 2 poetry run python run.py\n```\n\n## Setup From Scratch\n\n### Requirement\n\n* ^python3.8\n* poetry 1.1.13\n* make (GNU Make 3.81)\n\n### Setup\n\n```bash\nmake setup-environment\n```\n\nUpdate package\n```bash\nmake update\n```\n\n### Test\n\n```bash\nexport PYTHONPATH="${PYTHONPATH}:src"\nmake test type=unit\n```\n\n### Docker\n\nThe reason `docker` is used in the source code here, is to be able to build up an encapsulated\nenvironment of the codebase, and do `unit/integration and load tests`.\n\n```bash\nmake build-container-image\n```\n\n```bash\nmake get-container-info-environment\nmake run-container-tests type=unit\n```\n\n\n### Docker\n\n```bash\nmake build-container-image DOCKER_BUILD="buildx build --platform linux/amd64" CONTEXT=.\n```\n',
+    'long_description': '# deltalake-redis-lock\n\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/merge.yaml/badge.svg)\n![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/pr.yaml/badge.svg)\n\nA library creating an interface for a write lock for [delta-rs](https://pypi.org/project/deltalake/).\n\n## Library Usage\n\nWhen using this client, it can be used from multiple hosts. Below follow a minimal example\nto mimic this behaviour.\n\n### Redis Env Variables\n\nMake sure to set these `envs` before executing code.\n```bash\nREDIS_HOST=<host>\nREDIS_PORT=<port>  # default 6739\nREDIS_DB=<0>  # default 0\n```\n\n### Concurrent Write Example\n```python\n# run.py\nimport logging\nimport os\nimport string\nfrom random import choices\nfrom multiprocessing import Pool\n\nfrom pandas import DataFrame\n\nfrom src.delta_rs import write_redis_lock_deltalake\n\n\ndef fake_worker(args):\n    df, table_name = args\n\n    logging.basicConfig(\n        level=logging.INFO,\n        format=\'%(asctime)s [%(levelname)s] %(message)s\',\n        datefmt=\'%Y-%m-%d %H:%M:%S\'\n    )\n\n    write_redis_lock_deltalake(\n        table_or_uri=f"{os.getcwd()}/{table_name}",\n        lock_table_name=table_name,\n        mode="append",\n        data=df,\n        overwrite_schema=True,\n    )\n\n\ndef define_datasets(_table_name: str) -> None:\n    df1 = DataFrame({"id": [1]})\n    df2 = DataFrame({"id": [2]})\n    df3 = DataFrame({"id": [3]})\n    df4 = DataFrame({"id": [4]})\n\n    datasets = [(df1, table_name), (df2, table_name), (df3, table_name), (df4, table_name)]\n\n    with Pool() as pool:\n        pool.map(fake_worker, datasets)\n\n\ndef generate_random_string(length):\n    return "".join(choices(string.ascii_lowercase, k=length))\n\n\nif __name__ == \'__main__\':\n    random_string = generate_random_string(3)\n    table_name = f"test_run_{random_string}"\n\n    define_datasets(_table_name=table_name)\n```\n\nThis can be exeucted with something like:\n\n```bash\nseq 2 | xargs -I{} -P 2 poetry run python run.py\n```\n\n## Setup From Scratch\n\n### Requirement\n\n* ^python3.9\n* poetry 1.1.13\n* make (GNU Make 3.81)\n\n### Setup\n\n```bash\nmake setup-environment\n```\n\nUpdate package\n```bash\nmake update\n```\n\n### Test\n\n```bash\nexport PYTHONPATH="${PYTHONPATH}:src"\nmake test type=unit\n```\n\n### Docker\n\nThe reason `docker` is used in the source code here, is to be able to build up an encapsulated\nenvironment of the codebase, and do `unit/integration and load tests`.\n\n```bash\nmake build-container-image\n```\n\n```bash\nmake get-container-info-environment\nmake run-container-tests type=unit\n```\n\n\n### Docker\n\n```bash\nmake build-container-image DOCKER_BUILD="buildx build --platform linux/amd64" CONTEXT=.\n```\n',
     'author': 'Simon Thelin',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/wrapbytes/deltalake-redis-lock',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `deltalake-redis-lock-0.0.1a0/PKG-INFO` & `deltalake-redis-lock-0.0.1a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltalake-redis-lock
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: deltalake-redis-lock
 Home-page: https://github.com/wrapbytes/deltalake-redis-lock
 Author: Simon Thelin
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,14 @@
 Project-URL: Repository, https://github.com/wrapbytes/deltalake-redis-lock
 Description-Content-Type: text/markdown
 
 # deltalake-redis-lock
 
 ![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/merge.yaml/badge.svg)
 ![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/pr.yaml/badge.svg)
-![example workflow](https://github.com/wrapbytes/deltalake-redis-lock/actions/workflows/wily.yaml/badge.svg)
 
 A library creating an interface for a write lock for [delta-rs](https://pypi.org/project/deltalake/).
 
 ## Library Usage
 
 When using this client, it can be used from multiple hosts. Below follow a minimal example
 to mimic this behaviour.
@@ -40,15 +39,15 @@
 ### Concurrent Write Example
 ```python
 # run.py
 import logging
 import os
 import string
 from random import choices
-from multiprocessing import Pool, freeze_support
+from multiprocessing import Pool
 
 from pandas import DataFrame
 
 from src.delta_rs import write_redis_lock_deltalake
 
 
 def fake_worker(args):
@@ -82,16 +81,14 @@
 
 
 def generate_random_string(length):
     return "".join(choices(string.ascii_lowercase, k=length))
 
 
 if __name__ == '__main__':
-    freeze_support()
-
     random_string = generate_random_string(3)
     table_name = f"test_run_{random_string}"
 
     define_datasets(_table_name=table_name)
 ```
 
 This can be exeucted with something like:
@@ -100,15 +97,15 @@
 seq 2 | xargs -I{} -P 2 poetry run python run.py
 ```
 
 ## Setup From Scratch
 
 ### Requirement
 
-* ^python3.8
+* ^python3.9
 * poetry 1.1.13
 * make (GNU Make 3.81)
 
 ### Setup
 
 ```bash
 make setup-environment
```

