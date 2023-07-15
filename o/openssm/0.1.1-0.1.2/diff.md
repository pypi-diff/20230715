# Comparing `tmp/openssm-0.1.1.tar.gz` & `tmp/openssm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssm-0.1.1.tar", max compression
+gzip compressed data, was "openssm-0.1.2.tar", max compression
```

## Comparing `openssm-0.1.1.tar` & `openssm-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,40 @@
--rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     7182 2023-07-03 00:52:17.391051 openssm-0.1.1/README.md
--rw-r--r--   0        0        0     2155 2023-07-01 21:58:27.291702 openssm-0.1.1/openssm/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.796606 openssm-0.1.1/openssm/__init__.py
--rw-r--r--   0        0        0       19 2023-06-30 08:00:20.798353 openssm-0.1.1/openssm/core/__init__.py
--rw-r--r--   0        0        0     1460 2023-07-04 00:52:59.822256 openssm-0.1.1/openssm/core/adapter/abstract_adapter.py
--rw-r--r--   0        0        0      787 2023-07-04 00:53:21.362156 openssm-0.1.1/openssm/core/adapter/base_adapter.py
--rw-r--r--   0        0        0     2511 2023-06-30 08:00:20.799517 openssm-0.1.1/openssm/core/adapter/llama_index_adapter.py
--rw-r--r--   0        0        0      199 2023-06-30 08:00:20.799799 openssm-0.1.1/openssm/core/backend/abstract_backend.py
--rw-r--r--   0        0        0      197 2023-06-30 08:00:20.800029 openssm-0.1.1/openssm/core/backend/base_backend.py
--rw-r--r--   0        0        0      131 2023-07-02 02:54:05.726183 openssm-0.1.1/openssm/core/config.py
--rw-r--r--   0        0        0      937 2023-07-04 00:53:07.955563 openssm-0.1.1/openssm/core/slm/abstract_slm.py
--rw-r--r--   0        0        0      541 2023-07-04 00:53:28.106772 openssm-0.1.1/openssm/core/slm/base_slm.py
--rw-r--r--   0        0        0     2816 2023-07-04 00:53:46.345313 openssm-0.1.1/openssm/core/slm/gpt3_slm.py
--rw-r--r--   0        0        0      417 2023-06-30 08:00:20.801854 openssm-0.1.1/openssm/core/slm/memory/conversation_db.py
--rw-r--r--   0        0        0     2557 2023-06-30 08:00:20.801951 openssm-0.1.1/openssm/core/slm/memory/db.py
--rw-r--r--   0        0        0     2159 2023-06-30 08:00:20.802090 openssm-0.1.1/openssm/core/slm/memory/sqlite_conversation_db.py
--rw-r--r--   0        0        0     2502 2023-07-04 00:48:07.330715 openssm-0.1.1/openssm/core/ssm/abstract_ssm.py
--rw-r--r--   0        0        0     2416 2023-07-04 00:53:59.598963 openssm-0.1.1/openssm/core/ssm/base_ssm.py
--rw-r--r--   0        0        0     1416 2023-07-04 00:54:09.537284 openssm-0.1.1/openssm/core/ssm/gpt3_llama_index_ssm.py
--rw-r--r--   0        0        0      713 2023-07-04 00:54:27.315086 openssm-0.1.1/openssm/core/ssm/gpt3_ssm.py
--rw-r--r--   0        0        0       58 2023-06-30 08:00:20.803155 openssm-0.1.1/openssm/industrial/interpretability/README.md
--rw-r--r--   0        0        0       60 2023-06-30 08:00:20.803373 openssm-0.1.1/openssm/industrial/monitoring/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803462 openssm-0.1.1/openssm/industrial/security/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803611 openssm-0.1.1/openssm/industrial/security/audit/README.md
--rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803745 openssm-0.1.1/openssm/industrial/security/best_practices/README.md
--rw-r--r--   0        0        0       63 2023-06-30 08:00:20.803985 openssm-0.1.1/openssm/integration/README.md
--rw-r--r--   0        0        0     3574 2023-06-30 08:00:20.804216 openssm-0.1.1/openssm/integration/llamaindex/README.md
--rw-r--r--   0        0        0       34 2023-06-30 08:00:20.804401 openssm-0.1.1/openssm/integration/testing_tools/README.md
--rw-r--r--   0        0        0      466 2023-07-04 00:59:33.571271 openssm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 openssm-0.1.1/setup.py
--rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 openssm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     6946 2023-07-14 16:35:00.896701 openssm-0.1.2/README.md
+-rw-r--r--   0        0        0       79 2023-07-07 18:20:26.251547 openssm-0.1.2/openssm/Makefile
+-rw-r--r--   0        0        0     2553 2023-07-10 09:13:36.452086 openssm-0.1.2/openssm/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.796606 openssm-0.1.2/openssm/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-12 04:07:00.397143 openssm-0.1.2/openssm/config.py
+-rw-r--r--   0        0        0      754 2023-07-12 04:07:00.397716 openssm-0.1.2/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-12 04:07:00.397936 openssm-0.1.2/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
+-rw-r--r--   0        0        0     1010 2023-07-12 04:07:00.398136 openssm-0.1.2/openssm/contrib/ssms/mri_operator_ssm/__init__.py
+-rw-r--r--   0        0        0     1610 2023-07-12 04:07:00.398292 openssm-0.1.2/openssm/contrib/ssms/semiconductor_ssm/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-30 08:00:20.798353 openssm-0.1.2/openssm/core/__init__.py
+-rw-r--r--   0        0        0     2203 2023-07-14 05:15:42.916155 openssm-0.1.2/openssm/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0     3399 2023-07-14 16:15:33.092368 openssm-0.1.2/openssm/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     2926 2023-07-14 02:34:13.823441 openssm-0.1.2/openssm/core/adapter/llama_index_adapter.py
+-rw-r--r--   0        0        0     1159 2023-07-14 02:34:13.823890 openssm-0.1.2/openssm/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0     1595 2023-07-14 15:59:33.058040 openssm-0.1.2/openssm/core/backend/base_backend.py
+-rw-r--r--   0        0        0     1658 2023-07-14 02:34:13.824322 openssm-0.1.2/openssm/core/backend/text_backend.py
+-rw-r--r--   0        0        0      720 2023-07-10 18:00:54.628456 openssm-0.1.2/openssm/core/inferencer/abstract_inferencer.py
+-rw-r--r--   0        0        0      458 2023-07-12 04:07:00.400091 openssm-0.1.2/openssm/core/inferencer/base_inferencer.py
+-rw-r--r--   0        0        0      885 2023-07-12 04:07:00.400461 openssm-0.1.2/openssm/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0     1626 2023-07-12 04:07:00.400690 openssm-0.1.2/openssm/core/slm/base_slm.py
+-rw-r--r--   0        0        0     6760 2023-07-14 02:34:13.824686 openssm-0.1.2/openssm/core/slm/huggingface_slm.py
+-rw-r--r--   0        0        0      417 2023-07-07 18:30:35.408067 openssm-0.1.2/openssm/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     1620 2023-07-12 04:07:00.401194 openssm-0.1.2/openssm/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     2053 2023-07-12 04:07:00.401379 openssm-0.1.2/openssm/core/slm/openai_slm.py
+-rw-r--r--   0        0        0     2307 2023-07-12 04:07:00.401590 openssm-0.1.2/openssm/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     3037 2023-07-12 04:07:00.401769 openssm-0.1.2/openssm/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0      454 2023-07-14 02:34:13.824917 openssm-0.1.2/openssm/core/ssm/gpt3_llama_index_ssm.py
+-rw-r--r--   0        0        0      747 2023-07-12 04:07:00.402181 openssm-0.1.2/openssm/core/ssm/huggingface_ssm.py
+-rw-r--r--   0        0        0      770 2023-07-14 02:34:13.825086 openssm-0.1.2/openssm/core/ssm/openai_ssm.py
+-rw-r--r--   0        0        0       58 2023-06-30 08:00:20.803155 openssm-0.1.2/openssm/industrial/interpretability/README.md
+-rw-r--r--   0        0        0       60 2023-06-30 08:00:20.803373 openssm-0.1.2/openssm/industrial/monitoring/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803462 openssm-0.1.2/openssm/industrial/security/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803611 openssm-0.1.2/openssm/industrial/security/audit/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803745 openssm-0.1.2/openssm/industrial/security/best_practices/README.md
+-rw-r--r--   0        0        0       63 2023-06-30 08:00:20.803985 openssm-0.1.2/openssm/integration/README.md
+-rw-r--r--   0        0        0     3574 2023-06-30 08:00:20.804216 openssm-0.1.2/openssm/integration/llamaindex/README.md
+-rw-r--r--   0        0        0       34 2023-06-30 08:00:20.804401 openssm-0.1.2/openssm/integration/testing_tools/README.md
+-rw-r--r--   0        0        0      688 2023-07-15 00:47:49.708064 openssm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7709 1970-01-01 00:00:00.000000 openssm-0.1.2/PKG-INFO
```

### Comparing `openssm-0.1.1/LICENSE.md` & `openssm-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.1/README.md` & `openssm-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,68 @@
 # OpenSSM – “Small Specialist Models” for Industrial AI
 
-OpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing
-trust, reliability, and safety in Industrial-AI applications. Harnessing the power of domain expertise, SSMs operate either
-alone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving
-capabilities.
-
-Unlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and
-designed specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers,
-and developers seeking specialized and robust AI solutions for industrial applications.
+OpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing trust, reliability, and safety in Industrial-AI applications.  Harnessing the power of domain expertise, SSMs operate either alone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving capabilities.
+
+Unlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and designed specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers, and developers seeking specialized and robust AI solutions for industrial applications.
 
 ![SSM in Industrial AI](./docs/diagrams/ssm-industrial-use-case.drawio.png)
 
-A prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM
-represents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this
-framework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and
-industrial problems.
+A prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM represents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this framework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and industrial problems.
 
 ## Why SSM?
 
 The trend towards specialization in AI models is a clear trajectory seen by many in the field.
 
-> Specialization is crucial for quality .. not general purpose Al models – Eric Schmidt, Schmidt Foundation
-> .. small models .. for a specific task that are good –  Matei Zaharia, Databricks
-> .. small agents working together .. specific and best in their tasks – Harrison Chase, Langchain
-> .. small but highly capable expert models – Andrej Karpathy, OpenAI
-> .. small models are .. a massive paradigm shift .. about deploying AI models at scale – Rob Toews, Radical Ventures
+> _Specialization is crucial for quality .. not general purpose Al models_ – Eric Schmidt, Schmidt Foundation
+
+> _.. small models .. for a specific task that are good_ –  Matei Zaharia, Databricks
+
+> _.. small agents working together .. specific and best in their tasks_ – Harrison Chase, Langchain
+
+> _.. small but highly capable expert models_ – Andrej Karpathy, OpenAI
 
