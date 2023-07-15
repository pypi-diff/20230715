# Comparing `tmp/paper-qa-3.3.0.tar.gz` & `tmp/paper-qa-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.3.0.tar", last modified: Wed Jul 12 20:44:11 2023, max compression
+gzip compressed data, was "paper-qa-3.3.1.tar", last modified: Sat Jul 15 05:00:01 2023, max compression
```

## Comparing `paper-qa-3.3.0.tar` & `paper-qa-3.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.043539 paper-qa-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 20:43:24.000000 paper-qa-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-12 20:44:11.039539 paper-qa-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-12 20:43:24.000000 paper-qa-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.035539 paper-qa-3.3.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.039539 paper-qa-3.3.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.039539 paper-qa-3.3.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:44:11.043539 paper-qa-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-12 20:43:24.000000 paper-qa-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.039539 paper-qa-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-12 20:43:24.000000 paper-qa-3.3.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 04:59:24.000000 paper-qa-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-15 05:00:01.616127 paper-qa-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-15 04:59:24.000000 paper-qa-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.612127 paper-qa-3.3.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 05:00:01.616127 paper-qa-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-15 04:59:24.000000 paper-qa-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-15 04:59:25.000000 paper-qa-3.3.1/tests/test_paperqa.py
```

### Comparing `paper-qa-3.3.0/LICENSE` & `paper-qa-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/PKG-INFO` & `paper-qa-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.0
+Version: 3.3.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.0/README.md` & `paper-qa-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.3.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.0
+Version: 3.3.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.0/paperqa/chains.py` & `paper-qa-3.3.1/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/paperqa/contrib/zotero.py` & `paper-qa-3.3.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/paperqa/docs.py` & `paper-qa-3.3.1/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,30 +592,30 @@
             citation = c.text.doc.citation
             # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
             if name_in_text(name, answer_text):
                 bib[name] = citation
         bib_str = "\n\n".join(
             [f"{i+1}. ({k}): {c}" for i, (k, c) in enumerate(bib.items())]
         )
-        formatted_answer = f"Question: {query}\n\n{answer_text}\n"
+        formatted_answer = f"Question: {answer.question}\n\n{answer_text}\n"
         if len(bib) > 0:
             formatted_answer += f"\nReferences\n\n{bib_str}\n"
         answer.answer = answer_text
         answer.formatted_answer = formatted_answer
         answer.references = bib_str
 
         if self.prompts.post is not None:
             chain = make_chain(
                 self.prompts.post,
                 cast(BaseLanguageModel, self.llm),
                 memory=self.memory_model,
             )
             post = await chain.arun(**answer.dict(), callbacks=get_callbacks("post"))
             answer.answer = post
-            answer.formatted_answer = f"Question: {query}\n\n{post}\n"
+            answer.formatted_answer = f"Question: {answer.question}\n\n{post}\n"
             if len(bib) > 0:
                 answer.formatted_answer += f"\nReferences\n\n{bib_str}\n"
         if self.memory_model is not None:
             answer.memory = self.memory_model.load_memory_variables(inputs={})["memory"]
             self.memory_model.save_context(
                 {"Question": answer.question}, {"Answer": answer.answer}
             )
```

### Comparing `paper-qa-3.3.0/paperqa/prompts.py` & `paper-qa-3.3.1/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/paperqa/readers.py` & `paper-qa-3.3.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/paperqa/types.py` & `paper-qa-3.3.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/paperqa/utils.py` & `paper-qa-3.3.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/setup.py` & `paper-qa-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.0/tests/test_paperqa.py` & `paper-qa-3.3.1/tests/test_paperqa.py`

 * *Files identical despite different names*

