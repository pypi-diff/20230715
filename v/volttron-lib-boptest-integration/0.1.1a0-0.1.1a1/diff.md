# Comparing `tmp/volttron_lib_boptest_integration-0.1.1a0.tar.gz` & `tmp/volttron_lib_boptest_integration-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_boptest_integration-0.1.1a0.tar", max compression
+gzip compressed data, was "volttron_lib_boptest_integration-0.1.1a1.tar", max compression
```

## Comparing `volttron_lib_boptest_integration-0.1.1a0.tar` & `volttron_lib_boptest_integration-0.1.1a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11927 2023-07-14 19:58:17.798318 volttron_lib_boptest_integration-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     7253 2023-07-14 19:58:17.798318 volttron_lib_boptest_integration-0.1.1a0/README.md
--rw-r--r--   0        0        0     1855 2023-07-14 19:59:52.986713 volttron_lib_boptest_integration-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/__init__.py
--rw-r--r--   0        0        0    13693 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/boptest_integration.py
--rw-r--r--   0        0        0      108 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/__init__.py
--rw-r--r--   0        0        0     3252 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/controller.py
--rw-r--r--   0        0        0     1537 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/pid.py
--rw-r--r--   0        0        0     4610 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/pidTwoZones.py
--rw-r--r--   0        0        0     1179 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/sup.py
--rw-r--r--   0        0        0     9666 2023-07-14 19:58:17.802318 volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/interface.py
--rw-r--r--   0        0        0     8524 1970-01-01 00:00:00.000000 volttron_lib_boptest_integration-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-15 00:12:36.654376 volttron_lib_boptest_integration-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     9044 2023-07-15 00:12:36.654376 volttron_lib_boptest_integration-0.1.1a1/README.md
+-rw-r--r--   0        0        0     1855 2023-07-15 00:14:29.579721 volttron_lib_boptest_integration-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/__init__.py
+-rw-r--r--   0        0        0    13693 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/boptest_integration.py
+-rw-r--r--   0        0        0      108 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/__init__.py
+-rw-r--r--   0        0        0     3252 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/controller.py
+-rw-r--r--   0        0        0     1537 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/pid.py
+-rw-r--r--   0        0        0     4610 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/pidTwoZones.py
+-rw-r--r--   0        0        0     1179 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/sup.py
+-rw-r--r--   0        0        0     9666 2023-07-15 00:12:36.658376 volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/interface.py
+-rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 volttron_lib_boptest_integration-0.1.1a1/PKG-INFO
```

### Comparing `volttron_lib_boptest_integration-0.1.1a0/LICENSE` & `volttron_lib_boptest_integration-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/README.md` & `volttron_lib_boptest_integration-0.1.1a1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # boptest-integration
 
-This python library is used for integrating boptest simulation into VOLTTRON platform. 
+This python library is used for integrating boptest simulation into VOLTTRON platform.
 
 BOPTEST is designed to facilitate
 the performance evaluation and benchmarking of building control strategies, which
 contains these key components:
 
 1. Run-Time Environment (RTE): Deployed with Docker and accessed with a RESTful HTTP API, use the RTE to set up tests,
    control building emulators, access data, and report KPIs.
@@ -45,36 +45,68 @@
 
 </details>
 
 # Installation
 
 The following recipe walks through the steps to install and run use case example.
 