-As predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.”
-SSMs are the central part in the architecture of these systems.
+> _.. small models are .. a massive paradigm shift .. about deploying AI models at scale_ – Rob Toews, Radical Ventures
+
+As predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.” SSMs are the central part in the architecture of these systems.
 
 ## What OpenSSM Offers
 
 OpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:
 
-- **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique
-requirements of trustworthiness, safety, reliability, and scalability inherent to this sector.
+- **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique requirements of trustworthiness, safety, reliability, and scalability inherent to this sector.
 
-- **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible
-and cost-effective particularly for industrial usage where time and resources are critical factors.
+- **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible and cost-effective particularly for industrial usage where time and resources are critical factors.
 
 - **Easy Knowledge Capture:** OpenSSM has easy-to-use tools for capturing domain knowledge in diverse forms: books, operaring manuals, databases, knowledge graphs, text files, and code.
 
 - **Powerful Operations on Captured Knowledge:** OpenSSM enables both knowledge query and inferencing/predictive capabilities based on the domain-specific knowledge.
 
 - **Collaborative Problem-Solving**: SSMs are designed to work in problem-solving "teams". Multi-SSM collaboration is a first-class design feature, not an afterthought.
 
-- **Reliable Domain Expertise:** Each SSM has expertise in a particular field or equipment, offering precise and specialized
-knowledge, thereby enhancing trustworthiness, reliability, and safety for Industrial-AI applications. With self-reasoning,
-causal reasoning, and retrieval-based knowledge, SSMs provide a trustable source of domain expertise.
+- **Reliable Domain Expertise:** Each SSM has expertise in a particular field or equipment, offering precise and specialized knowledge, thereby enhancing trustworthiness, reliability, and safety for Industrial-AI applications. With self-reasoning, causal reasoning, and retrieval-based knowledge, SSMs provide a trustable source of domain expertise.
 
-- **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering
-freedom from vendor lock-in and security concerns.
+- **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering freedom from vendor lock-in and security concerns.
 
 - **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.
 
 ## Target Audience
 
 Our primary audience includes:
 
-- **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive
-computational resources or large vendor solutions.
+- **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive computational resources or large vendor solutions.
 
 - **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.
 
-- **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven
-project focused on building and sharing specialized AI models.
+- **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven project focused on building and sharing specialized AI models.
 
-- **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing
-the reliability and trustworthiness of AI solutions in an industrial setting.
+- **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing the reliability and trustworthiness of AI solutions in an industrial setting.
 
 ## SSM Architecture
 
-At a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of
-back-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not,
-and may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.
+At a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of back-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not, and may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.
 
 ![High-Level SSM Architecture](./docs/diagrams/ssm-key-components.drawio.png)
 
 The above diagram illustrates the high-level architecture of an SSM, which comprises three main components:
 
 1. Small Language Model (SLM): This forms the communication frontend of an SSM.
 
@@ -89,42 +74,36 @@
 
 ![SSM Composability](./docs/diagrams/ssm-composability.drawio.png)
 
 The composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.
 
 ## Getting Started
 
-See some example user programs in the [examples](./examples) directory. For example, to run the `chatssm` example, do:
-
-```bash
-% cd examples/chatssm
-% make clean
-% make
-```
-
-then open your browser to `http://localhost:8080` and chat with the SSM.
-
-You can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting
-Started Guide](link-to-guide) for more information.
+See our [Getting Started Guide](./GETTING_STARTED.md) for more information.
 
 ## Roadmap
 
 - Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge
+
 - Create SSMs in your own development environment, and integrate SSMs into your own AI apps
+
 - Capture domain knowledge in various forms into your SSMs
+
 - Train SLMs via distillation of LLMs, teacher/student approaches, etc.
+
 - Apply SSMs in collaborative problem-solving AI systems
 
 ## Community
 
