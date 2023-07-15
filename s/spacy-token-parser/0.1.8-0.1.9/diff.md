# Comparing `tmp/spacy-token-parser-0.1.8.tar.gz` & `tmp/spacy-token-parser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-token-parser-0.1.8.tar", max compression
+gzip compressed data, was "spacy-token-parser-0.1.9.tar", max compression
```

## Comparing `spacy-token-parser-0.1.8.tar` & `spacy-token-parser-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      507 2022-09-16 22:47:09.327675 spacy-token-parser-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      230 2022-09-16 22:47:05.019173 spacy-token-parser-0.1.8/spacy_token_parser/__init__.py
--rw-r--r--   0        0        0      458 2022-09-16 22:14:32.059673 spacy-token-parser-0.1.8/spacy_token_parser/dmo/__init__.py
--rw-r--r--   0        0        0     2094 2022-09-16 22:13:17.582673 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_coordinates.py
--rw-r--r--   0        0        0     3231 2022-09-16 22:13:15.195173 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_normalize.py
--rw-r--r--   0        0        0     1709 2022-09-16 22:30:29.119173 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_postprocess.py
--rw-r--r--   0        0        0     1341 2022-09-16 22:13:05.678674 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_punctuation.py
--rw-r--r--   0        0        0     5051 2022-09-16 22:13:02.179173 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_resultset.py
--rw-r--r--   0        0        0     1670 2022-09-16 22:13:00.069673 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_spacy.py
--rw-r--r--   0        0        0     1736 2022-09-16 22:12:56.719673 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_squots.py
--rw-r--r--   0        0        0     1655 2022-09-16 22:12:51.907673 spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_wordnet.py
--rw-r--r--   0        0        0       66 2022-09-16 22:10:41.393173 spacy-token-parser-0.1.8/spacy_token_parser/dto/__init__.py
--rw-r--r--   0        0        0     2292 2022-09-16 22:44:09.385673 spacy-token-parser-0.1.8/spacy_token_parser/dto/normalizer.py
--rw-r--r--   0        0        0      435 2022-08-31 16:53:29.714486 spacy-token-parser-0.1.8/spacy_token_parser/dto/stemmer.py
--rw-r--r--   0        0        0      112 2022-09-16 22:46:53.734173 spacy-token-parser-0.1.8/spacy_token_parser/svc/__init__.py
--rw-r--r--   0        0        0     2309 2022-08-31 17:24:33.676913 spacy-token-parser-0.1.8/spacy_token_parser/svc/generate_displacy_output.py
--rw-r--r--   0        0        0     2352 2022-09-16 22:14:49.468173 spacy-token-parser-0.1.8/spacy_token_parser/svc/parse_input_tokens.py
--rw-r--r--   0        0        0      746 2022-09-16 22:48:01.132673 spacy-token-parser-0.1.8/setup.py
--rw-r--r--   0        0        0      341 2022-09-16 22:48:01.133173 spacy-token-parser-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      519 2022-09-17 20:05:34.895074 spacy-token-parser-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      646 2022-09-17 20:01:38.361995 spacy-token-parser-0.1.9/spacy_token_parser/__init__.py
+-rw-r--r--   0        0        0      458 2022-09-16 22:14:32.059673 spacy-token-parser-0.1.9/spacy_token_parser/dmo/__init__.py
+-rw-r--r--   0        0        0     2094 2022-09-16 22:13:17.582673 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_coordinates.py
+-rw-r--r--   0        0        0     3231 2022-09-16 22:13:15.195173 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_normalize.py
+-rw-r--r--   0        0        0     1709 2022-09-16 22:30:29.119173 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_postprocess.py
+-rw-r--r--   0        0        0     1341 2022-09-16 22:13:05.678674 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_punctuation.py
+-rw-r--r--   0        0        0     5051 2022-09-16 22:13:02.179173 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_resultset.py
+-rw-r--r--   0        0        0     1670 2022-09-16 22:13:00.069673 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_spacy.py
+-rw-r--r--   0        0        0     1736 2022-09-16 22:12:56.719673 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_squots.py
+-rw-r--r--   0        0        0     1655 2022-09-16 22:12:51.907673 spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_wordnet.py
+-rw-r--r--   0        0        0      242 2022-09-17 19:56:57.211686 spacy-token-parser-0.1.9/spacy_token_parser/dto/__init__.py
+-rw-r--r--   0        0        0     2292 2022-09-16 22:44:09.385673 spacy-token-parser-0.1.9/spacy_token_parser/dto/normalizer.py
+-rw-r--r--   0        0        0      675 2022-09-17 20:00:18.349265 spacy-token-parser-0.1.9/spacy_token_parser/dto/project_types.py
+-rw-r--r--   0        0        0      435 2022-08-31 16:53:29.714486 spacy-token-parser-0.1.9/spacy_token_parser/dto/stemmer.py
+-rw-r--r--   0        0        0      170 2022-09-17 19:29:26.428973 spacy-token-parser-0.1.9/spacy_token_parser/svc/__init__.py
+-rw-r--r--   0        0        0     5564 2022-09-17 19:57:07.785145 spacy-token-parser-0.1.9/spacy_token_parser/svc/create_graph_structure.py
+-rw-r--r--   0        0        0     2335 2022-09-17 20:04:58.624250 spacy-token-parser-0.1.9/spacy_token_parser/svc/generate_displacy_output.py
+-rw-r--r--   0        0        0     2484 2022-09-17 19:56:15.144873 spacy-token-parser-0.1.9/spacy_token_parser/svc/parse_input_tokens.py
+-rw-r--r--   0        0        0      746 2022-09-17 20:06:10.420098 spacy-token-parser-0.1.9/setup.py
+-rw-r--r--   0        0        0      341 2022-09-17 20:06:10.420098 spacy-token-parser-0.1.9/PKG-INFO
```

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_coordinates.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_coordinates.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_normalize.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_normalize.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_postprocess.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_postprocess.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_punctuation.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_resultset.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_resultset.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_spacy.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_spacy.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_squots.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_squots.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dmo/token_parser_wordnet.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dmo/token_parser_wordnet.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/dto/normalizer.py` & `spacy-token-parser-0.1.9/spacy_token_parser/dto/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/svc/generate_displacy_output.py` & `spacy-token-parser-0.1.9/spacy_token_parser/svc/generate_displacy_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     def _navigation(self,
                     data):
         if type(data) == list:
             [self._navigation(x) for x in data]
 
         elif type(data) == dict:
+            print (data)
 
             if 'type' in data and data['type'] == 'sentence':  # this is a sentence
 
                 if len(self._d_buffer):
                     self._master.append(self._d_buffer)
 
                 self._d_buffer = {
```

