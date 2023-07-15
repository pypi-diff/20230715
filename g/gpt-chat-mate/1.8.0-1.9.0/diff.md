# Comparing `tmp/gpt-chat-mate-1.8.0.tar.gz` & `tmp/gpt-chat-mate-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-chat-mate-1.8.0.tar", last modified: Fri Mar 31 22:49:24 2023, max compression
+gzip compressed data, was "gpt-chat-mate-1.9.0.tar", last modified: Sat Apr  1 00:35:28 2023, max compression
```

## Comparing `gpt-chat-mate-1.8.0.tar` & `gpt-chat-mate-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 22:49:24.566754 gpt-chat-mate-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)    35076 2023-03-31 22:49:15.000000 gpt-chat-mate-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2191 2023-03-31 22:49:24.566754 gpt-chat-mate-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-03-31 22:49:15.000000 gpt-chat-mate-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 22:49:24.564753 gpt-chat-mate-1.8.0/gpt_chat_mate/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-03-31 22:49:15.000000 gpt-chat-mate-1.8.0/gpt_chat_mate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14185 2023-03-31 22:49:15.000000 gpt-chat-mate-1.8.0/gpt_chat_mate/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 22:49:24.566754 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2191 2023-03-31 22:49:24.000000 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      298 2023-03-31 22:49:24.000000 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 22:49:24.000000 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-31 22:49:24.000000 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-31 22:49:24.000000 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-31 22:49:24.000000 gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 22:49:24.566754 gpt-chat-mate-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-03-31 22:49:15.000000 gpt-chat-mate-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 00:35:28.509164 gpt-chat-mate-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35076 2023-04-01 00:35:18.000000 gpt-chat-mate-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-04-01 00:35:28.508164 gpt-chat-mate-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-01 00:35:18.000000 gpt-chat-mate-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 00:35:28.506164 gpt-chat-mate-1.9.0/gpt_chat_mate/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-01 00:35:18.000000 gpt-chat-mate-1.9.0/gpt_chat_mate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15256 2023-04-01 00:35:18.000000 gpt-chat-mate-1.9.0/gpt_chat_mate/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 00:35:28.508164 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-04-01 00:35:28.000000 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-01 00:35:28.000000 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 00:35:28.000000 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-01 00:35:28.000000 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-01 00:35:28.000000 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-01 00:35:28.000000 gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 00:35:28.509164 gpt-chat-mate-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-04-01 00:35:18.000000 gpt-chat-mate-1.9.0/setup.py
```

### Comparing `gpt-chat-mate-1.8.0/LICENSE` & `gpt-chat-mate-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-chat-mate-1.8.0/PKG-INFO` & `gpt-chat-mate-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gpt-chat-mate
-Version: 1.8.0
+Version: 1.9.0
 Summary: A cli app for communicating with chatGPT
 Home-page: https://gitlab.com/fizzizist/gpt-chat-mate
 Author: Fizzizist
 Author-email: gpt-chat-mate@fizzizist.33mail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GPTChatMate v1.8.0
+# GPTChatMate v1.9.0
 A python cli front-end for the chatGPT API.
 
 ## Installation
 Note: This app requires `sqlite3` version `>3.35.0`.
 ```
 pip install gpt-chat-mate
 ```
@@ -35,14 +35,16 @@
 that the app will send in a single API call.
 Note: the user will still be shown the full conversation history even if the token limits the conversation sent
 to the API.
 
 `openai_req_timeout` - The OpenAI API request can sometimes hang for an insane amount of time, so this sets a timeout.
 The default is 60.
 
+`default_editor` - The editor to use for things like editing an existing system prompt. The default is `vim`.
+
 ## Usage
 Install via pip, and run via the package name.
 ```
 gpt-chat-mate
 ```
 
 ### Commands
@@ -53,14 +55,16 @@
 
 `list`,`ls` - List existing chats stored in the database.
 
 `duplicate <ID>` - duplicates a chat with just the system prompt. (Does not duplicate the whole chat)
 
 `rename <ID> optional[<name>]` - rename a chat. If `<name>` is not given, chatGPT is used to rename it.
 
