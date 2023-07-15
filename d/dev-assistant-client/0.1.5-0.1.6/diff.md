# Comparing `tmp/dev-assistant-client-0.1.5.tar.gz` & `tmp/dev-assistant-client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.5.tar", last modified: Wed Jul 12 11:26:03 2023, max compression
+gzip compressed data, was "dev-assistant-client-0.1.6.tar", last modified: Sat Jul 15 02:27:22 2023, max compression
```

## Comparing `dev-assistant-client-0.1.5.tar` & `dev-assistant-client-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:26:03.929432 dev-assistant-client-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-06-27 03:10:31.000000 dev-assistant-client-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      343 2023-07-12 11:26:03.927435 dev-assistant-client-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2023-07-12 07:22:20.000000 dev-assistant-client-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 11:26:03.926434 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/
--rw-rw-rw-   0        0        0      343 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 11:26:03.929432 dev-assistant-client-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-07-12 11:25:56.000000 dev-assistant-client-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 02:26:55.000000 dev-assistant-client-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-15 02:26:55.000000 dev-assistant-client-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/setup.py
```

### Comparing `dev-assistant-client-0.1.5/README.md` & `dev-assistant-client-0.1.6/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-# Dev Assistant
-
-Welcome to the [Dev Assistant](https://devassistant.tonet.dev) plugin for ChatGPT.
-
-## What is it?
-
-[Dev Assistant](https://devassistant.tonet.dev) is a plugin for ChatGPT that assists us developers by executing tasks directly on our devices.
-
-Dev Assistant Client (this repo) is a Python package that is basically the core component of the project. It receives instructions from ChatGPT via Dev Assistant plugin, executes it on any of your devices and send the response back.
-
-## Features
-
-The Dev Assistant Local Client is designed to streamline your development process by offering a range of functionalities:
-
-- **File Management**: Create, read, update, and delete files. List the contents of a directory.
-
-- **Git Version Control**: Initialize a Git repository, add changes to the staging area, commit changes, and push changes to a remote repository. Get the status of the Git repository.
-
-- **Terminal Commands Execution**: Execute commands directly in the terminal.
-
-## Requirements
-
-- 👌🏼 Python 3.6+
-- 👌🏼 pip
-- 💸 ChatGPT Plus subscription _(for plugins store access)_
-
-## Installation
-
-- Create a Dev Assistant account at [devassistant.tonet.dev](https://devassistant.tonet.dev)
-- Generate a token at [devassistant.tonet.dev/token](https://devassistant.tonet.dev/token) for ChatGPT and save it. You'll need it later.
-- Install the local client:
-  - [Install Python](https://www.python.org/downloads/)
-  - [Install pip](https://pip.pypa.io/en/stable/installing/)
-  - Run `pip install dev-assistant-client` in your terminal
-  - You will be prompted to enter your email and password. Enter the credentials you used to create your Dev Assistant account.
-  - If everything went well, you should see a message saying "Successfully logged in!" and the client will be listening for instructions from ChatGPT.
-- Install the ChatGPT plugin:
-  - On the [ChatGPT Plugins Store](https://chat.openai.com/plugins), click in the **"Install an unverified plugin"** at bottom of Plugin store dialog window, paste the <https://devassistant.tonet.dev> and click on "Find plugin".
-  - ChatGPT will ask you to enter your credentials. Insert the token generated in the previous step and click "Install plugin".
-  - Enable the plugin in the list of installed plugins and you're good to go!
- 
-## Usage
-
-Once installed, you can use the `dev-assistant` command in your terminal to start the client.
-
-If you're not already logged in, you'll be prompted to enter your email and password. Once authenticated, the client will automatically establish a connection with the server.
-
-You can now ask ChatGPT to execute commands on your device.
-
-You can do `CRTL+C` to stop the client at any time.
-
-To log out, use:
-
-```bash
-dev-assistant logout
-```
-
-This command will remove your saved authentication token, ensuring your security.
-
-## Contributing
-
-We welcome contributions! If you have an idea for an improvement or have found a bug, please open an issue. Feel free to fork the repository and submit a pull request if you'd like to contribute code.
-
-## License
-
-The Dev Assistant Local Client is open-source software, licensed under the [MIT license](LICENSE).
-
-## Support
-
-If you encounter any problems or have any questions, don't hesitate to open an issue on GitHub. We're here to help!
-
-## Acknowledgements
-
-A big thank you to all contributors and users for your support! We couldn't do it without you.
-
-## Authors
-
-- [Luciano T.](https://github.com/lucianotonet)
-- [ChatGPT](https://chat.openai.com/)
+# Dev Assistant
+
+Welcome to the [Dev Assistant](https://devassistant.tonet.dev) plugin for ChatGPT.
+
+## What is it?
+
+[Dev Assistant](https://devassistant.tonet.dev) is a plugin for ChatGPT that assists us developers by executing tasks directly on our devices.
+
+Dev Assistant Client (this repo) is a Python package that is basically the core component of the project. It receives instructions from ChatGPT via Dev Assistant plugin, executes it on any of your devices and send the response back.
+
+## Features
+
+The Dev Assistant Local Client is designed to streamline your development process by offering a range of functionalities:
+
+- **File Management**: Create, read, update, and delete files. List the contents of a directory.
+
+- **Git Version Control**: Initialize a Git repository, add changes to the staging area, commit changes, and push changes to a remote repository. Get the status of the Git repository.
+
+- **Terminal Commands Execution**: Execute commands directly in the terminal.
+
+## Requirements
+
+- 👌🏼 Python 3.6+
+- 👌🏼 pip
+- 💸 ChatGPT Plus subscription _(for plugins store access)_
+
+## Installation
+
+- Create a Dev Assistant account at [devassistant.tonet.dev](https://devassistant.tonet.dev)
+- Generate a token at [devassistant.tonet.dev/token](https://devassistant.tonet.dev/token) for ChatGPT and save it. You'll need it later.
+- Install the local client:
+  - [Install Python](https://www.python.org/downloads/)
+  - [Install pip](https://pip.pypa.io/en/stable/installing/)
+  - Run `pip install dev-assistant-client` in your terminal
+  - You will be prompted to enter your email and password. Enter the credentials you used to create your Dev Assistant account.
+  - If everything went well, you should see a message saying "Successfully logged in!" and the client will be listening for instructions from ChatGPT.
+- Install the ChatGPT plugin:
+  - On the [ChatGPT Plugins Store](https://chat.openai.com/plugins), click in the **"Install an unverified plugin"** at bottom of Plugin store dialog window, paste the <https://devassistant.tonet.dev> and click on "Find plugin".
+  - ChatGPT will ask you to enter your credentials. Insert the token generated in the previous step and click "Install plugin".
+  - Enable the plugin in the list of installed plugins and you're good to go!
+ 
+## Usage
+
+Once installed, you can use the `dev-assistant` command in your terminal to start the client.
+
+If you're not already logged in, you'll be prompted to enter your email and password. Once authenticated, the client will automatically establish a connection with the server.
+
+You can now ask ChatGPT to execute commands on your device.
+
+You can do `CRTL+C` to stop the client at any time.
+
+To log out, use:
+
+```bash
+dev-assistant logout
+```
+
+This command will remove your saved authentication token, ensuring your security.
+
+## Contributing
+
+We welcome contributions! If you have an idea for an improvement or have found a bug, please open an issue. Feel free to fork the repository and submit a pull request if you'd like to contribute code.
+
+## License
+
+The Dev Assistant Local Client is open-source software, licensed under the [MIT license](LICENSE).
+
+## Support
+
+If you encounter any problems or have any questions, don't hesitate to open an issue on GitHub. We're here to help!
+
+## Acknowledgements
+
+A big thank you to all contributors and users for your support! We couldn't do it without you.
+
+## Authors
+
+- [Luciano T.](https://github.com/lucianotonet)
+- [ChatGPT](https://chat.openai.com/)
 - [GitHub Copilot](https://copilot.github.com/)
```

### Comparing `dev-assistant-client-0.1.5/setup.py` & `dev-assistant-client-0.1.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup, find_packages
-
-with open('requirements.txt') as f:
-    required = f.read().splitlines()
-
-setup(
-    name='dev-assistant-client',
-    version='0.1.5',
-    url='https://github.com/lucianotonet/dev-assistant-client',
-    author='Luciano Tonet',
-    author_email='tonetlds@gmail.com',
-    description='A local extension for ChatGPT plugin DevAssistant, which helps you with your development tasks straight in your machine.',
-    packages=find_packages(),
-    install_requires=required,
-    entry_points={
-        'console_scripts': [
-            'dev-assistant=dev_assistant_client.main:run',
-            'devassistant=dev_assistant_client.main:run',
-            'dev-assistant-client=dev_assistant_client.main:run',
-        ],
-    },
+from setuptools import setup, find_packages
+
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
+setup(
+    name='dev-assistant-client',
+    version='0.1.6',
+    url='https://github.com/lucianotonet/dev-assistant-client',
+    author='Luciano Tonet',
+    author_email='tonetlds@gmail.com',
+    description='A local extension for ChatGPT plugin DevAssistant, which helps you with your development tasks straight in your machine.',
+    packages=find_packages(),
+    install_requires=required,
+    entry_points={
+        'console_scripts': [
+            'dev-assistant=dev_assistant_client.main:run',
+            'devassistant=dev_assistant_client.main:run',
+            'dev-assistant-client=dev_assistant_client.main:run',
+        ],
+    },
 )
```

