# Comparing `tmp/langdash-1.7.5.tar.gz` & `tmp/langdash-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.7.5.tar", last modified: Fri Jul 14 03:46:15 2023, max compression
+gzip compressed data, was "langdash-1.8.0.tar", last modified: Sat Jul 15 20:32:17 2023, max compression
```

## Comparing `langdash-1.7.5.tar` & `langdash-1.8.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.403521 langdash-1.7.5/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.5/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.5/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-14 03:46:15.403521 langdash-1.7.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.7.5/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-14 03:45:48.000000 langdash-1.7.5/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.5/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    15388 2023-07-11 02:58:29.000000 langdash-1.7.5/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.5/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.5/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.395520 langdash-1.7.5/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.5/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6868 2023-07-11 03:00:19.000000 langdash-1.7.5/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.7.5/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.5/langdash/llm.py
--rw-r--r--   0 user      (1000) user      (1000)      739 2023-07-11 02:58:29.000000 langdash-1.7.5/langdash/llm_config.py
--rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.5/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.5/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.5/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.5/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.403521 langdash-1.7.5/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.5/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-07-09 01:44:13.000000 langdash-1.7.5/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.5/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.5/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.5/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     6112 2023-07-11 02:58:29.000000 langdash-1.7.5/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5810 2023-07-11 02:58:30.000000 langdash-1.7.5/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.5/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    11977 2023-07-11 03:04:01.000000 langdash-1.7.5/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.5/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.5/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.5/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.395520 langdash-1.7.5/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.5/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.5/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.5/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-14 03:46:15.403521 langdash-1.7.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.294276 langdash-1.8.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.8.0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.8.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-15 20:32:17.294276 langdash-1.8.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.8.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.286276 langdash-1.8.0/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-15 20:31:59.000000 langdash-1.8.0/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.8.0/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15394 2023-07-15 19:43:23.000000 langdash-1.8.0/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9603 2023-07-15 19:44:32.000000 langdash-1.8.0/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.8.0/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.282276 langdash-1.8.0/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.8.0/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.8.0/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.8.0/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.8.0/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.8.0/langdash/llm_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10076 2023-07-15 19:57:10.000000 langdash-1.8.0/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.8.0/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.0/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3775 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.294276 langdash-1.8.0/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.0/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1610 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2361 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1622 2023-07-15 19:25:51.000000 langdash-1.8.0/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      745 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6211 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5910 2023-07-15 19:27:43.000000 langdash-1.8.0/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.8.0/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12084 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5731 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.8.0/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.8.0/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.286276 langdash-1.8.0/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.8.0/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.8.0/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.8.0/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-15 20:32:17.294276 langdash-1.8.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.8.0/setup.py
```

### Comparing `langdash-1.7.5/LICENSE.txt` & `langdash-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/PKG-INFO` & `langdash-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.5
+Version: 1.8.0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.5/README.md` & `langdash-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/chains/chains.py` & `langdash-1.8.0/langdash/chains/chains.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     else:
       session = self._ld.session_for_model(ctx)
       assert isinstance(
         session, LLMGenerationSession
       ), "context must be LLMGenerationSession"
       return session
 
-  def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs) \
+  def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs = {},) \
     -> Generator[Response, None, None]:
     for node in self._node_pass(session, args):
       if isinstance(node, (LDReturns, LDChoice)):
         yield RespReturns(key=node._returns)
       yield from node(session, args)
 
   def stream(self, ctx: Union[str, "LLMGenerationSession"], **kwargs) \
```

### Comparing `langdash-1.7.5/langdash/chains/nodes.py` & `langdash-1.8.0/langdash/chains/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import List, Union, Optional, Tuple, TYPE_CHECKING
+from typing import List, Union, Optional, Tuple, Callable, TYPE_CHECKING
 import random
 from weakref import WeakKeyDictionary
 from math import inf
 
 from langdash.response import RespInfer, RespInject, RespReturns
 from langdash.infer import InferArgs
 
@@ -96,31 +96,36 @@
     self,
     ld: "Langdash",
     returns: str,
     end: Optional[Union[str, int]],
     padleft: str = "",
     infer_args: Optional[InferArgs] = None,
     end_is_token: bool = False,
+    logit_preprocessors: Optional[List[Callable[List[int], None]]] = None,
   ):
     super().__init__(ld)
     self._returns = returns
     self._end = end
     self._padleft = padleft
     self._infer_args = infer_args
     self._end_is_token = end_is_token