+Note: For the ease of reproducibility, in this demo, we
+will git clone the [volttron-boptest](https://github.com/eclipse-volttron/volttron-boptest) repo to the `~/sandbox/`
+path. Feel free to modify the workflow as desired.
+
+   ```shell
+   kefei@ubuntu-22:~/sandbox$ git clone https://github.com/eclipse-volttron/volttron-boptest.git
+   Cloning into 'volttron-boptest'...
+   remote: Enumerating objects: 450, done.
+   remote: Counting objects: 100% (450/450), done.
+   remote: Compressing objects: 100% (242/242), done.
+   remote: Total 450 (delta 192), reused 424 (delta 170), pack-reused 0
+   Receiving objects: 100% (450/450), 3.66 MiB | 7.06 MiB/s, done.
+   Resolving deltas: 100% (192/192), done.
+   kefei@ubuntu-22:~/sandbox$ cd volttron-boptest/
+   kefei@ubuntu-22:~/sandbox/volttron-boptest$ 
+   ```
+
 1. Create and activate a virtual environment.
 
    It is recommended to use a virtual environment for installing library.
 
     ```shell
-    python -m venv env
-    source env/bin/activate
+    kefei@ubuntu-22:~/sandbox/volttron-boptest$ python -m venv env
+    kefei@ubuntu-22:~/sandbox/volttron-boptest$ source env/bin/activate
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
     ```
 
 
 1. Install the "volttron-boptest-integration" library.
 
-   There are two options to install "volttron-boptest-integration". You can install this library using the version on PyPi or install
+   There are two options to install "volttron-boptest-integration". You can install this library using the version on
+   PyPi or install
    it from the source code (`git clone` might be required.)
 
     ```shell
     # option 1: install from pypi
     pip install volttron-lib-boptest-integration
     
     # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)
     pip install [-e] <path-to-the-source-code-root>/volttron-lib-boptest-integration/
     ```
+   
+    ```shell
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip install volttron-lib-boptest-integration
+    Collecting volttron-lib-boptest-integration
+      Downloading volttron_lib_boptest_integration-0.1.1a0-py3-none-any.whl (20 kB)
+    Collecting pandas>0.0.0
+    ...
+   
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip list | grep volttron
+    volttron                         10.0.4rc1
+    volttron-lib-boptest-integration 0.1.1a0
+    ...
+    ```
 
 # Basic Usage
 
 In order to demonstrate the basic usage of volttron-lib-boptest-integration, we need to setup the boptest simulation
 server.
 
 ### Setup the boptest simulation server locally.
@@ -120,24 +152,28 @@
    boptest_1  |  * Debug mode: off
    boptest_1  | 07/13/2023 09:59:42 PM UTC werkzeug            INFO         * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
    ```
    Or use detach mode
    ```shell
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-compose.yml up --detach 
    Starting project1-boptest_boptest_1 ... done
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls
+   CONTAINER ID   IMAGE          COMMAND                  CREATED        STATUS          PORTS                      NAMES
+   ddd0f2cc1f99   boptest_base   "/bin/sh -c 'python …"   23 hours ago   Up 12 seconds   127.0.0.1:5000->5000/tcp   project1-boptest_boptest_1
+
    ```
 
    Note: Use `docker-compose down` to shut down the service.
 
 1. Run example usecases.
-   
+
    There are several exmaple usecases available at [examples/](examples). In this demo,
-   we will run [testcase1.py](examples/tescase1.py). 
+   we will run [testcase1.py](examples/tescase1.py).
    ```shell
-   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python <examples-path>/testcase1.py
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python volttron-lib-boptest-integration/examples/testcase1.py
    INFO:root:=========== run_workflow
    INFO:root:
    TEST CASE INFORMATION
    ---------------------
    INFO:root:Name:                         testcase1
    ...
    INFO:root:======== run workflow completed.======
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -13,23 +13,40 @@
 Ubuntu 22.04) ## Python  To install specific Python version (e.g., Python
 3.10), we recommend using pyenv. ```shell # install pyenv git clone https://
 github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also put these three
 lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export
 PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.10 pyenv
 install 3.10 # make it available globally pyenv global system 3.10 ```  #
 Installation The following recipe walks through the steps to install and run
