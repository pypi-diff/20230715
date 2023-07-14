# Comparing `tmp/codeinterpreterapi-0.0.1.tar.gz` & `tmp/codeinterpreterapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.1.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.2.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.1.tar` & `codeinterpreterapi-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.1/LICENSE
--rw-r--r--   0        0        0       91 2023-07-13 22:02:58.392781 codeinterpreterapi-0.0.1/README.md
--rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.1/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      932 2023-07-14 11:48:28.467799 codeinterpreterapi-0.0.1/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.1/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     3103 2023-07-14 09:32:35.455031 codeinterpreterapi-0.0.1/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0     1839 2023-07-14 09:33:47.559928 codeinterpreterapi-0.0.1/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      343 2023-07-14 10:21:21.788397 codeinterpreterapi-0.0.1/codeinterpreterapi/config.py
--rw-r--r--   0        0        0     9991 2023-07-14 13:56:53.960303 codeinterpreterapi-0.0.1/codeinterpreterapi/functions_agent.py
--rw-r--r--   0        0        0       77 2023-07-14 09:57:55.931208 codeinterpreterapi-0.0.1/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1593 2023-07-14 09:31:34.473034 codeinterpreterapi-0.0.1/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      460 2023-07-14 09:40:31.074021 codeinterpreterapi-0.0.1/codeinterpreterapi/schemas.py
--rw-r--r--   0        0        0     7740 2023-07-14 12:50:16.496400 codeinterpreterapi-0.0.1/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      548 2023-07-13 22:06:04.249861 codeinterpreterapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1859 2023-07-14 17:41:09.158967 codeinterpreterapi-0.0.2/README.md
+-rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.2/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.2/codeinterpreterapi/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.2/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.2/codeinterpreterapi/chains/functions_agent.py
+-rw-r--r--   0        0        0     3054 2023-07-14 17:11:05.973711 codeinterpreterapi-0.0.2/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0     1836 2023-07-14 17:11:05.948871 codeinterpreterapi-0.0.2/codeinterpreterapi/chains/remove_download_link.py
+-rw-r--r--   0        0        0      336 2023-07-14 17:11:05.942603 codeinterpreterapi-0.0.2/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0       78 2023-07-14 17:11:05.936317 codeinterpreterapi-0.0.2/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.2/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.2/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     1578 2023-07-14 17:11:05.961530 codeinterpreterapi-0.0.2/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.2/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.2/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0     7960 2023-07-14 17:36:03.828238 codeinterpreterapi-0.0.2/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      640 2023-07-14 17:42:41.115270 codeinterpreterapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.2/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.1/LICENSE` & `codeinterpreterapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.1/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.2/codeinterpreterapi/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,23 @@
     from codeinterpreterapi.session import CodeInterpreterSession
 
 
 class CodeCallbackHandler(AsyncIteratorCallbackHandler):
     def __init__(self, session: "CodeInterpreterSession"):
         self.session = session
         super().__init__()
-    
+
     async def on_agent_action(
         self,
         action: AgentAction,
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> None:
         """Run on agent action."""
         if action.tool == "python":
             await self.session.show_code(
                 f"⚙️ Running code: ```python\n{action.tool_input['code']}\n```"  # type: ignore
             )
         else:
-            raise ValueError(f"Unknown action: {action.tool}")
+            raise ValueError(f"Unknown action: {action.tool}")
```

### Comparing `codeinterpreterapi-0.0.1/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.0.2/codeinterpreterapi/chains/modifications_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,70 +14,69 @@
     SystemMessage,
 )
 
 
 prompt = ChatPromptTemplate(
     input_variables=["code"],
     messages=[
-        SystemMessage(content=
-            "The user will input some code and you will need to determine if the code makes any changes to the file system. \n"
+        SystemMessage(
+            content="The user will input some code and you will need to determine if the code makes any changes to the file system. \n"
             "With changes it means creating new files or modifying exsisting ones.\n"
             "Answer with a function call `determine_modifications` and list them inside.\n"
             "If the code does not make any changes to the file system, still answer with the function call but return an empty list.\n",
         ),
-        HumanMessagePromptTemplate.from_template("{code}")
-    ]
+        HumanMessagePromptTemplate.from_template("{code}"),
+    ],
 )
 
 functions = [
     {
         "name": "determine_modifications",
-        "description": 
-            "Based on code of the user determine if the code makes any changes to the file system. \n"
-            "With changes it means creating new files or modifying exsisting ones.\n",
+        "description": "Based on code of the user determine if the code makes any changes to the file system. \n"
+        "With changes it means creating new files or modifying exsisting ones.\n",
         "parameters": {
             "type": "object",
             "properties": {
                 "modifications": {
                     "type": "array",
-                    "items": { "type": "string" },
+                    "items": {"type": "string"},
                     "description": "The filenames that are modified by the code.",
                 },
             },
             "required": ["modifications"],
         },
     }
 ]
 
 
 async def get_file_modifications(
-    code: str, 
+    code: str,
     llm: BaseLanguageModel,
     retry: int = 2,
 ) -> List[str] | None:
-    if retry < 1: 
+    if retry < 1:
         return None
     messages = prompt.format_prompt(code=code).to_messages()
     message = await llm.apredict_messages(messages, functions=functions)
-    
+
     if not isinstance(message, AIMessage):
         raise OutputParserException("Expected an AIMessage")
-    
+
     function_call = message.additional_kwargs.get("function_call", None)
-    
+
     if function_call is None:
-        return await get_file_modifications(code, llm, retry=retry-1)
-    else: 
+        return await get_file_modifications(code, llm, retry=retry - 1)
+    else:
         function_call = json.loads(function_call["arguments"])
         return function_call["modifications"]
-    
+
 
 async def test():
     llm = ChatOpenAI(model="gpt-3.5-turbo-0613")  # type: ignore
-    
+
     code = """
     import matplotlib.pyplot as plt
 
     x = list(range(1, 11))
     y = [29, 39, 23, 32, 4, 43, 43, 23, 43, 77]
 
     plt.plot(x, y, marker='o')
@@ -85,19 +84,20 @@
     plt.ylabel('Value')
     plt.title('Data Plot')
 
     plt.show()
     """
 
     code2 = "import pandas as pd\n\n# Read the Excel file\ndata = pd.read_excel('Iris.xlsx')\n\n# Convert the data to CSV\ndata.to_csv('Iris.csv', index=False)"
-    
+
     modifications = await get_file_modifications(code2, llm)
-    
+
     print(modifications)
 
 
 if __name__ == "__main__":
     import asyncio
     from dotenv import load_dotenv
+
     load_dotenv()
-    
+
     asyncio.run(test())
```

### Comparing `codeinterpreterapi-0.0.1/codeinterpreterapi/chains/remove_download_link.py` & `codeinterpreterapi-0.0.2/codeinterpreterapi/chains/remove_download_link.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,55 +4,58 @@
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
 from langchain.schema import (
     AIMessage,
     OutputParserException,
     SystemMessage,
-    HumanMessage
+    HumanMessage,
 )
 
 
 prompt = ChatPromptTemplate(
     input_variables=["input_response"],
     messages=[
-        SystemMessage(content=
-            "The user will send you a response and you need to remove the download link from it.\n"
+        SystemMessage(
+            content="The user will send you a response and you need to remove the download link from it.\n"
             "Reformat the remaining message so no whitespace or half sentences are still there.\n"
             "If the response does not contain a download link, return the response as is.\n"
         ),
-        HumanMessage(content="The dataset has been successfully converted to CSV format. You can download the converted file [here](sandbox:/Iris.csv)."),
+        HumanMessage(
+            content="The dataset has been successfully converted to CSV format. You can download the converted file [here](sandbox:/Iris.csv)."
+        ),
         AIMessage(content="The dataset has been successfully converted to CSV format."),
-        HumanMessagePromptTemplate.from_template("{input_response}")
-    ]
+        HumanMessagePromptTemplate.from_template("{input_response}"),
+    ],
 )
 
 
 async def remove_download_link(
-    input_response: str, 
+    input_response: str,
     llm: BaseLanguageModel,
 ) -> str:
     messages = prompt.format_prompt(input_response=input_response).to_messages()
     message = await llm.apredict_messages(messages)
-    
+
     if not isinstance(message, AIMessage):
         raise OutputParserException("Expected an AIMessage")
