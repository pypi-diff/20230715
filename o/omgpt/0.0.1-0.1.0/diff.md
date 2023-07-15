# Comparing `tmp/omgpt-0.0.1.tar.gz` & `tmp/omgpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.1.tar", max compression
+gzip compressed data, was "omgpt-0.1.0.tar", max compression
```

## Comparing `omgpt-0.0.1.tar` & `omgpt-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.1/LICENSE
--rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.1/README.md
--rw-r--r--   0        0        0     2820 2023-07-15 01:17:15.977115 omgpt-0.0.1/omgpt.py
--rw-r--r--   0        0        0      530 2023-07-15 01:17:01.235919 omgpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    11536 1970-01-01 00:00:00.000000 omgpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.1.0/LICENSE
+-rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.1.0/README.md
+-rw-r--r--   0        0        0     2438 2023-07-14 07:40:38.582140 omgpt-0.1.0/omgpt.py
+-rw-r--r--   0        0        0      530 2023-07-15 00:51:14.729745 omgpt-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11536 1970-01-01 00:00:00.000000 omgpt-0.1.0/PKG-INFO
```

### Comparing `omgpt-0.0.1/LICENSE` & `omgpt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.1/README.md` & `omgpt-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.1/omgpt.py` & `omgpt-0.1.0/omgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 from langchain.agents import AgentType, initialize_agent
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationBufferMemory
 from langchain.prompts import MessagesPlaceholder
 from langchain.schema import SystemMessage
-from langchain.tools import Tool
 from prompt_toolkit import PromptSession, prompt
 from prompt_toolkit.history import FileHistory
 
-from shtool import ShellTool, ShellToolSchema
+from shtool import make_shell_tool
 
 DEFAULT_CONFIG = {
     "settings": {
         "chat_model": "gpt-3.5-turbo-0613",
         "system_prompt": "You are a shell. Your name is OMGpt.",
         "temperature": "0",
     },
@@ -26,29 +25,36 @@
 def load_config():
     config = configparser.ConfigParser()
     config.read_dict(DEFAULT_CONFIG)
     config.read("config.ini")
     return config
 
 
-def init_agent_with_tools(tools, config, verbose):
+def load_tools():
+    return [
+        make_shell_tool(),
+    ]
+
+
+def init_agent_with_tools(config, verbose):
     system_prompt = SystemMessage(content=config.get("settings", "system_prompt"))
     agent_kwargs = {
         "extra_prompt_messages": [MessagesPlaceholder(variable_name="memory")],
         "system_message": system_prompt,
     }
     memory = ConversationBufferMemory(memory_key="memory", return_messages=True)
     chat = ChatOpenAI(
         model=config.get("settings", "chat_model"),
         temperature=float(config.get("settings", "temperature")),
         openai_api_key=config.get("api", "openai_api_key"),
         request_timeout=60,
         streaming=True,
         callbacks=[StreamingStdOutCallbackHandler()],
     )
+    tools = load_tools()
     agent = initialize_agent(
         tools,
         chat,
         agent=AgentType.OPENAI_FUNCTIONS,
         verbose=verbose,
         agent_kwargs=agent_kwargs,
         memory=memory,
@@ -71,26 +77,14 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-v", "--verbose", action="store_true", help="Increase output verbosity"
     )
     args = parser.parse_args()
 
     config = load_config()
-    shell_tool = ShellTool()
-    try:
-        tools = [
-            Tool.from_function(
-                func=shell_tool,
-                name="sh",
-                description="Useful when you need to run a shell command and get standard output and errors.",
-                args_schema=ShellToolSchema,
-                handle_tool_error=True,
-            )
-        ]
-        agent = init_agent_with_tools(tools, config, verbose=args.verbose)
-        run(agent)
-    finally:
-        shell_tool.close()
+    agent = init_agent_with_tools(config, verbose=args.verbose)
+
+    run(agent)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `omgpt-0.0.1/pyproject.toml` & `omgpt-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omgpt"
-version = "0.0.1"
+version = "0.1.0"
 description = "An AI-powered command-line interface"
 authors = ["Youngwook Kim <youngwook.kim@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 langchain = "^0.0.230"
```

### Comparing `omgpt-0.0.1/PKG-INFO` & `omgpt-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.1
+Version: 0.1.0
 Summary: An AI-powered command-line interface
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