-Join our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI
-through SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).
+Join our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI through SSMs.  Participate in the discussions, share your ideas, or ask for help on our [Community Discussions](https://github.com/aitomatic/openssm/discussions).
 
 ## Contribute
 
-OpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it's enhancing existing models,
-creating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our
-[Contribution Guide](docs/CONTRIBUTING.md) for more details.
+OpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it's enhancing existing models, creating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our [Contribution Guide](docs/CONTRIBUTING.md) for more details.
 
 ## License
 
 OpenSSM is released under the [Apache 2.0 License](./LICENSE.md).
+
+## Links
+
+- [GETTING_STARTED](./GETTING_STARTED.md)
```

### Comparing `openssm-0.1.1/openssm/README.md` & `openssm-0.1.2/openssm/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 ![OpenSSM High-Level Class Diagram](../docs/diagrams/ssm-class-diagram.drawio.png)
 
 ## Package Structure
 
 - `openssm`: Root package for OpenSSM.
   - `openssm.core`: Core functionalities of the SSMs.
     - `openssm.core.ssm`: Small Specialist Model (SSM) functionality.
+      - `openssm.core.ssm.openai_ssm`: OpenAI API SSM implementations.
+      - `openssm.core.ssm.huggingface_ssm`: HuggingFace API SSM implementations.
     - `openssm.core.slm`: Component: Small Language Model (SLM) functionality.
+      - `openssm.core.ssm.openai_slm`: OpenAI API SLM implementations.
+      - `openssm.core.ssm.huggingface_slm`: HuggingFace API SLM implementations.
     - `openssm.core.adapter`: Component: Interface between the SLM and the domain-knowledge backends.
     - `openssm.core.backend`: Component: Interfaces to a variety of domain-knowledge backends.
+    - `openssm.core.inferencer`: Component: Inference wrapper for models behind SSM backends.
   - `openssm.capture`: Tools and APIs for capturing and encoding domain knowledge into various backends.
   - `openssm.composer`: Tools for composing multiple SSMs together.
   - `openssm.industrial`: Industrial-AI specific tools and APIs (trust, reliability, safety, etc.)
   - `openssm.integration`: Tools for integrating SSMs into industrial applications.
 
 - `tests`: Unit tests for the framework's components (located at the top level of the project).
```

### Comparing `openssm-0.1.1/openssm/core/adapter/abstract_adapter.py` & `openssm-0.1.2/openssm/core/adapter/abstract_adapter.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,50 +6,64 @@
     """
     The AbstractAdapter serves as the base for all concrete Adapter classes.
     It provides an interface for interaction between the Small Language Model
     (SLM) and the Backend.
     """
 
     @abstractmethod
+    def query(self, conversation_id: str, user_input: str) -> list({}):
+        """
+        Queries the backends for a response to the user's input.
+        :param user_query: The user's input.
+        :return: The backend's response.
+        """
+
+    @abstractmethod
     def get_backends(self) -> list[AbstractBackend]:
         """Returns our backends"""
-        pass
 
     @abstractmethod
     def add_backend(self, backend: AbstractBackend):
         """Adds a backend to our adapter"""
-        pass
 
     @abstractmethod
     def set_backends(self, backends: list):
         """Sets our backends"""
-        pass
 
     @abstractmethod
-    def list_facts(self):
+    def list_facts(self) -> list[str]:
         """Lists all known facts."""
-        pass
+        facts = set()
+        for backend in self.get_backends():
+            if backend is AbstractBackend:
+                facts.add(backend.list_facts())
+        return facts
 
     @abstractmethod
     def list_inferencers(self):
         """Lists all known inferencers."""
-        pass
+        inferencers = set()
+        for backend in self.get_backends():
+            if backend is AbstractBackend:
+                inferencers.add(backend.list_inferencers())
+        return inferencers
 
     @abstractmethod
     def list_heuristics(self):
         """Lists all known heuristics."""
-        pass
+        heuristics = set()
+        for backend in self.get_backends():
+            if backend is AbstractBackend:
+                heuristics.add(backend.list_inferencers())
+        return heuristics
 
     @abstractmethod
     def select_facts(self, criteria):
         """Selects or searches for facts based on provided criteria."""
-        pass
 
     @abstractmethod
     def select_inferencers(self, criteria):
         """Selects or searches for inferencers based on provided criteria."""
-        pass
 
     @abstractmethod
     def select_heuristics(self, criteria):
         """Selects or searches for heuristics based on provided criteria."""
-        pass
```

### Comparing `openssm-0.1.1/openssm/core/slm/abstract_slm.py` & `openssm-0.1.2/openssm/core/slm/abstract_slm.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,24 @@
     (SLMs). It provides an interface for natural language communication and
     structured API interactions.
     """
 
     @abstractmethod
     def get_adapter(self) -> AbstractAdapter:
         """Returns our adapter"""
-        pass
 
     @abstractmethod
     def set_adapter(self, adapter: AbstractAdapter):
         """Sets our adapter"""
-        pass
 
     @abstractmethod
     def discuss(self,
                 conversation_id: str,
                 user_input: list[dict]) -> list[dict]:
         """
         Processes a natural language conversation input
         and returns a list of replies
         """
-        pass
 
     @abstractmethod
     def reset_memory(self):
         """Resets our conversation memory"""
-        pass
```

### Comparing `openssm-0.1.1/openssm/core/slm/gpt3_slm.py` & `openssm-0.1.2/openssm/core/slm/openai_slm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,58 @@
-from openssm.core.config import Config
-from .base_slm import BaseSLM
-from openssm.core.adapter.abstract_adapter import AbstractAdapter
-from abc import abstractmethod
-import openai
 import ast
+import openai
+from openssm.core.slm.base_slm import BaseSLM
+from openssm.config import Config
+from openssm.core.adapter.abstract_adapter import AbstractAdapter
 
 
 class GPT3BaseSLM(BaseSLM):
     def __init__(self, adapter: AbstractAdapter = None):
         super().__init__(adapter)
+        if Config.OPENAI_API_KEY is None:
+            raise ValueError("Config.OPENAI_API_KEY is not set")
         openai.api_key = Config.OPENAI_API_KEY
-        self.conversations = {}  # dict of conversation_id: list of messages
 
-    @abstractmethod
-    def call_openai(self, conversation: list[dict]) -> list[dict]:
-        """Call OpenAI's API and return the response"""
-        pass
-
-    def discuss(self,
-                conversation_id: str,
-                user_input: list[dict]) -> list[dict]:
-        """Send user input to OpenAI's API and return the replies"""
-
-        # If conversation is new, start a new one, else continue from previous
-        conversation = self.conversations.get(conversation_id, [])
-        conversation.extend(user_input)
-
-        replies = self.call_openai(conversation)
-
-        # Save response to the conversation
-        conversation.extend(replies)
-        self.conversations[conversation_id] = conversation
-
-        # Return the model's replies
-        return replies
-
-    def reset_memory(self):
-        # Clear all conversations
-        self.conversations = {}
+
+class GPT3ChatCompletionSLM(GPT3BaseSLM):
+    def __init__(self, adapter: AbstractAdapter = None):
+        super().__init__(adapter)
+
+    def call_lm_api(self, conversation: list[dict]) -> list[dict]:
+        response = openai.ChatCompletion.create(
+            model="gpt-3.5-turbo",
+            messages=conversation,
+            # max_tokens=150,
+            temperature=0.7
+        )
+        return [response.choices[0].message]
 
 
 class GPT3CompletionSLM(GPT3BaseSLM):
     def __init__(self, adapter: AbstractAdapter = None):
         super().__init__(adapter)
 
-    def call_openai(self, conversation: list[dict]) -> list[dict]:
-        # Convert conversation to string
+    def convert_conversation_to_string(self, conversation: list[dict]) -> str:
         list_conversation = []
         for item in conversation:
             role = item["role"].replace('"', '\\"')
             content = item["content"].replace('"', '\\"')
             list_conversation.append(
                 f'{{"role": "{role}", "content": "{content}"}}'
             )
+        return ", ".join(list_conversation)
 
-        prompt = "\n".join(list_conversation)
+    def call_lm_api(self, conversation: list[dict]) -> list[dict]:
+        prompt = self.convert_conversation_to_string(conversation)
         prompt = (f"Complete this conversation with the assistant’s response, "
                   f"up to 500 words, in JSON, with quotes escaped with \\:\n"
                   f"{prompt}")
 
         response = openai.Completion.create(
             engine="text-davinci-002",
             prompt=prompt,
             temperature=0.7,
             max_tokens=500
         )
         reply = response.choices[0].text.strip()
         reply_dict = ast.literal_eval(reply)
         return [reply_dict]
-
-
-class GPT3ChatCompletionSLM(GPT3BaseSLM):
-    def __init__(self, adapter: AbstractAdapter = None):
-        super().__init__(adapter)
-
-    def call_openai(self, conversation: list[dict]) -> list[dict]:
-        response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo",
-            messages=conversation,
-            # max_tokens=150,
-            temperature=0.7
-        )
-        return [response.choices[0].message]
```

### Comparing `openssm-0.1.1/openssm/core/slm/memory/sqlite_conversation_db.py` & `openssm-0.1.2/openssm/core/slm/memory/sqlite_conversation_db.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-import abc
 import sqlite3