-    
+
     return message.content
-    
+
 
 async def test():
     llm = ChatOpenAI(model="gpt-3.5-turbo-0613")  # type: ignore
-    
+
     example = "I have created the plot to your dataset.\n\nLink to the file [here](sandbox:/plot.png)."
-    
+
     modifications = await remove_download_link(example, llm)
-    
+
     print(modifications)
 
 
 if __name__ == "__main__":
     import asyncio
     import dotenv
+
     dotenv.load_dotenv()
-    
+
     asyncio.run(test())
```

### Comparing `codeinterpreterapi-0.0.1/codeinterpreterapi/functions_agent.py` & `codeinterpreterapi-0.0.2/codeinterpreterapi/chains/functions_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,27 +101,29 @@
     messages = []
 
     for intermediate_step in intermediate_steps:
         agent_action, observation = intermediate_step
         messages.extend(_convert_agent_action_to_messages(agent_action, observation))
 
     return messages
-    
 
-async def _parse_ai_message(message: BaseMessage, llm: BaseLanguageModel) -> Union[AgentAction, AgentFinish]:
+
+async def _parse_ai_message(
+    message: BaseMessage, llm: BaseLanguageModel
+) -> Union[AgentAction, AgentFinish]:
     """Parse an AI message."""
     if not isinstance(message, AIMessage):
         raise TypeError(f"Expected an AI message got {type(message)}")
 
     function_call = message.additional_kwargs.get("function_call", {})
 
     if function_call:
         function_call = message.additional_kwargs["function_call"]
         function_name = function_call["name"]
-        try:    
+        try:
             _tool_input = json.loads(function_call["arguments"])
         except JSONDecodeError:
             if function_name == "python":
                 code = function_call["arguments"]
                 _tool_input = {
                     "code": code,
                 }
@@ -195,16 +197,17 @@
         """Get input keys. Input refers to user input here."""
         return ["input"]
 
     @property
     def functions(self) -> List[dict]:
         return [dict(format_tool_to_openai_function(t)) for t in self.tools]
 