-use case example. 1. Create and activate a virtual environment. It is
+use case example. Note: For the ease of reproducibility, in this demo, we will
+git clone the [volttron-boptest](https://github.com/eclipse-volttron/volttron-
+boptest) repo to the `~/sandbox/` path. Feel free to modify the workflow as
+desired. ```shell kefei@ubuntu-22:~/sandbox$ git clone https://github.com/
+eclipse-volttron/volttron-boptest.git Cloning into 'volttron-boptest'...
+remote: Enumerating objects: 450, done. remote: Counting objects: 100% (450/
+450), done. remote: Compressing objects: 100% (242/242), done. remote: Total
+450 (delta 192), reused 424 (delta 170), pack-reused 0 Receiving objects: 100%
+(450/450), 3.66 MiB | 7.06 MiB/s, done. Resolving deltas: 100% (192/192), done.
+kefei@ubuntu-22:~/sandbox$ cd volttron-boptest/ kefei@ubuntu-22:~/sandbox/
+volttron-boptest$ ``` 1. Create and activate a virtual environment. It is
 recommended to use a virtual environment for installing library. ```shell
-python -m venv env source env/bin/activate ``` 1. Install the "volttron-
-boptest-integration" library. There are two options to install "volttron-
-boptest-integration". You can install this library using the version on PyPi or
-install it from the source code (`git clone` might be required.) ```shell #
-option 1: install from pypi pip install volttron-lib-boptest-integration #
-option 2: install from the source code (Note: `-e` option to use editable mode,
-useful for development.) pip install [-e] /volttron-lib-boptest-integration/
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ python -m venv env kefei@ubuntu-22:
+~/sandbox/volttron-boptest$ source env/bin/activate (env) kefei@ubuntu-22:~/
+sandbox/volttron-boptest$ ``` 1. Install the "volttron-boptest-integration"
+library. There are two options to install "volttron-boptest-integration". You
+can install this library using the version on PyPi or install it from the
+source code (`git clone` might be required.) ```shell # option 1: install from
+pypi pip install volttron-lib-boptest-integration # option 2: install from the
+source code (Note: `-e` option to use editable mode, useful for development.)
+pip install [-e] /volttron-lib-boptest-integration/ ``` ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip install volttron-lib-boptest-
+integration Collecting volttron-lib-boptest-integration Downloading
+volttron_lib_boptest_integration-0.1.1a0-py3-none-any.whl (20 kB) Collecting
+pandas>0.0.0 ... (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip list |
+grep volttron volttron 10.0.4rc1 volttron-lib-boptest-integration 0.1.1a0 ...
 ``` # Basic Usage In order to demonstrate the basic usage of volttron-lib-
 boptest-integration, we need to setup the boptest simulation server. ### Setup
 the boptest simulation server locally. (Please see more details about boptest
 quick-start at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/
 project1-boptest#quick-start-to-deploy-a-test-case)) 1. Download [IBPSA Project
 1 - BOPTEST](https://github.com/ibpsa/project1-boptest) repository to . For
 demo purpose, let boptest_repo be `/tmp/project1-boptest`. ```shell git clone
@@ -51,21 +68,25 @@
 boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized
 successfully to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:
 42 PM UTC root INFO Test case scenario was set successfully. ... boptest_1 | *
 Debug mode: off boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running
 on http://0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell
 (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-
 compose --file /tmp/project1-boptest/docker-compose.yml up --detach Starting
-project1-boptest_boptest_1 ... done ``` Note: Use `docker-compose down` to shut
-down the service. 1. Run example usecases. There are several exmaple usecases
-available at [examples/](examples). In this demo, we will run [testcase1.py]
-(examples/tescase1.py). ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-
-boptest$ python /testcase1.py INFO:root:=========== run_workflow INFO:root:
-TEST CASE INFORMATION --------------------- INFO:root:Name: testcase1 ... INFO:
-root:======== run workflow completed.====== ======= kpi {'cost_tot':
+project1-boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-
+boptest$ docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS
+NAMES ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12
+seconds 127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use
+`docker-compose down` to shut down the service. 1. Run example usecases. There
+are several exmaple usecases available at [examples/](examples). In this demo,
+we will run [testcase1.py](examples/tescase1.py). ```shell (env) kefei@ubuntu-
+22:~/sandbox/volttron-boptest$ python volttron-lib-boptest-integration/
+examples/testcase1.py INFO:root:=========== run_workflow INFO:root: TEST CASE
+INFORMATION --------------------- INFO:root:Name: testcase1 ... INFO:root:
+======== run workflow completed.====== ======= kpi {'cost_tot':
 0.075149821513246, 'emis_tot': 0.2147137757521314, 'ener_tot':
 1.073568878760657, 'idis_tot': 508.47225004790033, 'pdih_tot': None,
 'pele_tot': None, 'pgas_tot': 0.09615811655434148, 'tdis_tot':
 5.316029375566828, 'time_rat': 1.531114146269157e-05} ``` Note: the example
 usecase must match the test case that is running. For example when
 TESTCASE=testcase1, we can run [testcase1.py](examples/testcase1.py) and
 [testcase1_scenario.py](examples/testcase1_scenario.py), but not [testcase2.py]
```

### Comparing `volttron_lib_boptest_integration-0.1.1a0/pyproject.toml` & `volttron_lib_boptest_integration-0.1.1a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-boptest-integration"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "A Volttron library for boptest simulation integration."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-boptest"
 repository = "https://github.com/eclipse-volttron/volttron-boptest"
```

### Comparing `volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/boptest_integration.py` & `volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/boptest_integration.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/controller.py` & `volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/pid.py` & `volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/pid.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/pidTwoZones.py` & `volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/pidTwoZones.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/controllers/sup.py` & `volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/controllers/sup.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/src/boptest_integration/interface.py` & `volttron_lib_boptest_integration-0.1.1a1/src/boptest_integration/interface.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1a0/PKG-INFO` & `volttron_lib_boptest_integration-0.1.1a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-boptest-integration
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A Volttron library for boptest simulation integration.
 Home-page: https://github.com/eclipse-volttron/volttron-boptest
 License: Apache-2.0
 Keywords: volttron,boptest,simulation,integration
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
@@ -26,15 +26,15 @@
 Requires-Dist: volttron (>=10.0.4rc1)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-boptest/issues
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-boptest
 Description-Content-Type: text/markdown
 
 # boptest-integration
 
-This python library is used for integrating boptest simulation into VOLTTRON platform. 
+This python library is used for integrating boptest simulation into VOLTTRON platform.
 
 BOPTEST is designed to facilitate
 the performance evaluation and benchmarking of building control strategies, which
 contains these key components:
 
 1. Run-Time Environment (RTE): Deployed with Docker and accessed with a RESTful HTTP API, use the RTE to set up tests,
    control building emulators, access data, and report KPIs.
@@ -75,36 +75,68 @@
 
 </details>
 
 # Installation
 
 The following recipe walks through the steps to install and run use case example.
 
+Note: For the ease of reproducibility, in this demo, we
+will git clone the [volttron-boptest](https://github.com/eclipse-volttron/volttron-boptest) repo to the `~/sandbox/`
+path. Feel free to modify the workflow as desired.
+
+   ```shell
+   kefei@ubuntu-22:~/sandbox$ git clone https://github.com/eclipse-volttron/volttron-boptest.git
+   Cloning into 'volttron-boptest'...
+   remote: Enumerating objects: 450, done.
+   remote: Counting objects: 100% (450/450), done.
+   remote: Compressing objects: 100% (242/242), done.
+   remote: Total 450 (delta 192), reused 424 (delta 170), pack-reused 0
+   Receiving objects: 100% (450/450), 3.66 MiB | 7.06 MiB/s, done.
+   Resolving deltas: 100% (192/192), done.
+   kefei@ubuntu-22:~/sandbox$ cd volttron-boptest/
+   kefei@ubuntu-22:~/sandbox/volttron-boptest$ 
+   ```
+
 1. Create and activate a virtual environment.
 
    It is recommended to use a virtual environment for installing library.
 
     ```shell
-    python -m venv env
-    source env/bin/activate
+    kefei@ubuntu-22:~/sandbox/volttron-boptest$ python -m venv env
+    kefei@ubuntu-22:~/sandbox/volttron-boptest$ source env/bin/activate
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
     ```
 
 
 1. Install the "volttron-boptest-integration" library.
 
-   There are two options to install "volttron-boptest-integration". You can install this library using the version on PyPi or install
+   There are two options to install "volttron-boptest-integration". You can install this library using the version on
+   PyPi or install
    it from the source code (`git clone` might be required.)
 
     ```shell
     # option 1: install from pypi
     pip install volttron-lib-boptest-integration
     
     # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)
     pip install [-e] <path-to-the-source-code-root>/volttron-lib-boptest-integration/
     ```
+   
+    ```shell
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip install volttron-lib-boptest-integration
+    Collecting volttron-lib-boptest-integration
+      Downloading volttron_lib_boptest_integration-0.1.1a0-py3-none-any.whl (20 kB)
+    Collecting pandas>0.0.0
+    ...
+   
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip list | grep volttron
+    volttron                         10.0.4rc1
+    volttron-lib-boptest-integration 0.1.1a0
+    ...
+    ```
 
 # Basic Usage
 
 In order to demonstrate the basic usage of volttron-lib-boptest-integration, we need to setup the boptest simulation
 server.
 
 ### Setup the boptest simulation server locally.
@@ -150,24 +182,28 @@
    boptest_1  |  * Debug mode: off
    boptest_1  | 07/13/2023 09:59:42 PM UTC werkzeug            INFO         * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
    ```
    Or use detach mode
    ```shell
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-compose.yml up --detach 
    Starting project1-boptest_boptest_1 ... done
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls
+   CONTAINER ID   IMAGE          COMMAND                  CREATED        STATUS          PORTS                      NAMES
+   ddd0f2cc1f99   boptest_base   "/bin/sh -c 'python …"   23 hours ago   Up 12 seconds   127.0.0.1:5000->5000/tcp   project1-boptest_boptest_1
+
    ```
 
    Note: Use `docker-compose down` to shut down the service.
 
 1. Run example usecases.
-   
+
    There are several exmaple usecases available at [examples/](examples). In this demo,
-   we will run [testcase1.py](examples/tescase1.py). 
+   we will run [testcase1.py](examples/tescase1.py).
    ```shell
-   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python <examples-path>/testcase1.py
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python volttron-lib-boptest-integration/examples/testcase1.py
    INFO:root:=========== run_workflow
    INFO:root:
    TEST CASE INFORMATION
    ---------------------
    INFO:root:Name:                         testcase1
    ...
    INFO:root:======== run workflow completed.======
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-boptest-integration Version: 0.1.1a0
+Metadata-Version: 2.1 Name: volttron-lib-boptest-integration Version: 0.1.1a1
 Summary: A Volttron library for boptest simulation integration. Home-page:
 https://github.com/eclipse-volttron/volttron-boptest License: Apache-2.0
 Keywords: volttron,boptest,simulation,integration Author: Kefei Mo Author-
 email: kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email:
 volttron@pnnl.gov Requires-Python: >=3.10,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
@@ -29,24 +29,41 @@
 with Python3.10) * Linux OS (tested with Ubuntu 22.04) ## Python  To install
 specific Python version (e.g., Python 3.10), we recommend using pyenv. ```shell
 # install pyenv git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv
 (you should also put these three lines in .bashrc or similar) export PATH="$
 {HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv
 init -)" # install Python 3.10 pyenv install 3.10 # make it available globally
 pyenv global system 3.10 ```  # Installation The following recipe walks through
-the steps to install and run use case example. 1. Create and activate a virtual
-environment. It is recommended to use a virtual environment for installing
-library. ```shell python -m venv env source env/bin/activate ``` 1. Install the
-"volttron-boptest-integration" library. There are two options to install
-"volttron-boptest-integration". You can install this library using the version
-on PyPi or install it from the source code (`git clone` might be required.)
-```shell # option 1: install from pypi pip install volttron-lib-boptest-
-integration # option 2: install from the source code (Note: `-e` option to use
-editable mode, useful for development.) pip install [-e] /volttron-lib-boptest-
-integration/ ``` # Basic Usage In order to demonstrate the basic usage of
+the steps to install and run use case example. Note: For the ease of
+reproducibility, in this demo, we will git clone the [volttron-boptest](https:/
+/github.com/eclipse-volttron/volttron-boptest) repo to the `~/sandbox/` path.
+Feel free to modify the workflow as desired. ```shell kefei@ubuntu-22:~/
+sandbox$ git clone https://github.com/eclipse-volttron/volttron-boptest.git
+Cloning into 'volttron-boptest'... remote: Enumerating objects: 450, done.
+remote: Counting objects: 100% (450/450), done. remote: Compressing objects:
+100% (242/242), done. remote: Total 450 (delta 192), reused 424 (delta 170),
+pack-reused 0 Receiving objects: 100% (450/450), 3.66 MiB | 7.06 MiB/s, done.
+Resolving deltas: 100% (192/192), done. kefei@ubuntu-22:~/sandbox$ cd volttron-
+boptest/ kefei@ubuntu-22:~/sandbox/volttron-boptest$ ``` 1. Create and activate
+a virtual environment. It is recommended to use a virtual environment for
+installing library. ```shell kefei@ubuntu-22:~/sandbox/volttron-boptest$ python
+-m venv env kefei@ubuntu-22:~/sandbox/volttron-boptest$ source env/bin/activate
+(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ ``` 1. Install the "volttron-
+boptest-integration" library. There are two options to install "volttron-
+boptest-integration". You can install this library using the version on PyPi or
+install it from the source code (`git clone` might be required.) ```shell #
+option 1: install from pypi pip install volttron-lib-boptest-integration #
+option 2: install from the source code (Note: `-e` option to use editable mode,
+useful for development.) pip install [-e] /volttron-lib-boptest-integration/
+``` ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ pip install
+volttron-lib-boptest-integration Collecting volttron-lib-boptest-integration
+Downloading volttron_lib_boptest_integration-0.1.1a0-py3-none-any.whl (20 kB)
+Collecting pandas>0.0.0 ... (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+pip list | grep volttron volttron 10.0.4rc1 volttron-lib-boptest-integration
+0.1.1a0 ... ``` # Basic Usage In order to demonstrate the basic usage of
 volttron-lib-boptest-integration, we need to setup the boptest simulation
 server. ### Setup the boptest simulation server locally. (Please see more
 details about boptest quick-start at [Quick-Start to Deploy a Test Case](https:
 //github.com/ibpsa/project1-boptest#quick-start-to-deploy-a-test-case)) 1.
 Download [IBPSA Project 1 - BOPTEST](https://github.com/ibpsa/project1-boptest)
 repository to . For demo purpose, let boptest_repo be `/tmp/project1-boptest`.
 ```shell git clone https://github.com/ibpsa/project1-boptest /tmp/project1-
@@ -67,39 +84,42 @@
 set successfully. boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test
 simulation initialized successfully to 0.0s with warmup period of 0.0s.
 boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test case scenario was set
 successfully. ... boptest_1 | * Debug mode: off boptest_1 | 07/13/2023 09:59:42
 PM UTC werkzeug INFO * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
 ``` Or use detach mode ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-
 boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-
-compose.yml up --detach Starting project1-boptest_boptest_1 ... done ``` Note:
-Use `docker-compose down` to shut down the service. 1. Run example usecases.
-There are several exmaple usecases available at [examples/](examples). In this
-demo, we will run [testcase1.py](examples/tescase1.py). ```shell (env)
-kefei@ubuntu-22:~/sandbox/volttron-boptest$ python /testcase1.py INFO:root:
-=========== run_workflow INFO:root: TEST CASE INFORMATION --------------------
-- INFO:root:Name: testcase1 ... INFO:root:======== run workflow
-completed.====== ======= kpi {'cost_tot': 0.075149821513246, 'emis_tot':
-0.2147137757521314, 'ener_tot': 1.073568878760657, 'idis_tot':
-508.47225004790033, 'pdih_tot': None, 'pele_tot': None, 'pgas_tot':
-0.09615811655434148, 'tdis_tot': 5.316029375566828, 'time_rat':
-1.531114146269157e-05} ``` Note: the example usecase must match the test case
-that is running. For example when TESTCASE=testcase1, we can run [testcase1.py]
-(examples/testcase1.py) and [testcase1_scenario.py](examples/
-testcase1_scenario.py), but not [testcase2.py](examples/testcase2.py). #
-Development Please see the following for contributing guidelines [contributing]
-(https://github.com/eclipse-volttron/volttron-core/blob/develop/
-CONTRIBUTING.md). Please see the following helpful guide about [developing
-modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/
-blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer Notice This material was
-prepared as an account of work sponsored by an agency of the United States
-Government. Neither the United States Government nor the United States
-Department of Energy, nor Battelle, nor any of their employees, nor any
-jurisdiction or organization that has cooperated in the development of these
-materials, makes any warranty, express or implied, or assumes any legal
+compose.yml up --detach Starting project1-boptest_boptest_1 ... done (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls CONTAINER ID
+IMAGE COMMAND CREATED STATUS PORTS NAMES ddd0f2cc1f99 boptest_base "/bin/sh -
+c 'python â¦" 23 hours ago Up 12 seconds 127.0.0.1:5000->5000/tcp project1-
+boptest_boptest_1 ``` Note: Use `docker-compose down` to shut down the service.
+1. Run example usecases. There are several exmaple usecases available at
+[examples/](examples). In this demo, we will run [testcase1.py](examples/
+tescase1.py). ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ python
+volttron-lib-boptest-integration/examples/testcase1.py INFO:root:===========
+run_workflow INFO:root: TEST CASE INFORMATION --------------------- INFO:root:
+Name: testcase1 ... INFO:root:======== run workflow completed.====== =======
+kpi {'cost_tot': 0.075149821513246, 'emis_tot': 0.2147137757521314, 'ener_tot':
+1.073568878760657, 'idis_tot': 508.47225004790033, 'pdih_tot': None,
+'pele_tot': None, 'pgas_tot': 0.09615811655434148, 'tdis_tot':
+5.316029375566828, 'time_rat': 1.531114146269157e-05} ``` Note: the example
+usecase must match the test case that is running. For example when
+TESTCASE=testcase1, we can run [testcase1.py](examples/testcase1.py) and
+[testcase1_scenario.py](examples/testcase1_scenario.py), but not [testcase2.py]
+(examples/testcase2.py). # Development Please see the following for
+contributing guidelines [contributing](https://github.com/eclipse-volttron/
+volttron-core/blob/develop/CONTRIBUTING.md). Please see the following helpful
+guide about [developing modular VOLTTRON agents](https://github.com/eclipse-
+volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md) # Disclaimer
+Notice This material was prepared as an account of work sponsored by an agency
+of the United States Government. Neither the United States Government nor the
+United States Department of Energy, nor Battelle, nor any of their employees,
+nor any jurisdiction or organization that has cooperated in the development of
+these materials, makes any warranty, express or implied, or assumes any legal
 liability or responsibility for the accuracy, completeness, or usefulness or
 any information, apparatus, product, software, or process disclosed, or
 represents that its use would not infringe privately owned rights. Reference
 herein to any specific commercial product, process, or service by trade name,
 trademark, manufacturer, or otherwise does not necessarily constitute or imply
 its endorsement, recommendation, or favoring by the United States Government or
 any agency thereof, or Battelle Memorial Institute. The views and opinions of
```