+`esp <ID>` - (e)dit (s)ystem (p)rompt allows you to edit the system prompt of a chat. (This has only been tested on a unix system).
+
 `help` - List available commands.
 
 `exit` - Exit the program.
 
 ### Special Prompt Keywords
 
 `paste` - You can use the paste command as a prompt to enter paste mode. Paste mode allows you to freely type or paste
```

### Comparing `gpt-chat-mate-1.8.0/README.md` & `gpt-chat-mate-1.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GPTChatMate v1.8.0
+# GPTChatMate v1.9.0
 A python cli front-end for the chatGPT API.
 
 ## Installation
 Note: This app requires `sqlite3` version `>3.35.0`.
 ```
 pip install gpt-chat-mate
 ```
@@ -20,14 +20,16 @@
 that the app will send in a single API call.
 Note: the user will still be shown the full conversation history even if the token limits the conversation sent
 to the API.
 
 `openai_req_timeout` - The OpenAI API request can sometimes hang for an insane amount of time, so this sets a timeout.
 The default is 60.
 
+`default_editor` - The editor to use for things like editing an existing system prompt. The default is `vim`.
+
 ## Usage
 Install via pip, and run via the package name.
 ```
 gpt-chat-mate
 ```
 
 ### Commands
@@ -38,14 +40,16 @@
 
 `list`,`ls` - List existing chats stored in the database.
 
 `duplicate <ID>` - duplicates a chat with just the system prompt. (Does not duplicate the whole chat)
 
 `rename <ID> optional[<name>]` - rename a chat. If `<name>` is not given, chatGPT is used to rename it.
 
+`esp <ID>` - (e)dit (s)ystem (p)rompt allows you to edit the system prompt of a chat. (This has only been tested on a unix system).
+
 `help` - List available commands.
 
 `exit` - Exit the program.
 
 ### Special Prompt Keywords
 
 `paste` - You can use the paste command as a prompt to enter paste mode. Paste mode allows you to freely type or paste
```

### Comparing `gpt-chat-mate-1.8.0/gpt_chat_mate/main.py` & `gpt-chat-mate-1.9.0/gpt_chat_mate/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import cmd
 import json
 import os
 import readline
 import sqlite3
+import subprocess
+import tempfile
 from dataclasses import asdict, dataclass
 
 import openai
 import tiktoken
 from func_timeout import FunctionTimedOut, func_timeout
 from pyfiglet import Figlet
 from pygments import highlight
@@ -19,14 +21,15 @@
 @dataclass
 class Config:
     db_filename: str
     gpt_model: str
     print_style: str
     token_limit: int
     openai_req_timeout: int = 60
+    default_editor: str = "vim"
 
 
 class ColorPalette:
     CYAN = "\033[96m"
     ENDC = "\033[0m"
 
 
@@ -320,15 +323,17 @@
 
     def do_ls(self, line):
         """Alias of list command"""
         return self.do_list(line)
 
     def do_duplicate(self, line):
         """
-        Duplicates a chat's system prompt into a new chat so that this doesn't have to be done manually by the user.
+        duplicate <ID>
+            Duplicates a chat's system prompt into a new chat so that this
+            doesn't have to be done manually by the user.
         """
         if not self.valid_id(line):
             return
 
         chat_id = self.db_query(
             """
             INSERT INTO chat (name)
@@ -342,15 +347,18 @@
             INSERT INTO message (chat_id, role, content)
             SELECT ?, role, content FROM message WHERE role = 'system' AND chat_id = ?;
         """,
             (chat_id, line),
         )
 
     def do_rename(self, line):
-        """Allows user to rename a chat."""
+        """
+        rename <ID> optional[<name>]
+            Allows user to rename a chat.
+        """
         args = line.split(" ")
         if not self.valid_id(args[0]):
             return
 
         chat_id = args[0]
         if len(args) > 1:
             new_name = " ".join(args[1:])
