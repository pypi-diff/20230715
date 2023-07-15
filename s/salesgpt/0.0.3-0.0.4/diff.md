# Comparing `tmp/salesgpt-0.0.3.tar.gz` & `tmp/salesgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesgpt-0.0.3.tar", last modified: Tue Jul  4 17:51:44 2023, max compression
+gzip compressed data, was "salesgpt-0.0.4.tar", last modified: Sat Jul 15 13:51:46 2023, max compression
```

## Comparing `salesgpt-0.0.3.tar` & `salesgpt-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.433331 salesgpt-0.0.3/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1071 2023-06-19 23:47:34.000000 salesgpt-0.0.3/LICENSE
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       24 2023-06-30 17:23:56.000000 salesgpt-0.0.3/MANIFEST.in
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-07-04 17:51:44.432949 salesgpt-0.0.3/PKG-INFO
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     5977 2023-06-30 17:23:56.000000 salesgpt-0.0.3/README.md
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      103 2023-06-30 17:23:56.000000 salesgpt-0.0.3/requirements.txt
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.428948 salesgpt-0.0.3/salesgpt/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        0 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/__init__.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     7930 2023-07-04 17:48:11.000000 salesgpt-0.0.3/salesgpt/agents.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6447 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/chains.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1119 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/logger.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1606 2023-06-30 17:23:56.000000 salesgpt-0.0.3/salesgpt/stages.py
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       50 2023-07-04 17:48:59.000000 salesgpt-0.0.3/salesgpt/version.py
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.431755 salesgpt-0.0.3/salesgpt.egg-info/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     6750 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/PKG-INFO
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      354 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/SOURCES.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        1 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/dependency_links.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)      157 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/requires.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)        9 2023-07-04 17:51:44.000000 salesgpt-0.0.3/salesgpt.egg-info/top_level.txt
--rw-r--r--   0 filipmichalsky   (501) staff       (20)       38 2023-07-04 17:51:44.433451 salesgpt-0.0.3/setup.cfg
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1924 2023-07-04 17:49:45.000000 salesgpt-0.0.3/setup.py
-drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-04 17:51:44.432250 salesgpt-0.0.3/tests/
--rw-r--r--   0 filipmichalsky   (501) staff       (20)     1585 2023-06-30 17:23:56.000000 salesgpt-0.0.3/tests/test_salesgpt.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-15 13:51:46.842731 salesgpt-0.0.4/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1071 2023-06-19 23:47:34.000000 salesgpt-0.0.4/LICENSE
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       24 2023-06-30 17:23:56.000000 salesgpt-0.0.4/MANIFEST.in
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     8785 2023-07-15 13:51:46.842198 salesgpt-0.0.4/PKG-INFO
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     8012 2023-07-15 13:50:06.000000 salesgpt-0.0.4/README.md
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      136 2023-07-15 13:50:06.000000 salesgpt-0.0.4/requirements.txt
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-15 13:51:46.839298 salesgpt-0.0.4/salesgpt/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        0 2023-06-30 17:23:56.000000 salesgpt-0.0.4/salesgpt/__init__.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)    11402 2023-07-15 13:50:06.000000 salesgpt-0.0.4/salesgpt/agents.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     6447 2023-07-13 22:04:08.000000 salesgpt-0.0.4/salesgpt/chains.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1119 2023-06-30 17:23:56.000000 salesgpt-0.0.4/salesgpt/logger.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1544 2023-07-15 13:50:06.000000 salesgpt-0.0.4/salesgpt/parsers.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     3399 2023-07-15 13:50:06.000000 salesgpt-0.0.4/salesgpt/prompts.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1606 2023-06-30 17:23:56.000000 salesgpt-0.0.4/salesgpt/stages.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1254 2023-07-15 13:50:06.000000 salesgpt-0.0.4/salesgpt/templates.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1300 2023-07-15 13:50:06.000000 salesgpt-0.0.4/salesgpt/tools.py
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       50 2023-07-15 13:50:27.000000 salesgpt-0.0.4/salesgpt/version.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-15 13:51:46.841118 salesgpt-0.0.4/salesgpt.egg-info/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     8785 2023-07-15 13:51:46.000000 salesgpt-0.0.4/salesgpt.egg-info/PKG-INFO
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      434 2023-07-15 13:51:46.000000 salesgpt-0.0.4/salesgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        1 2023-07-15 13:51:46.000000 salesgpt-0.0.4/salesgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)      190 2023-07-15 13:51:46.000000 salesgpt-0.0.4/salesgpt.egg-info/requires.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)        9 2023-07-15 13:51:46.000000 salesgpt-0.0.4/salesgpt.egg-info/top_level.txt
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)       38 2023-07-15 13:51:46.842890 salesgpt-0.0.4/setup.cfg
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     1924 2023-07-14 15:19:01.000000 salesgpt-0.0.4/setup.py
+drwxr-xr-x   0 filipmichalsky   (501) staff       (20)        0 2023-07-15 13:51:46.841490 salesgpt-0.0.4/tests/
+-rw-r--r--   0 filipmichalsky   (501) staff       (20)     5019 2023-07-15 13:50:06.000000 salesgpt-0.0.4/tests/test_salesgpt.py
```

### Comparing `salesgpt-0.0.3/LICENSE` & `salesgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.3/PKG-INFO` & `salesgpt-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: SalesGPT - Your Context-Aware AI Sales Assistant
 Home-page: https://github.com/filip-michalsky/SalesGPT
 Author: Filip Michalsky
 License: Apache 2.0
 Keywords: openai sales gpt autonomous agi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,88 +20,113 @@
 License-File: LICENSE
 
 # :robot: SalesGPT - Your Context-Aware AI Sales Assistant
 
 This repo demonstrates an implementation of a **context-aware** AI Sales Assistant using LLMs.
 
 SalesGPT is context-aware, which means it can understand what section of a sales conversation it is in and act accordingly.
