# Comparing `tmp/cmdcomp-1.1.8.tar.gz` & `tmp/cmdcomp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.8.tar", max compression
+gzip compressed data, was "cmdcomp-1.2.0.tar", max compression
```

## Comparing `cmdcomp-1.1.8.tar` & `cmdcomp-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1512 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/README.md
--rw-r--r--   0        0        0       79 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2451 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/exception.py
--rw-r--r--   0        0        0       85 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/main.py
--rw-r--r--   0        0        0      131 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1732 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1696 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/README.md
+-rw-r--r--   0        0        0       79 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2446 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/app.py
+-rw-r--r--   0        0        0     2070 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3319 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/exception.py
+-rw-r--r--   0        0        0       85 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/main.py
+-rw-r--r--   0        0        0      131 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/shell.py
+-rw-r--r--   0        0        0     1732 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.2.0/PKG-INFO
```

### Comparing `cmdcomp-1.1.8/README.md` & `cmdcomp-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.8/cmdcomp/app.py` & `cmdcomp-1.2.0/cmdcomp/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         from rich.console import Console
         from rich.logging import RichHandler
 
         from cmdcomp import __version__
         from cmdcomp.completion import generate
         from cmdcomp.config.config import load
-        from cmdcomp.shell_type import ShellType
+        from cmdcomp.shell import ShellType
 
         parser = ArgumentParser(
             prog="cmdcomp",
             description="A command-line tool for comparing commands.",
         )
 
         parser.add_argument(
```

### Comparing `cmdcomp-1.1.8/cmdcomp/completion.py` & `cmdcomp-1.2.0/cmdcomp/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Command,
     Completions,
     SubCommandsCommand,
     get_candidates,
     get_targets,
 )
 from cmdcomp.config.config import Config
-from cmdcomp.shell_type import ShellType
+from cmdcomp.shell import ShellType
 
 
 def generate(shell: ShellType, config: Config):
     from jinja2 import Environment, FileSystemLoader
 
     env = Environment(
         loader=FileSystemLoader(Path(__file__).parent / "templates"),
@@ -48,15 +48,17 @@
 ):
     if keys is None:
         keys = []
 
     if not isinstance(command, SubCommandsCommand):
         return
 
-    for name, subcommand in command.subcommands.items():
+    for name, optional_subcommand in command.subcommands.items():
+        subcommand = optional_subcommand or SubCommandsCommand.model_validate({})
+
         new_keys = keys + ["|".join(get_targets(name, subcommand))]
 
         _update_completions_list(completions_list, subcommand, new_keys)
 
         candidates: Candidates = get_candidates(subcommand)
 
         if len(candidates) == 0:
```

### Comparing `cmdcomp-1.1.8/cmdcomp/config/app_info.py` & `cmdcomp-1.2.0/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.8/cmdcomp/config/command/command.py` & `cmdcomp-1.2.0/cmdcomp/config/command/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         StrOptions,
         Field(
             title="options of the command.",
             default_factory=list,
         ),
     ]
 
-    subcommands: OrderedDict[SubcommandName, "Command"] = Field(
+    subcommands: OrderedDict[SubcommandName, "Command | None"] = Field(
         title="subcommands of the command.",
         default_factory=OrderedDict,
     )
 
     @property
     def aliases(self) -> list[str]:
         if isinstance(self.alias, str):
@@ -83,15 +83,15 @@
             return [self.alias]
         else:
             return self.alias
 
 
 Command = SubCommandsCommand | SpecificOptionsCommand
 
-Subcommands = OrderedDict[SubcommandName, Command]
+Subcommands = OrderedDict[SubcommandName, Command | None]
 
 
 def get_targets(name: SubcommandName, subcommand: Command) -> list[str]:
     return [name] + subcommand.aliases
 
 
 def get_candidates(command: Command) -> Candidates:
@@ -100,15 +100,18 @@
             return (
                 [command.options]
                 if isinstance(command.options, str)
                 else command.options
             ) + reduce(
                 add,
                 [
-                    get_targets(name, subcommand)
+                    get_targets(
+                        name,
+                        subcommand or SubCommandsCommand.model_validate({}),
+                    )
                     for name, subcommand in command.subcommands.items()
                 ],
                 [],
             )
         case SpecificOptionsCommand():
             if isinstance(command.options, CommandOption):
                 return [{"command": f"$({command.options.execute})"}]
```

### Comparing `cmdcomp-1.1.8/cmdcomp/config/config.py` & `cmdcomp-1.2.0/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.8/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.2.0/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.8/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.2.0/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.8/pyproject.toml` & `cmdcomp-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.8"
+version = "1.2.0"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-1.1.8/PKG-INFO` & `cmdcomp-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.8
+Version: 1.2.0
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.8 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.2.0 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

