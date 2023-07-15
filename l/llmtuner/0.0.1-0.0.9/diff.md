# Comparing `tmp/llmtuner-0.0.1.tar.gz` & `tmp/llmtuner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.0.1.tar", last modified: Fri Jul 14 20:01:34 2023, max compression
+gzip compressed data, was "llmtuner-0.0.9.tar", last modified: Sat Jul 15 09:18:28 2023, max compression
```

## Comparing `llmtuner-0.0.1.tar` & `llmtuner-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,68 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.475078 llmtuner-0.0.1/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-14 20:01:16.000000 llmtuner-0.0.1/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13436 2023-07-14 20:01:34.475078 llmtuner-0.0.1/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12787 2023-07-14 20:01:21.000000 llmtuner-0.0.1/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-14 20:01:21.000000 llmtuner-0.0.1/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-14 20:01:34.475078 llmtuner-0.0.1/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-14 20:01:22.000000 llmtuner-0.0.1/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.199077 llmtuner-0.0.1/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.207077 llmtuner-0.0.1/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      121 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.219077 llmtuner-0.0.1/src/llmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      105 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2565 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/dsets/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8194 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/dsets/preprocess.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.283077 llmtuner-0.0.1/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2628 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      211 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      443 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1716 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/save_and_load.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6433 2023-07-14 20:01:18.000000 llmtuner-0.0.1/src/llmtuner/extras/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.295077 llmtuner-0.0.1/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5012 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3738 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.307077 llmtuner-0.0.1/src/llmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      130 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.403077 llmtuner-0.0.1/src/llmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3812 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6925 2023-07-14 20:01:19.000000 llmtuner-0.0.1/src/llmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6386 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4055 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.431078 llmtuner-0.0.1/src/llmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2069 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3059 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-14 20:01:20.000000 llmtuner-0.0.1/src/llmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.211077 llmtuner-0.0.1/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13436 2023-07-14 20:01:34.000000 llmtuner-0.0.1/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1275 2023-07-14 20:01:34.000000 llmtuner-0.0.1/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-14 20:01:34.000000 llmtuner-0.0.1/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      206 2023-07-14 20:01:34.000000 llmtuner-0.0.1/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       15 2023-07-14 20:01:34.000000 llmtuner-0.0.1/src/llmtuner.egg-info/top_level.txt
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:34.447078 llmtuner-0.0.1/src/utils/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:21.000000 llmtuner-0.0.1/src/utils/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2207 2023-07-14 20:01:21.000000 llmtuner-0.0.1/src/utils/pairwise.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 20:01:21.000000 llmtuner-0.0.1/src/utils/peft_trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9662 2023-07-14 20:01:21.000000 llmtuner-0.0.1/src/utils/ppo.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.413016 llmtuner-0.0.9/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-15 09:06:30.000000 llmtuner-0.0.9/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13532 2023-07-15 09:18:28.413016 llmtuner-0.0.9/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    12888 2023-07-15 09:06:30.000000 llmtuner-0.0.9/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-15 09:06:30.000000 llmtuner-0.0.9/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-15 09:18:28.413016 llmtuner-0.0.9/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-15 09:06:30.000000 llmtuner-0.0.9/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.285015 llmtuner-0.0.9/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.309016 llmtuner-0.0.9/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      285 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.317016 llmtuner-0.0.9/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5783 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.341016 llmtuner-0.0.9/src/llmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      105 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2565 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8194 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/preprocess.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.349016 llmtuner-0.0.9/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3101 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      211 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      443 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1716 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/save_and_load.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6433 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/extras/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.353016 llmtuner-0.0.9/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5012 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3738 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.357016 llmtuner-0.0.9/src/llmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.393016 llmtuner-0.0.9/src/llmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6975 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6400 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.401016 llmtuner-0.0.9/src/llmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8765 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2926 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.401016 llmtuner-0.0.9/src/llmtuner/tuner/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2884 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.409016 llmtuner-0.0.9/src/llmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1482 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2741 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.409016 llmtuner-0.0.9/src/llmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 09:06:30.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2069 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3059 2023-07-15 09:06:30.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4264 2023-07-15 09:06:30.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.313016 llmtuner-0.0.9/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13532 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1641 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      206 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.0.1/LICENSE` & `llmtuner-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/PKG-INFO` & `llmtuner-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.0.1
+Version: 0.0.9
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -115,15 +115,15 @@
 ```
 
 ## Requirement
 
 - Python 3.8+ and PyTorch 1.13.1+
 - 🤗Transformers, Datasets, Accelerate, PEFT and TRL
 - jieba, rouge-chinese and nltk (used at evaluation)
-- gradio and mdtex2html (used in web_demo.py)
+- gradio and matplotlib (used in web_demo.py)
 - uvicorn, fastapi and sse-starlette (used in api_demo.py)
 
 And **powerful GPUs**!
 
 If you want to enable quantized LoRA (QLoRA) on the Windows platform, you should install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
 
 ```bash
