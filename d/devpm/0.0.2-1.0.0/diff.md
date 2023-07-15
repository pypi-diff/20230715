# Comparing `tmp/devpm-0.0.2.tar.gz` & `tmp/devpm-1.0.0.tar.gz`

## Comparing `devpm-0.0.2.tar` & `devpm-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,20 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 devpm-0.0.2/.DS_Store
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-0.0.2/src/devpm/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 devpm-0.0.2/src/devpm/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 devpm-0.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-0.0.2/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 devpm-0.0.2/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 devpm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 devpm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 devpm-1.0.0/devpackage.schema.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/cli/base_command.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/cli/main.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/commands/install.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/bash.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/code.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/context.py
+-rw-r--r--   0        0        0     8503 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/git.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/log.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/pip.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.0.0/LICENSE
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 devpm-1.0.0/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 devpm-1.0.0/PKG-INFO
```

### Comparing `devpm-0.0.2/.gitignore` & `devpm-1.0.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -154,7 +154,14 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# macOS
+.DS_Store
+
+# devpm
+dev_modules/
+.pre-commit-config.yaml
```

### Comparing `devpm-0.0.2/LICENSE` & `devpm-1.0.0/LICENSE`

 * *Files identical despite different names*