+Morever, SalesGPT has access to tools, such as your own pre-defined product knowledge base, significantly reducing hallucinations!
 
-We leverage the [`langchain`](https://github.com/hwchase17/langchain) library in this implementation and are inspired by [BabyAGI](https://github.com/yoheinakajima/babyagi) architecture .
+We leverage the [`langchain`](https://github.com/hwchase17/langchain) library in this implementation, specifically [Custom Agent Configuration](https://langchain-langchain.vercel.app/docs/modules/agents/how_to/custom_agent_with_tool_retrieval) and are inspired by [BabyAGI](https://github.com/yoheinakajima/babyagi) architecture.
 
 ## Our Vision: Build the Best Open-Source Autonomous Sales Agent
 
 We are building SalesGPT to power your best Autonomous Sales Agents. Hence, we would love to learn more about use cases you are building towards which will fuel SalesGPT development roadmap.
 
 **If you want us to build better towards your needs, please fill out our 45 seconds [SalesGPT Use Case Survey](https://5b7mfhwiany.typeform.com/to/xmJbWIjG)**
 
-## :red_circle: Latest News
+### If you looking for help building your Autonomous Sales Agents
 
-### Demo: SalesGPT Outbound Prospecting: A New Way to Sell? 🤔
+I am currently open to freelancing opps - please contact me through [my website](https://odysseypartners.ai?utm_source=SalesGPT) if you think I can help  you.
 
-https://github.com/filip-michalsky/SalesGPT/assets/31483888/2b13ba28-4e07-41dc-a8bf-4084d25247ca
+## :red_circle: Latest News
 
+- Sales Agent can now take advantage of **tools**, such as look up products in a product catalog!
 
-### If you looking for help building your Autonomous Sales Agents
+### Demo: SalesGPT Outbound Prospecting: A New Way to Sell? 🤔
 
-I am currently open to freelancing opps - please contact me through [my website](https://odysseypartners.ai?utm_source=SalesGPT) if you think I can help  you.
+https://github.com/filip-michalsky/SalesGPT/assets/31483888/2b13ba28-4e07-41dc-a8bf-4084d25247ca
 
 ## Quickstart
 
 ```python
 import os
 from salesgpt.agents import SalesGPT
 from langchain.chat_models import ChatOpenAI
 
 os.environ['OPENAI_API_KEY'] = 'sk-xxx' # fill me in
 
-llm = ChatOpenAI(temperature=0.9)
-
-sales_agent = SalesGPT.from_llm(llm, verbose=False,
+llm = ChatOpenAI(temperature=0.4)
+                            
+sales_agent = SalesGPT.from_llm(llm, use_tools=True, verbose=False,
+                            product_catalog = "examples/sample_product_catalog.txt",
                             salesperson_name="Ted Lasso",
                             salesperson_role="Sales Representative",
                             company_name="Sleep Haven",
                             company_business='''Sleep Haven 
                             is a premium mattress company that provides
                             customers with the most comfortable and
                             supportive sleeping experience possible. 
                             We offer a range of high-quality mattresses,
                             pillows, and bedding accessories 
                             that are designed to meet the unique 
-                            needs of our customers.''')
-
+                            needs of our customers.'''
+                            )
 sales_agent.seed_agent()
 sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
 
 # agent 
 sales_agent.step()
 
 # user
 user_input = input('Your response: ') # Yea, sure
 sales_agent.human_step(user_input)
 
 # agent
 sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
 sales_agent.step()
+
+# user
+user_input = input('Your response: ') # What pricing do you have for your mattresses?
+sales_agent.human_step(user_input)
+
+# agent
+sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
+sales_agent.step()
 ```
 > Conversation Stage: 
 > Introduction: Start the conversation by introducing yourself and your company. 
 
+> Thought: Do I need to use a tool? No <br>
 > Ted Lasso: Hello, my name is Ted Lasso and I'm calling on behalf of Sleep Haven. We are a premium mattress company that provides customers with the most comfortable and supportive sleeping experience possible. I was wondering if you would be interested in learning more about our products and how they can improve your sleep?
 
 > User: Yea, sure
 
 > Conversation Stage: 
 > Value proposition: Briefly explain how your product/service can benefit the prospect. 
 
+> Thought: Do I need to use a tool? No <br>
 > Ted Lasso: Great to hear that! Our mattresses are specially designed to contour to your body shape, providing the perfect level of support and comfort for a better night's sleep. Plus, they're made with high-quality materials that are built to last. Would you like to hear more about our different mattress options?
 
+> User:  What pricing do you have for your mattresses?
+
+> Thought: Do I need to use a tool? Yes --> AI Agent uses tools here.<br>
+> Action: ProductSearch<br>
+> ActionInput pricing for mattresses<br>
+> Observation: Sleep Haven offers three mattresses: the Classic Harmony Spring Mattress for $1,299, the Plush Serenity Bamboo Mattress for $2,599, and the Luxury Cloud-Comfort Memory Foam Mattress for $999. The sizes available vary by mattress.<br>
+> Ted Lasso: Sleep Haven offers three mattresses at different price points. The Classic Harmony Spring Mattress is priced at $1,299, the Plush Serenity Bamboo Mattress is priced at $2,599, and the Luxury Cloud-Comfort Memory Foam Mattress is priced at $999. The prices may vary depending on the size you choose. Would you like more information about the specific sizes and features of each mattress? 
+
+## Product Knowledge Base
+
+The AI Sales Agent has access to tools, such as your internal Product Knowledge base.
+This allows the agent to only talk about your own products and significantly reduces hallucinations.
 
 ## Understanding Context
 
-The bot understands the conversation stage (you can define your own stages fitting your needs):
+The AI Sales Agent understands the conversation stage (you can define your own stages fitting your needs):
 
 - Introduction: Start the conversation by introducing yourself and your company. 
 - Qualification: Qualify the prospect by confirming if they are the right person to talk to regarding your product/service.
 - Value proposition: Briefly explain how your product/service can benefit the prospect. 
 - Needs analysis: Ask open-ended questions to uncover the prospect's needs and pain points. 
 - Solution presentation: Based on the prospect's needs, present your product/service as the solution that can address their pain points.
 - Objection handling: Address any objections that the prospect may have regarding your product/service. 
@@ -109,15 +134,15 @@
 - End Conversation: The user does not want to continue the conversation, so end the call.
  
 As such, this agent can have a natural sales conversation with a prospect and behaves based on the conversation stage. Hence, this notebook demonstrates how we can use AI to automate sales development representatives activites, such as outbound sales calls. 
 
 
 ## Architecture
 
-<img src="https://images-genai.s3.us-east-1.amazonaws.com/architecture2.png"  width="800" height="400">
+<img src="https://singularity-assets-public.s3.amazonaws.com/new_flow.png"  width="800" height="440">
 
 ## Installation
 
 Make sure your have a python 3.10+ and run:
 
 `pip install -r requirements.txt`
 
@@ -129,32 +154,39 @@
 
 `pip install salesgpt`
 
 ## Try it out 
 
 To get a feel for a conversation with the AI Sales agent, you can run:
 
-`python run.py`
+`python run.py --verbose True --config examples/example_agent_setup.json`
 
 from your terminal.
 
 ## Contact Us
 
 For questions, you can [contact the repo author](mailto:filipmichalsky@gmail.com).
 
 Follow me at [@FilipMichalsky](https://twitter.com/FilipMichalsky)
 
 
 ## SalesGPT Roadmap
 
-- Knowledge base for products/services a Sales Agent can offer (so that LLM does not make it up)
-- Convert LLM Chains (linear workflow) to an Agent (decides what to do based on user's input)
-    - What tools should the agent have? (e.g., the ability to search the internet)
-    - Add the ability of Sales Agent to interact with AI plugins on your website (.well-known/ai-plugin.json)
-    
+
+- Add the ability of Sales Agent to interact with AI plugins on your website (.well-known/ai-plugin.json)
+
+- What tools should the agent have? (e.g., the ability to search the internet)
+
 ~~-
  Add the ability to stop generation when user interupts the agent~~
-- Add a vectorstore to incorporate a real product knowledge base vs. the LLM making it up.
+
+~~- Add a vectorstore to incorporate a real product knowledge base vs. the LLM making it up.~~
+
+~~- Knowledge base for products/services a Sales Agent can offer (so that LLM does not make it up)~~
+
+~~- Convert LLM Chains (linear workflow) to an Agent (decides what to do based on user's input)~~
+
+
 
 ## Contributing
 
-Contributions are highly encouraged!
+Contributions are highly encouraged! Please fork and submit a PR.
```

### Comparing `salesgpt-0.0.3/README.md` & `salesgpt-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,111 @@
 # :robot: SalesGPT - Your Context-Aware AI Sales Assistant
 
 This repo demonstrates an implementation of a **context-aware** AI Sales Assistant using LLMs.
 
 SalesGPT is context-aware, which means it can understand what section of a sales conversation it is in and act accordingly.
+Morever, SalesGPT has access to tools, such as your own pre-defined product knowledge base, significantly reducing hallucinations!
 
-We leverage the [`langchain`](https://github.com/hwchase17/langchain) library in this implementation and are inspired by [BabyAGI](https://github.com/yoheinakajima/babyagi) architecture .
+We leverage the [`langchain`](https://github.com/hwchase17/langchain) library in this implementation, specifically [Custom Agent Configuration](https://langchain-langchain.vercel.app/docs/modules/agents/how_to/custom_agent_with_tool_retrieval) and are inspired by [BabyAGI](https://github.com/yoheinakajima/babyagi) architecture.
 
 ## Our Vision: Build the Best Open-Source Autonomous Sales Agent
 
 We are building SalesGPT to power your best Autonomous Sales Agents. Hence, we would love to learn more about use cases you are building towards which will fuel SalesGPT development roadmap.
 
 **If you want us to build better towards your needs, please fill out our 45 seconds [SalesGPT Use Case Survey](https://5b7mfhwiany.typeform.com/to/xmJbWIjG)**
 
-## :red_circle: Latest News
+### If you looking for help building your Autonomous Sales Agents
 
-### Demo: SalesGPT Outbound Prospecting: A New Way to Sell? 🤔
+I am currently open to freelancing opps - please contact me through [my website](https://odysseypartners.ai?utm_source=SalesGPT) if you think I can help  you.
 
-https://github.com/filip-michalsky/SalesGPT/assets/31483888/2b13ba28-4e07-41dc-a8bf-4084d25247ca
+## :red_circle: Latest News
 
+- Sales Agent can now take advantage of **tools**, such as look up products in a product catalog!
 
-### If you looking for help building your Autonomous Sales Agents
+### Demo: SalesGPT Outbound Prospecting: A New Way to Sell? 🤔
 
-I am currently open to freelancing opps - please contact me through [my website](https://odysseypartners.ai?utm_source=SalesGPT) if you think I can help  you.
+https://github.com/filip-michalsky/SalesGPT/assets/31483888/2b13ba28-4e07-41dc-a8bf-4084d25247ca
 
 ## Quickstart
 
 ```python
 import os
 from salesgpt.agents import SalesGPT
 from langchain.chat_models import ChatOpenAI
 
 os.environ['OPENAI_API_KEY'] = 'sk-xxx' # fill me in
 
-llm = ChatOpenAI(temperature=0.9)
-
-sales_agent = SalesGPT.from_llm(llm, verbose=False,
+llm = ChatOpenAI(temperature=0.4)
+                            
+sales_agent = SalesGPT.from_llm(llm, use_tools=True, verbose=False,
+                            product_catalog = "examples/sample_product_catalog.txt",
                             salesperson_name="Ted Lasso",
                             salesperson_role="Sales Representative",
                             company_name="Sleep Haven",
                             company_business='''Sleep Haven 
                             is a premium mattress company that provides
                             customers with the most comfortable and
                             supportive sleeping experience possible. 
                             We offer a range of high-quality mattresses,
                             pillows, and bedding accessories 
                             that are designed to meet the unique 
-                            needs of our customers.''')
-
+                            needs of our customers.'''
+                            )
 sales_agent.seed_agent()
 sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
 
 # agent 
 sales_agent.step()
 
 # user
 user_input = input('Your response: ') # Yea, sure
 sales_agent.human_step(user_input)
 
 # agent
 sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
 sales_agent.step()
+
+# user
+user_input = input('Your response: ') # What pricing do you have for your mattresses?
+sales_agent.human_step(user_input)
+
+# agent
+sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
+sales_agent.step()
 ```
 > Conversation Stage: 
 > Introduction: Start the conversation by introducing yourself and your company. 
 
+> Thought: Do I need to use a tool? No <br>
 > Ted Lasso: Hello, my name is Ted Lasso and I'm calling on behalf of Sleep Haven. We are a premium mattress company that provides customers with the most comfortable and supportive sleeping experience possible. I was wondering if you would be interested in learning more about our products and how they can improve your sleep?
 
 > User: Yea, sure
 
 > Conversation Stage: 
 > Value proposition: Briefly explain how your product/service can benefit the prospect. 
 
+> Thought: Do I need to use a tool? No <br>
 > Ted Lasso: Great to hear that! Our mattresses are specially designed to contour to your body shape, providing the perfect level of support and comfort for a better night's sleep. Plus, they're made with high-quality materials that are built to last. Would you like to hear more about our different mattress options?
 
+> User:  What pricing do you have for your mattresses?
+
+> Thought: Do I need to use a tool? Yes --> AI Agent uses tools here.<br>
+> Action: ProductSearch<br>
+> ActionInput pricing for mattresses<br>
+> Observation: Sleep Haven offers three mattresses: the Classic Harmony Spring Mattress for $1,299, the Plush Serenity Bamboo Mattress for $2,599, and the Luxury Cloud-Comfort Memory Foam Mattress for $999. The sizes available vary by mattress.<br>
+> Ted Lasso: Sleep Haven offers three mattresses at different price points. The Classic Harmony Spring Mattress is priced at $1,299, the Plush Serenity Bamboo Mattress is priced at $2,599, and the Luxury Cloud-Comfort Memory Foam Mattress is priced at $999. The prices may vary depending on the size you choose. Would you like more information about the specific sizes and features of each mattress? 
+
+## Product Knowledge Base
+
+The AI Sales Agent has access to tools, such as your internal Product Knowledge base.
+This allows the agent to only talk about your own products and significantly reduces hallucinations.
 
 ## Understanding Context
 
-The bot understands the conversation stage (you can define your own stages fitting your needs):
+The AI Sales Agent understands the conversation stage (you can define your own stages fitting your needs):
 
 - Introduction: Start the conversation by introducing yourself and your company. 
 - Qualification: Qualify the prospect by confirming if they are the right person to talk to regarding your product/service.
 - Value proposition: Briefly explain how your product/service can benefit the prospect. 
 - Needs analysis: Ask open-ended questions to uncover the prospect's needs and pain points. 
 - Solution presentation: Based on the prospect's needs, present your product/service as the solution that can address their pain points.
 - Objection handling: Address any objections that the prospect may have regarding your product/service. 
@@ -88,15 +113,15 @@
 - End Conversation: The user does not want to continue the conversation, so end the call.
  
 As such, this agent can have a natural sales conversation with a prospect and behaves based on the conversation stage. Hence, this notebook demonstrates how we can use AI to automate sales development representatives activites, such as outbound sales calls. 
 
 
 ## Architecture
 
-<img src="https://images-genai.s3.us-east-1.amazonaws.com/architecture2.png"  width="800" height="400">
+<img src="https://singularity-assets-public.s3.amazonaws.com/new_flow.png"  width="800" height="440">
 
 ## Installation
 
 Make sure your have a python 3.10+ and run:
 
 `pip install -r requirements.txt`
 
@@ -108,32 +133,39 @@
 
 `pip install salesgpt`
 
 ## Try it out 
 
 To get a feel for a conversation with the AI Sales agent, you can run:
 
-`python run.py`
+`python run.py --verbose True --config examples/example_agent_setup.json`
 
 from your terminal.
 
 ## Contact Us
 
 For questions, you can [contact the repo author](mailto:filipmichalsky@gmail.com).
 
 Follow me at [@FilipMichalsky](https://twitter.com/FilipMichalsky)
 
 
 ## SalesGPT Roadmap
 
-- Knowledge base for products/services a Sales Agent can offer (so that LLM does not make it up)
-- Convert LLM Chains (linear workflow) to an Agent (decides what to do based on user's input)
-    - What tools should the agent have? (e.g., the ability to search the internet)
-    - Add the ability of Sales Agent to interact with AI plugins on your website (.well-known/ai-plugin.json)
-    
+
+- Add the ability of Sales Agent to interact with AI plugins on your website (.well-known/ai-plugin.json)
+
+- What tools should the agent have? (e.g., the ability to search the internet)
+
 ~~-
  Add the ability to stop generation when user interupts the agent~~
-- Add a vectorstore to incorporate a real product knowledge base vs. the LLM making it up.
+
+~~- Add a vectorstore to incorporate a real product knowledge base vs. the LLM making it up.~~
+
+~~- Knowledge base for products/services a Sales Agent can offer (so that LLM does not make it up)~~
+
+~~- Convert LLM Chains (linear workflow) to an Agent (decides what to do based on user's input)~~
+
+
 
 ## Contributing
 
-Contributions are highly encouraged!
+Contributions are highly encouraged! Please fork and submit a PR.
```

### Comparing `salesgpt-0.0.3/salesgpt/chains.py` & `salesgpt-0.0.4/salesgpt/chains.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.3/salesgpt/logger.py` & `salesgpt-0.0.4/salesgpt/logger.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.3/salesgpt/stages.py` & `salesgpt-0.0.4/salesgpt/stages.py`

 * *Files identical despite different names*

### Comparing `salesgpt-0.0.3/salesgpt.egg-info/PKG-INFO` & `salesgpt-0.0.4/salesgpt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: SalesGPT - Your Context-Aware AI Sales Assistant
 Home-page: https://github.com/filip-michalsky/SalesGPT
 Author: Filip Michalsky
 License: Apache 2.0
 Keywords: openai sales gpt autonomous agi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,88 +20,113 @@
 License-File: LICENSE
 
 # :robot: SalesGPT - Your Context-Aware AI Sales Assistant
 
 This repo demonstrates an implementation of a **context-aware** AI Sales Assistant using LLMs.
 
 SalesGPT is context-aware, which means it can understand what section of a sales conversation it is in and act accordingly.
+Morever, SalesGPT has access to tools, such as your own pre-defined product knowledge base, significantly reducing hallucinations!
 
-We leverage the [`langchain`](https://github.com/hwchase17/langchain) library in this implementation and are inspired by [BabyAGI](https://github.com/yoheinakajima/babyagi) architecture .
+We leverage the [`langchain`](https://github.com/hwchase17/langchain) library in this implementation, specifically [Custom Agent Configuration](https://langchain-langchain.vercel.app/docs/modules/agents/how_to/custom_agent_with_tool_retrieval) and are inspired by [BabyAGI](https://github.com/yoheinakajima/babyagi) architecture.
 
 ## Our Vision: Build the Best Open-Source Autonomous Sales Agent
 
 We are building SalesGPT to power your best Autonomous Sales Agents. Hence, we would love to learn more about use cases you are building towards which will fuel SalesGPT development roadmap.
 
 **If you want us to build better towards your needs, please fill out our 45 seconds [SalesGPT Use Case Survey](https://5b7mfhwiany.typeform.com/to/xmJbWIjG)**
 
-## :red_circle: Latest News
+### If you looking for help building your Autonomous Sales Agents
 
-### Demo: SalesGPT Outbound Prospecting: A New Way to Sell? 🤔
+I am currently open to freelancing opps - please contact me through [my website](https://odysseypartners.ai?utm_source=SalesGPT) if you think I can help  you.
 
-https://github.com/filip-michalsky/SalesGPT/assets/31483888/2b13ba28-4e07-41dc-a8bf-4084d25247ca
+## :red_circle: Latest News
 
+- Sales Agent can now take advantage of **tools**, such as look up products in a product catalog!
 
-### If you looking for help building your Autonomous Sales Agents
+### Demo: SalesGPT Outbound Prospecting: A New Way to Sell? 🤔
 
-I am currently open to freelancing opps - please contact me through [my website](https://odysseypartners.ai?utm_source=SalesGPT) if you think I can help  you.
+https://github.com/filip-michalsky/SalesGPT/assets/31483888/2b13ba28-4e07-41dc-a8bf-4084d25247ca
 
 ## Quickstart
 
 ```python
 import os
 from salesgpt.agents import SalesGPT
 from langchain.chat_models import ChatOpenAI
 
 os.environ['OPENAI_API_KEY'] = 'sk-xxx' # fill me in
 
-llm = ChatOpenAI(temperature=0.9)
-
-sales_agent = SalesGPT.from_llm(llm, verbose=False,
+llm = ChatOpenAI(temperature=0.4)
+                            
+sales_agent = SalesGPT.from_llm(llm, use_tools=True, verbose=False,
+                            product_catalog = "examples/sample_product_catalog.txt",
                             salesperson_name="Ted Lasso",
                             salesperson_role="Sales Representative",
                             company_name="Sleep Haven",
                             company_business='''Sleep Haven 
                             is a premium mattress company that provides
                             customers with the most comfortable and
                             supportive sleeping experience possible. 
                             We offer a range of high-quality mattresses,
                             pillows, and bedding accessories 
                             that are designed to meet the unique 
-                            needs of our customers.''')
-
+                            needs of our customers.'''
+                            )
 sales_agent.seed_agent()
 sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
 
 # agent 
 sales_agent.step()
 
 # user
 user_input = input('Your response: ') # Yea, sure
 sales_agent.human_step(user_input)
 
 # agent
 sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
 sales_agent.step()
+
+# user
+user_input = input('Your response: ') # What pricing do you have for your mattresses?
+sales_agent.human_step(user_input)
+
+# agent
+sales_agent.determine_conversation_stage() # optional for demonstration, built into the prompt
+sales_agent.step()
 ```
 > Conversation Stage: 
 > Introduction: Start the conversation by introducing yourself and your company. 
 
+> Thought: Do I need to use a tool? No <br>
 > Ted Lasso: Hello, my name is Ted Lasso and I'm calling on behalf of Sleep Haven. We are a premium mattress company that provides customers with the most comfortable and supportive sleeping experience possible. I was wondering if you would be interested in learning more about our products and how they can improve your sleep?
 
 > User: Yea, sure
 
 > Conversation Stage: 
 > Value proposition: Briefly explain how your product/service can benefit the prospect. 
 
+> Thought: Do I need to use a tool? No <br>
 > Ted Lasso: Great to hear that! Our mattresses are specially designed to contour to your body shape, providing the perfect level of support and comfort for a better night's sleep. Plus, they're made with high-quality materials that are built to last. Would you like to hear more about our different mattress options?
 
+> User:  What pricing do you have for your mattresses?
+
+> Thought: Do I need to use a tool? Yes --> AI Agent uses tools here.<br>
+> Action: ProductSearch<br>
+> ActionInput pricing for mattresses<br>
+> Observation: Sleep Haven offers three mattresses: the Classic Harmony Spring Mattress for $1,299, the Plush Serenity Bamboo Mattress for $2,599, and the Luxury Cloud-Comfort Memory Foam Mattress for $999. The sizes available vary by mattress.<br>
+> Ted Lasso: Sleep Haven offers three mattresses at different price points. The Classic Harmony Spring Mattress is priced at $1,299, the Plush Serenity Bamboo Mattress is priced at $2,599, and the Luxury Cloud-Comfort Memory Foam Mattress is priced at $999. The prices may vary depending on the size you choose. Would you like more information about the specific sizes and features of each mattress? 
+
+## Product Knowledge Base
+
+The AI Sales Agent has access to tools, such as your internal Product Knowledge base.
+This allows the agent to only talk about your own products and significantly reduces hallucinations.
 
 ## Understanding Context
 
-The bot understands the conversation stage (you can define your own stages fitting your needs):
+The AI Sales Agent understands the conversation stage (you can define your own stages fitting your needs):
 
 - Introduction: Start the conversation by introducing yourself and your company. 
 - Qualification: Qualify the prospect by confirming if they are the right person to talk to regarding your product/service.
 - Value proposition: Briefly explain how your product/service can benefit the prospect. 
 - Needs analysis: Ask open-ended questions to uncover the prospect's needs and pain points. 
 - Solution presentation: Based on the prospect's needs, present your product/service as the solution that can address their pain points.
 - Objection handling: Address any objections that the prospect may have regarding your product/service. 
@@ -109,15 +134,15 @@
 - End Conversation: The user does not want to continue the conversation, so end the call.
  
 As such, this agent can have a natural sales conversation with a prospect and behaves based on the conversation stage. Hence, this notebook demonstrates how we can use AI to automate sales development representatives activites, such as outbound sales calls. 
 
 
 ## Architecture
 
-<img src="https://images-genai.s3.us-east-1.amazonaws.com/architecture2.png"  width="800" height="400">
+<img src="https://singularity-assets-public.s3.amazonaws.com/new_flow.png"  width="800" height="440">
 
 ## Installation
 
 Make sure your have a python 3.10+ and run:
 
 `pip install -r requirements.txt`
 
@@ -129,32 +154,39 @@
 
 `pip install salesgpt`
 
 ## Try it out 
 
 To get a feel for a conversation with the AI Sales agent, you can run:
 
-`python run.py`
+`python run.py --verbose True --config examples/example_agent_setup.json`
 
 from your terminal.
 
 ## Contact Us
 
 For questions, you can [contact the repo author](mailto:filipmichalsky@gmail.com).
 
 Follow me at [@FilipMichalsky](https://twitter.com/FilipMichalsky)
 
 
 ## SalesGPT Roadmap
 
-- Knowledge base for products/services a Sales Agent can offer (so that LLM does not make it up)
-- Convert LLM Chains (linear workflow) to an Agent (decides what to do based on user's input)
-    - What tools should the agent have? (e.g., the ability to search the internet)
-    - Add the ability of Sales Agent to interact with AI plugins on your website (.well-known/ai-plugin.json)
-    
+
+- Add the ability of Sales Agent to interact with AI plugins on your website (.well-known/ai-plugin.json)
+
+- What tools should the agent have? (e.g., the ability to search the internet)
+
 ~~-
  Add the ability to stop generation when user interupts the agent~~
-- Add a vectorstore to incorporate a real product knowledge base vs. the LLM making it up.
+
+~~- Add a vectorstore to incorporate a real product knowledge base vs. the LLM making it up.~~
+
+~~- Knowledge base for products/services a Sales Agent can offer (so that LLM does not make it up)~~
+
+~~- Convert LLM Chains (linear workflow) to an Agent (decides what to do based on user's input)~~
+
+
 
 ## Contributing
 
-Contributions are highly encouraged!
+Contributions are highly encouraged! Please fork and submit a PR.
```

### Comparing `salesgpt-0.0.3/setup.py` & `salesgpt-0.0.4/setup.py`

 * *Files identical despite different names*

