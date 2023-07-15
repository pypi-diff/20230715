# Comparing `tmp/sign_language_translator-0.4.2.tar.gz` & `tmp/sign_language_translator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sign_language_translator-0.4.2.tar", max compression
+gzip compressed data, was "sign_language_translator-0.5.0.tar", max compression
```

## Comparing `sign_language_translator-0.4.2.tar` & `sign_language_translator-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
--rw-r--r--   0        0        0    12937 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/README.md
--rw-r--r--   0        0        0     1083 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2565 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/sign_language_translator/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/sign_language_translator/config/__init__.py
--rw-r--r--   0        0        0     1287 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/sign_language_translator/config/enums.py
--rw-r--r--   0        0        0      616 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/config/helpers.py
--rw-r--r--   0        0        0      329 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/config/settings.py
--rw-r--r--   0        0        0        0 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/__init__.py
--rwxr-xr-x   0        0        0    10252 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/completeness.py
--rwxr-xr-x   0        0        0     7713 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/scraping.py
--rwxr-xr-x   0        0        0     2107 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/synonyms.py
--rw-r--r--   0        0        0      250 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/__init__.py
--rw-r--r--   0        0        0      642 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/__init__.py
--rw-r--r--   0        0        0     4982 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/mapping_rules.py
--rw-r--r--   0        0        0     7759 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/pakistan_sign_language.py
--rw-r--r--   0        0        0     3773 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/sign_language.py
--rw-r--r--   0        0        0      355 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/__init__.py
--rw-r--r--   0        0        0       80 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/english.py
--rw-r--r--   0        0        0     1070 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/text_language.py
--rw-r--r--   0        0        0    12816 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/urdu.py
--rw-r--r--   0        0        0     2453 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/utils.py
--rw-r--r--   0        0        0    11710 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/vocab.py
--rw-r--r--   0        0        0      573 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/__init__.py
--rw-r--r--   0        0        0      455 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/__init__.py
--rwxr-xr-x   0        0        0     1171 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/abstract_language_model.py
--rwxr-xr-x   0        0        0     3277 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/beam_sampling.py
--rwxr-xr-x   0        0        0     2785 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/mixer.py
--rwxr-xr-x   0        0        0     9002 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/simple_language_model.py
--rwxr-xr-x   0        0        0       74 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/transformer_language_model.py
--rw-r--r--   0        0        0        0 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/sign_to_text/__init__.py
--rw-r--r--   0        0        0      158 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/__init__.py
--rw-r--r--   0        0        0     3237 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
--rw-r--r--   0        0        0      536 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/t2s_model.py
--rw-r--r--   0        0        0     1100 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/utils.py
--rw-r--r--   0        0        0      446 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/__init__.py
--rwxr-xr-x   0        0        0     3320 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/metrics.py
--rwxr-xr-x   0        0        0      882 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/preprocess.py
--rwxr-xr-x   0        0        0     1333 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/subtitles.py
--rw-r--r--   0        0        0     4194 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/tagger.py
--rw-r--r--   0        0        0     4800 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/tokenizer.py
--rwxr-xr-x   0        0        0     9223 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/utils.py
--rwxr-xr-x   0        0        0       43 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/__init__.py
--rwxr-xr-x   0        0        0     3675 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/data_loader.py
--rwxr-xr-x   0        0        0    13542 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/landmarks_info.py
--rwxr-xr-x   0        0        0    10351 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/sign_data_attributes.py
--rwxr-xr-x   0        0        0     2822 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/tree.py
--rw-r--r--   0        0        0        0 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/__init__.py
--rwxr-xr-x   0        0        0    18024 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/concatenate.py
--rwxr-xr-x   0        0        0     7980 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/embed.py
--rwxr-xr-x   0        0        0    33628 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/transforms.py
--rwxr-xr-x   0        0        0    30236 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/visualization.py
--rw-r--r--   0        0        0    14366 1970-01-01 00:00:00.000000 sign_language_translator-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    14574 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/README.md
+-rw-r--r--   0        0        0     1180 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2567 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/__init__.py
+-rw-r--r--   0        0        0     3330 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/cli.py
+-rw-r--r--   0        0        0      513 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/__init__.py
+-rw-r--r--   0        0        0     2381 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/enums.py
+-rw-r--r--   0        0        0     2184 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/helpers.py
+-rw-r--r--   0        0        0     1704 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/settings.py
+-rw-r--r--   0        0        0     1382 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/urls.yaml
+-rw-r--r--   0        0        0        0 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/__init__.py
+-rwxr-xr-x   0        0        0    10252 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/completeness.py
+-rwxr-xr-x   0        0        0     7713 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/scraping.py
+-rwxr-xr-x   0        0        0     2107 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/synonyms.py
+-rw-r--r--   0        0        0      250 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/__init__.py
+-rw-r--r--   0        0        0     4982 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/mapping_rules.py
+-rw-r--r--   0        0        0     7987 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/pakistan_sign_language.py
+-rw-r--r--   0        0        0     3773 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/sign_language.py
+-rw-r--r--   0        0        0      355 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/__init__.py
+-rw-r--r--   0        0        0       80 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/english.py
+-rw-r--r--   0        0        0     1070 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/text_language.py
+-rw-r--r--   0        0        0    13072 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/urdu.py
+-rw-r--r--   0        0        0     2083 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/utils.py
+-rw-r--r--   0        0        0    12426 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/vocab.py
+-rw-r--r--   0        0        0      571 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/__init__.py
+-rwxr-xr-x   0        0        0     1171 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/abstract_language_model.py
+-rwxr-xr-x   0        0        0     3277 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/beam_sampling.py
+-rwxr-xr-x   0        0        0     2785 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/mixer.py
+-rwxr-xr-x   0        0        0     9002 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/simple_language_model.py
+-rwxr-xr-x   0        0        0       74 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/transformer_language_model.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/sign_to_text/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/__init__.py
+-rw-r--r--   0        0        0     3237 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
+-rw-r--r--   0        0        0      536 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/t2s_model.py
+-rw-r--r--   0        0        0     1845 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/models/utils.py
+-rw-r--r--   0        0        0      446 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/__init__.py
+-rwxr-xr-x   0        0        0     3320 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/metrics.py
+-rwxr-xr-x   0        0        0      882 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/preprocess.py
+-rwxr-xr-x   0        0        0     1333 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/subtitles.py
+-rw-r--r--   0        0        0     4248 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/tagger.py
+-rw-r--r--   0        0        0     4800 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/tokenizer.py
+-rwxr-xr-x   0        0        0     9223 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/utils.py
+-rwxr-xr-x   0        0        0      590 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3675 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/data_loader.py
+-rw-r--r--   0        0        0     4376 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/download.py
+-rwxr-xr-x   0        0        0    13542 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/landmarks_info.py
+-rwxr-xr-x   0        0        0    10351 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/sign_data_attributes.py
+-rwxr-xr-x   0        0        0     2822 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/tree.py
+-rw-r--r--   0        0        0      535 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/__init__.py
+-rwxr-xr-x   0        0        0    18024 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/concatenate.py
+-rwxr-xr-x   0        0        0     7980 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/embed.py
+-rwxr-xr-x   0        0        0    33628 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/transforms.py
+-rwxr-xr-x   0        0        0    30236 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/visualization.py
+-rw-r--r--   0        0        0    16076 1970-01-01 00:00:00.000000 sign_language_translator-0.5.0/PKG-INFO
```

### Comparing `sign_language_translator-0.4.2/README.md` & `sign_language_translator-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,108 @@
 # Sign Language Translator ⠎⠇⠞
 
 [![python](https://img.shields.io/pypi/pyversions/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
 [![PyPi](https://img.shields.io/pypi/v/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
-[![Downloads](https://pepy.tech/badge/sign-language-translator)](https://pepy.tech/project/sign-language-translator)
+[![Downloads](https://static.pepy.tech/personalized-badge/sign-language-translator?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/sign-language-translator)
 
 1. [Overview](#overview)
    1. [Solution](#solution)
    2. [Major Components and Goals](#major-components-and-goals)
-   3. [Datasets](#datasets)
 2. [How to install the package](#how-to-install-the-package)
 3. [Usage](#usage)
-   1. [basic translation](#basic-translation)
-   2. [text language processor](#text-language-processor)
-   3. [sign language processor](#sign-language-processor)
-   4. [language models](#language-models)
+   1. [Command Line](#command-line)
+      <!-- 1. [configure](#configure) -->
+      1. [download](#download)
+      2. [translate](#translate)
+   2. [Python](#python)
+      1. [basic translation](#basic-translation)
+      2. [text language processor](#text-language-processor)
+      3. [sign language processor](#sign-language-processor)
+      4. [language models](#language-models)
 4. [Directory Tree](#directory-tree)
 5. [Research Paper](#research-paper)
 6. [Credits and Gratitude](#credits-and-gratitude)
 7. [Bonus](#bonus)
    1. number of lines of code
    2. just for fun
    3. publish package on PyPI
 
 ## Overview
 
 Sign language consists of gestures and expressions used mainly by the hearing-impaired to talk. This project is an effort to bridge the communication gap between the hearing and the hearing-impaired community using Artificial Intelligence.
 
-The goal is to provide a user friendly API to novel Sign Language Translation solutions that can easily adapt to any regional sign language. This is the package that powers the [slt_ai website](https://github.com/mdsrqbl/slt_ai).
+The goal is to provide a user friendly API to novel Sign Language Translation solutions that can easily adapt to any regional sign language. Unlike most other projects, this python library can translate full sentences and not just the alphabet. This is the package that powers the [slt_ai website](https://github.com/mdsrqbl/slt_ai).
 
-A bigger hurdle is the lack of datasets and frameworks that deep learning engineers and software developers can use to build useful products for the target community. That is what this project aims to deliver.
+A bigger hurdle is the lack of datasets and frameworks that deep learning engineers and software developers can use to build useful products for the target community. This project aims to empower sign language translation by providing robust components, tools and models for both sign language to text and text to sign language conversion. It seeks to advance the development of sign language translators for various regions while providing a way to sign language standardization.
 
 ### Solution
 
-We've have built an *extensible rule-based* text-to-sign translation system that can be used to *train Deep Learning* models.
+We've have built an *extensible rule-based* text-to-sign translation system that can be used to *train Deep Learning* models for both sign to text & text to sign translation.
 
-Just inherit the TextLanguage and SignLanguage classes to build a rule-based translation system for your regional language. Later you can use that system to fine-tune our AI models.
+To create a rule-based translation system for your regional language, you can inherit the TextLanguage and SignLanguage classes and pass them as arguments to the ConcatenativeSynthesis class. Later you can use that system to fine-tune our AI models.
 
 ### Major Components and Goals
 
 1. `Sign language to Text`
 
-    - Features such as pose vectors (2D or 3D) are extracted from video, and to be mapped to text corresponding to the performed signs, they are fed into a neural network which could be a checkpoint of a SOTA speech-to-text model fine-tuned using gradual unfreezing starting from the layers near input towards the output layers.
+    - Extract pose vectors (2D or 3D) from videos and map them to corresponding text representations of the performed signs.
+    - Fine-tuned a neural network, such as a state-of-the-art speech-to-text model, with gradual unfreezing starting from the input layers to convert pose vectors to text.
 
 2. `Text to Sign Language`
-    - This is a relatively easier task as it can even be solved with HashTables. Just parse the input text and play appropriate video clip for each word.
+    - This is a relatively easier task if you parse input text and play appropriate video clips for each word.
 
     1. Motion Transfer
-        - The idea is to concatenate pose vectors in the time dimension and transfer the movements onto any given image of any person. This allows for seamless transitions between the clips.
+         - Concatenate pose vectors in the time dimension and transfer the movements onto any given image of a person. This ensures smooth transitions between video clips.
     2. Sign Feature Synthesis
-        - This is similar to speech synthesis. It solves the challenge of unknown synonyms or hard to tokenize/process words/phrases.
-        - It can be achieved by conditioning a pose sequence generating model on a pre-trained text encoder (e.g finetune the decoder of a multilingual T5 to output pose vectors instead of text tokens).
+         - Condition a pose sequence generation model on a pre-trained text encoder (e.g., fine-tuned decoder of a multilingual T5) to output pose vectors instead of text tokens. This solves challenges related to unknown synonyms or hard-to-tokenize/process words or phrases.
 
-1. `Preprocessing Utilities`
+3. `Preprocessing Utilities`
     1. Pose Extraction
-        - Mediapipe 3D world coordinates and 2D image coordinates
-        - Pose Visualization
+        - Mediapipe 3D world coordinates
+        - Pose Visualization to aid in analysis and understanding.
     2. Text normalization
-        - Since the supported vocabulary is handcrafted, unknown words (or spellings) must be substituted with the supported words and ambiguous words must be disambiguated.
+        - Normalize text input by substituting unknown characters/spellings with supported words.
+        - Disambiguate ambiguous words to ensure accurate translation.
 
-2. `Data Collection and Creation`
-    Sign languages are very diverse and every small region will require their own translator. So, the product needed first is the one that can help build sign language translators. This project is designed with the capacity to handle all the variations and even lead to sign standardization.
+4. `Data Collection and Creation`
+    - Capture variations in signs in a scalable and diversity accommodating way and enable advancing sign language standardization efforts.
 
-   1. Clip extraction from long videos
-   2. Multithreaded Web scraping
-   3. Language Models to write sentences of supported words
+      1. Clip extraction from long videos using timestamps
+      2. Multithreaded Web scraping
+      3. Language Models to generate sentences composed of supported word
 
-### Datasets
+5. `Datasets`
 
-The sign videos are categorized by:
+    The sign videos are categorized by:
 
-1. country
-2. source organization
-3. session number
-4. camera angle
-5. person code ((d: deaf | h: hearing)(m: male | f: female)000001)
-6. equivalent text language word
+    ```text
+    1. country
+    2. source organization
+    3. session number
+    4. camera angle
+    5. person code ((d: deaf | h: hearing)(m: male | f: female)000001)
+    6. equivalent text language word
+    ```
 
-The files are labeled as follows:
-`country_organization_sessionNumber_cameraAngle_personCode_word.extension`
+    The files are labeled as follows:
 
-The text data includes:
+    ```text
+    country_organization_sessionNumber_cameraAngle_personCode_word.extension
+    ```
 
-1. word/sentence mappings to videos
-2. spoken language sentences and phrases
-3. spoken language sentences & corresponding sign video label sequences
-4. preprocessing data such as word-to-numbers, misspellings, named-entities etc
+    The text data includes:
 
-[See the *sign-language-datasets* repo and its *release files* for the actual data & details](https://github.com/sign-language-translator/sign-language-datasets)
+    ```text
+    1. word/sentence mappings to videos
+    2. spoken language sentences and phrases
+    3. spoken language sentences & corresponding sign video label sequences
+    4. preprocessing data such as word-to-numbers, misspellings, named-entities etc
+    ```
+
+    [See the *sign-language-datasets* repo and its *release files* for the actual data & details](https://github.com/sign-language-translator/sign-language-datasets)
 
 ## How to install the package
 
 Production mode:
 
 ```bash
 pip install sign-language-translator
@@ -101,22 +113,61 @@
 ```bash
 git clone https://github.com/sign-language-translator/sign-language-translator.git
 cd sign-language-translator
 pip install -e .
 ```
 
 ```bash
-pip install -e git+https://github.com/sign-language-translator/sign-language-translator.git
+pip install -e git+https://github.com/sign-language-translator/sign-language-translator.git#egg=sign_language_translator
 ```
 
 ## Usage
 
 see the *test cases* or [the *notebooks* repo](https://github.com/sign-language-translator/notebooks) for detailed use
 
-###### basic translation
+### Command Line
+
+<!-- #### configure
+
+(Optional) Set the dataset directory.
+
+```bash
+slt configure --dataset-dir "/path/to/sign-language-datasets"
+``` -->
+
+#### Download
+
+Download dataset files or models. The parameters are regular expressions.
+
+```bash
+slt download --overwrite true '.*\.json' '.*\.txt'
+```
+
+```bash
+slt download --progress-bar true 't2s_model_base.pth'
+```
+
+(By default, the dataset is downloaded into `/install-directory/sign_language_translator/sign-language-datasets/`)
+
+#### Translate
+
+Translate text to sign language using a rule-based model
+
+```bash
+slt translate \
+--model-code "concatenative" \
+--text-lang urdu --sign-lang psl \
+--sign-features 'mp-landmarks' \
+"وہ سکول گیا تھا۔" \
+'مجھے COVID نہیں ہے!'
+```
+
+### Python
+
+#### basic translation
 
 ```python
 import sign_language_translator as slt
 
 # download dataset (by default, dataset is downloaded within the install directory)
 # slt.set_dataset_dir("path/to/sign-language-datasets") # optional
 # slt.download("id")
@@ -206,24 +257,30 @@
 
 ```
 
 ## Directory Tree
 
 ```text
 sign-language-translator
+├── MANIFEST.in
 ├── README.md
+├── poetry.lock
 ├── pyproject.toml
 ├── requirements.txt
 ├── roadmap.md
 ├── tests
+│   └── *
+│
 └── sign_language_translator
+    ├── cli.py
     ├── config
     │   ├── enums.py
     │   ├── helpers.py
-    │   └── settings.py
+    │   ├── settings.py
+    │   └── urls.yaml
     │
     ├── data_collection
     │   ├── completeness.py
     │   ├── scraping.py
     │   └── synonyms.py
     │
     ├── languages
@@ -249,24 +306,28 @@
     │   │   └── transformer_language_model.py
     │   │
     │   ├── sign_to_text
     │   └── text_to_sign
     │       ├── concatenative_synthesis.py
     │       └── t2s_model.py
     │
+    ├── sign-language-datasets
+    │   └── *
+    │
     ├── text
     │   ├── metrics.py
     │   ├── preprocess.py
     │   ├── subtitles.py
     │   ├── tagger.py
     │   ├── tokenizer.py
     │   └── utils.py
     │
     ├── utils
     │   ├── data_loader.py
+    │   ├── download.py
     │   ├── landmarks_info.py
     │   ├── sign_data_attributes.py
     │   └── tree.py
     │
     └── vision
         ├── concatenate.py
         ├── embed.py
@@ -291,15 +352,15 @@
 - [Hamza Foundation](https://www.youtube.com/@pslhamzafoundationacademyf7624/videos) (especially Ms Benish, Ms Rashda & Mr Zeeshan) for agreeing for collaboration and providing the reference clips, hearing-impaired performers for data creation, and creating the text2gloss dataset.
 - [UrduHack](https://github.com/urduhack/urduhack) (espacially Ikram Ali) for their work on Urdu character normalization.
 
 - [Telha Bilal](https://github.com/TelhaBilal) for help in designing the architecture of some modules.
 
 ## Bonus
 
-Count total number of **lines of code** (Package: **6595** + Tests: **781**):
+Count total number of **lines of code** (Package: **7064** + Tests: **774**):
 
 ```bash
 git ls-files | grep '\.py' | xargs wc -l
 ```
 
 **Just for fun**
```

### Comparing `sign_language_translator-0.4.2/pyproject.toml` & `sign_language_translator-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sign_language_translator"
-version = "0.4.2"
+version = "0.5.0"
 description = "Translate between spoken/text and sign language using AI."
 authors = ["Mudassar Iqbal <mdsriqb@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "sign_language_translator"}]
 repository = "https://github.com/sign-language-translator/sign-language-translator"
 keywords = ["sign", "translation", "pose", "pakistan", "deep-learning", "computer-vision", "nlp", "sign-language", "sign-language-translation"]
@@ -21,20 +21,25 @@
 scipy = "^1.11.1"
 torch = "^2.0.1"
 scikit-image = "^0.21.0"
 beautifulsoup4 = "^4.12.2"
 deep-translator = "^1.11.4"
 opencv-contrib-python = "^4.8.0.74"
 tqdm = "^4.65.0"
+pyyaml = "^6.0"
+click = "^8.1.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-vv "
 filterwarnings = [
     "ignore::DeprecationWarning",
 ]
 
 [tool.isort]
-profile = "black"
+profile = "black"
+
+[tool.poetry.scripts]
+slt = "sign_language_translator.cli:slt"
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/__init__.py` & `sign_language_translator-0.5.0/sign_language_translator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,21 @@
     languages,
     models,
     text,
     utils,
     vision,
 )
 from sign_language_translator.config import enums
-from sign_language_translator.config.settings import Settings
-from sign_language_translator.config.helpers import set_dataset_dir
+from sign_language_translator.config.settings import Settings, set_dataset_dir
 from sign_language_translator.languages import get_sign_language, get_text_language
 from sign_language_translator.models import get_model
 
+
+__version__ = config.helpers.get_package_version()
+
 __all__ = [
     "set_dataset_dir",
     "Settings",
     "vision",
     "text",
     "data_collection",
     "models",
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/data_collection/completeness.py` & `sign_language_translator-0.5.0/sign_language_translator/data_collection/completeness.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/data_collection/scraping.py` & `sign_language_translator-0.5.0/sign_language_translator/data_collection/scraping.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/data_collection/synonyms.py` & `sign_language_translator-0.5.0/sign_language_translator/data_collection/synonyms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/sign/__init__.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/sign/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/sign/mapping_rules.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/sign/mapping_rules.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/sign/pakistan_sign_language.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/sign/pakistan_sign_language.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,21 @@
             if rule.is_applicable(token, tag, context):
                 if rule.priority < priority or (
                     rule.priority == priority and random.random() < 0.5
                 ):
                     sign = rule.apply(token)
                     priority = rule.priority
 
+        if sign is None and tag == Tags.AMBIGUOUS:
+            raise ValueError(
+                f"Token '{token}' is ambiguous."
+                + f"Try from {self.vocab.ambiguous_to_unambiguous.get(token,[])}."
+            )
         if sign is None:
-            raise ValueError(f"No PakistanSL sign could be inferred for {token = }")
+            raise ValueError(f"No PakistanSL sign could be inferred for {token = }.")
 
         return sign
 
     def restructure_sentence(
         self,
         sentence: Iterable[str],
         tags: Iterable[Any] | None = None,
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/sign/sign_language.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/sign/sign_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/text/text_language.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/text/text_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/text/urdu.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/text/urdu.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             if (("double-handed-letter)" in wc) and (not w.isascii()))
             or (len(w) == 1 and w.isalpha())
         }
 
         self.tokenizer = SignTokenizer(
             word_regex=self.word_regex(),
             compound_words=(
-                self.vocab.supported_words
+                self.vocab.supported_words # TODO why does this variable exist?
                 | self.vocab.supported_words_with_word_sense
                 | {
                     w
                     for word in self.vocab.words_to_numbers.keys()
                     for w in [word, word.replace("-", " ")]
                 }
             ),  # TODO: | one-hundred twenty-three (\d[ \d]*): ["100", "23"] --> ["123"]
@@ -100,14 +100,20 @@
                 lambda token: (
                     bool(re.match(r"^\d+(?:\.\d+)?$", token))
                     or token in self.vocab.words_to_numbers
                 ),
                 Tags.NUMBER,
                 4,
             ),
+            # e.g. "میں" -> ["میں(i)", "میں(in)"]
+            Rule(
+                lambda token: token in self.vocab.ambiguous_to_unambiguous,
+                Tags.AMBIGUOUS,
+                2,
+            ),
         ]
         self.tagger = Tagger(
             rules=self.tagging_rules,
             default=Tags.DEFAULT,
         )
 
     def preprocess(self, text: str) -> str:
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/languages/vocab.py` & `sign_language_translator-0.5.0/sign_language_translator/languages/vocab.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import json
 import os
 import re
 from typing import Any, Dict, Iterable, List, Set
 
 from sign_language_translator.config.settings import Settings
+from sign_language_translator.utils import download_resource
 
 
 class Vocab:
     """loads data from files for a specific language and specified sign_collections"""
 
     def __init__(
         self,
@@ -115,38 +116,41 @@
             print(without_word_sense)  # Output: "this is a spring. those are glasses."
         """
 
         without_word_sense = re.sub(self.word_sense_regex, "", text)
         return without_word_sense
 
     def __load_label_to_words(self):
+        self._download_resource(self.label_to_words_path)
         with open(
             self.label_to_words_path,
             "r",
             encoding="utf-8",
         ) as file_pointer:
             collection_to_label_to_language_to_words: Dict[
                 str, Dict[str, Dict[str, List[str]]]
             ] = json.load(file_pointer)
 
         return collection_to_label_to_language_to_words
 
     def __load_constructable_words(self):
+        self._download_resource(self.constructed_words_path)
         with open(
             self.constructed_words_path,
             "r",
             encoding="utf-8",
         ) as file_pointer:
             organization_to_language_to_constructable_words: Dict[
                 str, List[Dict[str, List[str]]]
             ] = json.load(file_pointer)
 
         return organization_to_language_to_constructable_words
 
     def __load_preprocessing(self, language: str, regex: bool = True) -> Dict[str, Any]:
+        self._download_resource(self.preprocessing_path)
         with open(
             self.preprocessing_path,
             "r",
             encoding="utf-8",
         ) as file_pointer:
             raw_data: Dict[str, Dict[str, Any]] = json.load(file_pointer)
 
@@ -156,14 +160,15 @@
             for lang in lang_to_data
             if self.__check_text_in_list(lang, [language], regex=regex)
         }
 
         return preprocessing_map
 
     def __load_token_to_id(self, language: str, regex: bool = True) -> Dict[str, int]:
+        self._download_resource(self.token_to_id_path)
         with open(
             self.token_to_id_path,
             "r",
             encoding="utf-8",
         ) as file_pointer:
             raw_data: Dict[str, Dict[str, int]] = json.load(file_pointer)
 
@@ -295,13 +300,23 @@
             if without_word_sense != word:
                 if without_word_sense not in ambiguous_2_unambiguous:
                     ambiguous_2_unambiguous[without_word_sense] = []
                 ambiguous_2_unambiguous[without_word_sense].append(word)
 
         return ambiguous_2_unambiguous
 
+    def _download_resource(self, full_path: str):
+        if not Settings.AUTO_DOWNLOAD:
+            return
+        if os.path.exists(full_path):
+            return
+        if full_path.startswith(Settings.DATASET_ROOT_DIRECTORY):
+            filename = full_path[len(Settings.DATASET_ROOT_DIRECTORY) :]
+            filename = re.escape(filename.strip(os.path.sep))
+            download_resource(filename, overwrite=False)
+
     # load sign video/features
 
 
 __all__ = [
     "Vocab",
 ]
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/__init__.py` & `sign_language_translator-0.5.0/sign_language_translator/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from sign_language_translator.models import language_models, sign_to_text, text_to_sign
-from sign_language_translator.models.text_to_sign import ConcatenativeSynthesis
-from sign_language_translator.models.utils import get_model
-
 from sign_language_translator.models.language_models import (
-    SimpleLanguageModel,
     BeamSampling,
-    Mixer,
     LanguageModel,
+    Mixer,
+    SimpleLanguageModel,
 )
-
+from sign_language_translator.models.text_to_sign import ConcatenativeSynthesis
+from sign_language_translator.models.utils import get_model
 
 __all__ = [
     "get_model",
     "language_models",
     "sign_to_text",
     "text_to_sign",
     "ConcatenativeSynthesis",
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/language_models/abstract_language_model.py` & `sign_language_translator-0.5.0/sign_language_translator/models/language_models/abstract_language_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/language_models/beam_sampling.py` & `sign_language_translator-0.5.0/sign_language_translator/models/language_models/beam_sampling.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/language_models/mixer.py` & `sign_language_translator-0.5.0/sign_language_translator/models/language_models/mixer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/language_models/simple_language_model.py` & `sign_language_translator-0.5.0/sign_language_translator/models/language_models/simple_language_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/concatenative_synthesis.py` & `sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/t2s_model.py` & `sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/t2s_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/text/metrics.py` & `sign_language_translator-0.5.0/sign_language_translator/text/metrics.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/text/preprocess.py` & `sign_language_translator-0.5.0/sign_language_translator/text/preprocess.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/text/subtitles.py` & `sign_language_translator-0.5.0/sign_language_translator/text/subtitles.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/text/tagger.py` & `sign_language_translator-0.5.0/sign_language_translator/text/tagger.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     NUMBER = "NUMBER"
     ACRONYM = "ACRONYM"
     PUNCTUATION = "PUNCTUATION"
     SUPPORTED_WORD = "SUPPORTED_WORD"
     DEFAULT = ""
     END_OF_SEQUENCE = "EOS"
     START_OF_SEQUENCE = "SOS"
+    AMBIGUOUS = "AMBIGUOUS"
+    WORDLESS = "WORDLESS"
     # WORD_SENSE = "(anything)"
     # PERSON = {
     #     'id': 'PERSON',
     #     'name': 'Person',
     #     'description': 'Represents a person',
     #     'example': 'John Doe',
     # }
```

### Comparing `sign_language_translator-0.4.2/sign_language_translator/text/tokenizer.py` & `sign_language_translator-0.5.0/sign_language_translator/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/text/utils.py` & `sign_language_translator-0.5.0/sign_language_translator/text/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/utils/data_loader.py` & `sign_language_translator-0.5.0/sign_language_translator/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/utils/landmarks_info.py` & `sign_language_translator-0.5.0/sign_language_translator/utils/landmarks_info.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/utils/sign_data_attributes.py` & `sign_language_translator-0.5.0/sign_language_translator/utils/sign_data_attributes.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/utils/tree.py` & `sign_language_translator-0.5.0/sign_language_translator/utils/tree.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/vision/concatenate.py` & `sign_language_translator-0.5.0/sign_language_translator/vision/concatenate.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/vision/embed.py` & `sign_language_translator-0.5.0/sign_language_translator/vision/embed.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/vision/transforms.py` & `sign_language_translator-0.5.0/sign_language_translator/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/sign_language_translator/vision/visualization.py` & `sign_language_translator-0.5.0/sign_language_translator/vision/visualization.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.2/PKG-INFO` & `sign_language_translator-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,142 @@
 Metadata-Version: 2.1
 Name: sign-language-translator
-Version: 0.4.2
+Version: 0.5.0
 Summary: Translate between spoken/text and sign language using AI.
 Home-page: https://github.com/sign-language-translator/sign-language-translator
 License: Apache-2.0
 Keywords: sign,translation,pose,pakistan,deep-learning,computer-vision,nlp,sign-language,sign-language-translation
 Author: Mudassar Iqbal
 Author-email: mdsriqb@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: deep-translator (>=1.11.4,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: mediapipe (==0.9.1.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: opencv-contrib-python (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/sign-language-translator/sign-language-translator
 Description-Content-Type: text/markdown
 
 # Sign Language Translator ⠎⠇⠞
 
 [![python](https://img.shields.io/pypi/pyversions/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
 [![PyPi](https://img.shields.io/pypi/v/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
-[![Downloads](https://pepy.tech/badge/sign-language-translator)](https://pepy.tech/project/sign-language-translator)
+[![Downloads](https://static.pepy.tech/personalized-badge/sign-language-translator?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/sign-language-translator)
 
 1. [Overview](#overview)
    1. [Solution](#solution)
    2. [Major Components and Goals](#major-components-and-goals)
-   3. [Datasets](#datasets)
 2. [How to install the package](#how-to-install-the-package)
 3. [Usage](#usage)
-   1. [basic translation](#basic-translation)
-   2. [text language processor](#text-language-processor)
-   3. [sign language processor](#sign-language-processor)
-   4. [language models](#language-models)
+   1. [Command Line](#command-line)
+      <!-- 1. [configure](#configure) -->
+      1. [download](#download)
+      2. [translate](#translate)
+   2. [Python](#python)
+      1. [basic translation](#basic-translation)
+      2. [text language processor](#text-language-processor)
+      3. [sign language processor](#sign-language-processor)
+      4. [language models](#language-models)
 4. [Directory Tree](#directory-tree)
 5. [Research Paper](#research-paper)
 6. [Credits and Gratitude](#credits-and-gratitude)
 7. [Bonus](#bonus)
    1. number of lines of code
    2. just for fun
    3. publish package on PyPI
 
 ## Overview
 
 Sign language consists of gestures and expressions used mainly by the hearing-impaired to talk. This project is an effort to bridge the communication gap between the hearing and the hearing-impaired community using Artificial Intelligence.
 
-The goal is to provide a user friendly API to novel Sign Language Translation solutions that can easily adapt to any regional sign language. This is the package that powers the [slt_ai website](https://github.com/mdsrqbl/slt_ai).
+The goal is to provide a user friendly API to novel Sign Language Translation solutions that can easily adapt to any regional sign language. Unlike most other projects, this python library can translate full sentences and not just the alphabet. This is the package that powers the [slt_ai website](https://github.com/mdsrqbl/slt_ai).
 
-A bigger hurdle is the lack of datasets and frameworks that deep learning engineers and software developers can use to build useful products for the target community. That is what this project aims to deliver.
+A bigger hurdle is the lack of datasets and frameworks that deep learning engineers and software developers can use to build useful products for the target community. This project aims to empower sign language translation by providing robust components, tools and models for both sign language to text and text to sign language conversion. It seeks to advance the development of sign language translators for various regions while providing a way to sign language standardization.
 
 ### Solution
 
-We've have built an *extensible rule-based* text-to-sign translation system that can be used to *train Deep Learning* models.
+We've have built an *extensible rule-based* text-to-sign translation system that can be used to *train Deep Learning* models for both sign to text & text to sign translation.
 
-Just inherit the TextLanguage and SignLanguage classes to build a rule-based translation system for your regional language. Later you can use that system to fine-tune our AI models.
+To create a rule-based translation system for your regional language, you can inherit the TextLanguage and SignLanguage classes and pass them as arguments to the ConcatenativeSynthesis class. Later you can use that system to fine-tune our AI models.
 
 ### Major Components and Goals
 
 1. `Sign language to Text`
 
-    - Features such as pose vectors (2D or 3D) are extracted from video, and to be mapped to text corresponding to the performed signs, they are fed into a neural network which could be a checkpoint of a SOTA speech-to-text model fine-tuned using gradual unfreezing starting from the layers near input towards the output layers.
+    - Extract pose vectors (2D or 3D) from videos and map them to corresponding text representations of the performed signs.
+    - Fine-tuned a neural network, such as a state-of-the-art speech-to-text model, with gradual unfreezing starting from the input layers to convert pose vectors to text.
 
 2. `Text to Sign Language`
-    - This is a relatively easier task as it can even be solved with HashTables. Just parse the input text and play appropriate video clip for each word.
+    - This is a relatively easier task if you parse input text and play appropriate video clips for each word.
 
     1. Motion Transfer
-        - The idea is to concatenate pose vectors in the time dimension and transfer the movements onto any given image of any person. This allows for seamless transitions between the clips.
+         - Concatenate pose vectors in the time dimension and transfer the movements onto any given image of a person. This ensures smooth transitions between video clips.
     2. Sign Feature Synthesis
-        - This is similar to speech synthesis. It solves the challenge of unknown synonyms or hard to tokenize/process words/phrases.
-        - It can be achieved by conditioning a pose sequence generating model on a pre-trained text encoder (e.g finetune the decoder of a multilingual T5 to output pose vectors instead of text tokens).
+         - Condition a pose sequence generation model on a pre-trained text encoder (e.g., fine-tuned decoder of a multilingual T5) to output pose vectors instead of text tokens. This solves challenges related to unknown synonyms or hard-to-tokenize/process words or phrases.
 
-1. `Preprocessing Utilities`
+3. `Preprocessing Utilities`
     1. Pose Extraction
-        - Mediapipe 3D world coordinates and 2D image coordinates
-        - Pose Visualization
+        - Mediapipe 3D world coordinates
+        - Pose Visualization to aid in analysis and understanding.
     2. Text normalization
-        - Since the supported vocabulary is handcrafted, unknown words (or spellings) must be substituted with the supported words and ambiguous words must be disambiguated.
+        - Normalize text input by substituting unknown characters/spellings with supported words.
+        - Disambiguate ambiguous words to ensure accurate translation.
 
-2. `Data Collection and Creation`
-    Sign languages are very diverse and every small region will require their own translator. So, the product needed first is the one that can help build sign language translators. This project is designed with the capacity to handle all the variations and even lead to sign standardization.
+4. `Data Collection and Creation`
+    - Capture variations in signs in a scalable and diversity accommodating way and enable advancing sign language standardization efforts.
 
-   1. Clip extraction from long videos
-   2. Multithreaded Web scraping
-   3. Language Models to write sentences of supported words
+      1. Clip extraction from long videos using timestamps
+      2. Multithreaded Web scraping
+      3. Language Models to generate sentences composed of supported word
 
-### Datasets
+5. `Datasets`
 
-The sign videos are categorized by:
+    The sign videos are categorized by:
 
-1. country
-2. source organization
-3. session number
-4. camera angle
-5. person code ((d: deaf | h: hearing)(m: male | f: female)000001)
-6. equivalent text language word
+    ```text
+    1. country
+    2. source organization
+    3. session number
+    4. camera angle
+    5. person code ((d: deaf | h: hearing)(m: male | f: female)000001)
+    6. equivalent text language word
+    ```
 
-The files are labeled as follows:
-`country_organization_sessionNumber_cameraAngle_personCode_word.extension`
+    The files are labeled as follows:
 
-The text data includes:
+    ```text
+    country_organization_sessionNumber_cameraAngle_personCode_word.extension
+    ```
 
-1. word/sentence mappings to videos
-2. spoken language sentences and phrases
-3. spoken language sentences & corresponding sign video label sequences
-4. preprocessing data such as word-to-numbers, misspellings, named-entities etc
+    The text data includes:
 
-[See the *sign-language-datasets* repo and its *release files* for the actual data & details](https://github.com/sign-language-translator/sign-language-datasets)
+    ```text
+    1. word/sentence mappings to videos
+    2. spoken language sentences and phrases
+    3. spoken language sentences & corresponding sign video label sequences
+    4. preprocessing data such as word-to-numbers, misspellings, named-entities etc
+    ```
+
+    [See the *sign-language-datasets* repo and its *release files* for the actual data & details](https://github.com/sign-language-translator/sign-language-datasets)
 
 ## How to install the package
 
 Production mode:
 
 ```bash
 pip install sign-language-translator
@@ -133,22 +147,61 @@
 ```bash
 git clone https://github.com/sign-language-translator/sign-language-translator.git
 cd sign-language-translator
 pip install -e .
 ```
 
 ```bash
-pip install -e git+https://github.com/sign-language-translator/sign-language-translator.git
+pip install -e git+https://github.com/sign-language-translator/sign-language-translator.git#egg=sign_language_translator
 ```
 
 ## Usage
 
 see the *test cases* or [the *notebooks* repo](https://github.com/sign-language-translator/notebooks) for detailed use
 
-###### basic translation
+### Command Line
+
+<!-- #### configure
+
+(Optional) Set the dataset directory.
+
+```bash
+slt configure --dataset-dir "/path/to/sign-language-datasets"
+``` -->
+
+#### Download
+
+Download dataset files or models. The parameters are regular expressions.
+
+```bash
+slt download --overwrite true '.*\.json' '.*\.txt'
+```
+
+```bash
+slt download --progress-bar true 't2s_model_base.pth'
+```
+
+(By default, the dataset is downloaded into `/install-directory/sign_language_translator/sign-language-datasets/`)
+
+#### Translate
+
+Translate text to sign language using a rule-based model
+
+```bash
+slt translate \
+--model-code "concatenative" \
+--text-lang urdu --sign-lang psl \
+--sign-features 'mp-landmarks' \
+"وہ سکول گیا تھا۔" \
+'مجھے COVID نہیں ہے!'
+```
+
+### Python
+
+#### basic translation
 
 ```python
 import sign_language_translator as slt
 
 # download dataset (by default, dataset is downloaded within the install directory)
 # slt.set_dataset_dir("path/to/sign-language-datasets") # optional
 # slt.download("id")
@@ -238,24 +291,30 @@
 
 ```
 
 ## Directory Tree
 
 ```text
 sign-language-translator
+├── MANIFEST.in
 ├── README.md
+├── poetry.lock
 ├── pyproject.toml
 ├── requirements.txt
 ├── roadmap.md
 ├── tests
+│   └── *
+│
 └── sign_language_translator
+    ├── cli.py
     ├── config
     │   ├── enums.py
     │   ├── helpers.py
-    │   └── settings.py
+    │   ├── settings.py
+    │   └── urls.yaml
     │
     ├── data_collection
     │   ├── completeness.py
     │   ├── scraping.py
     │   └── synonyms.py
     │
     ├── languages
@@ -281,24 +340,28 @@
     │   │   └── transformer_language_model.py
     │   │
     │   ├── sign_to_text
     │   └── text_to_sign
     │       ├── concatenative_synthesis.py
     │       └── t2s_model.py
     │
+    ├── sign-language-datasets
+    │   └── *
+    │
     ├── text
     │   ├── metrics.py
     │   ├── preprocess.py
     │   ├── subtitles.py
     │   ├── tagger.py
     │   ├── tokenizer.py
     │   └── utils.py
     │
     ├── utils
     │   ├── data_loader.py
+    │   ├── download.py
     │   ├── landmarks_info.py
     │   ├── sign_data_attributes.py
     │   └── tree.py
     │
     └── vision
         ├── concatenate.py
         ├── embed.py
@@ -323,15 +386,15 @@
 - [Hamza Foundation](https://www.youtube.com/@pslhamzafoundationacademyf7624/videos) (especially Ms Benish, Ms Rashda & Mr Zeeshan) for agreeing for collaboration and providing the reference clips, hearing-impaired performers for data creation, and creating the text2gloss dataset.
 - [UrduHack](https://github.com/urduhack/urduhack) (espacially Ikram Ali) for their work on Urdu character normalization.
 
 - [Telha Bilal](https://github.com/TelhaBilal) for help in designing the architecture of some modules.
 
 ## Bonus
 
-Count total number of **lines of code** (Package: **6595** + Tests: **781**):
+Count total number of **lines of code** (Package: **7064** + Tests: **774**):
 
 ```bash
 git ls-files | grep '\.py' | xargs wc -l
 ```
 
 **Just for fun**
```