-import ...config
-import conversation_db
+from conversation_db import ConversationDB
+
 
 class SQLiteConversationDB(ConversationDB):
     def __init__(self, db_name):
         self.db_name = db_name
+        self.conversation_db = None
+        self.cursor = None
 
     def connect(self):
         self.conversation_db = sqlite3.connect(self.db_name)
         self.cursor = self.conversation_db.cursor()
 
     def create_table(self):
         self.cursor.execute('''CREATE TABLE IF NOT EXISTS conversations
                                 (id text PRIMARY KEY, history text)''')
         self.conversation_db.commit()
 
     def append_conversation(self, conversation_id, user_input):
-        self.cursor.execute('SELECT * FROM conversations WHERE id=?', (conversation_id,))
+        self.cursor.execute(
+            'SELECT * FROM conversations WHERE id=?',
+            (conversation_id,))
         conversation = self.cursor.fetchone()
         if conversation is None:
-            self.cursor.execute("INSERT INTO conversations VALUES (?,?)", (conversation_id, user_input))
+            self.cursor.execute(
+                "INSERT INTO conversations VALUES (?,?)",
+                (conversation_id, user_input))
         else:
             updated_conversation = conversation[1] + "\n" + user_input
-            self.cursor.execute("UPDATE conversations SET history = ? WHERE id = ?", (updated_conversation, conversation_id))
+            self.cursor.execute(
+                "UPDATE conversations SET history = ? WHERE id = ?",
+                (updated_conversation, conversation_id))
         self.conversation_db.commit()
 
     def get_conversation(self, conversation_id):