@@ -157,15 +157,16 @@
 python -m transformers.models.llama.convert_llama_weights_to_hf \
     --input_dir path_to_llama_weights --model_size 7B --output_dir path_to_llama_model
 ```
 
 ### (Continually) Pre-Training
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_pt.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage pt \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset wiki_demo \
     --finetuning_type lora \
     --output_dir path_to_pt_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
@@ -178,15 +179,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### Supervised Fine-Tuning
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_sft.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage sft \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
@@ -199,15 +201,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### Reward Model Training
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_rm.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage rm \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset comparison_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
@@ -219,15 +222,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### PPO Training (RLHF)
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_ppo.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage ppo \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
@@ -242,15 +246,15 @@
     --plot_loss
 ```
 
 ### Distributed Training
 
 ```bash
 accelerate config # configure the environment
-accelerate launch src/train_XX.py # arguments (same as above)
+accelerate launch src/train_bash.py # arguments (same as above)
 ```
 
 <details><summary>Example configuration for full-tuning with DeepSpeed ZeRO-2</summary>
 
 ```yaml
 compute_environment: LOCAL_MACHINE
 deepspeed_config:
@@ -276,15 +280,16 @@
 ```
 
 </details>
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_sft.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage pt \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
```

### Comparing `llmtuner-0.0.1/README.md` & `llmtuner-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 ```
 
 ## Requirement
 
 - Python 3.8+ and PyTorch 1.13.1+
 - 🤗Transformers, Datasets, Accelerate, PEFT and TRL
 - jieba, rouge-chinese and nltk (used at evaluation)
-- gradio and mdtex2html (used in web_demo.py)
+- gradio and matplotlib (used in web_demo.py)
 - uvicorn, fastapi and sse-starlette (used in api_demo.py)
 
 And **powerful GPUs**!
 
 If you want to enable quantized LoRA (QLoRA) on the Windows platform, you should install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
 
 ```bash
@@ -133,15 +133,16 @@
 python -m transformers.models.llama.convert_llama_weights_to_hf \
     --input_dir path_to_llama_weights --model_size 7B --output_dir path_to_llama_model
 ```
 
 ### (Continually) Pre-Training
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_pt.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage pt \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset wiki_demo \
     --finetuning_type lora \
     --output_dir path_to_pt_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
@@ -154,15 +155,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### Supervised Fine-Tuning
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_sft.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage sft \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
@@ -175,15 +177,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### Reward Model Training
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_rm.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage rm \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset comparison_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
@@ -195,15 +198,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### PPO Training (RLHF)
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_ppo.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage ppo \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
@@ -218,15 +222,15 @@
     --plot_loss
 ```
 
 ### Distributed Training
 
 ```bash
 accelerate config # configure the environment
-accelerate launch src/train_XX.py # arguments (same as above)
+accelerate launch src/train_bash.py # arguments (same as above)
 ```
 
 <details><summary>Example configuration for full-tuning with DeepSpeed ZeRO-2</summary>
 
 ```yaml
 compute_environment: LOCAL_MACHINE
 deepspeed_config:
@@ -252,15 +256,16 @@
 ```
 
 </details>
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_sft.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage pt \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
```

### Comparing `llmtuner-0.0.1/setup.py` & `llmtuner-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/dsets/callbacks.py` & `llmtuner-0.0.9/src/llmtuner/dsets/callbacks.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/dsets/loader.py` & `llmtuner-0.0.9/src/llmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/dsets/preprocess.py` & `llmtuner-0.0.9/src/llmtuner/dsets/preprocess.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/extras/callbacks.py` & `llmtuner-0.0.9/src/llmtuner/extras/callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,30 @@
 
 from transformers import (
     TrainerCallback,
     TrainerControl,
     TrainerState,
     TrainingArguments
 )
+from transformers.trainer_callback import TrainerControl, TrainerState
+from transformers.training_args import TrainingArguments
 
 
 class LogCallback(TrainerCallback):
 
     def __init__(self, runner=None):
         self.runner = runner
-        self.start_time = time.time()
         self.tracker = {}
 
