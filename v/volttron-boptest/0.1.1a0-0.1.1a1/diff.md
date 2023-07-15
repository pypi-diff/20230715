# Comparing `tmp/volttron_boptest-0.1.1a0.tar.gz` & `tmp/volttron_boptest-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_boptest-0.1.1a0.tar", max compression
+gzip compressed data, was "volttron_boptest-0.1.1a1.tar", max compression
```

## Comparing `volttron_boptest-0.1.1a0.tar` & `volttron_boptest-0.1.1a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11927 2023-07-14 19:58:17.794319 volttron_boptest-0.1.1a0/LICENSE
--rw-r--r--   0        0        0    15931 2023-07-14 19:58:17.794319 volttron_boptest-0.1.1a0/README.md
--rw-r--r--   0        0        0     1843 2023-07-14 19:59:51.378707 volttron_boptest-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/__init__.py
--rw-r--r--   0        0        0    15888 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/agent.py
--rw-r--r--   0        0        0     1525 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/custom_kpi/README.md
--rw-r--r--   0        0        0       77 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/custom_kpi/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/custom_kpi/custom_kpi_calculator.py
--rw-r--r--   0        0        0      499 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/custom_kpi/custom_kpis_example.config
--rw-r--r--   0        0        0     1152 2023-07-14 19:58:17.798318 volttron_boptest-0.1.1a0/src/boptest/custom_kpi/custom_kpis_example.py
--rw-r--r--   0        0        0    17213 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-15 00:12:36.650376 volttron_boptest-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0    16770 2023-07-15 00:12:36.650376 volttron_boptest-0.1.1a1/README.md
+-rw-r--r--   0        0        0     1843 2023-07-15 00:14:27.511627 volttron_boptest-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/__init__.py
+-rw-r--r--   0        0        0    15888 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/agent.py
+-rw-r--r--   0        0        0     1525 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/README.md
+-rw-r--r--   0        0        0       77 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpi_calculator.py
+-rw-r--r--   0        0        0      499 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpis_example.config
+-rw-r--r--   0        0        0     1152 2023-07-15 00:12:36.654376 volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpis_example.py
+-rw-r--r--   0        0        0    18052 1970-01-01 00:00:00.000000 volttron_boptest-0.1.1a1/PKG-INFO
```

### Comparing `volttron_boptest-0.1.1a0/LICENSE` & `volttron_boptest-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a0/README.md` & `volttron_boptest-0.1.1a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,33 @@
 
 # Quick-start
 
 ### Setup environment and VOLTTRON platform
 
 The following recipe walks through the steps to install and demonstrate basic usage of "volttron-boptest" agent.
 
+The following recipe walks through the steps to install and run use case example.
+
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
 
    It is recommended to use a virtual environment for installing volttron.
 
     ```shell
     python -m venv env
     source env/bin/activate
@@ -126,14 +145,17 @@
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
    ```
 
    Note: Use `docker-compose down` to shut down the service.
 
 ### Install volttron boptest agent
 
 1. Install the "volttron-boptest" dependency.
@@ -151,58 +173,27 @@
     
     # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)
     pip install [-e] <path-to-the-source-code-root>/volttron-boptest/
     ```
 
 1. Install and start the "volttron-boptest" agent.
 
-   Prepare the default config files:
-
-    ```shell
-    # Create config file place holders
-    mkdir config
-    touch config/boptest_integration-agent-config.json
-    ```
-
-   Edit the `testcase1_config.yml` as follows:
-    ```yaml
-    {
-     "testcase_name": "testcase1",
-     "initialize":  # for GET/initialize
-     {
-       "start_time": 0,
-       "warmup_period": 0
-     },
-     "scenario": null,
-     "step": 300,
-     "length": 86400,
-   
-     "controller":
-     {
-       "type": "pid",  # currently support "pid", "sup", pidTwoZones"
-       "u":
-       {
-         "oveAct_u": 0,
-         "oveAct_activate": 1
-       }
-     }
-   
-   }
-    ```
-
-   Please see [examples/](examples) for other example config files.
+   We will use the [testcase1.config](examples/testcase1.config) as the agent config for this demo. Please
+   see [examples/](examples) for other example config files.
 
    Use `vctl install` command to register to the volttron home path.
    Note: for demo purposes and reproducibility, we assign vip-identity as "volttron_boptest_agent", but you can choose
    any other valid agent identity as desired.
 
     ```shell