-    def plan(self): raise NotImplementedError
-    
+    def plan(self):
+        raise NotImplementedError
+
     async def aplan(
         self,
         intermediate_steps: List[Tuple[AgentAction, str]],
         callbacks: Callbacks = None,
         **kwargs: Any,
     ) -> Union[AgentAction, AgentFinish]:
         """Given input, decided what to do.
@@ -225,15 +228,15 @@
         prompt = self.prompt.format_prompt(**full_inputs)
         messages = prompt.to_messages()
         predicted_message = await self.llm.apredict_messages(
             messages, functions=self.functions, callbacks=callbacks
         )
         agent_decision = await _parse_ai_message(predicted_message, self.llm)
         return agent_decision
-    
+
     @classmethod
     def create_prompt(
         cls,
         system_message: Optional[SystemMessage] = SystemMessage(
             content="You are a helpful AI assistant."
         ),
         extra_prompt_messages: Optional[List[BaseMessagePromptTemplate]] = None,
```

### Comparing `codeinterpreterapi-0.0.1/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.2/codeinterpreterapi/prompts/system_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from langchain.schema import SystemMessage
 
 
-system_message = SystemMessage(content="""
+system_message = SystemMessage(
+    content="""
 Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. 
 As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 Assistant is constantly learning and improving, and its capabilities are constantly evolving. 
 It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, Assistant is able to generate its own text based on the input it receives, 
 allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
 
 This version of Assistant is called "Code Interpreter" and capable of using a python code interpreter (sandboxed jupyter kernel) to run code. 
 The human also maybe thinks this code interpreter is for writing code but it is more for data science, data analysis, and data visualization, file manipulation, and other things that can be done using a jupyter kernel/ipython runtime.
 Tell the human if they use the code interpreter incorrectly.
 Already installed packages are: (numpy pandas matplotlib seaborn scikit-learn yfinance scipy statsmodels sympy bokeh plotly dash networkx).
 If you encounter an error, try again and fix the code.
-""")
+"""
+)
```

### Comparing `codeinterpreterapi-0.0.1/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.2/codeinterpreterapi/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,180 +5,189 @@
 from langchain.tools import StructuredTool
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts.chat import MessagesPlaceholder
 from langchain.agents import AgentExecutor, BaseSingleActionAgent
 from langchain.memory import ConversationBufferMemory
 
-from codeinterpreterapi.schemas import CodeInterpreterResponse, CodeInput, File, UserRequest # type: ignore
+from codeinterpreterapi.schema import CodeInterpreterResponse, CodeInput, File, UserRequest  # type: ignore
 from codeinterpreterapi.config import settings
-from codeinterpreterapi.functions_agent import OpenAIFunctionsAgent
+from codeinterpreterapi.chains.functions_agent import OpenAIFunctionsAgent
 from codeinterpreterapi.prompts import code_interpreter_system_message
 from codeinterpreterapi.callbacks import CodeCallbackHandler
 from codeinterpreterapi.chains.modifications_check import get_file_modifications
 from codeinterpreterapi.chains.remove_download_link import remove_download_link
 
 
-class CodeInterpreterSession():
-    
+class CodeInterpreterSession:
     def __init__(self, model=None, openai_api_key=None) -> None:
         self.codebox = CodeBox()
         self.tools: list[StructuredTool] = self._tools()
         self.llm: BaseChatModel = self._llm(model, openai_api_key)
         self.agent_executor: AgentExecutor = self._agent_executor()
         self.input_files: list[File] = []
         self.output_files: list[File] = []
     
-    async def _init(self) -> None:
+    async def astart(self) -> None:
         await self.codebox.astart()
-    
-    async def _close(self) -> None:
-        await self.codebox.astop()
-    
+
     def _tools(self) -> list[StructuredTool]:
         return [
             StructuredTool(
-                name = "python",
-                description = 
-                    # TODO: variables as context to the agent
-                    # TODO: current files as context to the agent
-                    "Input a string of code to a python interpreter (jupyter kernel). "
-                    "Variables are preserved between runs. ",
-                func = self.codebox.run,
-                coroutine = self.arun_handler,
-                args_schema = CodeInput,
+                name="python",
+                description=
+                # TODO: variables as context to the agent
+                # TODO: current files as context to the agent
+                "Input a string of code to a python interpreter (jupyter kernel). "
+                "Variables are preserved between runs. ",
+                func=self.codebox.run,
+                coroutine=self.arun_handler,
+                args_schema=CodeInput,
             ),
         ]
-        
+
     def _llm(self, model: str | None, openai_api_key: str | None) -> BaseChatModel:
         if model is None:
             model = "gpt-4"
-        
+
         if openai_api_key is None:
             if settings.OPENAI_API_KEY is None:
                 raise ValueError("OpenAI API key missing.")
             else:
                 openai_api_key = settings.OPENAI_API_KEY
-        
+
         return ChatOpenAI(
             temperature=0.03,
-            model=model, 
+            model=model,
             openai_api_key=openai_api_key,
             max_retries=3,
-            request_timeout=60*3,
+            request_timeout=60 * 3,
         )  # type: ignore
-    
+
     def _agent(self) -> BaseSingleActionAgent:
         return OpenAIFunctionsAgent.from_llm_and_tools(
             llm=self.llm,
             tools=self.tools,
             system_message=code_interpreter_system_message,
             extra_prompt_messages=[MessagesPlaceholder(variable_name="memory")],
         )
-        
+
     def _agent_executor(self) -> AgentExecutor:
         return AgentExecutor.from_agent_and_tools(
             agent=self._agent(),
             callbacks=[CodeCallbackHandler(self)],
             max_iterations=9,
             tools=self.tools,
             verbose=settings.VERBOSE,
             memory=ConversationBufferMemory(memory_key="memory", return_messages=True),
         )
-    
+
     async def show_code(self, code: str) -> None:
-        """ Callback function to show code to the user. """
+        """Callback function to show code to the user."""
         if settings.VERBOSE:
             print(code)
-    
-    def run_handler(self, code: str): 
+
+    def run_handler(self, code: str):
         raise NotImplementedError("Use arun_handler for now.")
-    
+
     async def arun_handler(self, code: str):
-        """ Run code in container and send the output to the user """
+        """Run code in container and send the output to the user"""
         # TODO: upload files
         output: CodeBoxOutput = await self.codebox.arun(code)
-        
+
         if not isinstance(output.content, str):
             raise TypeError("Expected output.content to be a string.")
-        
+
         if output.type == "image/png":
             filename = f"image-{uuid.uuid4()}.png"
             file_buffer = BytesIO(base64.b64decode(output.content))
             file_buffer.name = filename
             self.output_files.append(File(name=filename, content=file_buffer.read()))
             return f"Image {filename} got send to the user."
 
-        elif output.type == "error": 
-            # TODO: check if package install is required
+        elif output.type == "error":
+            if "ModuleNotFoundError" in output.content:
+                if package := re.search(
+                    r"ModuleNotFoundError: No module named '(.*)'", output.content
+                ):
+                    await self.codebox.ainstall(package.group(1))
+                    return f"{package.group(1)} was missing but got installed now. Please try again."
             # TODO: preanalyze error to optimize next code generation
             print("Error:", output.content)
-        
-        elif (modifications := await get_file_modifications(code, self.llm)):
+
+        elif modifications := await get_file_modifications(code, self.llm):
             for filename in modifications:
-                if filename in [file.name for file in self.input_files]: 
+                if filename in [file.name for file in self.input_files]:
                     continue
                 fileb = await self.codebox.adownload(filename)
-                if not fileb.content: 
+                if not fileb.content:
                     continue
                 file_buffer = BytesIO(fileb.content)
                 file_buffer.name = filename
-                self.output_files.append(File(name=filename, content=file_buffer.read()))
-            
+                self.output_files.append(
+                    File(name=filename, content=file_buffer.read())
+                )
+
         return output.content
-    
+
     async def input_handler(self, request: UserRequest):
-        if not request.files: 
+        if not request.files:
             return
         if not request.content:
-            request.content = "I uploaded, just text me back and confirm that you got the file(s)."
+            request.content = (
+                "I uploaded, just text me back and confirm that you got the file(s)."
+            )
         request.content += "\n**The user uploaded the following files: **\n"
         for file in request.files:
             self.input_files.append(file)
             request.content += f"[Attachment: {file.name}]\n"
             await self.codebox.aupload(file.name, file.content)
         request.content += "**File(s) are now available in the cwd. **\n"
-    
+
     async def output_handler(self, final_response: str) -> CodeInterpreterResponse:
-        """ Embed images in the response """
+        """Embed images in the response"""
         for file in self.output_files:
             if str(file.name) in final_response:
                 # rm ![Any](file.name) from the response
                 final_response = re.sub(rf"\n\n!\[.*\]\(.*\)", "", final_response)
-        
+
         if self.output_files and re.search(rf"\n\[.*\]\(.*\)", final_response):
             final_response = await remove_download_link(final_response, self.llm)
-        
+
         return CodeInterpreterResponse(content=final_response, files=self.output_files)
-    
+
     async def generate_response(
-        self, 
-        user_msg: str, 
+        self,
+        user_msg: str,
         files: list[File] = [],
         detailed_error: bool = False,
     ) -> CodeInterpreterResponse:
-        """ Generate a Code Interpreter response based on the user's input."""
+        """Generate a Code Interpreter response based on the user's input."""
         user_request = UserRequest(content=user_msg, files=files)
         try:
             await self.input_handler(user_request)
             response = await self.agent_executor.arun(input=user_request.content)
             return await self.output_handler(response)
         except Exception as e:
             if settings.VERBOSE:
                 import traceback
+
                 traceback.print_exc()
             if detailed_error:
-                return CodeInterpreterResponse(content=
-                    f"Error in CodeInterpreterSession: {e.__class__.__name__}  - {e}"
+                return CodeInterpreterResponse(
+                    content=f"Error in CodeInterpreterSession: {e.__class__.__name__}  - {e}"
                 )
             else:
-                return CodeInterpreterResponse(content=
-                    "Sorry, something went while generating your response."
+                return CodeInterpreterResponse(
+                    content="Sorry, something went while generating your response."
                     "Please try again or restart the session."
                 )
 
+    async def astop(self) -> None:
+        await self.codebox.astop()
+    
     async def __aenter__(self) -> "CodeInterpreterSession":
-        await self._init()
+        await self.astart()
         return self
-    
+
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
-        await self._close()
+        await self.astop()
```

