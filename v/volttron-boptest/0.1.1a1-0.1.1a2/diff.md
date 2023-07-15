# Comparing `tmp/volttron_boptest-0.1.1a1.tar.gz` & `tmp/volttron_boptest-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_boptest-0.1.1a1.tar", max compression
+gzip compressed data, was "volttron_boptest-0.1.1a2.tar", max compression
```

## Comparing `volttron_boptest-0.1.1a1.tar` & `volttron_boptest-0.1.1a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11927 2023-07-15 00:12:36.650376 volttron_boptest-0.1.1a1/LICENSE
--rw-r--r--   0        0        0    16770 2023-07-15 00:12:36.650376 volttron_boptest-0.1.1a1/README.md
--rw-r--r--   0        0        0     1843 2023-07-15 00:14:27.511627 volttron_boptest-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/__init__.py
--rw-r--r--   0        0        0    15888 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/agent.py
--rw-r--r--   0        0        0     1525 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/README.md
--rw-r--r--   0        0        0       77 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpi_calculator.py
--rw-r--r--   0        0        0      499 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpis_example.config
--rw-r--r--   0        0        0     1152 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpis_example.py
--rw-r--r--   0        0        0    18052 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-15 05:07:28.872501 volttron_boptest-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0    17029 2023-07-15 05:07:28.872501 volttron_boptest-0.1.1a2/README.md
+-rw-r--r--   0        0        0     1843 2023-07-15 05:09:11.802768 volttron_boptest-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/__init__.py
+-rw-r--r--   0        0        0    15888 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/agent.py
+-rw-r--r--   0        0        0     1525 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/custom_kpi/README.md
+-rw-r--r--   0        0        0       77 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/custom_kpi/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/custom_kpi/custom_kpi_calculator.py
+-rw-r--r--   0        0        0      499 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/custom_kpi/custom_kpis_example.config
+-rw-r--r--   0        0        0     1152 2023-07-15 05:07:28.876502 volttron_boptest-0.1.1a2/src/boptest/custom_kpi/custom_kpis_example.py
+-rw-r--r--   0        0        0    18311 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1a2/PKG-INFO
```

### Comparing `volttron_boptest-0.1.1a1/LICENSE` & `volttron_boptest-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a1/README.md` & `volttron_boptest-0.1.1a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
 
 In order to demonstrate the basic usage of volttron-boptest-agent, we need to setup the boptest simulation server.
 
 (Please see more details about boptest quick-start
 at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-boptest#quick-start-to-deploy-a-test-case))
 
 1. Download [IBPSA Project 1 - BOPTEST](https://github.com/ibpsa/project1-boptest) repository to <boptest_repo>. For
-   demo purpose, let boptest_repo be `/tmp/project1-boptest`.
+   demo purpose, let boptest_repo be `~/project1-boptest`.
 
    ```shell
-   git clone https://github.com/ibpsa/project1-boptest /tmp/project1-boptest
+   git clone https://github.com/ibpsa/project1-boptest ~/project1-boptest
    ```
 
 1. Install [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/).
 
    (Optional) Verify with `docker-compose version` to verify the installation
    ```shell
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose version
@@ -129,37 +129,43 @@
 1. Build and deploy a test case.
 
    The basic command to start a test case is by using `TESTCASE=<testcase_name> docker-compose up`.
 
    For demo purpose, we will build and deploy testcase1, for avialbe testcases please
    see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/testcases)
    ```shell
-   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-compose.yml up
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml up
    Creating network "boptest-net" with the default driver
    Creating project1-boptest_boptest_1 ... done
    Attaching to project1-boptest_boptest_1
    boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Control step set successfully.
    boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized successfully to 0.0s with warmup period of
    0.0s.
    boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test case scenario was set successfully.
    ...
    boptest_1  |  * Debug mode: off
    boptest_1  | 07/13/2023 09:59:42 PM UTC werkzeug            INFO         * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
    ```
    Or use detach mode
    ```shell
-   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-compose.yml up --detach 
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml up --detach 
    Starting project1-boptest_boptest_1 ... done
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls
    CONTAINER ID   IMAGE          COMMAND                  CREATED        STATUS          PORTS                      NAMES
    ddd0f2cc1f99   boptest_base   "/bin/sh -c 'python …"   23 hours ago   Up 12 seconds   127.0.0.1:5000->5000/tcp   project1-boptest_boptest_1
    ```
 
    Note: Use `docker-compose down` to shut down the service.
 
+   Verify boptest simulation server is running properly:
+   ```shell
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ curl http://127.0.0.1:5000/name
+   {"message":"Queried the name of the test case successfully.","payload":{"name":"testcase1"},"status":200}
+   ```
+
 ### Install volttron boptest agent
 
 1. Install the "volttron-boptest" dependency.
 
    There are two options to install volttron-boptest. You can install this library using the version on PyPi or install
    it from the source code (`git clone` might be required.)
    Note: the `vctl install` command in the following step can handle dependency installation using pypi. However, in
```

#### html2text {}

```diff
@@ -42,52 +42,55 @@
 VOLTTRON_HOME= # Start platform with output going to volttron.log volttron -vv
 -l volttron.log & ``` ### Setup the boptest simulation server locally. In order
 to demonstrate the basic usage of volttron-boptest-agent, we need to setup the
 boptest simulation server. (Please see more details about boptest quick-start
 at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
 boptest#quick-start-to-deploy-a-test-case)) 1. Download [IBPSA Project 1 -
 BOPTEST](https://github.com/ibpsa/project1-boptest) repository to . For demo
-purpose, let boptest_repo be `/tmp/project1-boptest`. ```shell git clone https:
-//github.com/ibpsa/project1-boptest /tmp/project1-boptest ``` 1. Install
-[Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://
+purpose, let boptest_repo be `~/project1-boptest`. ```shell git clone https://
+github.com/ibpsa/project1-boptest ~/project1-boptest ``` 1. Install [Docker]
+(https://docs.docker.com/get-docker/) and [Docker Compose](https://
 docs.docker.com/compose/install/). (Optional) Verify with `docker-compose
 version` to verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/
 volttron-boptest$ docker-compose version docker-compose version 1.29.2, build
 unknown docker-py version: 5.0.3 CPython version: 3.10.6 OpenSSL version:
 OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build and deploy a test case. The basic
 command to start a test case is by using `TESTCASE= docker-compose up`. For
 demo purpose, we will build and deploy testcase1, for avialbe testcases please
 see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/
 testcases) ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
-TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-
-compose.yml up Creating network "boptest-net" with the default driver Creating
-project1-boptest_boptest_1 ... done Attaching to project1-boptest_boptest_1
-boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Control step set successfully.
-boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized
-successfully to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:
-42 PM UTC root INFO Test case scenario was set successfully. ... boptest_1 | *
-Debug mode: off boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running
-on http://0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell
-(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-
-compose --file /tmp/project1-boptest/docker-compose.yml up --detach Starting
-project1-boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-
-boptest$ docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS
-NAMES ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12
-seconds 127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use
-`docker-compose down` to shut down the service. ### Install volttron boptest
-agent 1. Install the "volttron-boptest" dependency. There are two options to
-install volttron-boptest. You can install this library using the version on
-PyPi or install it from the source code (`git clone` might be required.) Note:
-the `vctl install` command in the following step can handle dependency
-installation using pypi. However, in this demo we demonstrate what is happening
-under the neath the hood by separating the dependency installation and agent
-registry steps. ```shell # option 1: install from pypi pip install volttron-
-boptest # option 2: install from the source code (Note: `-e` option to use
-editable mode, useful for development.) pip install [-e] /volttron-boptest/ ```
-1. Install and start the "volttron-boptest" agent. We will use the
+TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml
+up Creating network "boptest-net" with the default driver Creating project1-
+boptest_boptest_1 ... done Attaching to project1-boptest_boptest_1 boptest_1 |
+07/13/2023 09:59:42 PM UTC root INFO Control step set successfully. boptest_1 |
+07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized successfully
+to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:42 PM UTC root
+INFO Test case scenario was set successfully. ... boptest_1 | * Debug mode: off
+boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running on http://
+0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose -
+-file ~/project1-boptest/docker-compose.yml up --detach Starting project1-
+boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS NAMES
+ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12 seconds
+127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use `docker-
+compose down` to shut down the service. Verify boptest simulation server is
+running properly: ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+curl http://127.0.0.1:5000/name {"message":"Queried the name of the test case
+successfully.","payload":{"name":"testcase1"},"status":200} ``` ### Install
+volttron boptest agent 1. Install the "volttron-boptest" dependency. There are
+two options to install volttron-boptest. You can install this library using the
+version on PyPi or install it from the source code (`git clone` might be
+required.) Note: the `vctl install` command in the following step can handle
+dependency installation using pypi. However, in this demo we demonstrate what
+is happening under the neath the hood by separating the dependency installation
+and agent registry steps. ```shell # option 1: install from pypi pip install
+volttron-boptest # option 2: install from the source code (Note: `-e` option to
+use editable mode, useful for development.) pip install [-e] /volttron-boptest/
+``` 1. Install and start the "volttron-boptest" agent. We will use the
 [testcase1.config](examples/testcase1.config) as the agent config for this
 demo. Please see [examples/](examples) for other example config files. Use
 `vctl install` command to register to the volttron home path. Note: for demo
 purposes and reproducibility, we assign vip-identity as
 "volttron_boptest_agent", but you can choose any other valid agent identity as
 desired. ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl
 install volttron-boptest \ --agent-config volttron-boptest-agent/examples/
```

### Comparing `volttron_boptest-0.1.1a1/pyproject.toml` & `volttron_boptest-0.1.1a2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-boptest"
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = "A Volttron agent that runs boptest simulation."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-boptest"
 repository = "https://github.com/eclipse-volttron/volttron-boptest"
@@ -37,15 +37,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-volttron-lib-boptest-integration = "^0.1.1a1"
+volttron-lib-boptest-integration = "^0.1.1a2"
 numpy = ">0.0.0"
 pandas = ">0.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=6.2.4"
 pytest-cov = ">=3.0.0"
 pytest-env = ">0.0.0"
```

### Comparing `volttron_boptest-0.1.1a1/src/boptest/agent.py` & `volttron_boptest-0.1.1a2/src/boptest/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a1/src/boptest/custom_kpi/README.md` & `volttron_boptest-0.1.1a2/src/boptest/custom_kpi/README.md`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpi_calculator.py` & `volttron_boptest-0.1.1a2/src/boptest/custom_kpi/custom_kpi_calculator.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpis_example.py` & `volttron_boptest-0.1.1a2/src/boptest/custom_kpi/custom_kpis_example.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a1/PKG-INFO` & `volttron_boptest-0.1.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-boptest
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A Volttron agent that runs boptest simulation.
 Home-page: https://github.com/eclipse-volttron/volttron-boptest
 License: Apache-2.0
 Keywords: volttron,agent,boptest,simulation,application
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Dist: numpy (>0.0.0)
 Requires-Dist: pandas (>0.0.0)
-Requires-Dist: volttron-lib-boptest-integration (>=0.1.1a1,<0.2.0)
+Requires-Dist: volttron-lib-boptest-integration (>=0.1.1a2,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-boptest/issues
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-boptest
 Description-Content-Type: text/markdown
 
 # boptest-agent
 
 The volttron-boptest-agent utilizes the volttron-lib-boptest-integration library to perform simulation control and
@@ -134,18 +134,18 @@
 
 In order to demonstrate the basic usage of volttron-boptest-agent, we need to setup the boptest simulation server.
 
 (Please see more details about boptest quick-start
 at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-boptest#quick-start-to-deploy-a-test-case))
 
 1. Download [IBPSA Project 1 - BOPTEST](https://github.com/ibpsa/project1-boptest) repository to <boptest_repo>. For
-   demo purpose, let boptest_repo be `/tmp/project1-boptest`.
+   demo purpose, let boptest_repo be `~/project1-boptest`.
 
    ```shell
-   git clone https://github.com/ibpsa/project1-boptest /tmp/project1-boptest
+   git clone https://github.com/ibpsa/project1-boptest ~/project1-boptest
    ```
 
 1. Install [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/).
 
    (Optional) Verify with `docker-compose version` to verify the installation
    ```shell
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker-compose version
@@ -159,37 +159,43 @@
 1. Build and deploy a test case.
 
    The basic command to start a test case is by using `TESTCASE=<testcase_name> docker-compose up`.
 
    For demo purpose, we will build and deploy testcase1, for avialbe testcases please
    see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/testcases)
    ```shell
-   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-compose.yml up
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml up
    Creating network "boptest-net" with the default driver
    Creating project1-boptest_boptest_1 ... done
    Attaching to project1-boptest_boptest_1
    boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Control step set successfully.
    boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized successfully to 0.0s with warmup period of
    0.0s.
    boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test case scenario was set successfully.
    ...
    boptest_1  |  * Debug mode: off
    boptest_1  | 07/13/2023 09:59:42 PM UTC werkzeug            INFO         * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
    ```
    Or use detach mode
    ```shell
-   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-compose.yml up --detach 
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml up --detach 
    Starting project1-boptest_boptest_1 ... done
    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ docker container ls
    CONTAINER ID   IMAGE          COMMAND                  CREATED        STATUS          PORTS                      NAMES
    ddd0f2cc1f99   boptest_base   "/bin/sh -c 'python …"   23 hours ago   Up 12 seconds   127.0.0.1:5000->5000/tcp   project1-boptest_boptest_1
    ```
 
    Note: Use `docker-compose down` to shut down the service.
 
+   Verify boptest simulation server is running properly:
+   ```shell
+   (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ curl http://127.0.0.1:5000/name
+   {"message":"Queried the name of the test case successfully.","payload":{"name":"testcase1"},"status":200}
+   ```
+
 ### Install volttron boptest agent
 
 1. Install the "volttron-boptest" dependency.
 
    There are two options to install volttron-boptest. You can install this library using the version on PyPi or install
    it from the source code (`git clone` might be required.)
    Note: the `vctl install` command in the following step can handle dependency installation using pypi. However, in
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1a1 Summary: A
+Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1a2 Summary: A
 Volttron agent that runs boptest simulation. Home-page: https://github.com/
 eclipse-volttron/volttron-boptest License: Apache-2.0 Keywords:
 volttron,agent,boptest,simulation,application Author: Kefei Mo Author-email:
 kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Home Automation Classifier:
 Topic :: Software Development :: Embedded Systems Requires-Dist: numpy (>0.0.0)
 Requires-Dist: pandas (>0.0.0) Requires-Dist: volttron-lib-boptest-integration
-(>=0.1.1a1,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
+(>=0.1.1a2,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
 volttron/volttron-boptest/issues Project-URL: Repository, https://github.com/
 eclipse-volttron/volttron-boptest Description-Content-Type: text/markdown #
 boptest-agent The volttron-boptest-agent utilizes the volttron-lib-boptest-
 integration library to perform simulation control and benchmark tasks. BOPTEST
 is designed to facilitate the performance evaluation and benchmarking of
 building control strategies, which contains these key components: 1. Run-Time
 Environment (RTE): Deployed with Docker and accessed with a RESTful HTTP API,
@@ -59,52 +59,55 @@
 VOLTTRON_HOME= # Start platform with output going to volttron.log volttron -vv
 -l volttron.log & ``` ### Setup the boptest simulation server locally. In order
 to demonstrate the basic usage of volttron-boptest-agent, we need to setup the
 boptest simulation server. (Please see more details about boptest quick-start
 at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
 boptest#quick-start-to-deploy-a-test-case)) 1. Download [IBPSA Project 1 -
 BOPTEST](https://github.com/ibpsa/project1-boptest) repository to . For demo
-purpose, let boptest_repo be `/tmp/project1-boptest`. ```shell git clone https:
-//github.com/ibpsa/project1-boptest /tmp/project1-boptest ``` 1. Install
-[Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://
+purpose, let boptest_repo be `~/project1-boptest`. ```shell git clone https://
+github.com/ibpsa/project1-boptest ~/project1-boptest ``` 1. Install [Docker]
+(https://docs.docker.com/get-docker/) and [Docker Compose](https://
 docs.docker.com/compose/install/). (Optional) Verify with `docker-compose
 version` to verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/
 volttron-boptest$ docker-compose version docker-compose version 1.29.2, build
 unknown docker-py version: 5.0.3 CPython version: 3.10.6 OpenSSL version:
 OpenSSL 3.0.2 15 Mar 2022 ``` 1. Build and deploy a test case. The basic
 command to start a test case is by using `TESTCASE= docker-compose up`. For
 demo purpose, we will build and deploy testcase1, for avialbe testcases please
 see [testcases/](https://github.com/ibpsa/project1-boptest/tree/master/
 testcases) ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
-TESTCASE=testcase1 docker-compose --file /tmp/project1-boptest/docker-
-compose.yml up Creating network "boptest-net" with the default driver Creating
-project1-boptest_boptest_1 ... done Attaching to project1-boptest_boptest_1
-boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Control step set successfully.
-boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized
-successfully to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:
-42 PM UTC root INFO Test case scenario was set successfully. ... boptest_1 | *
-Debug mode: off boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running
-on http://0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell
-(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-
-compose --file /tmp/project1-boptest/docker-compose.yml up --detach Starting
-project1-boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-
-boptest$ docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS
-NAMES ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12
-seconds 127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use
-`docker-compose down` to shut down the service. ### Install volttron boptest
-agent 1. Install the "volttron-boptest" dependency. There are two options to
-install volttron-boptest. You can install this library using the version on
-PyPi or install it from the source code (`git clone` might be required.) Note:
-the `vctl install` command in the following step can handle dependency
-installation using pypi. However, in this demo we demonstrate what is happening
-under the neath the hood by separating the dependency installation and agent
-registry steps. ```shell # option 1: install from pypi pip install volttron-
-boptest # option 2: install from the source code (Note: `-e` option to use
-editable mode, useful for development.) pip install [-e] /volttron-boptest/ ```
-1. Install and start the "volttron-boptest" agent. We will use the
+TESTCASE=testcase1 docker-compose --file ~/project1-boptest/docker-compose.yml
+up Creating network "boptest-net" with the default driver Creating project1-
+boptest_boptest_1 ... done Attaching to project1-boptest_boptest_1 boptest_1 |
+07/13/2023 09:59:42 PM UTC root INFO Control step set successfully. boptest_1 |
+07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized successfully
+to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:42 PM UTC root
+INFO Test case scenario was set successfully. ... boptest_1 | * Debug mode: off
+boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running on http://
+0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell (env)
+kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-compose -
+-file ~/project1-boptest/docker-compose.yml up --detach Starting project1-
+boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS NAMES
+ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12 seconds
+127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use `docker-
+compose down` to shut down the service. Verify boptest simulation server is
+running properly: ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$
+curl http://127.0.0.1:5000/name {"message":"Queried the name of the test case
+successfully.","payload":{"name":"testcase1"},"status":200} ``` ### Install
+volttron boptest agent 1. Install the "volttron-boptest" dependency. There are
+two options to install volttron-boptest. You can install this library using the
+version on PyPi or install it from the source code (`git clone` might be
+required.) Note: the `vctl install` command in the following step can handle
+dependency installation using pypi. However, in this demo we demonstrate what
+is happening under the neath the hood by separating the dependency installation
+and agent registry steps. ```shell # option 1: install from pypi pip install
+volttron-boptest # option 2: install from the source code (Note: `-e` option to
+use editable mode, useful for development.) pip install [-e] /volttron-boptest/
+``` 1. Install and start the "volttron-boptest" agent. We will use the
 [testcase1.config](examples/testcase1.config) as the agent config for this
 demo. Please see [examples/](examples) for other example config files. Use
 `vctl install` command to register to the volttron home path. Note: for demo
 purposes and reproducibility, we assign vip-identity as
 "volttron_boptest_agent", but you can choose any other valid agent identity as
 desired. ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl
 install volttron-boptest \ --agent-config volttron-boptest-agent/examples/
```