-    vctl install volttron-boptest --agent-config <path-to-agent-config> \
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl install volttron-boptest \
+   --agent-config volttron-boptest-agent/examples/testcase1.config \
    --vip-identity volttron_boptest_agent \
    --start
+   Agent a0fd6f5c-3751-4312-9f59-ca541b8aac4e installed and started [4980]
     ```
 
    Observe Data
 
    The volttron-boptest agent publishes events on the message bus. To see these events in the Volttron log file, install
    a [Listener Agent](https://pypi.org/project/volttron-listener/):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -14,29 +14,40 @@
 (e.g., Python 3.10), we recommend using pyenv. ```shell # install pyenv git
 clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also
 put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:$
 {PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install
 Python 3.10 pyenv install 3.10 # make it available globally pyenv global system
 3.10 ```  # Quick-start ### Setup environment and VOLTTRON platform The
 following recipe walks through the steps to install and demonstrate basic usage
-of "volttron-boptest" agent. 1. Create and activate a virtual environment. It
-is recommended to use a virtual environment for installing volttron. ```shell
-python -m venv env source env/bin/activate pip install volttron ``` 1. Install
-volttron and start the platform. > **Note**: > According to the [volttron-
-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup
-VOLTTRON_HOME > environment variable is mandatory: > ... if you have/had in the
-past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME >
-$HOME/.volttron. This modular version of VOLTTRON cannot work with
-volttron_home used by monolithic version of > VOLTTRON(version 8.3 or earlier)
-```shell # Setup environment variable `VOLTTRON_HOME` export VOLTTRON_HOME= #
-Start platform with output going to volttron.log volttron -vv -l volttron.log &
-``` ### Setup the boptest simulation server locally. In order to demonstrate
-the basic usage of volttron-boptest-agent, we need to setup the boptest
-simulation server. (Please see more details about boptest quick-start at
-[Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
+of "volttron-boptest" agent. The following recipe walks through the steps to
+install and run use case example. Note: For the ease of reproducibility, in
+this demo, we will git clone the [volttron-boptest](https://github.com/eclipse-
+volttron/volttron-boptest) repo to the `~/sandbox/` path. Feel free to modify
+the workflow as desired. ```shell kefei@ubuntu-22:~/sandbox$ git clone https://
+github.com/eclipse-volttron/volttron-boptest.git Cloning into 'volttron-
+boptest'... remote: Enumerating objects: 450, done. remote: Counting objects:
+100% (450/450), done. remote: Compressing objects: 100% (242/242), done.
+remote: Total 450 (delta 192), reused 424 (delta 170), pack-reused 0 Receiving
+objects: 100% (450/450), 3.66 MiB | 7.06 MiB/s, done. Resolving deltas: 100%
+(192/192), done. kefei@ubuntu-22:~/sandbox$ cd volttron-boptest/ kefei@ubuntu-
+22:~/sandbox/volttron-boptest$ ``` 1. Create and activate a virtual
+environment. It is recommended to use a virtual environment for installing
+volttron. ```shell python -m venv env source env/bin/activate pip install
+volttron ``` 1. Install volttron and start the platform. > **Note**: >
+According to the [volttron-core#README](https://github.com/eclipse-volttron/
+volttron-core#readme), setup VOLTTRON_HOME > environment variable is mandatory:
+> ... if you have/had in the past, a monolithic VOLTTRON version that used the
+default VOLTTRON_HOME > $HOME/.volttron. This modular version of VOLTTRON
+cannot work with volttron_home used by monolithic version of > VOLTTRON(version
+8.3 or earlier) ```shell # Setup environment variable `VOLTTRON_HOME` export
+VOLTTRON_HOME= # Start platform with output going to volttron.log volttron -vv
+-l volttron.log & ``` ### Setup the boptest simulation server locally. In order
+to demonstrate the basic usage of volttron-boptest-agent, we need to setup the
+boptest simulation server. (Please see more details about boptest quick-start
+at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
 boptest#quick-start-to-deploy-a-test-case)) 1. Download [IBPSA Project 1 -
 BOPTEST](https://github.com/ibpsa/project1-boptest) repository to . For demo
 purpose, let boptest_repo be `/tmp/project1-boptest`. ```shell git clone https:
 //github.com/ibpsa/project1-boptest /tmp/project1-boptest ``` 1. Install
 [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://
 docs.docker.com/compose/install/). (Optional) Verify with `docker-compose
 version` to verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/
@@ -54,43 +65,44 @@
 boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized
 successfully to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:
 42 PM UTC root INFO Test case scenario was set successfully. ... boptest_1 | *
 Debug mode: off boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running
 on http://0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell
 (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-
 compose --file /tmp/project1-boptest/docker-compose.yml up --detach Starting
-project1-boptest_boptest_1 ... done ``` Note: Use `docker-compose down` to shut
-down the service. ### Install volttron boptest agent 1. Install the "volttron-
-boptest" dependency. There are two options to install volttron-boptest. You can
-install this library using the version on PyPi or install it from the source
-code (`git clone` might be required.) Note: the `vctl install` command in the
-following step can handle dependency installation using pypi. However, in this
-demo we demonstrate what is happening under the neath the hood by separating
-the dependency installation and agent registry steps. ```shell # option 1:
-install from pypi pip install volttron-boptest # option 2: install from the
-source code (Note: `-e` option to use editable mode, useful for development.)
-pip install [-e] /volttron-boptest/ ``` 1. Install and start the "volttron-
-boptest" agent. Prepare the default config files: ```shell # Create config file
-place holders mkdir config touch config/boptest_integration-agent-config.json
-``` Edit the `testcase1_config.yml` as follows: ```yaml { "testcase_name":
-"testcase1", "initialize": # for GET/initialize { "start_time": 0,
-"warmup_period": 0 }, "scenario": null, "step": 300, "length": 86400,
-"controller": { "type": "pid", # currently support "pid", "sup", pidTwoZones"
-"u": { "oveAct_u": 0, "oveAct_activate": 1 } } } ``` Please see [examples/]
-(examples) for other example config files. Use `vctl install` command to
-register to the volttron home path. Note: for demo purposes and
-reproducibility, we assign vip-identity as "volttron_boptest_agent", but you
-can choose any other valid agent identity as desired. ```shell vctl install
-volttron-boptest --agent-config  \ --vip-identity volttron_boptest_agent \ --
-start ``` Observe Data The volttron-boptest agent publishes events on the
-message bus. To see these events in the Volttron log file, install a [Listener
-Agent](https://pypi.org/project/volttron-listener/): ``` vctl install volttron-
-listener --start ``` (Optional) Use `vctl stauts` to verify the installation
-```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl status UUID
-AGENT IDENTITY TAG PRIORITY STATUS HEALTH a volttron-boptest-agent-0.0.1
+project1-boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-
+boptest$ docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS
+NAMES ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12
+seconds 127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use
+`docker-compose down` to shut down the service. ### Install volttron boptest
+agent 1. Install the "volttron-boptest" dependency. There are two options to
+install volttron-boptest. You can install this library using the version on
+PyPi or install it from the source code (`git clone` might be required.) Note:
+the `vctl install` command in the following step can handle dependency
+installation using pypi. However, in this demo we demonstrate what is happening
+under the neath the hood by separating the dependency installation and agent
+registry steps. ```shell # option 1: install from pypi pip install volttron-
+boptest # option 2: install from the source code (Note: `-e` option to use
+editable mode, useful for development.) pip install [-e] /volttron-boptest/ ```
+1. Install and start the "volttron-boptest" agent. We will use the
+[testcase1.config](examples/testcase1.config) as the agent config for this
+demo. Please see [examples/](examples) for other example config files. Use
+`vctl install` command to register to the volttron home path. Note: for demo
+purposes and reproducibility, we assign vip-identity as
+"volttron_boptest_agent", but you can choose any other valid agent identity as
+desired. ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl
+install volttron-boptest \ --agent-config volttron-boptest-agent/examples/
+testcase1.config \ --vip-identity volttron_boptest_agent \ --start Agent
+a0fd6f5c-3751-4312-9f59-ca541b8aac4e installed and started [4980] ``` Observe
+Data The volttron-boptest agent publishes events on the message bus. To see
+these events in the Volttron log file, install a [Listener Agent](https://
+pypi.org/project/volttron-listener/): ``` vctl install volttron-listener --
+start ``` (Optional) Use `vctl stauts` to verify the installation ```shell
+(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl status UUID AGENT
+IDENTITY TAG PRIORITY STATUS HEALTH a volttron-boptest-agent-0.0.1
 volttron_boptest_agent running [59108] GOOD 2 volttron-listener-0.2.0rc0
 volttron-listener-0.2.0rc0_1 running [59096] GOOD ``` 1. (optional) Inspect the
 volttron.log file   Within the volttron.log, we should see similar logs as
 follows ```shell # Create config file place holders KPI RESULTS ----------
 - 2023-07-13 18:27:51,124 (volttron-boptest-agent-0.0.1 59108) root(186) INFO:
 emis_tot: 0.2147137757521314 KgCO2/m$^2$ 2023-07-13 18:27:51,174 (volttron-
 boptest-agent-0.0.1 59108) root(186) INFO: ener_tot: 1.073568878760657 kWh/
```

### Comparing `volttron_boptest-0.1.1a0/pyproject.toml` & `volttron_boptest-0.1.1a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-boptest"
-version = "0.1.1a0"
+version = "0.1.1a1"
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
-volttron-lib-boptest-integration = "^0.1.1a0"
+volttron-lib-boptest-integration = "^0.1.1a1"
 numpy = ">0.0.0"
 pandas = ">0.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=6.2.4"
 pytest-cov = ">=3.0.0"
 pytest-env = ">0.0.0"
```

### Comparing `volttron_boptest-0.1.1a0/src/boptest/agent.py` & `volttron_boptest-0.1.1a1/src/boptest/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a0/src/boptest/custom_kpi/README.md` & `volttron_boptest-0.1.1a1/src/boptest/custom_kpi/README.md`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a0/src/boptest/custom_kpi/custom_kpi_calculator.py` & `volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpi_calculator.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a0/src/boptest/custom_kpi/custom_kpis_example.py` & `volttron_boptest-0.1.1a1/src/boptest/custom_kpi/custom_kpis_example.py`

 * *Files identical despite different names*

### Comparing `volttron_boptest-0.1.1a0/PKG-INFO` & `volttron_boptest-0.1.1a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-boptest
-Version: 0.1.1a0
+Version: 0.1.1a1
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
-Requires-Dist: volttron-lib-boptest-integration (>=0.1.1a0,<0.2.0)
+Requires-Dist: volttron-lib-boptest-integration (>=0.1.1a1,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-boptest/issues
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-boptest
 Description-Content-Type: text/markdown
 
 # boptest-agent
 
 The volttron-boptest-agent utilizes the volttron-lib-boptest-integration library to perform simulation control and
@@ -78,14 +78,33 @@
 
 # Quick-start
 
 ### Setup environment and VOLTTRON platform
 
 The following recipe walks through the steps to install and demonstrate basic usage of "volttron-boptest" agent.
 
+The following recipe walks through the steps to install and run use case example.
+
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
 
    It is recommended to use a virtual environment for installing volttron.
 
     ```shell
     python -m venv env
     source env/bin/activate
@@ -156,14 +175,17 @@
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
    ```
 
    Note: Use `docker-compose down` to shut down the service.
 
 ### Install volttron boptest agent
 
 1. Install the "volttron-boptest" dependency.
@@ -181,58 +203,27 @@
     
     # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)
     pip install [-e] <path-to-the-source-code-root>/volttron-boptest/
     ```
 
 1. Install and start the "volttron-boptest" agent.
 
-   Prepare the default config files:
-
-    ```shell
-    # Create config file place holders
-    mkdir config
-    touch config/boptest_integration-agent-config.json
-    ```
-
-   Edit the `testcase1_config.yml` as follows:
-    ```yaml
-    {
-     "testcase_name": "testcase1",
-     "initialize":  # for GET/initialize
-     {
-       "start_time": 0,
-       "warmup_period": 0
-     },
-     "scenario": null,
-     "step": 300,
-     "length": 86400,
-   
-     "controller":
-     {
-       "type": "pid",  # currently support "pid", "sup", pidTwoZones"
-       "u":
-       {
-         "oveAct_u": 0,
-         "oveAct_activate": 1
-       }
-     }
-   
-   }
-    ```
-
-   Please see [examples/](examples) for other example config files.
+   We will use the [testcase1.config](examples/testcase1.config) as the agent config for this demo. Please
+   see [examples/](examples) for other example config files.
 
    Use `vctl install` command to register to the volttron home path.
    Note: for demo purposes and reproducibility, we assign vip-identity as "volttron_boptest_agent", but you can choose
    any other valid agent identity as desired.
 
     ```shell
-    vctl install volttron-boptest --agent-config <path-to-agent-config> \
+    (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl install volttron-boptest \
+   --agent-config volttron-boptest-agent/examples/testcase1.config \
    --vip-identity volttron_boptest_agent \
    --start
+   Agent a0fd6f5c-3751-4312-9f59-ca541b8aac4e installed and started [4980]
     ```
 
    Observe Data
 
    The volttron-boptest agent publishes events on the message bus. To see these events in the Volttron log file, install
    a [Listener Agent](https://pypi.org/project/volttron-listener/):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1a0 Summary: A
+Metadata-Version: 2.1 Name: volttron-boptest Version: 0.1.1a1 Summary: A
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
-(>=0.1.1a0,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
+(>=0.1.1a1,<0.2.0) Project-URL: Bug Tracker, https://github.com/eclipse-
 volttron/volttron-boptest/issues Project-URL: Repository, https://github.com/
 eclipse-volttron/volttron-boptest Description-Content-Type: text/markdown #
 boptest-agent The volttron-boptest-agent utilizes the volttron-lib-boptest-
 integration library to perform simulation control and benchmark tasks. BOPTEST
 is designed to facilitate the performance evaluation and benchmarking of
 building control strategies, which contains these key components: 1. Run-Time
 Environment (RTE): Deployed with Docker and accessed with a RESTful HTTP API,
@@ -31,29 +31,40 @@
 (e.g., Python 3.10), we recommend using pyenv. ```shell # install pyenv git
 clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also
 put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:$
 {PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install
 Python 3.10 pyenv install 3.10 # make it available globally pyenv global system
 3.10 ```  # Quick-start ### Setup environment and VOLTTRON platform The
 following recipe walks through the steps to install and demonstrate basic usage
-of "volttron-boptest" agent. 1. Create and activate a virtual environment. It
-is recommended to use a virtual environment for installing volttron. ```shell
-python -m venv env source env/bin/activate pip install volttron ``` 1. Install
-volttron and start the platform. > **Note**: > According to the [volttron-
-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup
-VOLTTRON_HOME > environment variable is mandatory: > ... if you have/had in the
-past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME >
-$HOME/.volttron. This modular version of VOLTTRON cannot work with
-volttron_home used by monolithic version of > VOLTTRON(version 8.3 or earlier)
-```shell # Setup environment variable `VOLTTRON_HOME` export VOLTTRON_HOME= #
-Start platform with output going to volttron.log volttron -vv -l volttron.log &
-``` ### Setup the boptest simulation server locally. In order to demonstrate
-the basic usage of volttron-boptest-agent, we need to setup the boptest
-simulation server. (Please see more details about boptest quick-start at
-[Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
+of "volttron-boptest" agent. The following recipe walks through the steps to
+install and run use case example. Note: For the ease of reproducibility, in
+this demo, we will git clone the [volttron-boptest](https://github.com/eclipse-
+volttron/volttron-boptest) repo to the `~/sandbox/` path. Feel free to modify
+the workflow as desired. ```shell kefei@ubuntu-22:~/sandbox$ git clone https://
+github.com/eclipse-volttron/volttron-boptest.git Cloning into 'volttron-
+boptest'... remote: Enumerating objects: 450, done. remote: Counting objects:
+100% (450/450), done. remote: Compressing objects: 100% (242/242), done.
+remote: Total 450 (delta 192), reused 424 (delta 170), pack-reused 0 Receiving
+objects: 100% (450/450), 3.66 MiB | 7.06 MiB/s, done. Resolving deltas: 100%
+(192/192), done. kefei@ubuntu-22:~/sandbox$ cd volttron-boptest/ kefei@ubuntu-
+22:~/sandbox/volttron-boptest$ ``` 1. Create and activate a virtual
+environment. It is recommended to use a virtual environment for installing
+volttron. ```shell python -m venv env source env/bin/activate pip install
+volttron ``` 1. Install volttron and start the platform. > **Note**: >
+According to the [volttron-core#README](https://github.com/eclipse-volttron/
+volttron-core#readme), setup VOLTTRON_HOME > environment variable is mandatory:
+> ... if you have/had in the past, a monolithic VOLTTRON version that used the
+default VOLTTRON_HOME > $HOME/.volttron. This modular version of VOLTTRON
+cannot work with volttron_home used by monolithic version of > VOLTTRON(version
+8.3 or earlier) ```shell # Setup environment variable `VOLTTRON_HOME` export
+VOLTTRON_HOME= # Start platform with output going to volttron.log volttron -vv
+-l volttron.log & ``` ### Setup the boptest simulation server locally. In order
+to demonstrate the basic usage of volttron-boptest-agent, we need to setup the
+boptest simulation server. (Please see more details about boptest quick-start
+at [Quick-Start to Deploy a Test Case](https://github.com/ibpsa/project1-
 boptest#quick-start-to-deploy-a-test-case)) 1. Download [IBPSA Project 1 -
 BOPTEST](https://github.com/ibpsa/project1-boptest) repository to . For demo
 purpose, let boptest_repo be `/tmp/project1-boptest`. ```shell git clone https:
 //github.com/ibpsa/project1-boptest /tmp/project1-boptest ``` 1. Install
 [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://
 docs.docker.com/compose/install/). (Optional) Verify with `docker-compose
 version` to verify the installation ```shell (env) kefei@ubuntu-22:~/sandbox/
@@ -71,43 +82,44 @@
 boptest_1 | 07/13/2023 09:59:42 PM UTC root INFO Test simulation initialized
 successfully to 0.0s with warmup period of 0.0s. boptest_1 | 07/13/2023 09:59:
 42 PM UTC root INFO Test case scenario was set successfully. ... boptest_1 | *
 Debug mode: off boptest_1 | 07/13/2023 09:59:42 PM UTC werkzeug INFO * Running
 on http://0.0.0.0:5000/ (Press CTRL+C to quit) ``` Or use detach mode ```shell
 (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ TESTCASE=testcase1 docker-
 compose --file /tmp/project1-boptest/docker-compose.yml up --detach Starting
-project1-boptest_boptest_1 ... done ``` Note: Use `docker-compose down` to shut
-down the service. ### Install volttron boptest agent 1. Install the "volttron-
-boptest" dependency. There are two options to install volttron-boptest. You can
-install this library using the version on PyPi or install it from the source
-code (`git clone` might be required.) Note: the `vctl install` command in the
-following step can handle dependency installation using pypi. However, in this
-demo we demonstrate what is happening under the neath the hood by separating
-the dependency installation and agent registry steps. ```shell # option 1:
-install from pypi pip install volttron-boptest # option 2: install from the
-source code (Note: `-e` option to use editable mode, useful for development.)
-pip install [-e] /volttron-boptest/ ``` 1. Install and start the "volttron-
-boptest" agent. Prepare the default config files: ```shell # Create config file
-place holders mkdir config touch config/boptest_integration-agent-config.json
-``` Edit the `testcase1_config.yml` as follows: ```yaml { "testcase_name":
-"testcase1", "initialize": # for GET/initialize { "start_time": 0,
-"warmup_period": 0 }, "scenario": null, "step": 300, "length": 86400,
-"controller": { "type": "pid", # currently support "pid", "sup", pidTwoZones"
-"u": { "oveAct_u": 0, "oveAct_activate": 1 } } } ``` Please see [examples/]
-(examples) for other example config files. Use `vctl install` command to
-register to the volttron home path. Note: for demo purposes and
-reproducibility, we assign vip-identity as "volttron_boptest_agent", but you
-can choose any other valid agent identity as desired. ```shell vctl install
-volttron-boptest --agent-config  \ --vip-identity volttron_boptest_agent \ --
-start ``` Observe Data The volttron-boptest agent publishes events on the
-message bus. To see these events in the Volttron log file, install a [Listener
-Agent](https://pypi.org/project/volttron-listener/): ``` vctl install volttron-
-listener --start ``` (Optional) Use `vctl stauts` to verify the installation
-```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl status UUID
-AGENT IDENTITY TAG PRIORITY STATUS HEALTH a volttron-boptest-agent-0.0.1
+project1-boptest_boptest_1 ... done (env) kefei@ubuntu-22:~/sandbox/volttron-
+boptest$ docker container ls CONTAINER ID IMAGE COMMAND CREATED STATUS PORTS
+NAMES ddd0f2cc1f99 boptest_base "/bin/sh -c 'python â¦" 23 hours ago Up 12
+seconds 127.0.0.1:5000->5000/tcp project1-boptest_boptest_1 ``` Note: Use
+`docker-compose down` to shut down the service. ### Install volttron boptest
+agent 1. Install the "volttron-boptest" dependency. There are two options to
+install volttron-boptest. You can install this library using the version on
+PyPi or install it from the source code (`git clone` might be required.) Note:
+the `vctl install` command in the following step can handle dependency
+installation using pypi. However, in this demo we demonstrate what is happening
+under the neath the hood by separating the dependency installation and agent
+registry steps. ```shell # option 1: install from pypi pip install volttron-
+boptest # option 2: install from the source code (Note: `-e` option to use
+editable mode, useful for development.) pip install [-e] /volttron-boptest/ ```
+1. Install and start the "volttron-boptest" agent. We will use the
+[testcase1.config](examples/testcase1.config) as the agent config for this
+demo. Please see [examples/](examples) for other example config files. Use
+`vctl install` command to register to the volttron home path. Note: for demo
+purposes and reproducibility, we assign vip-identity as
+"volttron_boptest_agent", but you can choose any other valid agent identity as
+desired. ```shell (env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl
+install volttron-boptest \ --agent-config volttron-boptest-agent/examples/
+testcase1.config \ --vip-identity volttron_boptest_agent \ --start Agent
+a0fd6f5c-3751-4312-9f59-ca541b8aac4e installed and started [4980] ``` Observe
+Data The volttron-boptest agent publishes events on the message bus. To see
+these events in the Volttron log file, install a [Listener Agent](https://
+pypi.org/project/volttron-listener/): ``` vctl install volttron-listener --
+start ``` (Optional) Use `vctl stauts` to verify the installation ```shell
+(env) kefei@ubuntu-22:~/sandbox/volttron-boptest$ vctl status UUID AGENT
+IDENTITY TAG PRIORITY STATUS HEALTH a volttron-boptest-agent-0.0.1
 volttron_boptest_agent running [59108] GOOD 2 volttron-listener-0.2.0rc0
 volttron-listener-0.2.0rc0_1 running [59096] GOOD ``` 1. (optional) Inspect the
 volttron.log file   Within the volttron.log, we should see similar logs as
 follows ```shell # Create config file place holders KPI RESULTS ----------
 - 2023-07-13 18:27:51,124 (volttron-boptest-agent-0.0.1 59108) root(186) INFO:
 emis_tot: 0.2147137757521314 KgCO2/m$^2$ 2023-07-13 18:27:51,174 (volttron-
 boptest-agent-0.0.1 59108) root(186) INFO: ener_tot: 1.073568878760657 kWh/
```