@@ -361,14 +369,41 @@
             )[0][0]
             new_name = self.generate_chat_name(system_prompt)
 
         self.db_query(
             "UPDATE chat SET name = ? WHERE chat_id = ?;", (new_name, chat_id)
         )
 
+    def do_esp(self, line):
+        """
+        esp <ID>
+            (e)dit (s)ystem (p)rompt allows user to edit the system prompt of a chat
+        """
+        if not self.valid_id(line):
+            return
+
+        system_prompt = self.db_query(
+            "SELECT content FROM message WHERE chat_id = ? AND role = 'system'",
+            (line,),
+        )[0][0]
+        with tempfile.NamedTemporaryFile(mode="w+", suffix=".tmp") as tmp_file:
+            tmp_file.write(system_prompt)
+            tmp_file.flush()
+
+            subprocess.call([self.config.default_editor, tmp_file.name])
+
+            tmp_file.seek(0)
+            system_prompt = tmp_file.read().strip()
+
+        self.db_query(
+            "UPDATE message SET content = ? WHERE role = 'system' AND chat_id = ?",
+            (system_prompt, line),
+        )
+        print(f"System prompt for chat {line} now set to:\n\n{system_prompt}")
+
     def set_config(self):
         if os.path.exists(".config.json"):
             with open(".config.json") as f:
                 self.config = Config(**json.load(f))
             return
 
         print("No config found. Generating one.")
```

### Comparing `gpt-chat-mate-1.8.0/gpt_chat_mate.egg-info/PKG-INFO` & `gpt-chat-mate-1.9.0/gpt_chat_mate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gpt-chat-mate
-Version: 1.8.0
+Version: 1.9.0
 Summary: A cli app for communicating with chatGPT
 Home-page: https://gitlab.com/fizzizist/gpt-chat-mate
 Author: Fizzizist
 Author-email: gpt-chat-mate@fizzizist.33mail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GPTChatMate v1.8.0
+# GPTChatMate v1.9.0
 A python cli front-end for the chatGPT API.
 
 ## Installation
 Note: This app requires `sqlite3` version `>3.35.0`.
 ```
 pip install gpt-chat-mate
 ```
@@ -35,14 +35,16 @@
 that the app will send in a single API call.
 Note: the user will still be shown the full conversation history even if the token limits the conversation sent
 to the API.
 
 `openai_req_timeout` - The OpenAI API request can sometimes hang for an insane amount of time, so this sets a timeout.
 The default is 60.
 
+`default_editor` - The editor to use for things like editing an existing system prompt. The default is `vim`.
+
 ## Usage
 Install via pip, and run via the package name.
 ```
 gpt-chat-mate
 ```
 
 ### Commands
@@ -53,14 +55,16 @@
 
 `list`,`ls` - List existing chats stored in the database.
 
 `duplicate <ID>` - duplicates a chat with just the system prompt. (Does not duplicate the whole chat)
 
 `rename <ID> optional[<name>]` - rename a chat. If `<name>` is not given, chatGPT is used to rename it.
 
+`esp <ID>` - (e)dit (s)ystem (p)rompt allows you to edit the system prompt of a chat. (This has only been tested on a unix system).
+
 `help` - List available commands.
 
 `exit` - Exit the program.
 
 ### Special Prompt Keywords
 
 `paste` - You can use the paste command as a prompt to enter paste mode. Paste mode allows you to freely type or paste
```

### Comparing `gpt-chat-mate-1.8.0/setup.py` & `gpt-chat-mate-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     ld = f.read()
 
 setup(
     name="gpt-chat-mate",
-    version="1.8.0",
+    version="1.9.0",
     description="A cli app for communicating with chatGPT",
     license="GPLv3",
     url="https://gitlab.com/fizzizist/gpt-chat-mate",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "gpt-chat-mate=gpt_chat_mate.main:main",
```