+    self._logit_preprocessors = logit_preprocessors
 
   def __repr__(self):
     return f"<Returns arg={self._returns}>"
 
   def __call__(
     self, session: "LLMGenerationSession", args: "LDNodeArgs"
   ) -> "LDNodeGenerator":
     for i, respinfer in enumerate(
       session.infer(
-        end=self._end, args=self._infer_args, end_is_token=self._end_is_token
+        end=self._end,
+        args=self._infer_args,
+        end_is_token=self._end_is_token,
+        logit_preprocessors=self._logit_preprocessors,
       )
     ):
       if i == 0:
         if self._padleft and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       elif respinfer.tokid == -1:  # end
         if self._padleft and respinfer.running_infer.startswith(self._padleft):
```

### Comparing `langdash-1.7.5/langdash/classify/token_qa.py` & `langdash-1.8.0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/core.py` & `langdash-1.8.0/langdash/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,22 +154,27 @@
 
   def returns(self, *args, **kwargs):
     """
     Create a new return node for the specified return value.
 
     Args:
       returns (str): The name of the return value.
-      end (str):
+      end (Optional[Union[str, int]]):
         Where to stop the inference. Either a string, or a token id.
-        If None is passed, the inference will continue forever (for streaming).
+        If `None` is passed, the inference will continue forever (for streaming).
       padleft (str):
         The left padding value for the return. If the generated string starts with
         *padleft* then it will be stripped.
       infer_args (Optional[InferArgs]):
         Optional inference arguments for generation.
+      end_is_token (bool):
+        True if the *end* argument should be interpreted as a single token.
+      logit_preprocessors (Optional[LogitPreprocessorList]):
+        Optional list of logit preprocessor functions to be
+        called before sampling.
 
     Returns:
       The return node.
     """
     return chains.LDReturns(self, *args, **kwargs)
 
   def choice(self, *args, **kwargs):
```

### Comparing `langdash-1.7.5/langdash/infer.py` & `langdash-1.8.0/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/llm.py` & `langdash-1.8.0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/llm_config.py` & `langdash-1.8.0/langdash/llm_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @dataclass(frozen=True)
 class LLMConfig:
   """
   Data class used to store unified LLM config.
   
   Attributes:
     model:
-      the name, or the path of the model. Defaults to 0.
+      the name, or the path of the model. Defaults to None.
     batch_size:
       the number of tokens per batch size for inference.
       Defaults to -1 for auto.
     threads:
       the number of threads used for inference.
       Defaults to -1 for auto.
     context_length:
```

### Comparing `langdash-1.7.5/langdash/llm_session.py` & `langdash-1.8.0/langdash/llm_session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import TypeVar, Generic, Optional, List, Generator, Union, Tuple, TYPE_CHECKING
+from typing import TypeVar, Generic, Optional, List, Generator, Union, Tuple, Callable, Sequence, Mapping, TYPE_CHECKING
 import copy
 
 from langdash.response import RespInfer
 from langdash.chains import CalledNode, LDNodeArgs, LDNode
 from langdash.infer import InferArgs
 from langdash.llm import LLM
 
 if TYPE_CHECKING:
   from langdash.core import Langdash
 
+LogitPreprocessorList = List[Callable[Sequence[int], None]]
+
 T_LLM = TypeVar("T_LLM", bound=LLM)
 
 
 class LLMSession(Generic[T_LLM]):
   """
   Base class for a session for a language model.
   """
@@ -173,58 +175,87 @@
     """
     raise NotImplementedError("next_token_probs")
 
   def flush_token(self):
     raise NotImplementedError("flush_token")
 
   def _infer(
-    self, end: Optional[Union[str, int]], args: InferArgs, end_is_token: bool
-  ) -> Generator[RespInfer, None, None]:
-    raise NotImplementedError("_infer")
-
-  def infer(
     self,
     end: Optional[Union[str, int]],
-    args: Optional[InferArgs] = None,
-    end_is_token: bool = False,
+    args: InferArgs,
+    end_is_token: bool,
+    logit_preprocessors: Optional[LogitPreprocessorList],
   ) -> Generator[RespInfer, None, None]:
+    raise NotImplementedError("_infer")
+
+  def infer(self,
+            args: InferArgs = None,
+            **kwargs) -> Generator[RespInfer, None, None]:
     """
     Infer the next tokens from the input sequence.
 
     Args:
       end (Optional[Union[str, int]]):
         The end of the output sequence.
         If set to `None`, the output sequence will be generated until the maximum number of tokens is reached.
         
         Defaults to `None`.
       args (Optional[InferArgs]):
         Optional inference parameters. Defaults to `None`.
       end_is_token (bool):
         If true, then the end string will be interpreted as a token. Defaults to `False`.
+      logit_preprocessors (Optional[LogitPreprocessorList]):
+        Optional list of logit preprocessor functions to be
+        called before sampling.
         
     Returns:
       (Generator[RespInfer, None, None]) Generator yielding inference events.
     """
     if not args:
       args = self.default_infer_args
-    yield from self._infer(end=end, args=args, end_is_token=end_is_token)
+    yield from self._infer(args=args, **kwargs)
 
   def inject(
     self,
     text: Union[str, int, List[int]],
     add_special_tokens: bool = False
   ) -> int:
     raise NotImplementedError("inject")
 
   def get_context_length(self) -> int:
     """
     Returns the context length of the model, or zero for models that don't support one.
     """
     return 0
 
+  def scratch_state(self) -> "LLMGenerationSessionStateManager":
+    """
+    Returns a context manager that manages setting and unloading temporary state.
+    """
+    return LLMGenerationSessionStateManager(self)
+
+  def get_vocab(self) -> Mapping[str, int]:
+    """
+    Returns a mapping of token strings to their respective ids.
+    """
+    raise NotImplementedError("tokens_to_id")
+
+
+class LLMGenerationSessionStateManager:
+
+  def __init__(self, session: LLMGenerationSession):
+    self._session = session
+    self._old_state = self._session.clone_state()
+
+  def __enter__(self):
+    return self._session
+
+  def __exit__(self, exc_type, exc_value, traceback):
+    self._session.set_state(self._old_state)
+
 
 T_Tensor = TypeVar("T_Tensor")
 
 
 class LLMGenerationSessionForRawText(
   LLMGenerationSession, Generic[T_LLM, T_LLMState, T_Tensor]
 ):
```

### Comparing `langdash-1.7.5/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.8.0/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import Generator, Optional, Union, Any, Tuple, List
+from typing import Generator, Optional, Union, Any, Tuple, List, TYPE_CHECKING
 from math import inf
 from torch import Tensor
 
 from langdash.response import RespInfer
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
 from .._tokenizer.tokenizer import BufferedToken
 
+if TYPE_CHECKING:
+  from langdash.llm_session import LogitPreprocessorList
+
 
 class TensorBasedInferMixin:
   _model: Any
   _logits: Optional[Tensor]
   _next_token: Optional[Tuple[int, str]]
 
   def _eval(self, token: int) -> Tensor:
@@ -19,15 +22,19 @@
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     raise NotImplementedError("tokenize")
 
   def decode(self, tokids: List[int]) -> str:
     raise NotImplementedError("decode")
 
   def _infer(
-    self, end: Optional[Union[str, int]], args: InferArgs, end_is_token: bool
+    self,
+    end: Optional[Union[str, int]],
+    args: InferArgs,
+    end_is_token: bool,
+    logit_preprocessors: Optional["LogitPreprocessorList"],
   ) -> Generator[RespInfer, None, None]:
     generated = ""
     buffered_tokens: Optional[BufferedToken] = None
     ctx: List[int] = []
 
     if isinstance(end, str):
       if len(end) == 0:
@@ -38,15 +45,17 @@
         end = endtoks[0]
 
     if self._logits is None:
       if self._next_token is not None:
         self._logits = self._eval(self._next_token[0])
         self._next_token = None
       else:
-        raise ValueError("no prompt provided")
+        raise ValueError(
+          "Initial prompt is not provided. Please inject a prompt into the model before generation."
+        )
 
     for i in range(args.max_new_tokens):
       strip_left: Optional[str] = None
 
       if i == 0 and self._next_token is not None:
         for logits_tokid in self._model.tokenizer.tokens_starting_with(
           self._next_token[0]
@@ -60,14 +69,18 @@
           strip_left = self._next_token[1]
 
         self._next_token = None
 
       if args.min_new_tokens > 0 and i < args.min_new_tokens:
         self._logits[end] = -inf
 
+      if logit_preprocessors is not None:
+        for pp in logit_preprocessors:
+          pp(self._logits)
+
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
 
       if tokid == self._model.eos_token:  # implies end is int
         break
 
       tokstr: Optional[str] = None
```

### Comparing `langdash-1.7.5/langdash/models/_tokenizer/_bpe.py` & `langdash-1.8.0/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.8.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Generator
+from typing import List, Union, Optional, Generator, Mapping
 from .tokenizer import Tokenizer, BufferedToken
 
 
 class BytesDictTokenizer(Tokenizer):
 
   def __init__(self, encode_func, decode_func, mapping: List[bytes]):
     self.encode_func = encode_func
@@ -24,14 +24,17 @@
 
   def tokens_starting_with(self, token_id: int) -> Generator[int, None, None]:
     tokstr = self.mapping[token_id]
     for logits_tokid, logits_tokstr in enumerate(self.mapping):
       if not logits_tokstr.startswith(tokstr):
         yield logits_tokid
 
+  def get_vocab(self) -> Mapping[str, int]:
+    return self.mapping
+
 
 class BytesDictBufferedToken(BufferedToken):
 
   def __init__(self, tokenizer: BytesDictTokenizer, token_bytes: bytes):
     self.tokenizer = tokenizer
     self.token_bytes = token_bytes
```

### Comparing `langdash-1.7.5/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.8.0/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Generator
+from typing import List, Union, Optional, Generator, Mapping
 import warnings
 from .tokenizer import Tokenizer, BufferedToken
 from ._bpe import decode as bpe_decode
 
 
 class HFTokenizer(Tokenizer):
   vocab: List[str]
@@ -48,14 +48,17 @@
       tokstr = self.tokenizer.decode(token_id)
       for logits_tokid, logits_tokstr in enumerate(self.vocab):
         if not logits_tokstr.startswith(tokstr):
           yield logits_tokid
     except UnicodeDecodeError:
       return
 
+  def get_vocab(self) -> Mapping[str, int]:
+    return self.tokenizer.get_vocab()
+
 
 class HFBufferedToken(BufferedToken):
 
   def __init__(self, tokenizer: HFTokenizer, token_id: int):
     self.tokenizer = tokenizer
     self.tokens: List[int] = [token_id]
```

### Comparing `langdash-1.7.5/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.8.0/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Generator
+from typing import List, Union, Optional, Generator, Mapping
 from .tokenizer import Tokenizer, BufferedToken
 from ._bpe import decode as bpe_decode
 
 
 class RwkvTokenizer(Tokenizer):
 
   def __init__(self, tokenizer):
@@ -29,14 +29,17 @@
 
   def tokens_starting_with(self, token_id: int) -> Generator[int, None, None]:
     tokstr = self.decode([token_id])
     for logits_tokstr, logits_tokid in self.vocab.items():
       if not logits_tokstr.startswith(tokstr):
         yield logits_tokid
 
+  def get_vocab(self) -> Mapping[str, int]:
+    return self.vocab
+
 
 class RwkvBufferedToken(BufferedToken):
 
   def __init__(self, tokenizer: RwkvTokenizer, token_id: int):
     self.tokenizer = tokenizer
     self.token_ids = [token_id]
```

### Comparing `langdash-1.7.5/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.8.0/langdash/models/_tokenizer/tokenizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Generator
+from typing import List, Union, Optional, Generator, Mapping
 from abc import ABC, abstractmethod
 
 
 class BufferedToken(ABC):
 
   @abstractmethod
   def add_token_id(self, token_id: int) -> Optional[str]:
@@ -26,7 +26,11 @@
   @abstractmethod
   def decode_once(self, token_id: int) -> Union[str, BufferedToken]:
     pass
 
   @abstractmethod
   def tokens_starting_with(self, token_id: int) -> Generator[int, None, None]:
     pass
+
+  @abstractmethod
+  def get_vocab(self) -> Mapping[str, int]:
+    pass
```

### Comparing `langdash-1.7.5/langdash/models/ctransformers.py` & `langdash-1.8.0/langdash/models/ctransformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Any
+from typing import List, Optional, Any, Mapping
 import weakref
 import torch
 
 from langdash.llm import LLM
 from langdash.llm_config import LLMConfig
 from langdash.llm_session import LLMGenerationSessionForRawText
 import langdash.sampling as sampling
@@ -142,14 +142,17 @@
 
   def clone_state(self) -> CTransformersState:
     return self._model.clone_state(self)
 
   def get_context_length(self) -> int:
     return self._model.get_context_length(self)
 
+  def get_vocab(self) -> Mapping[str, int]:
+    return self._model.tokenizer.get_vocab()
+
   # Wrapper for public functions to flush the old session states
 
   def inject(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
   def flush_token(self, *a, **k):
```

### Comparing `langdash-1.7.5/langdash/models/llama_cpp.py` & `langdash-1.8.0/langdash/models/llama_cpp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Mapping
 import weakref
 import torch
 from llama_cpp import Llama, LlamaState, llama_token_to_str  # type: ignore
 
 from langdash.llm import LLM
 from langdash.llm_config import LLMConfig
 from langdash.llm_session import LLMGenerationSessionForRawText
@@ -130,15 +130,18 @@
     return self._model.tokenizer.decode(tokens)
 
   def _on_first_inject(self):
     self._model.model.reset()
     self._eval(self._model.bos_token)
 
   def get_context_length(self) -> int:
-    return self.model.get_context_length(self)
+    return self._model.get_context_length(self)
+
+  def get_vocab(self) -> Mapping[str, int]:
+    return self._model.tokenizer.get_vocab()
 
   # Wrapper for public functions to flush the old session states
 
   def inject(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
```

### Comparing `langdash-1.7.5/langdash/models/mock.py` & `langdash-1.8.0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/models/rwkv_cpp.py` & `langdash-1.8.0/langdash/models/rwkv_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Mapping
 from dataclasses import dataclass
 import copy
 import os
 import sys
 import torch
 import tokenizers  # type: ignore
 
@@ -290,14 +290,17 @@
 
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
+  def get_vocab(self) -> Mapping[str, int]:
+    return self._model.tokenizer.get_vocab()
+
 
 class RwkvCppModel(LLM[RwkvCppSession]):
   """
   rwkv.cpp model
   """
 
   _model_path: str
@@ -317,22 +320,22 @@
     **model_kwargs
   ):
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
   
     You can pass the following environment variables to set compile flags:
   
-    * LANGDASH_RWKV_CPP_COMMIT: hash of the commit to compile
-    * LANGDASH_RWKV_CPP_FORCE_RECOMPILE: '1' to force recompilation
-    * LANGDASH_RWKV_CPP_PATCH_MAX_NODES: '1' to patch the ggml library in rwkv.cpp
+    * `LANGDASH_RWKV_CPP_COMMIT`: hash of the commit to compile
+    * `LANGDASH_RWKV_CPP_FORCE_RECOMPILE`: '1' to force recompilation
+    * `LANGDASH_RWKV_CPP_PATCH_MAX_NODES`: '1' to patch the ggml library in rwkv.cpp
     so that large batch_size works (> 1)
   
     These environment variables can be used to set runtime flags:
   
-    * LANGDASH_RWKV_CPP_ENABLE_EVAL_SEQUENCE: enable sequence evaluation. This
+    * `LANGDASH_RWKV_CPP_ENABLE_EVAL_SEQUENCE`: enable sequence evaluation. This
     feature is locked behind a flag because it requires the ggml library to be patched.
   
     Args:
       model_path (str): Path to the model file.
       tokenizer_path (Optional[str]):
         Path to the tokenizer file.
         Defaults to `None`. If not set, the built-in tokenizer will be used.
```

### Comparing `langdash-1.7.5/langdash/models/sentence_transformers.py` & `langdash-1.8.0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/models/transformers.py` & `langdash-1.8.0/langdash/models/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Tuple, Union, Any
+from typing import List, Optional, Tuple, Union, Any, Mapping
 from dataclasses import dataclass
 import copy
 
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
 from ._tokenizer.hf_tokenizer import HFTokenizer
@@ -153,14 +153,17 @@
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def get_context_length(self) -> int:
     return self.model.get_context_length()
 
+  def get_vocab(self) -> Mapping[str, int]:
+    return self._model.tokenizer.get_vocab()
+
 
 class TransformersModel(LLM[TransformersSession]):
   """
   transformers model.
   """
   Session = TransformersSession
```

### Comparing `langdash-1.7.5/langdash/sampling.py` & `langdash-1.8.0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/search/embedding_search.py` & `langdash-1.8.0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/search/engine.py` & `langdash-1.8.0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash/search/multichoice_search.py` & `langdash-1.8.0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/langdash.egg-info/PKG-INFO` & `langdash-1.8.0/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.5
+Version: 1.8.0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.5/langdash.egg-info/SOURCES.txt` & `langdash-1.8.0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.5/setup.py` & `langdash-1.8.0/setup.py`

 * *Files identical despite different names*