### Comparing `spacy-token-parser-0.1.8/spacy_token_parser/svc/parse_input_tokens.py` & `spacy-token-parser-0.1.9/spacy_token_parser/svc/parse_input_tokens.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """ Use spaCy to Parse Input Tokens """
 
 
-from baseblock import Enforcer
-from baseblock import Stopwatch
-from baseblock import BaseObject
-
+from baseblock import Stopwatch  # type: ignore
+from baseblock import BaseObject  # type: ignore
 
 from spacy_token_parser.dmo import TokenParserSpacy
 from spacy_token_parser.dmo import TokenParserWordnet
 from spacy_token_parser.dmo import TokenParserNormalize
 from spacy_token_parser.dmo import TokenParserPunctuation
 from spacy_token_parser.dmo import TokenParserCoordinates
 from spacy_token_parser.dmo import TokenParserSquots
 from spacy_token_parser.dmo import TokenParserResultSet
 from spacy_token_parser.dmo import TokenParserPostProcess
 
+from spacy_token_parser.dto.project_types import InputTokens
+from spacy_token_parser.dto.project_types import ParseInputTokensResult
+
 
 class ParseInputTokens(BaseObject):
     """ Use spaCy to Parse Input Tokens """
 
     def __init__(self):
         """ Change Log
 
@@ -39,21 +40,18 @@
                 https://github.com/craigtrim/spacy-token-parser/issues/3
             *   rename all components
                 https://github.com/craigtrim/spacy-token-parser/issues/3
         """
         BaseObject.__init__(self, __name__)
 
     def process(self,
-                tokens: list) -> tuple:
+                tokens: InputTokens) -> ParseInputTokensResult:
 
         sw = Stopwatch()
 
-        if self.isEnabledForDebug:
-            Enforcer.is_list_of_str(tokens)
-
         tokens = TokenParserSquots().process(tokens)
         doc = TokenParserSpacy().process(' '.join(tokens))
 
         results = TokenParserResultSet().process(doc)
         results = TokenParserPunctuation().process(results)
         results = TokenParserNormalize().process(results)
         results = TokenParserCoordinates().process(results)
@@ -62,8 +60,11 @@
 
         if self.isEnabledForInfo:
             self.logger.info('\n'.join([
                 "Input Token Parsing Completed",
                 f"\tTotal Tokens: {len(results)}",
                 f"\tTotal Time: {str(sw)}"]))
 
-        return results, doc
+        return {
+            'tokens': results,
+            'doc': doc
+        }
```

### Comparing `spacy-token-parser-0.1.8/setup.py` & `spacy-token-parser-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'nltk==3.7', 'spacy==3.3', 'wordnet-lookup']
 
 setup_kwargs = {
     'name': 'spacy-token-parser',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Use spaCy to Parse Input Tokens',
     'long_description': None,
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