+    def on_train_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the beginning of training.
+        """
+        self.start_time = time.time()
+
     def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
         r"""
         Event called at the beginning of a training step. If using gradient accumulation, one training step
         might take several inputs.
         """
         if self.runner is not None and self.runner.aborted:
             control.should_epoch_stop = True
@@ -35,26 +42,28 @@
             control.should_epoch_stop = True
             control.should_training_stop = True
 
     def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
         r"""
         Event called after logging the last logs.
         """
-        if "loss" not in state.log_history[-1]:
+        if "step" not in state.log_history[-1]:
             return
         cur_time = time.time()
         cur_steps = state.log_history[-1].get("step")
         elapsed_time = cur_time - self.start_time
         avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
         remaining_steps = state.max_steps - cur_steps
         remaining_time = remaining_steps * avg_time_per_step
         self.tracker = {
             "current_steps": cur_steps,
             "total_steps": state.max_steps,
             "loss": state.log_history[-1].get("loss", None),
+            "eval_loss": state.log_history[-1].get("eval_loss", None),
+            "predict_loss": state.log_history[-1].get("predict_loss", None),
             "reward": state.log_history[-1].get("reward", None),
             "learning_rate": state.log_history[-1].get("learning_rate", None),
             "epoch": state.log_history[-1].get("epoch", None),
             "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
             "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
             "remaining_time": str(timedelta(seconds=int(remaining_time)))
         }
```

### Comparing `llmtuner-0.0.1/src/llmtuner/extras/misc.py` & `llmtuner-0.0.9/src/llmtuner/extras/misc.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/extras/ploting.py` & `llmtuner-0.0.9/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/extras/save_and_load.py` & `llmtuner-0.0.9/src/llmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/extras/template.py` & `llmtuner-0.0.9/src/llmtuner/extras/template.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/hparams/data_args.py` & `llmtuner-0.0.9/src/llmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.0.9/src/llmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.0.9/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/hparams/model_args.py` & `llmtuner-0.0.9/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/core/adapter.py` & `llmtuner-0.0.9/src/llmtuner/tuner/core/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     PeftModel,
     TaskType,
     LoraConfig,
     get_peft_model
 )
 from peft.utils import CONFIG_NAME, WEIGHTS_NAME
 
-from extras.logging import get_logger
-from extras.save_and_load import load_trainable_params
-from hparams import ModelArguments, FinetuningArguments
+from llmtuner.extras.logging import get_logger
+from llmtuner.extras.save_and_load import load_trainable_params
+from llmtuner.hparams import ModelArguments, FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 def init_adapter(
     model: PreTrainedModel,
```

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/core/loader.py` & `llmtuner-0.0.9/src/llmtuner/tuner/core/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import os
 import torch
 from typing import Literal, Optional, Tuple
 
 from transformers import (
     AutoConfig,
-    AutoModel,
+    AutoModelForCausalLM,
     AutoTokenizer,
     BitsAndBytesConfig
 )
 from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 from transformers.modeling_utils import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
 from trl import AutoModelForCausalLMWithValueHead
 
-from extras.logging import get_logger
-from extras.misc import prepare_model_for_training, print_trainable_params
-from extras.save_and_load import load_valuehead_params
-from hparams import ModelArguments, FinetuningArguments
-from pet.core.adapter import init_adapter
+from llmtuner.extras.logging import get_logger
+from llmtuner.extras.misc import prepare_model_for_training, print_trainable_params
+from llmtuner.extras.save_and_load import load_valuehead_params
+from llmtuner.hparams import ModelArguments, FinetuningArguments
+from llmtuner.tuner.core.adapter import init_adapter
 
 
 logger = get_logger(__name__)
 
 
 check_min_version("4.29.1")
 require_version("datasets>=2.12.0", "To fix: pip install datasets>=2.12.0")
 require_version("accelerate>=0.19.0", "To fix: pip install accelerate>=0.19.0")
 require_version("peft>=0.3.0", "To fix: pip install peft>=0.3.0")
 require_version("trl>=0.4.4", "To fix: pip install trl>=0.4.4")
 
 
-def load_pretrained(
-        model_args: ModelArguments,
-        finetuning_args: FinetuningArguments,
-        is_trainable: Optional[bool] = False,
-        stage: Optional[Literal["pt", "sft", "rm", "ppo"]] = "sft"
+def load_model_and_tokenizer(
+    model_args: ModelArguments,
+    finetuning_args: FinetuningArguments,
+    is_trainable: Optional[bool] = False,
+    stage: Optional[Literal["pt", "sft", "rm", "ppo"]] = "sft"
 ) -> Tuple[PreTrainedModel, PreTrainedTokenizer]:
     r"""
     Loads pretrained model and tokenizer.
 
     Support both training and inference.
     """
     if (not is_trainable) and model_args.checkpoint_dir is None:
@@ -118,15 +118,15 @@
     if hasattr(config, "auto_map") and "AutoTokenizer" in config.auto_map:
         tokenizer.__class__.register_for_auto_class()
     if hasattr(config, "auto_map") and "AutoModelForCausalLM" in config.auto_map:
         model.__class__.register_for_auto_class()
 
     # Initialize adapters
     model = prepare_model_for_training(model, finetuning_args.finetuning_type) if is_trainable else model
-    model = _init_adapter(model, model_args, finetuning_args, is_trainable, is_mergeable)
+    model = init_adapter(model, model_args, finetuning_args, is_trainable, is_mergeable)
 
     if stage == "rm" or stage == "ppo": # add value head
         model = AutoModelForCausalLMWithValueHead.from_pretrained(model)
 
         if stage == "rm" and model_args.checkpoint_dir is not None: # load valuehead weights to evaluate reward model
             logger.warning("Only the last checkpoint containing valuehead will be loaded as the valuehead.")
             if load_valuehead_params(model, model_args.checkpoint_dir[-1]):
```

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/core/parser.py` & `llmtuner-0.0.9/src/llmtuner/tuner/core/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 import torch
 import datasets
 import transformers
 from typing import Any, Dict, Optional, Tuple
 from transformers import HfArgumentParser, Seq2SeqTrainingArguments
 
-from extras.logging import get_logger
-from hparams import (
+from llmtuner.extras.logging import get_logger
+from llmtuner.hparams import (
     ModelArguments,
     DataArguments,
     FinetuningArguments,
     GeneratingArguments,
     GeneralArguments
 )
 
@@ -100,15 +100,15 @@
     # Set seed before initializing model.
     transformers.set_seed(training_args.seed)
 
     return model_args, data_args, training_args, finetuning_args, general_args
 
 
 def get_infer_args(
-        args: Optional[Dict[str, Any]] = None
+    args: Optional[Dict[str, Any]] = None
 ) -> Tuple[ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments]:
 
     parser = HfArgumentParser((ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments))
 
     if args is not None:
         model_args, data_args, finetuning_args, generating_args = parser.parse_dict(args)
     elif len(sys.argv) == 2 and sys.argv[1].endswith(".yaml"):
```

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/core/trainer.py` & `llmtuner-0.0.9/src/llmtuner/tuner/core/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     r"""
     Inherits Seq2SeqTrainer to support parameter-efficient checkpoints.
     """
 
     def __init__(self, finetuning_args: FinetuningArguments, **kwargs):
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
+        self._remove_log()
+
+    def _remove_log(self):
         if self.is_world_process_zero() and os.path.exists(os.path.join(self.args.output_dir, "trainer_log.jsonl")):
             logger.warning("Previous log file in this folder will be deleted.")
             os.remove(os.path.join(self.args.output_dir, "trainer_log.jsonl"))
 
     def _save(self, output_dir: Optional[str] = None, state_dict: Optional[Dict[str, torch.Tensor]] = None) -> None:
         r"""
         Saves trainable parameters as model checkpoint.
