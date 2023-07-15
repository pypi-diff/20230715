# Comparing `tmp/textmatchertoolkit-0.1.1.tar.gz` & `tmp/textmatchertoolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textmatchertoolkit-0.1.1.tar", max compression
+gzip compressed data, was "textmatchertoolkit-0.1.2.tar", max compression
```

## Comparing `textmatchertoolkit-0.1.1.tar` & `textmatchertoolkit-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      650 2023-07-14 22:41:49.558678 textmatchertoolkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 22:30:57.347983 textmatchertoolkit-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-14 22:30:57.347112 textmatchertoolkit-0.1.1/textmatchertoolkit/__init__.py
--rw-r--r--   0        0        0     6181 2023-07-14 22:32:35.192977 textmatchertoolkit-0.1.1/textmatchertoolkit/toolkit.py
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 textmatchertoolkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      650 2023-07-15 00:06:45.708379 textmatchertoolkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 22:30:57.347983 textmatchertoolkit-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 22:30:57.347112 textmatchertoolkit-0.1.2/textmatchertoolkit/__init__.py
+-rw-r--r--   0        0        0     6247 2023-07-15 00:06:28.395559 textmatchertoolkit-0.1.2/textmatchertoolkit/toolkit.py
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 textmatchertoolkit-0.1.2/PKG-INFO
```

### Comparing `textmatchertoolkit-0.1.1/pyproject.toml` & `textmatchertoolkit-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textmatchertoolkit"
-version = "0.1.1"
+version = "0.1.2"
 description = "In summary, this package provides a set of utility functions and matching algorithms that can be used to preprocess, analyze, and match text data in various applications such as natural language processing, information retrieval, and text similarity analysis."
 authors = ["Marco Cavallari <marco.cavallari.1999@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 transformers = "^4.30.2"
```

### Comparing `textmatchertoolkit-0.1.1/textmatchertoolkit/toolkit.py` & `textmatchertoolkit-0.1.2/textmatchertoolkit/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,25 @@
       df.loc[len(df.index)] = new_data
       return df
 
 
 
 class Matcher():
   def __init__(self):
+    self.d=0 if torch.cuda.is_available() else -1
     self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     self.similarity_model=SentenceTransformer('sentence-transformers/all-distilroberta-v1').to(self.device)
-    self.topic_model=pipeline("zero-shot-classification",model="valhalla/distilbart-mnli-12-1",device=0)#device=0
+    self.topic_model=pipeline("zero-shot-classification",model="valhalla/distilbart-mnli-12-1",device=self.d)#device=0
     self.candidate_topic_labels = ["Sports","Technology","Politics","Fashion","Health_Fitness","Travel","Business_Finance","Science_Education","Social_Issues"]
     self.utility=Utility()
     self.paraphrase_model=AutoModelForSequenceClassification.from_pretrained("Prompsit/paraphrase-bert-en").to(self.device)
     self.paraphrase_tokenizer=AutoTokenizer.from_pretrained("Prompsit/paraphrase-bert-en")
-    self.entailment_model=pipeline("text-classification",model="geckos/bart-fined-tuned-on-entailment-classification",tokenizer="geckos/bart-fined-tuned-on-entailment-classification",return_all_scores=True,device=0)#device=0
+    self.entailment_model=pipeline("text-classification",model="geckos/bart-fined-tuned-on-entailment-classification",tokenizer="geckos/bart-fined-tuned-on-entailment-classification",return_all_scores=True,device=self.d)#device=0
     #self.vectorizer = TfidfVectorizer()
-    self.subjectivity_model=pipeline(task="text-classification",model="cffl/bert-base-styleclassification-subjective-neutral",return_all_scores=True,device=0)#device=0
+    self.subjectivity_model=pipeline(task="text-classification",model="cffl/bert-base-styleclassification-subjective-neutral",return_all_scores=True,device=self.d)#device=0
 
   def compute_similarity(self,text1,text2):
     couple=(text1,text2)
     embeddings = self.similarity_model.encode(couple)
     cos_sim = dot(embeddings[0], embeddings[1])/(norm(embeddings[0])*norm(embeddings[1]))
     return cos_sim
```

### Comparing `textmatchertoolkit-0.1.1/PKG-INFO` & `textmatchertoolkit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textmatchertoolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: In summary, this package provides a set of utility functions and matching algorithms that can be used to preprocess, analyze, and match text data in various applications such as natural language processing, information retrieval, and text similarity analysis.
 Author: Marco Cavallari
 Author-email: marco.cavallari.1999@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

