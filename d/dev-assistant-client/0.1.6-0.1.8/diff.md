# Comparing `tmp/dev-assistant-client-0.1.6.tar.gz` & `tmp/dev-assistant-client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.6.tar", last modified: Sat Jul 15 02:27:22 2023, max compression
+gzip compressed data, was "dev-assistant-client-0.1.8.tar", last modified: Sat Jul 15 02:54:42 2023, max compression
```

## Comparing `dev-assistant-client-0.1.6.tar` & `dev-assistant-client-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 02:26:55.000000 dev-assistant-client-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-15 02:26:55.000000 dev-assistant-client-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/dev_assistant_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:27:22.548164 dev-assistant-client-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 02:27:22.000000 dev-assistant-client-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 02:54:21.000000 dev-assistant-client-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-15 02:54:21.000000 dev-assistant-client-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 02:54:21.000000 dev-assistant-client-0.1.8/setup.py
```

### Comparing `dev-assistant-client-0.1.6/LICENSE` & `dev-assistant-client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-assistant-client-0.1.6/README.md` & `dev-assistant-client-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 Dev Assistant Client (this repo) is a Python package that is basically the core component of the project. It receives instructions from ChatGPT via Dev Assistant plugin, executes it on any of your devices and send the response back.
 
 ## Features
 
 The Dev Assistant Local Client is designed to streamline your development process by offering a range of functionalities:
 
-- **File Management**: Create, read, update, and delete files. List the contents of a directory.
+- **File Management**: Create, read, update, and delete files. List the contents of a directory. You can manage your files without leaving your conversation with ChatGPT.
 
-- **Git Version Control**: Initialize a Git repository, add changes to the staging area, commit changes, and push changes to a remote repository. Get the status of the Git repository.
+- **Git Version Control**: Initialize a Git repository, add changes to the staging area, commit changes, and push changes to a remote repository. Get the status of the Git repository. You can manage your Git repositories directly through ChatGPT.
 
-- **Terminal Commands Execution**: Execute commands directly in the terminal.
+- **Terminal Commands Execution**: Execute commands directly in the terminal. You can run any command in your terminal directly from ChatGPT.
 
 ## Requirements
 
 - 👌🏼 Python 3.6+
 - 👌🏼 pip
 - 💸 ChatGPT Plus subscription _(for plugins store access)_
 
@@ -41,29 +41,29 @@
  
 ## Usage
 
 Once installed, you can use the `dev-assistant` command in your terminal to start the client.
 
 If you're not already logged in, you'll be prompted to enter your email and password. Once authenticated, the client will automatically establish a connection with the server.
 
-You can now ask ChatGPT to execute commands on your device.
+You can now ask ChatGPT to execute commands on your device. For example, you can ask ChatGPT to create a new file, add changes to a Git repository, or run a command in the terminal.
 
 You can do `CRTL+C` to stop the client at any time.
 
 To log out, use:
 
 ```bash
 dev-assistant logout
 ```
 
 This command will remove your saved authentication token, ensuring your security.
 
 ## Contributing
 
-We welcome contributions! If you have an idea for an improvement or have found a bug, please open an issue. Feel free to fork the repository and submit a pull request if you'd like to contribute code.
+We welcome contributions! If you have an idea for an improvement or have found a bug, please open an issue. Feel free to fork the repository and submit a pull request if you'd like to contribute code. Please follow the code style and conventions used in the existing codebase.
 
 ## License
 
 The Dev Assistant Local Client is open-source software, licensed under the [MIT license](LICENSE).
 
 ## Support
```

### Comparing `dev-assistant-client-0.1.6/setup.py` & `dev-assistant-client-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='dev-assistant-client',
-    version='0.1.6',
+    version='0.1.8',
     url='https://github.com/lucianotonet/dev-assistant-client',
     author='Luciano Tonet',
     author_email='tonetlds@gmail.com',
     description='A local extension for ChatGPT plugin DevAssistant, which helps you with your development tasks straight in your machine.',
     packages=find_packages(),
     install_requires=required,
     entry_points={
```