```

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/sft/metric.py` & `llmtuner-0.0.9/src/llmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/sft/trainer.py` & `llmtuner-0.0.9/src/llmtuner/tuner/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.1/src/llmtuner/tuner/sft/workflow.py` & `llmtuner-0.0.9/src/llmtuner/tuner/sft/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Inspired by: https://github.com/huggingface/transformers/blob/v4.29.2/examples/pytorch/summarization/run_summarization.py
 
 from typing import Optional, List
 from transformers import Seq2SeqTrainingArguments, DataCollatorForSeq2Seq, TrainerCallback
 
-from llmtuner.dsets import DataCollatorForChatGLM, get_dataset, preprocess_dataset
+from llmtuner.dsets import get_dataset, preprocess_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.constants import IGNORE_INDEX
 from llmtuner.extras.misc import get_logits_processor
 from llmtuner.extras.ploting import plot_loss
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.sft.metric import ComputeMetrics
@@ -48,15 +48,15 @@
     # Initialize our Trainer
     trainer = Seq2SeqPeftTrainer(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
-        callbacks=[LogCallback()],
+        callbacks=callbacks,
         compute_metrics=ComputeMetrics(tokenizer) if training_args.predict_with_generate else None,
         **trainer_kwargs
     )
 
     # Keyword arguments for `model.generate`
     gen_kwargs = {
         "do_sample": True,
```

