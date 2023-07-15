# Comparing `tmp/heregpt-0.1.2.tar.gz` & `tmp/heregpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heregpt-0.1.2.tar", max compression
+gzip compressed data, was "heregpt-0.2.0.tar", max compression
```

## Comparing `heregpt-0.1.2.tar` & `heregpt-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-07-11 20:32:40.357792 heregpt-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-06 19:18:12.014744 heregpt-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-06 19:18:30.712845 heregpt-0.1.2/heregpt/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-11 20:29:30.277856 heregpt-0.1.2/heregpt/main.py
--rw-r--r--   0        0        0      547 2023-07-10 20:18:18.359202 heregpt-0.1.2/heregpt/models.py
--rw-r--r--   0        0        0     1621 2023-07-10 20:18:46.582158 heregpt-0.1.2/heregpt/utils.py
--rw-r--r--   0        0        0      668 2023-07-11 20:35:37.897210 heregpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 heregpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-11 20:32:40.357792 heregpt-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-06 19:18:12.014744 heregpt-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 19:18:30.712845 heregpt-0.2.0/heregpt/__init__.py
+-rw-r--r--   0        0        0     1846 2023-07-15 11:38:32.743700 heregpt-0.2.0/heregpt/main.py
+-rw-r--r--   0        0        0      547 2023-07-10 20:18:18.359202 heregpt-0.2.0/heregpt/models.py
+-rw-r--r--   0        0        0     1621 2023-07-10 20:18:46.582158 heregpt-0.2.0/heregpt/utils.py
+-rw-r--r--   0        0        0      668 2023-07-15 11:53:14.846797 heregpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 heregpt-0.2.0/PKG-INFO
```

### Comparing `heregpt-0.1.2/LICENSE` & `heregpt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heregpt-0.1.2/heregpt/main.py` & `heregpt-0.2.0/heregpt/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 import os
+from dataclasses import dataclass
 
 import typer
 from rich import print
 from rich.console import Console
 from typing_extensions import Annotated
 
 from heregpt import utils
 from heregpt.models import TaskBase
 
 app = typer.Typer()
 
 console = Console()
 
 
-@app.command()
-def main(
-    tool: Annotated[str, typer.Argument(help="Name of the tool you want to use")],
-    task: Annotated[str, typer.Argument(help="Describe the task you want to execute")],
-    openai_key: Annotated[
-        str, typer.Option(help="Manually provided API key for OpenAI")
-    ] = None,
+@dataclass
+class CommonOptions:
+    # See this comment:
+    # https://github.com/tiangolo/typer/issues/153#issuecomment-1001993791
+    # for more details
+    openai_api_key: str
+
+
+@app.callback()
+def common(
+    ctx: typer.Context,
+    openai_key: str = typer.Option(None, help="Manually provided API key for OpenAI"),
 ):
+    """Common Entry Point"""
+    ctx.obj = CommonOptions(openai_key)
     if openai_key is not None:
         os.environ["OPENAI_API_KEY"] = openai_key
     if openai_key is None:
         if not utils.set_openai_api_key():
             console.print(
                 "The environment variable OPENAI_API_KEY is not defined. More details"
                 " here:"
             )
             console.print(utils.set_openai_api_key.__doc__)
             raise typer.Exit(42)
+
+
+@app.command()
+def generic(prompt: Annotated[str, typer.Argument(help="Provide a generic prompt")]):
+    response = utils.get_completion(prompt)
+    console.print(response)
+
+
+@app.command()
+def tool_help(
+    tool: Annotated[str, typer.Argument(help="Name of the tool you want to use")],
+    task: Annotated[str, typer.Argument(help="Describe the task you want to execute")],
+):
     task = TaskBase(tool=tool, task=task)
     task.build_prompt()
     console.print("About to send the following prompt🚀", style="#5f5fff")
     print(task.prompt)
     console.print("End of prompt", style="#5f5fff")
     abort = typer.confirm("Abort?", default=True)
     if abort:
```

### Comparing `heregpt-0.1.2/heregpt/models.py` & `heregpt-0.2.0/heregpt/models.py`

 * *Files identical despite different names*

### Comparing `heregpt-0.1.2/heregpt/utils.py` & `heregpt-0.2.0/heregpt/utils.py`

 * *Files identical despite different names*

### Comparing `heregpt-0.1.2/pyproject.toml` & `heregpt-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heregpt"
-version = "0.1.2"
+version = "0.2.0"
 description = "Have ChatGPT right_here_ within your shell"
 authors = ["Dror Atariah <drorata@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/drorata/heregpt"
```