-        self.cursor.execute('SELECT * FROM conversations WHERE id=?', (conversation_id,))
+        self.cursor.execute(
+            "SELECT * FROM conversations WHERE id=?",
+            (conversation_id,))
         conversation = self.cursor.fetchone()
         if conversation is not None:
             return conversation[1]
         return None
 
     def close(self):
         self.conversation_db.close()
-
-class BaseNLUSLM(AbstractSLM, ABC):
-    def __init__(self, adapter, config):
-        super().__init__(adapter)
-        self.db = SQLiteConversationDB(config.db_config)
-        self.db.connect()
-        self.db.create_table()
-
-    def append_conversation(self, conversation_id, user_input):
-        self.db.append_conversation(conversation_id, user_input)
-
-    def get_conversation(self, conversation_id):
-        return self.db.get_conversation(conversation_id)
-
-    def process(self, conversation_id, user_input):
-        self.append_conversation(conversation_id, user_input)
-        return self.translate_to_adapter_calls(self.get_conversation(conversation_id))
-
-    def close(self):
-        self.db.close()
```

### Comparing `openssm-0.1.1/openssm/core/ssm/abstract_ssm.py` & `openssm-0.1.2/openssm/core/ssm/abstract_ssm.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,80 +9,65 @@
     The AbstractSSM serves as the base for all concrete Small Specialist
     Models (SSMs).
     """
 
     @abstractmethod
     def get_slm(self) -> AbstractSLM:
         """Returns our small language model (SLM)"""
-        pass
 
     @abstractmethod
     def get_adapter(self) -> AbstractAdapter:
         """Returns our adapter"""
-        pass
 
     @abstractmethod
     def get_backends(self) -> list[AbstractBackend]:
         """Returns our backends"""
-        pass
 
     @abstractmethod
     def discuss(self,
                 conversation_id: str,
                 user_input: list[dict]) -> list[dict]:
         """Processes a natural language conversation input."""
-        pass
 
     @abstractmethod
     def api_call(self, function_name, *args, **kwargs):
         """Processes a structured API call."""
-        pass
 
     @abstractmethod
     def reset_memory(self):
         """Resets the conversation memory of the SSM."""
-        pass
 
     @abstractmethod
     def list_facts(self) -> list[str]:
         """Lists all known facts."""
-        pass
 
     @abstractmethod
     def list_inferencers(self) -> list[str]:
         """Lists all known inferencers."""
-        pass
 
     @abstractmethod
     def list_heuristics(self) -> list[str]:
         """Lists all known heuristics."""
-        pass
 
     @abstractmethod
     def select_facts(self, criteria: dict) -> list[str]:
         """Selects or searches for facts based on provided criteria."""
-        pass
 
     @abstractmethod
     def select_inferencers(self, criteria: dict) -> list[str]:
         """Selects or searches for inferencers based on provided criteria."""
-        pass
 
     @abstractmethod
     def select_heuristics(self, criteria) -> list[str]:
         """Selects or searches for heuristics based on provided criteria."""
-        pass
 
     @abstractmethod
     def infer(self, input_facts: list[str]) -> list[str]:
         """Makes inferences based on the provided input facts."""
-        pass
 
     @abstractmethod
     def solve_problem(self, problem_description: list[str]) -> list[str]:
         """Solves a problem based on the provided description."""
-        pass
 
     @abstractmethod
     def add_backend(self, backend: AbstractBackend):
         """Adds a backend to the SSM."""
-        pass
```

### Comparing `openssm-0.1.1/openssm/core/ssm/gpt3_ssm.py` & `openssm-0.1.2/openssm/core/ssm/openai_ssm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .base_ssm import BaseSSM
-from openssm.core.slm.gpt3_slm import GPT3CompletionSLM, GPT3ChatCompletionSLM
+from openssm.core.ssm.base_ssm import BaseSSM
+from openssm.core.slm.openai_slm import GPT3CompletionSLM
+from openssm.core.slm.openai_slm import GPT3ChatCompletionSLM
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class GPT3CompletionSSM(BaseSSM):
     def __init__(self,
                  adapter: AbstractAdapter = None,
```

### Comparing `openssm-0.1.1/openssm/integration/llamaindex/README.md` & `openssm-0.1.2/openssm/integration/llamaindex/README.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.1/setup.py` & `openssm-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,131 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openssm
+Version: 0.1.2
+Summary: OpenSSM – 'Small Specialist Models' for Industrial AI
+Author: Aitomatic Engineering
+Author-email: engineering@aitomatic.com
+Requires-Python: >=3.8.1,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: accelerate (>=0.20.3,<0.21.0)
+Requires-Dist: einops (>=0.6.1,<0.7.0)
+Requires-Dist: llama-hub (>=0.0.4)
+Requires-Dist: llama-index (>=0.6.33)
+Requires-Dist: pypdf (>=3.11.0)
+Requires-Dist: pytest (>=7.0.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: transformers (>=4.30.2,<5.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['openssm',
- 'openssm.core',
- 'openssm.core.adapter',
- 'openssm.core.backend',
- 'openssm.core.slm',
- 'openssm.core.slm.memory',
- 'openssm.core.ssm']
-
-package_data = \
-{'': ['*'],
- 'openssm': ['industrial/interpretability/*',
-             'industrial/monitoring/*',
-             'industrial/security/*',
-             'industrial/security/audit/*',
-             'industrial/security/best_practices/*',
-             'integration/*',
-             'integration/llamaindex/*',
-             'integration/testing_tools/*']}
-
-install_requires = \
-['llama-hub>=0.0.4', 'llama-index>=0.6.33', 'pypdf>=3.11.0', 'pytest>=7.0.0']
-
-setup_kwargs = {
-    'name': 'openssm',
-    'version': '0.1.1',
-    'description': "OpenSSM – 'Small Specialist Models' for Industrial AI",
-    'long_description': '# OpenSSM – “Small Specialist Models” for Industrial AI\n\nOpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing\ntrust, reliability, and safety in Industrial-AI applications. Harnessing the power of domain expertise, SSMs operate either\nalone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving\ncapabilities.\n\nUnlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and\ndesigned specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers,\nand developers seeking specialized and robust AI solutions for industrial applications.\n\n![SSM in Industrial AI](./docs/diagrams/ssm-industrial-use-case.drawio.png)\n\nA prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM\nrepresents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this\nframework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and\nindustrial problems.\n\n## Why SSM?\n\nThe trend towards specialization in AI models is a clear trajectory seen by many in the field.\n\n> Specialization is crucial for quality .. not general purpose Al models – Eric Schmidt, Schmidt Foundation\n> .. small models .. for a specific task that are good –  Matei Zaharia, Databricks\n> .. small agents working together .. specific and best in their tasks – Harrison Chase, Langchain\n> .. small but highly capable expert models – Andrej Karpathy, OpenAI\n> .. small models are .. a massive paradigm shift .. about deploying AI models at scale – Rob Toews, Radical Ventures\n\nAs predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.”\nSSMs are the central part in the architecture of these systems.\n\n## What OpenSSM Offers\n\nOpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:\n\n- **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique\nrequirements of trustworthiness, safety, reliability, and scalability inherent to this sector.\n\n- **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible\nand cost-effective particularly for industrial usage where time and resources are critical factors.\n\n- **Easy Knowledge Capture:** OpenSSM has easy-to-use tools for capturing domain knowledge in diverse forms: books, operaring manuals, databases, knowledge graphs, text files, and code.\n\n- **Powerful Operations on Captured Knowledge:** OpenSSM enables both knowledge query and inferencing/predictive capabilities based on the domain-specific knowledge.\n\n- **Collaborative Problem-Solving**: SSMs are designed to work in problem-solving "teams". Multi-SSM collaboration is a first-class design feature, not an afterthought.\n\n- **Reliable Domain Expertise:** Each SSM has expertise in a particular field or equipment, offering precise and specialized\nknowledge, thereby enhancing trustworthiness, reliability, and safety for Industrial-AI applications. With self-reasoning,\ncausal reasoning, and retrieval-based knowledge, SSMs provide a trustable source of domain expertise.\n\n- **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering\nfreedom from vendor lock-in and security concerns.\n\n- **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.\n\n## Target Audience\n\nOur primary audience includes:\n\n- **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive\ncomputational resources or large vendor solutions.\n\n- **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.\n\n- **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven\nproject focused on building and sharing specialized AI models.\n\n- **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing\nthe reliability and trustworthiness of AI solutions in an industrial setting.\n\n## SSM Architecture\n\nAt a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of\nback-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not,\nand may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.\n\n![High-Level SSM Architecture](./docs/diagrams/ssm-key-components.drawio.png)\n\nThe above diagram illustrates the high-level architecture of an SSM, which comprises three main components:\n\n1. Small Language Model (SLM): This forms the communication frontend of an SSM.\n\n2. Adapters (e.g., LlamaIndex): These provide the interface between the SLM and the domain-knowledge backends.\n\n3. Domain-Knowledge Backends: These include text files, documents, PDFs, databases, code, knowledge graphs, models, other SSMs, etc.\n\nSSMs communicate in both unstructured (natural language) and structured APIs, catering to a variety of real-world industrial systems.\n\n![SSM Composability](./docs/diagrams/ssm-composability.drawio.png)\n\nThe composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.\n\n## Getting Started\n\nSee some example user programs in the [examples](./examples) directory. For example, to run the `chatssm` example, do:\n\n```bash\n% cd examples/chatssm\n% make clean\n% make\n```\n\nthen open your browser to `http://localhost:8080` and chat with the SSM.\n\nYou can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting\nStarted Guide](link-to-guide) for more information.\n\n## Roadmap\n\n- Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge\n- Create SSMs in your own development environment, and integrate SSMs into your own AI apps\n- Capture domain knowledge in various forms into your SSMs\n- Train SLMs via distillation of LLMs, teacher/student approaches, etc.\n- Apply SSMs in collaborative problem-solving AI systems\n\n## Community\n\nJoin our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI\nthrough SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).\n\n## Contribute\n\nOpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it\'s enhancing existing models,\ncreating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our\n[Contribution Guide](docs/CONTRIBUTING.md) for more details.\n\n## License\n\nOpenSSM is released under the [Apache 2.0 License](./LICENSE.md).\n',
-    'author': 'Aitomatic Engineering',
-    'author_email': 'engineering@aitomatic.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0',
-}
+# OpenSSM – “Small Specialist Models” for Industrial AI
 
+OpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing trust, reliability, and safety in Industrial-AI applications.  Harnessing the power of domain expertise, SSMs operate either alone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving capabilities.
+
+Unlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and designed specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers, and developers seeking specialized and robust AI solutions for industrial applications.
+
+![SSM in Industrial AI](./docs/diagrams/ssm-industrial-use-case.drawio.png)
+
+A prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM represents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this framework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and industrial problems.
+
+## Why SSM?
+
+The trend towards specialization in AI models is a clear trajectory seen by many in the field.
+
+> _Specialization is crucial for quality .. not general purpose Al models_ – Eric Schmidt, Schmidt Foundation
+
+> _.. small models .. for a specific task that are good_ –  Matei Zaharia, Databricks
+
+> _.. small agents working together .. specific and best in their tasks_ – Harrison Chase, Langchain
+
+> _.. small but highly capable expert models_ – Andrej Karpathy, OpenAI
+
+> _.. small models are .. a massive paradigm shift .. about deploying AI models at scale_ – Rob Toews, Radical Ventures
+
+As predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.” SSMs are the central part in the architecture of these systems.
+
+## What OpenSSM Offers
+
+OpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:
+
+- **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique requirements of trustworthiness, safety, reliability, and scalability inherent to this sector.
+
+- **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible and cost-effective particularly for industrial usage where time and resources are critical factors.
+
+- **Easy Knowledge Capture:** OpenSSM has easy-to-use tools for capturing domain knowledge in diverse forms: books, operaring manuals, databases, knowledge graphs, text files, and code.
+
+- **Powerful Operations on Captured Knowledge:** OpenSSM enables both knowledge query and inferencing/predictive capabilities based on the domain-specific knowledge.
+
+- **Collaborative Problem-Solving**: SSMs are designed to work in problem-solving "teams". Multi-SSM collaboration is a first-class design feature, not an afterthought.
+
+- **Reliable Domain Expertise:** Each SSM has expertise in a particular field or equipment, offering precise and specialized knowledge, thereby enhancing trustworthiness, reliability, and safety for Industrial-AI applications. With self-reasoning, causal reasoning, and retrieval-based knowledge, SSMs provide a trustable source of domain expertise.
+
+- **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering freedom from vendor lock-in and security concerns.
+
+- **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.
+
+## Target Audience
+
+Our primary audience includes:
+
+- **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive computational resources or large vendor solutions.
+
+- **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.
+
+- **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven project focused on building and sharing specialized AI models.
+
+- **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing the reliability and trustworthiness of AI solutions in an industrial setting.
+
+## SSM Architecture
+
+At a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of back-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not, and may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.
+
+![High-Level SSM Architecture](./docs/diagrams/ssm-key-components.drawio.png)
+
+The above diagram illustrates the high-level architecture of an SSM, which comprises three main components:
+
+1. Small Language Model (SLM): This forms the communication frontend of an SSM.
+
+2. Adapters (e.g., LlamaIndex): These provide the interface between the SLM and the domain-knowledge backends.
+
+3. Domain-Knowledge Backends: These include text files, documents, PDFs, databases, code, knowledge graphs, models, other SSMs, etc.
+
+SSMs communicate in both unstructured (natural language) and structured APIs, catering to a variety of real-world industrial systems.
+
+![SSM Composability](./docs/diagrams/ssm-composability.drawio.png)
+
+The composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.
+
+## Getting Started
+
+See our [Getting Started Guide](./GETTING_STARTED.md) for more information.
+
+## Roadmap
+
+- Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge
+
+- Create SSMs in your own development environment, and integrate SSMs into your own AI apps
+
+- Capture domain knowledge in various forms into your SSMs
+
+- Train SLMs via distillation of LLMs, teacher/student approaches, etc.
+
+- Apply SSMs in collaborative problem-solving AI systems
+
+## Community
+
+Join our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI through SSMs.  Participate in the discussions, share your ideas, or ask for help on our [Community Discussions](https://github.com/aitomatic/openssm/discussions).
+
+## Contribute
+
+OpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it's enhancing existing models, creating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our [Contribution Guide](docs/CONTRIBUTING.md) for more details.
+
+## License
+
+OpenSSM is released under the [Apache 2.0 License](./LICENSE.md).
+
+## Links
+
+- [GETTING_STARTED](./GETTING_STARTED.md)
 
-setup(**setup_kwargs)
```