### Comparing `llmtuner-0.0.1/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.0.9/src/llmtuner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.0.1
+Version: 0.0.9
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -115,15 +115,15 @@
 ```
 
 ## Requirement
 
 - Python 3.8+ and PyTorch 1.13.1+
 - 🤗Transformers, Datasets, Accelerate, PEFT and TRL
 - jieba, rouge-chinese and nltk (used at evaluation)
-- gradio and mdtex2html (used in web_demo.py)
+- gradio and matplotlib (used in web_demo.py)
 - uvicorn, fastapi and sse-starlette (used in api_demo.py)
 
 And **powerful GPUs**!
 
 If you want to enable quantized LoRA (QLoRA) on the Windows platform, you should install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
 
 ```bash
@@ -157,15 +157,16 @@
 python -m transformers.models.llama.convert_llama_weights_to_hf \
     --input_dir path_to_llama_weights --model_size 7B --output_dir path_to_llama_model
 ```
 
 ### (Continually) Pre-Training
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_pt.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage pt \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset wiki_demo \
     --finetuning_type lora \
     --output_dir path_to_pt_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
@@ -178,15 +179,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### Supervised Fine-Tuning
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_sft.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage sft \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
@@ -199,15 +201,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### Reward Model Training
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_rm.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage rm \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset comparison_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
@@ -219,15 +222,16 @@
     --plot_loss \
     --fp16
 ```
 
 ### PPO Training (RLHF)
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_ppo.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage ppo \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
@@ -242,15 +246,15 @@
     --plot_loss
 ```
 
 ### Distributed Training
 
 ```bash
 accelerate config # configure the environment
-accelerate launch src/train_XX.py # arguments (same as above)
+accelerate launch src/train_bash.py # arguments (same as above)
 ```
 
 <details><summary>Example configuration for full-tuning with DeepSpeed ZeRO-2</summary>
 
 ```yaml
 compute_environment: LOCAL_MACHINE
 deepspeed_config:
@@ -276,15 +280,16 @@
 ```
 
 </details>
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_sft.py \
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage pt \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
```

### Comparing `llmtuner-0.0.1/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.0.9/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 setup.py
 src/llmtuner/__init__.py
 src/llmtuner.egg-info/PKG-INFO
 src/llmtuner.egg-info/SOURCES.txt
 src/llmtuner.egg-info/dependency_links.txt
 src/llmtuner.egg-info/requires.txt
 src/llmtuner.egg-info/top_level.txt
+src/llmtuner/api/__init__.py
+src/llmtuner/api/app.py
+src/llmtuner/api/protocol.py
 src/llmtuner/dsets/__init__.py
 src/llmtuner/dsets/callbacks.py
 src/llmtuner/dsets/loader.py
 src/llmtuner/dsets/preprocess.py
 src/llmtuner/extras/__init__.py
 src/llmtuner/extras/callbacks.py
 src/llmtuner/extras/constants.py
@@ -28,15 +31,22 @@
 src/llmtuner/hparams/model_args.py
 src/llmtuner/tuner/__init__.py
 src/llmtuner/tuner/core/__init__.py
 src/llmtuner/tuner/core/adapter.py
 src/llmtuner/tuner/core/loader.py
 src/llmtuner/tuner/core/parser.py
 src/llmtuner/tuner/core/trainer.py
+src/llmtuner/tuner/ppo/__init__.py
+src/llmtuner/tuner/ppo/trainer.py
+src/llmtuner/tuner/ppo/utils.py
+src/llmtuner/tuner/ppo/workflow.py
+src/llmtuner/tuner/pt/__init__.py
+src/llmtuner/tuner/pt/workflow.py
+src/llmtuner/tuner/rm/__init__.py
+src/llmtuner/tuner/rm/collator.py
+src/llmtuner/tuner/rm/metric.py
+src/llmtuner/tuner/rm/trainer.py
+src/llmtuner/tuner/rm/workflow.py
 src/llmtuner/tuner/sft/__init__.py
 src/llmtuner/tuner/sft/metric.py
 src/llmtuner/tuner/sft/trainer.py
-src/llmtuner/tuner/sft/workflow.py
-src/utils/__init__.py
-src/utils/pairwise.py
-src/utils/peft_trainer.py
-src/utils/ppo.py
+src/llmtuner/tuner/sft/workflow.py
```

